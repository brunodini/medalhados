<template>
  <div class="nota-individual">
    <aside>
      <h4>{{ subcategoria.nome }}</h4>
      <ui-icon-button
        @click="toggleModal"
        icon="help_outline"
        type="flat"
        hide-ripple-ink>
      </ui-icon-button>
    </aside>
    <ui-radio-group
      @change="novaNota"
      :options="notas | toString"
      :value.sync="selecionada | toString"
      :name="radioGroupName">
    </ui-radio-group>

    <ui-modal
      :show.sync="modal.show" :header="subcategoria.nome"
      :body="subcategoria.descricao"
      :hide-footer="true"
    ></ui-modal>
  </div>
</template>

<script>
  export default{
    props: {
      categoria: '',
      subcategoria: {},
      notas: [],
      selecionada: '',
      pontuacao: 0
    },

    data() {
      return {
        modal: {
          show: false
        }
      }
    },

    computed: {
      radioGroupName() {
        return this.categoria + this.subcategoria.nome
      },
    },

    methods: {
      novaNota() {
        var self = this
        var radios = document.getElementsByClassName('ui-radio-input')

        self.pontuacao = 0

        for(var i = 0; i < radios.length; i++)
          if(radios[i].checked)
            self.pontuacao += parseInt(radios[i].value)

        self.$dispatch('mudar-nota', self.pontuacao)
      },
      toggleModal() {
        this.modal.show = !this.modal.show
      }
    }
  }
</script>

<style lang="stylus">
  @import "../variables.styl"

  .nota-individual
    display table
    width 95%
    padding 0 2.5%
    aside, .ui-radio-group
      display block
      @media screen and (min-width: $tablet)
        display table-cell
    .ui-icon-button
      cursor pointer !important
    .ui-modal-body
      white-space pre-line
      line-height 20px
    aside
      white-space nowrap
      vertical-align middle
      width 100%
      padding 20px 0
      @media screen and (min-width: $tablet)
        width 20%
        padding 0
      h4, i
        display inline
        vertical-align middle
      .ui-icon-button-flat.color-default
        cursor default
        vertical-align middle
        display none
        &:hover
          background-color transparent
        @media screen and (min-width: $tablet)
          display inline-block
      i
        padding 0 10px
    .ui-radio-group-options-wrapper
      display block
      .ui-radio
        display inline-block
        width 19.5%
        height 100%
        margin-left 0
        padding 8px 0
        text-align center
        @media screen and (min-width: $tablet)
          text-align left
        &:last-child
          float right
      .ui-radio-input-wrapper, .ui-radio-label-text
        display inline-block
        vertical-align text-bottom
      .ui-radio-label-text
        margin-left 0
        @media screen and (min-width: $tablet)
          margin-left 16px
      .ui-radio-input-wrapper
        margin-top 3px
      .ui-radio-border
        width 16px
        height 16px
</style>
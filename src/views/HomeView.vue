<template>
  <div class="home-view">
    <header>
      <h1 class="logo">Medalhados</h1>
      <button class="login" v-link="{ name: 'login' }">Acessar</button>
      <button class="login assinar" @click="goTo('//assine.medalhados.com.br')">Assinar</button>
    </header>
    <article class="intro">
      <div>
        <h1>Medalhados</h1>
        <h3>O primeiro clube de degustadores de vinhos do Brasil.</h3>
        <h3>E talvez, do mundo.</h3>

        <iframe src="https://player.vimeo.com/video/198081334" class="video" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

        <!--<div class="form">-->
          <!--<input v-model="user.nome" type="text" placeholder="Seu Nome">-->
          <!--<input v-model="user.email" type="text" placeholder="Seu E-mail">-->
          <!--<input v-model="user.cidade" type="text" placeholder="Sua Cidade">-->

          <!--<span>Seus dados serão utilizados exclusivamente para lhe fornecer mais informações sobre o nosso clube</span>-->

          <!--<button class="submit" @click.prevent="enviarRegistro" :disabled="isSending">-->
            <!--<span v-if="!isSending">Enviar</span>-->
            <!--<ui-progress-circular :show="isSending" color="white" type="indeterminate"></ui-progress-circular>-->
          <!--</button>-->
        <!--</div>-->
      </div>
    </article>

    <article class="about">
      <div class="center">
        <p>Hoje, no Brasil, você já tem à disposição diversos Clubes de Vinhos que oferecerem uma curadoria de bom nível, para selecionar dentre as quase infinitas opções de rótulos aqueles que mais fazem sentido ao paladar e ao bolso do brasileiro.</p>
        <p>Medalhados é um clube de vinhos diferente: o foco não está no vinho, mas em quem o degusta.</p>
        <p>É um clube que pretende congregar gente iniciada no mundo do vinho e interessada em se aprofundar e ampliar seus conhecimentos nesse apaixonante universo.</p>

        <img src="/static/img/site/eduardo-viotti.png">

        <h2>Organizado por Eduardo Viotti - jornalista, editor, professor, empreendedor, jurado internacional e um dos mais respeitados nomes do mercado mundial de vinhos -, Medalhados oferece a seus associados a oportunidade única de:</h2>

        <ul>
          <li>Aprender com grandes especialistas como avaliar vinho</li>
          <li>Evoluir constantemente na capacidade de degustar e pontuar vinhos</li>
          <li>Organizar suas preferências enológicas para orientar suas compras</li>
          <li>Integrar-se a uma comunidade de pessoas de interesse e gosto semelhante ao seu</li>
          <li>Receber conteúdo do mais alto nível sobre vitivinicultura</li>
          <li>Participar, como jurado convidado, de degustações técnicas e concursos nacionais e internacionais de vinho</li>
          <li>Receber mensalmente amostras de vinhos premiados em concursos nacionais e internacionais</li>
          <li>Adquirir vinhos de alta qualidade, com conveniência e descontos crescentes, a partir de sua evolução como degustador e formador de opinião.</li>
        </ul>
      </div>
    </article>

    <article class="how-it-works">
      <div class="center">
        <h2>Todo mês, 2 vinhos pra você avaliar e descobrir</h2>

        <p>Participando do clube "Medalhados", todo mês você receberá no endereço que determinar, 2 vinhos, premiados em concursos e selecionados pelo curador Eduardo Viotti, para degustar "às cegas”.</p>
        <p>Serão 2 garrafas de 750ml, sem rótulo, identificadas apenas com a etiqueta do clube Medalhados e a numeração da amostra. Assim como é feito nos grandes concursos internacionais de vinho.</p>
        <p>Através do site medalhados.com.br, você receberá toda a orientação de como avaliar profissionalmente um vinho e poderá colocar em prática esse conhecimento, pontuando as diversas características visuais, olfativas e gustativas das amostras que recebeu.</p>
        <p>Somente após dar as suas notas, você poderá descobrir o rótulo que acabou de degustar e comparar a sua avaliação com a nota oficial de cada vinho.</p>
      </div>
      <ul class="advantages">
        <li>
          <img src="/static/img/site/port-1.jpeg">
          <h3>Compre a preços especiais os vinhos que mais lhe agradar.</h3>
          <p>Como degustador do clube “Medalhados”, você terá descontos especiais dos produtores e importadores dos vinhos degustados para adquirí-los a preços especiais. E quanto mais apurada for a sua capacidade de avaliar, maiores serão os descontos oferecidos.</p>
        </li>
        <li>
          <img src="/static/img/site/port-2.jpeg">
          <h3>Não só os vinhos, mas você também será avaliado.</h3>
          <p>A equipe de especialistas do clube “Medalhados” estará atenta a cada nota que você atribuir às amostras. Comparando a sua avaliação com a média dos integrantes do clube “Medalhados" e com a nota oficial de cada vinho - atribuída em concursos nacionais e internacionais ou pelo próprio curador do clube - a sua performance como “degustador de vinhos” também estará sendo avaliada.</p>
          <p>E toda essa informação estará disponível, através de um dashboard de fácil leitura e com total privacidade, para que você possa evoluir constantemente nessa sua nova competência.</p>
        </li>
        <li>
          <img src="/static/img/site/port-3.jpeg">
          <h3>O seu talento de degustador será reconhecido.</h3>
          <p>Periodicamente, os degustadores melhor avaliados serão convidados pela Vinho Magazine para participarem de degustações especiais da revista e até mesmo de consagrados concursos anuais de vinhos, como o "Concours Mondial de Bruxelles - Edição Brasil" e "The Best of Wine Weekend”.</p>
        </li>
        <li>
          <img src="/static/img/site/port-4.jpeg">
          <h3>Todas as suas preferências registradas para consulta na hora que você quiser.</h3>
          <p>Através do site medalhados.com.br, você terá acesso permanente a suas preferências, suas notas e os detalhes dos vinhos degustados, num registro organizado para consultar sempre que desejar.</p>
        </li>
        <li>
          <img src="/static/img/site/port-5.png">
          <h3>Acesso ao conteúdo das mais recentes edições de Vinho magazine.</h3>
          <p>Todos os participantes do clube “Medalhados" terão acesso às mais recentes edições digitais da revista Vinho Magazine para evoluirem em seu conhecimento sobre o apaixonante universo da vitivinicultura.</p>
        </li>
        <li>
          <img src="/static/img/site/port-6.jpeg">
          <h3>Encontre outros Degustadores de gosto semelhante ao seu.</h3>
          <p>No clube “Medalhados” você tem a oportunidade de conhecer outros degustadores de gosto semelhante ao seu, seja em contato direto ou através dos encontros a serem promovidos pelo clube durante eventos e degustações por todo o país.</p>
        </li>
      </ul>
    </article>

    <article class="exclusives">
      <div class="center">
        <h2>No nosso clube só entram produtores e importadores premiados.</h2>

        <ol>
          <li>
            <i class="fa fa-trophy"></i>
            <h4>Job Total</h4>
          </li>
          <li>
            <i class="fa fa-trophy"></i>
            <h4>Peterlongo</h4>
          </li>
          <li>
            <i class="fa fa-trophy"></i>
            <h4>Zanella</h4>
          </li>
          <li>
            <i class="fa fa-trophy"></i>
            <h4>Perini</h4>
          </li>
          <li>
            <i class="fa fa-trophy"></i>
            <h4>San Michele</h4>
          </li>
          <li>
            <i class="fa fa-trophy"></i>
            <h4>Ivini</h4>
          </li>
          <li>
            <i class="fa fa-trophy"></i>
            <h4>L'Aretuso</h4>
          </li>
          <li>
            <i class="fa fa-trophy"></i>
            <h4>Merit</h4>
          </li>
        </ol>
      </div>
    </article>

    <article class="marina-dini">
      <div class="center">
        <h3>Um clube para quem entende de vinho ou quer muito entender.</h3>
        <blockquote>
          <p>Sempre fui um grande consumidor de vinhos, frequento confrarias e leio muito a respeito. Mas a oportunidade de evolução que o clube Medalhados me dá é realmente única.</p>
          <cite>
            <img src="/static/img/site/daniel-siqueira.jpeg">
            <span>Daniel Siqueira, Advogado</span>
          </cite>
        </blockquote>
        <blockquote>
          <p>Descobri o vinho há pouco tempo e fiquei apaixonada. Estou no Medalhados porque é uma forma moderna e divertida de entender sobre o assunto, sem ter que conviver com enochatos.</p>
          <cite>
            <img src="/static/img/site/marina-dini.png">
            <span>Marina Dini, Estilista e Bordadeira</span>
          </cite>
        </blockquote>
      </div>
    </article>

    <article class="price">
      <div class="center">
        <h2>Entre para o primeiro clube de degustadores pelo preço de um clube de vinhos comum</h2>

        <div class="content">
          <aside class="plano-prices">
            <h4>PLANO "MEU MEDALHADOS"</h4>
            <h5>280</h5>
            <span>Usufruindo do benefício do Desconto Fidelidade com cobrança de 6 parcelas sem juros pelo Pag Seguro (todos os cartões), referentes a um pagamento no valor total semestral de R$1.680,00. Preço normal sem desconto: R$3.360,00</span>

            <div class="assine-wrapper">
              <button class="login" @click="goTo('//assine.medalhados.com.br')">Assinar</button>
            </div>
          </aside>
          <ul>
            <li>
              <i class="fa fa-trophy"></i>
              <aside>
                <h4>Receba vinhos premiados todo mês</h4>
                <p>2 garrafas mensais de 750ml de vinho premiado em concursos, com no mínimo medalha de prata</p>
              </aside>
            </li>
            <li>
              <i class="fa fa-smile-o"></i>
              <aside>
                <h4>Aprenda a Degustar</h4>
                <p>acesso ilimitado a conteúdos educacionais especialmente produzidos</p>
              </aside>
            </li>
            <li>
              <i class="fa fa-area-chart"></i>
              <aside>
                <h4>Acompanhe sua Perfomance</h4>
                <p>plataforma online de treinamento e acompanhamento de performance de degustação profissional</p>
              </aside>
            </li>
            <li>
              <i class="fa fa-book"></i>
              <aside>
                <h4>Vinho Magazine Online</h4>
                <p>acesso ilimitado às edições digitais da revista Vinho Magazine</p>
              </aside>
            </li>
            <li>
              <i class="fa fa-glass"></i>
              <aside>
                <h4>Participe de Degustações</h4>
                <p>convite para participação em eventos e degustações promovidos pelo clube</p>
              </aside>
            </li>
            <li>
              <i class="fa fa-shopping-cart"></i>
              <aside>
                <h4>Compre vinhos com descontos</h4>
                <p>descontos em compras de vinhos junto a produtores e importadores participantes</p>
              </aside>
            </li>
          </ul>
        </div>
      </div>
    </article>

    <footer>
      <nav>
        <a href="https://www.facebook.com/Medalhados" class="fa fa-facebook"></a>
        <a href="mailto:eu@zeluiztavares.com.br" target="_blank" class="fa fa-envelope-o"></a>
      </nav>
      <span>© 2016 Medalhados. All Rights Reserved</span>
      <h1 class="logo">Medalhados</h1>
    </footer>

    <div class="alert alert-success">
      <ui-alert type="success" :show="show.success">Você se cadastrou com Sucesso!</ui-alert>
    </div>

    <div class="alert alert-error">
      <ui-alert type="error" :show="show.error">Houve um problema com o envio dos seus dados. Por favor, tente novamente</ui-alert>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        user: {
          nome: '',
          email: '',
          cidade: ''
        },
        show: {
          success: false,
          error: false
        },
        isSending: false
      }
    },
    methods: {
      enviarRegistro() {
        var email = 'eu@zeluiztavares.com.br'

        this.isSending = true

        this.$http.post('https://formspree.io/' + email, this.user).then((response) => {
          this.show.success = true
          this.isSending = false
        }).catch((error) => {
          this.show.error = true
          this.isSending = false
        })
      },
      goTo(url) {
        window.location = url
      }
    }
  }
</script>

<style lang="stylus">
  .home-view
    background white
    article
      text-align center
    h2, h3
      font-weight 700
      text-transform uppercase
    h2
      font-size 1.8em
      @media screen and (min-width: 800px)
        font-size 36px
    h3
      font-size 1.3em
      @media screen and (min-width: 800px)
        font-size 22px
    h4
      font-weight 500
      padding 20px 0 70px 0
    p
      color #888
      font-size .9em
      line-height 20px
      margin 0 0 10px 0
      @media screen and (min-width: 800px)
        font-size 1.1em
        line-height 30px
        margin 0
    button,
    .login
      cursor pointer
    .login
      background white
      font-size .8em
      text-transform uppercase
      padding 10px 15px
      border-radius 5px
      border 1px solid black
    .assinar
      background #b71c1c
      color white
      border 1px solid white
    .logo
      display inline-block
      background url("/static/img/site/logo.png") no-repeat
      background-position center left
      background-size 80px
      height 90px
      width 100px
      text-indent -9999px
      vertical-align middle
    .video
      width 100%
      max-width 640px
      height 360px
      @media screen and (min-width: 800px)
        width 640px
        height 360px
    header
      background white
      position fixed
      top 0
      left 0
      width 90%
      padding 0 5%
      text-align left
      .logo
        width 40%
        @media screen and (min-width: 800px)
          width 75%
    .center
      display inline-block
      width 90%
      @media screen and (min-width: 800px)
        max-width 1140px

    .intro
      background url("/static/img/site/fundo.jpeg") center no-repeat
      color white
      text-align center
      padding 100px 5% 80px 5%
      margin 90px 0 0 0
      width 90%
      h1
        font-family 'American Typewriter'
        font-size 2.3em
        font-weight normal
        text-transform uppercase
        margin 0 0 20px 0
        text-shadow 1px 1px 1px rgba(0,0,0,.5)
        @media screen and (min-width: 800px)
          font-size 56px
      h3
        font-weight 400
        padding-bottom 10px
        text-shadow 1px 1px 1px rgba(0,0,0,.5)
      h4
        text-shadow 1px 1px 1px rgba(0,0,0,.5)
      span
        display block
        font-size .7em
        font-weight 400
        text-align left
        padding 10px 0 40px 0
        text-shadow 1px 1px 1px rgba(0,0,0,.5)
      .form
        float none
        width 100%
        margin 0 auto
        @media screen and (min-width: 800px)
          width 300px
        input
          width 95%
          padding 4% 2.5%
          border-radius 5px
          margin-bottom 20px
        .submit
          background #c28b4b
          color white
          width auto
          border none
          border-radius 3px
          font-size 1em
          padding 10px 80px
          span
            font-size 1em
            padding 0
    .about
      margin 40px 0
      @media screen and (min-width: 800px)
        margin 80px 0
      img
        margin 30px 0 0 0
        width 100%
        @media screen and (min-width: 800px)
          margin 60px 0 0 0
          width auto
      h2, ul
        display inline-block
        text-align left
        width 100%
        @media screen and (min-width: 800px)
          width 750px
      h2
        font-size 22px
        font-weight 400
        text-transform none
        color #222
        padding 25px 0 0 0
      ul
        width 100%
        @media screen and (min-width: 800px)
          width 750px
      li
        padding 13px 0 0 0
        &:before
          content '- '
    .how-it-works
      &:before
        content ''
        background url("/static/img/site/bottles.jpg") center no-repeat
        background-size cover
        display inline-block
        width 100%
        height 150px
      h2
        padding 80px 0 20px 0
    .advantages
      padding 60px 0 0 0
      width 100%
      @media screen and (min-width: 800px)
        width auto
      li
        display inline-block
        width 100%
        vertical-align top
        text-align center
        padding 0 0 60px 0
        margin 0
        @media screen and (min-width: 800px)
          width 360px
          margin 0 10px
      h3, p
        width 90%
        padding 15px 5%
        @media screen and (min-width: 800px)
          width auto
          padding 0
      h3
        line-height 28px
        padding 15px 0
      p
        font-size 15px
        line-height 24px
      img
        width 100%
        @media screen and (min-width: 800px)
          width auto
    .exclusives
      background rgba(148,21,46,.8)
      padding 80px 0
      .center
        text-align center
      h2
        font-size 32px
        color white
        padding 0 0 80px 0
      ol
        display inline-block
        width 90%
        padding 0 5%
        @media screen and (min-width: 800px)
          width 960px
      li
        display inline-block
        font-size 16px
        color white
        width 100%
        @media screen and (min-width: 800px)
          width 200px
      .fa-trophy
        font-size 48px
        color #f7e257
    .marina-dini
      padding 0 0 80px 0
      h3
        font-size 30px
        padding 90px 0 60px 0
      blockquote
        display inline-block
        vertical-align top
        width 96%
        padding 0 2% 30px 2%
        @media screen and (min-width: 800px)
          width 45%
          padding 0 2%
        cite
          text-align center
          img
            display inline-block
            border-radius 50%
            margin 20px 0
          span
            color #999
            float left
            font-style italic
            width 100%
        p
          color #ccc
          font-size 20px
          font-style italic
          &:before
            content '"'
          &:after
            content '"'
    .price
      background rgba(194,139,75,.9)
      padding 80px 0
      h2
        padding 0 0 50px 0
      h4
        text-transform uppercase
        padding 20px 0
        font-weight 300
      .content
        .plano-prices
          padding-right 5%
          margin-bottom 40px
          @media screen and (min-width: 800px)
            margin-bottom 0
          span
            display block
            width 100%
            line-height 1.5em
            text-align center
            @media screen and (min-width: 800px)
              text-align left
          .assine-wrapper
            width 100%
            text-align center
            padding 10px 0 0 0
          .login
            background transparent
      ul
        display block
        @media screen and (min-width: 800px)
          display flex
          flex 0 0 70%
          flex-wrap wrap
        li
          padding 0 3% 40px 3%
          @media screen and (min-width: 800px)
            display flex
            flex 0 0 43%
          .fa
            color rgba(250,250,250,.6)
            font-size 3em
            margin 10px 0
            @media screen and (min-width: 800px)
              margin 0 20px 0 0
      aside
        text-align left
        h4
          font-size 14px
          font-weight 700
          padding 0 0 20px 0
          text-align center
          @media screen and (min-width: 800px)
            text-align left
        p
          color black
          font-size .85em
          line-height 2em
          text-align center
          @media screen and (min-width: 800px)
            text-align left
      .content
        display block
        @media screen and (min-width: 800px)
          display flex
        span
          font-size .7em
      h5
        font-size 8em
        font-weight 700
        color #b6cf6c
        text-align center
        @media screen and (min-width: 800px)
          text-align left
        &:before
          content '$'
          font-weight 300
          font-size .3em
          vertical-align top
        &:after
          content '/mês'
          font-weight 300
          font-size .15em
    footer
      display flex
      align-items center
      width 95%
      padding 0 2.5%
      nav, span, .logo
        flex 1 auto
      nav
        text-align center
        @media screen and (min-width: 800px)
          text-align left
        a
          background none
          cursor pointer
          padding 10px
          border none
          color: #000
          text-decoration none
      span
        flex 3 auto
        font-size .7em
        text-align center
      .logo
        background-position center right
</style>
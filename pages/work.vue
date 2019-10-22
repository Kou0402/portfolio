<template>
  <main>
    <PageTitle>Work</PageTitle>
    <ContentsArea>
      <article>
        <h3>不動産会社業務システム改修</h3>
        <h4>概要</h4>
        <p>
          不動産会社の営業向け顧客管理パッケージソフトの改修案件。<br />
          顧客検索部分の新機能ページの追加を担当。
        </p>
        <h4>技術</h4>
        <p>PHP/JavaScript/Lumen/jQuery/PostgreSQL/Linux/Vagrant</p>
      </article>
      <article>
        <h3>ポータルサイトのデータ変換ツール</h3>
        <h4>概要</h4>
        <p>
          VBA案件。とある機関のポータルサイト改修プロジェクトの一環で、サイトに掲示するための資料データを、規格通りに整形するエクセルツールの作成を担当。
        </p>
        <h4>技術</h4>
        <p>VBA</p>
      </article>
      <article>
        <h3>大手企業基幹システム開発サポート</h3>
        <h4>概要</h4>
        <p>
          大手企業の基幹システムの改修プロジェクトのテストサポーターとして参画。
          テスト用データ作成や不具合発生時のパッチSQL作成などを担当。
        </p>
        <h4>技術</h4>
        <p>SQL/OracleDB</p>
      </article>
      <article>
        <h3>契約管理システムリプレイス</h3>
        <h4>概要</h4>
        <p>
          金融関連会社の社内システムのリプレイス案件。Flashで構成されたシステムをHTML5/CSS3にて再構成。
          主にjQueryによる画面動作部を担当。
        </p>
        <h4>技術</h4>
        <p>Java/JavaScript/Seasar2/jQuery/SQLServer</p>
      </article>
      <article>
        <h3>サーバーリプレイス</h3>
        <h4>概要</h4>
        <p>老朽化したサーバーとソフトウェアのリプレイス案件。主にバッチ系処理の製造を担当。</p>
        <h4>技術</h4>
        <p>WindowsServer/Java/VBS</p>
      </article>
    </ContentsArea>
  </main>
</template>

<script>
import PageTitle from '~/components/PageTitle.vue'
import ContentsArea from '~/components/ContentsArea.vue'

export default {
  components: {
    PageTitle,
    ContentsArea
  }
}
</script>

<style scoped lang="scss">
article {
  margin-bottom: 4rem;
  h3 {
    letter-spacing: 0.4vw;
    margin: 3vh 0;
  }
  p {
    letter-spacing: 0.1vw;
    line-height: 1.3em;
    font-size: 1.3rem;
    margin-top: 1.7rem;
  }
}
@media screen and (max-width: 896px) {
  article {
    h3 {
      font-size: 2rem;
    }
    p {
      letter-spacing: 0;
      line-height: 2em;
      font-size: 1.2rem;
    }
  }
}
</style>

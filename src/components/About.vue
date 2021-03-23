<template>
  <section id="about">
      <v-container>
        <v-row>
          <v-col sm="5">
            <g-image alt="Example image" src="~/profile.jpg" width="400" />
          </v-col>
          <v-col sm="6" class="d-flex flex-column justify-center">
            <h1>澁谷 将吾（しぶや しょうご）</h1>
            <div>
                <p>法政大学大学院理工学研究科応用情報工学専攻１年、知的情報処理研究室の澁谷将吾と申します。大学では主に画像処理や深層学習を勉強しています。現在研究室では農林水産省委託プロジェクト研究として24府県の農業試験場 農研機構などと共同でAI技術を用いた植物病害自動診断システム構築の研究に関わっています。</p>
                <p>学部生の時に「<a href="https://ipsj.ixsq.nii.ac.jp/ej/index.php?active_action=repository_view_main_item_detail&page_id=13&block_id=8&item_id=205376&item_no=1">中央領域に注目する Center Attention による頑健性の高い植物病害診断装置の構築</a>」を情報処理学会にて発表しました。</p>
                <p>趣味はイラストを描くことで、学部生の時には70名ほどの部員が所属する漫画研究会サークルの部長を務め、イラストの勉強会なども行っていました。</p>
                <p>メールアドレス: syogo.shibuya.5u@stu.hosei.ac.jp</p>
                <p>技術ブログ: <a href="https://hotcocoastudy.hatenablog.jp/">はてなブログ</a> 、 <a href="https://hotcocoastudy.hatenablog.jp/">Zenn</a></p>
                <p>GitHub: <a href="https://github.com/SyogoShibuya">SyogoShibuya</a></p>
                <p>イラストポートフォリオ: <a href="https://hotcocoagallery.jimdosite.com/">hotcocoagallery</a></p> 
                <p>今勉強中の本: Linuxで動かしながら学ぶTCP/IPネットワーク入門、体系的に学ぶ安全なWebアプリケーションの作り方、ゼロからOS自作入門、知識ゼロからきちんと学べる！Illustratorしっかり入門</p> 
            </div>
          </v-col>
        </v-row>
      </v-container>
  </section>
</template>

<style scoped>
.g-image {
    border-radius: 100%;
}
</style>
<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="mr40 mt20">
          <router-link to="/list-voucher">
            <img src="../../assets/icons/back.svg" />
          </router-link>
        </div>
        <div>
          <h1 class="m0">Add Voucher</h1>
          <p class="mt5 mb20 tc-green">
            Make your customers shop using vouchers
          </p>
        </div>
      </div>
      <hr class="uline-grey" />
      <div class="mt50 row">
        <div class="w20">
          <label class="form-label">Voucher Image</label>
        </div>
        <div class="w80">
          <input class="hidden" type="file" id="upload-file" />
          <img class="cursor-pointer" src="../../assets/images/Frame 531.png" alt="" @click="upload_file()" />
        </div>
      </div>
      <div class="mt30 row">
        <div class="w20">
          <label class="form-label">Voucher Code</label>
        </div>
        <div class="w80 relative">
          <input class="form-text" type="text" minlength="0" maxlength="6" placeholder="Masukkan Kode Voucher" />
          <span class="addon-right">| 0 / 6</span>
        </div>
      </div>
      <div class="mt30 row">
        <div class="w20">
          <label class="form-label">Voucher Name</label>
        </div>
        <div class="w80 relative">
          <input class="form-text" type="text" placeholder="Masukkan Nama Voucher" />
          <span class="addon-right">| 5 / 20</span>
        </div>
      </div>
      <div class="mt30 row">
        <div class="w20">
          <label class="form-label">Description</label>
        </div>
        <div class="w80 relative">
          <textarea class="form-text" cols="30" rows="10" placeholder="Masukkan Voucher Description"></textarea>
          <span class="addon-right">| 0 / 5000</span>
        </div>
      </div>
      <div class="mt30 row">
        <div class="w20">
          <label class="form-label">Type</label>
        </div>
        <div class="w80 relative">
          <input class="form-text" type="text" placeholder="Pilih Type" />
          <img width="15" class="addon-right" src="../../assets/images/edit-2.png" alt="" />
        </div>
      </div>
      <div class="mt30 row">
        <div class="w20">
          <label class="form-label">Min. Transaction</label>
        </div>
        <div class="w80">
          <input class="form-text" type="text" placeholder="Masukkan Minimal Transaction" />
        </div>
      </div>
      <div class="mt30 row">
        <div class="w20">
          <label class="form-label">Amount</label>
        </div>
        <div class="w80">
          <input class="form-text" type="text" placeholder="Masukkan Amount" />
        </div>
      </div>
      <div class="mt30 row">
        <div class="w20">
          <label class="form-label">valid From</label>
        </div>
        <div class="w80">
          <input class="form-text" type="text" placeholder="Masukkan Tanggal" />
        </div>
      </div>
      <div class="mt30 row">
        <div class="w20">
          <label class="form-label">Valid Until</label>
        </div>
        <div class="w80">
          <input class="form-text" type="text" placeholder="Masukkan Tanggal" />
        </div>
      </div>
      <div class="flex mt30">
        <router-link to="/list-voucher">
          <button class="bt-submit-green">Add Voucher</button>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "add-voucher",
  methods: {
    upload_file() {
      const input_file = document.querySelector("#upload-file");
      input_file.click();
    },
    // handle_article_name(event) {
    //   if (event.target.value.length > 20) {
    //     event.preventDefault();
    //   }
    // },
  },
};
</script>

<template>
  <div class="res-col-to-row" id="official-segment">
    <img
      alt="organization logo: hyrule"
      src="../assets/organization-logo.png"
    />
    <div class="verification">
      <label>VERIFIED CERTIFICATE</label>
      <p>Issued {{ certificateDate }}</p>
    </div>
    <div class="verification">
      <label>VALID CERTIFICATE ID</label>
      <p>{{ certificateID }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "DiplomaBottom",
  data: () => {
    return {
      certificateDate: "June 11, 2018",
      certificateID: "0a880bd84ab14c84aad91cd864e66e6a",
    };
  },
};
</script>

<style scoped>
label {
  font-weight: bold;
}

img {
  height: 5em;
  margin: 2.5em 0;
}

.verification {
  margin-top: 1em;
  margin-left: 3em;
}

.verification p {
  margin: 0.25rem;
  font-size: 0.8rem;
}

.res-col-to-row {
  display: flex;
  justify-content: space-between;
}

#official-segment {
  justify-content: flex-start;
  margin-bottom: 1em;
}

@media (max-width: 768px), (orientation: portrait) {
  .res-col-to-row {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }

  .verification {
    margin: 0em;
    margin-top: 1em;
  }
}
</style>

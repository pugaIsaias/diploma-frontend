<template>
  <div class="res-col-to-row">
    <div class="res-division">
      <p>This is to certify that</p>
      <p id="student-name">
        <b>{{ studentName }}</b>
      </p>
      <p>successfully completed and received a passing grade in</p>
      <p>
        <b id="certification-name">{{ certificateName }}</b>
      </p>
      <p>
        a course of study offered by UHx, an online learning initiative of The
        University of Hyrule.
      </p>
    </div>
    <div class="res-division">
      <ul>
        <li
          v-for="signator in signatories"
          :key="signator.id"
          class="signatory"
        >
          <p class="signatory-sign">{{ signator.sign }}</p>
          <p class="signatory-name">{{ signator.name }}</p>
          <p class="role">{{ signator.role }}</p>
          <p class="organization">{{ signator.organization }}</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "DiplomaMiddle",
  data: () => {
    return {
      studentName: "Isaias Samuel Puga Solares",
      certificateName: "BEING AWESOME AT RESPONSIVE FRONT-END",
      signatories: [
        {
          id: 0,
          sign: "Zelda",
          name: "Zelda Hyrule",
          role: "Director",
          organization: "Hyrule Castle Ruler",
        },
        {
          id: 1,
          sign: "Link",
          name: "Link Link",
          role: "Instructor",
          organization: "Hyrule Hero Guild",
        },
        {
          id: 2,
          sign: "Ganondorf",
          name: "Ganondorf Dragmire",
          role: "Principal",
          organization: "Hyrule Guidance Committee",
        },
      ],
    };
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Cedarville+Cursive");

b {
  color: black;
}

#student-name {
  font-size: 1.8rem;
}

#certification-name {
  font-size: 1.2rem;
}

.signatory {
  margin-bottom: 1em;
}

.signatory-sign {
  font-family: "Cedarville Cursive", cursive;
}

.signatory-name {
  font-weight: bold;
  color: #454545;
}

.signatory p {
  margin: 0.4rem;
}

.role {
  font-size: 0.9rem;
}

.organization {
  font-size: 0.9rem;
}

.res-col-to-row {
  display: flex;
  justify-content: space-between;
}

.organization {
  font-style: italic;
}

ul {
  list-style: none;
  padding: 0px;
}

li {
  text-align: right;
}

@media (max-width: 768px), (orientation: portrait) {
  .res-division {
    border-bottom: 0.05em solid gray;
    padding-bottom: 1em;
    margin-bottom: 1em;
    align-self: stretch;
  }

  .res-col-to-row {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }

  .signatory {
    text-align: center;
  }

  #student-name {
    font-size: 1.4rem;
  }
}
</style>

<template>
  <li class="list-group-item">
    <form>
      <!-- General Information Start -->
      <div>
        <p class="my-3 fs-5 fw-semibold">General Information</p>
        <div>
          <!-- Image Start -->
          <div class="mb-3">
            <base-input
              type="file"
              identity="recipeImage"
              label="Photo Recipe"
            ></base-input>
          </div>
          <!-- Image End -->

          <!-- Recipe Title Start -->
          <div class="mb-3">
            <base-input
              type="text"
              identity="recipeTitle"
              placeholder="Give your recipe a title"
              label="Photo Recipe"
            ></base-input>
          </div>
          <!-- Recipe Title  End -->

          <!-- Recipe Description Start -->
          <div class="mb-3">
            <BaseTextarea
              identity="”recipeDescription”"
              label="“Description”"
              placeholder="“Share"
              story
              behind
              recipe
              and
              what
              is
              make
              it
              special”
            ></BaseTextarea>
          </div>
          <!-- Recipe Description End -->

          <!-- Recipe Cateogry Start -->
          <div class="mb-3">
            <BaseSelect
              :data="['Breakfast', 'Lunch', 'Dinner', 'Meals', 'Snacks']"
            ></BaseSelect>
          </div>
          <!-- Recipe Category End -->
        </div>
      </div>
      <!-- General Information End -->

      <!-- Time Setting Start -->
      <div class="border-top py-1">
        <p class="my-3 fs-5 fw-semibold">Time Setting</p>
        <div>
          <!-- Preparation Time Start -->
          <div class="mb-3">
            <base-input
              type="number"
              identity="prepTime"
              placeholder="0"
              label="Prep Time"
            ></base-input>
          </div>
          <!-- Preparation Time End -->

          <!-- Cook Time Start -->
          <div class="mb-3">
            <base-input
              type="number"
              identity="cookTime"
              placeholder="0"
              label="Cook Time"
            ></base-input>
          </div>
          <!-- Cook Time End -->

          <!-- Total Time Start -->
          <div class="mb-3">
            <base-input
              type="number"
              identity="totalTime"
              placeholder="0"
              label="Total Time"
            ></base-input>
          </div>
          <!-- Total Time End -->
        </div>
      </div>
      <!-- Time Setting End -->

      <!-- Ingredients Start -->
      <div class="border-top py-1">
        <p class="my-3 fs-5 fw-semibold">Ingredients</p>
        <p>
          Enter one ingredient per line. Include the quantity (i.e. cups,
          tablespoons) and any special preparation (i.e. sifted, softened,
          chopped). Use optional headers to organize the different parts of the
          recipe (i.e. Cake, Frosting, Dressing).
        </p>
        <div>
          <div class="mb-3 row">
            <!-- Ingredient Input Start -->
            <div class="col-lg-11 col-11">
              <base-input
                type="text"
                identity="ingredient"
                placeholder="Ex: 1 cup sugar"
              ></base-input>
            </div>
            <!-- Ingredient Input End -->
            <div
              class="col-lg-1 col-1 col-form-label align-self-end delete-ingredient"
              style="color: #cb3a31"
            >
              <i class="fa-regular fa-trash-can px-1"></i
              ><span class="d-none d-md-inline">Delete</span>
            </div>
          </div>
        </div>
        <!-- Add More Button Start -->
        <BaseButton class="new-ingredient-btn px-3 py-2" type="button">
          Add More
        </BaseButton>
        <!-- Add More Button Start -->
      </div>
      <!-- Ingredients End -->

      <!-- Direction Start -->
      <div class="border-top my-3">
        <p class="my-3 fs-5 fw-semibold">Directions</p>
        <p>
          Explain how to make your recipe, including oven temperatures, baking
          or cooking times, and pan sizes, etc. Use optional headers to organize
          the different parts of the recipe
        </p>
        <div>
          <div class="mb-3 row">
            <!-- Direction Input Start -->
            <div class="col-lg-11 col-11">
              <base-input
                type="text"
                identity="direction"
                placeholder="Ex: 1 cup sugar"
              ></base-input>
            </div>
            <!-- Direction Input End -->
            <div
              class="col-lg-1 col-1 col-form-label align-self-end delete-ingredient"
              style="color: #cb3a31"
            >
              <i class="fa-regular fa-trash-can px-1"></i
              ><span class="d-none d-md-inline">Delete</span>
            </div>
          </div>
        </div>
        <!-- Add More Button Start -->
        <BaseButton class="new-ingredient-btn px-3 py-2" type="button">
          Add More
        </BaseButton>
        <!-- Add More Button End -->
      </div>
      <!-- Direction End -->

      <!-- Form Button Start -->
      <div class="border-top py-3 d-flex my-4 justify-content-end">
        <!-- Cancel Button Start -->
        <BaseButton class="cancel-btn px-3 py-2 ms-1"> Cancel </BaseButton>
        <!-- Cancel Button End -->

        <!-- Submit Button Start -->
        <BaseButton class="submit-recipe-btn px-3 py-2 ms-1">
          Submit
        </BaseButton>
        <!-- Submit Button End -->
      </div>
      <!-- Form Button End -->
    </form>
  </li>
</template>

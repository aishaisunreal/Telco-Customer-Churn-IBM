# Telco-Customer-Churn-IBM
<img width="793" height="400" alt="Untitled design (1)" src="https://github.com/user-attachments/assets/2a51657b-7e37-4663-a84e-3e0f163642b3" />


This sample data module tracks a fictional telco company's customer churn based on various factors. The churn column indicates whether the customer departed within the last month. Other columns include gender, dependents, monthly charges, and many with information about the types of services each customer has.

I built a Deep Learning Model to predict if customer departed within the last month, given other characteristics of the customer, such as gender, dependents, monthly charges, and many other information.

# Steps taken to make this Deep Learning Model
- Import libraries
- Exploring dataset 
- Placing preliminary observations
- Analysis and Data visualizations
- Data preprocessing
- Feature engineering and extraction
- Splitting and balancing data
- Encoding & Scaling
- Model training & Evaluation

# Characterstics of DL Model

 Model: "sequential_9"

 

┏━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━┓

┃ Layer (type)                    ┃ Output Shape           ┃       Param # ┃

├─────────────────────────────────┼────────────────────────┼───────────┤

│ dense_35 (Dense)                │ (None, 64)             │         3,072 │

├─────────────────────────────────┼────────────────────────┼───────────┤

│ dropout_10 (Dropout)            │ (None, 64)             │             0 │

├─────────────────────────────────┼────────────────────────┼───────────┤

│ dense_36 (Dense)                │ (None, 32)             │         2,080 │

├─────────────────────────────────┼────────────────────────┼───────────┤

│ dropout_11 (Dropout)            │ (None, 32)             │             0 │

├─────────────────────────────────┼────────────────────────┼───────────┤

│ dense_37 (Dense)                │ (None, 16)             │           528 │

├─────────────────────────────────┼────────────────────────┼───────────┤

│ dense_38 (Dense)                │ (None, 1)              │            17 │

└─────────────────────────────────┴────────────────────────┴───────────┘


 Total params: 5,697 (22.25 KB)

 Trainable params: 5,697 (22.25 KB)

 Non-trainable params: 0 (0.00 B)

optimizer: adam

loss: binary_crossentropy

epochs: 50

validation_split: 0.2

Verbose: 1

# Model Final Evaluation

**DL Model history**

Epoch 1/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 2s 5ms/step - accuracy: 0.5794 - loss: 0.6632 - val_accuracy: 0.7884 - val_loss: 0.6127

Epoch 2/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 3ms/step - accuracy: 0.7947 - loss: 0.4369 - val_accuracy: 0.8729 - val_loss: 0.4565

Epoch 3/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8019 - loss: 0.4171 - val_accuracy: 0.9200 - val_loss: 0.3219

Epoch 4/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8248 - loss: 0.3872 - val_accuracy: 0.9022 - val_loss: 0.3397

Epoch 5/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8319 - loss: 0.3790 - val_accuracy: 0.9120 - val_loss: 0.3464

Epoch 6/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8408 - loss: 0.3592 - val_accuracy: 0.9182 - val_loss: 0.3050

Epoch 7/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8486 - loss: 0.3406 - val_accuracy: 0.9333 - val_loss: 0.2857

Epoch 8/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8470 - loss: 0.3523 - val_accuracy: 0.9422 - val_loss: 0.2611

Epoch 9/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8473 - loss: 0.3429 - val_accuracy: 0.9084 - val_loss: 0.3168

Epoch 10/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8459 - loss: 0.3407 - val_accuracy: 0.9316 - val_loss: 0.2721

Epoch 11/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8436 - loss: 0.3459 - val_accuracy: 0.9387 - val_loss: 0.2603

Epoch 12/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 3ms/step - accuracy: 0.8480 - loss: 0.3338 - val_accuracy: 0.9200 - val_loss: 0.3055

Epoch 13/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8476 - loss: 0.3299 - val_accuracy: 0.8978 - val_loss: 0.3523

Epoch 14/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8472 - loss: 0.3368 - val_accuracy: 0.8924 - val_loss: 0.3471

Epoch 15/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 6ms/step - accuracy: 0.8499 - loss: 0.3282 - val_accuracy: 0.9511 - val_loss: 0.2172

Epoch 16/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 6ms/step - accuracy: 0.8536 - loss: 0.3180 - val_accuracy: 0.9013 - val_loss: 0.3258

Epoch 17/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 5ms/step - accuracy: 0.8519 - loss: 0.3238 - val_accuracy: 0.9182 - val_loss: 0.3040

Epoch 18/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8596 - loss: 0.3091 - val_accuracy: 0.9547 - val_loss: 0.2231

Epoch 19/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8601 - loss: 0.3047 - val_accuracy: 0.9484 - val_loss: 0.2313

Epoch 20/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8536 - loss: 0.3211 - val_accuracy: 0.9316 - val_loss: 0.2628

Epoch 21/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8683 - loss: 0.3008 - val_accuracy: 0.9182 - val_loss: 0.2944

Epoch 22/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8558 - loss: 0.3070 - val_accuracy: 0.9369 - val_loss: 0.2615

Epoch 23/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8579 - loss: 0.3151 - val_accuracy: 0.9520 - val_loss: 0.2364

Epoch 24/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8663 - loss: 0.2978 - val_accuracy: 0.9440 - val_loss: 0.2588

Epoch 25/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8552 - loss: 0.3001 - val_accuracy: 0.9289 - val_loss: 0.2725

Epoch 26/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8600 - loss: 0.3059 - val_accuracy: 0.9449 - val_loss: 0.2322

Epoch 27/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8716 - loss: 0.2894 - val_accuracy: 0.9333 - val_loss: 0.2775

Epoch 28/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8650 - loss: 0.2934 - val_accuracy: 0.8764 - val_loss: 0.3465

Epoch 29/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8646 - loss: 0.2880 - val_accuracy: 0.9324 - val_loss: 0.2580

Epoch 30/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8578 - loss: 0.2990 - val_accuracy: 0.9191 - val_loss: 0.2761

Epoch 31/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8632 - loss: 0.2947 - val_accuracy: 0.9129 - val_loss: 0.2853

Epoch 32/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8688 - loss: 0.2950 - val_accuracy: 0.9236 - val_loss: 0.2731

Epoch 33/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8736 - loss: 0.2848 - val_accuracy: 0.9289 - val_loss: 0.2753

Epoch 34/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8719 - loss: 0.2909 - val_accuracy: 0.9120 - val_loss: 0.2877

Epoch 35/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 5ms/step - accuracy: 0.8669 - loss: 0.2868 - val_accuracy: 0.9476 - val_loss: 0.2334

Epoch 36/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 5ms/step - accuracy: 0.8660 - loss: 0.2922 - val_accuracy: 0.9413 - val_loss: 0.2402

Epoch 37/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 5ms/step - accuracy: 0.8717 - loss: 0.2877 - val_accuracy: 0.9449 - val_loss: 0.2510

Epoch 38/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8808 - loss: 0.2759 - val_accuracy: 0.9129 - val_loss: 0.2883

Epoch 39/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8755 - loss: 0.2764 - val_accuracy: 0.9413 - val_loss: 0.2200

Epoch 40/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 3ms/step - accuracy: 0.8736 - loss: 0.2850 - val_accuracy: 0.9244 - val_loss: 0.2660

Epoch 41/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8828 - loss: 0.2680 - val_accuracy: 0.9449 - val_loss: 0.2274

Epoch 42/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8695 - loss: 0.2717 - val_accuracy: 0.9227 - val_loss: 0.2616

Epoch 43/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8789 - loss: 0.2609 - val_accuracy: 0.9360 - val_loss: 0.2556

Epoch 44/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8729 - loss: 0.2760 - val_accuracy: 0.9084 - val_loss: 0.2837

Epoch 45/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8789 - loss: 0.2712 - val_accuracy: 0.9307 - val_loss: 0.2457

Epoch 46/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8749 - loss: 0.2614 - val_accuracy: 0.9138 - val_loss: 0.2725

Epoch 47/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8662 - loss: 0.2809 - val_accuracy: 0.9289 - val_loss: 0.2411

Epoch 48/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8852 - loss: 0.2492 - val_accuracy: 0.9262 - val_loss: 0.2653

Epoch 49/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8884 - loss: 0.2497 - val_accuracy: 0.9147 - val_loss: 0.2883

Epoch 50/50

141/141 ━━━━━━━━━━━━━━━━━━━━ 1s 4ms/step - accuracy: 0.8766 - loss: 0.2656 - val_accuracy: 0.9298 - val_loss: 0.2634


**Loss and Accuracy Plot**

<img width="1989" height="790" alt="image" src="https://github.com/user-attachments/assets/2cf8c0ab-1cd3-47bc-a7c5-4b5874f4353d" />

# Confusion Matrix

<img width="519" height="413" alt="image" src="https://github.com/user-attachments/assets/b58fbd5b-82e8-483b-9748-6bc3e3053525" />


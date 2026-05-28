Men Kmeans orqali datani  guruhlarga ajratdim.
Asosiy maqsad datalar bilan ishlash va Kmeans algorithmidan foydalanish. 
Ishni asosiy boshqichlari:
  1- datani yuklash va uni head() orqali birinchi 5 ta obyektni ko'rish.
  2- uni virtual ko'rdim negaki datani ko'rinishini bilish uchun masalan outlier bo'rmikan degan maqsadda.
  3- bo'sh nuqtalar ya'ni missing values lar borligini tekshirdim sababi datada bo'lsa uni algorithmga ko'yish xatolarni keltirib chiqarishi mumkin agarda bo'lganda men KNN imputer yoki boshqa usullar bilan to'ldirgan bo'lar edim lekin bu datada yo'q ekan :)
  4- Gender degan ustunni songa o'tkazdim masalan bo'sh joy bo'lsa uni to'ldirish uchun KNN imputer qilsam ham xato bo'ladi sababi kategoriyali ustunlar bo'lgani uchun ularni Label Encoder bilan songa o'tkazdim.
  5- Normallashtirdim data da agar katta kichik qiymatlarga algorithm turlicha qarashi mumkin masalan 1000000 bilan 45 o'rtasida katta farq bor normallashtirish orqali shu tafovut yo'qoladi.
  6- Kmeans ni ishladitim faqat eng yaxshi K ni topish uchun Elbow dan foydalandim 1 dan to 11 gacha skilda 5 ni oldim.
  7- Elbow Method ni vizualli orqali elbow nuqtani topdim.
  8- Kmeans bilan fit_predict qilib Mijozlarni guruhlarga ajratdim.
  9- Va so'ngi holatdan keyin datani ko'rdim va natijani rasmini Jupyter notebookdan ham va rasmini ham tashlab ko'yaman.
Data ni men  https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python shu yerdan oldim.Datani qo'lda yozmaslik uchun.
Ishlatgan kutubxonalarim va boshqalar:
  Pandas

  Matplotlib

  Scikit-learn va  uning  modullar:

    LabelEncoder

    StandardScaler

    KMeans
  
Project Overview: Customer Segmentation using K-Means

Objective: To perform data analysis and implement the K-Means clustering algorithm.

Main Steps of the Process:

Data Loading: Loaded the dataset and used head() to inspect the first 5 objects.

Data Visualization: Created initial plots to understand the data distribution and check for outliers.

Missing Value Analysis: Checked for missing values to avoid algorithmic errors. No missing values were found; otherwise, methods like KNN Imputer would have been used.

Categorical Encoding: Converted the "Gender" column into numerical values using Label Encoder, as algorithms require numerical input.

Data Normalization: Applied scaling to the data to prevent the algorithm from giving undue weight to larger numerical ranges (e.g., comparing 1,000,000 to 45).

K-Means Implementation: Ran the algorithm for a range of K values (1 to 11) to find the optimal number of clusters.

Elbow Method: Visualized the results to identify the "elbow point," which was determined to be 5.

Clustering: Used fit_predict with K-Means to segment customers into groups.

Final Result: Reviewed the final clustered data and documented the results with images from the Jupyter Notebook.

Dataset Source: Kaggle - Customer Segmentation Tutorial

Libraries and Modules Used:

Pandas

Matplotlib

Scikit-learn:

LabelEncoder

StandardScaler

KMeans

プロジェクト概要：K-means法による顧客セグメンテーション

目的： データの分析およびK-meansクラスタリングアルゴリズムの実装。

主な手順：

データの読み込み： データセットを読み込み、head()を使用して最初の5つのオブジェクトを確認しました。

データの可視化： データの分布を把握し、外れ値（outlier）を確認するために初期プロットを作成しました。

欠損値の確認： アルゴリズムの欠損値によるエラーを避けるため、欠損値を確認しました。今回のデータには欠損値はありませんでしたが、もしあればKNN Imputerなどの手法で補完する予定でした。

カテゴリ変数のエンコーディング： アルゴリズムは数値を必要とするため、Label Encoderを使用して「性別（Gender）」列を数値に変換しました。

データの正規化（スケーリング）： アルゴリズムが大きな数値（例：1,000,000）を小さな数値（例：45）よりも重要視しすぎないよう、StandardScalerでスケーリングを行いました。

K-meansの実装： 最適なクラスタ数を探るため、Kの値を1から11の範囲でアルゴリズムを実行しました。

エルボー法（Elbow Method）： 結果を可視化し、最適なクラスタ数（エルボーポイント）が5であることを特定しました。

クラスタリング： K-meansのfit_predictを使用して、顧客をグループに分類しました。

最終結果の確認： 分類された最終データを確認し、Jupyter Notebookの結果と画像を保存しました。

データセットの出典： Kaggle - Customer Segmentation Tutorial

使用したライブラリとモジュール：

Pandas

Matplotlib

Scikit-learn:

LabelEncoder

StandardScaler

KMeans

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

age_data = {
    'Age Group': ['0-14','15-24','25-34','35-44',
                  '45-54','55-64','65-74','75-84','85+'],
    'Population (M)': [1900, 1200, 1170, 1060,
                        880,  720,  510,  260,  90]
}
gender_data = {
    'Gender': ['Male', 'Female'],
    'Population (M)': [3980, 3920]
}

df_age    = pd.DataFrame(age_data)
df_gender = pd.DataFrame(gender_data)


plt.figure(figsize=(10, 5))
sns.barplot(data=df_age, x='Age Group', y='Population (M)',
            palette='Greens_d')
plt.title('World Population by Age Group (2022)')
plt.xlabel('Age Group')
plt.ylabel('Population (millions)')
plt.tight_layout()
plt.savefig('age_distribution.png', dpi=150)
plt.show()

plt.figure(figsize=(6, 5))
sns.barplot(data=df_gender, x='Gender', y='Population (M)',
            palette=['#3266ad', '#D4537E'])
plt.title('World Population by Gender (2022)')
plt.xlabel('Gender')
plt.ylabel('Population (millions)')
plt.tight_layout()
plt.savefig('gender_distribution.png', dpi=150)
plt.show()


print(df_age.describe())
print(df_gender)
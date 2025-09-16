# IA simple pour conseiller un agriculteur selon la météo

def conseil_agricole(meteo):
    if meteo.lower() == "soleil":
        return "Il fait beau ☀️ : profitez-en pour arroser vos cultures tôt le matin."
    elif meteo.lower() == "pluie":
        return "Il pleut 🌧️ : pas besoin d'arroser aujourd'hui."
    elif meteo.lower() == "nuage":
        return "Temps nuageux ☁️ : vous pouvez semer ou entretenir vos champs."
    elif meteo.lower() == "vent":
        return "Attention au vent 🌬️ : protégez vos jeunes plants fragiles."
    else:
        return "Météo inconnue 🤔 : observez vos cultures avant de décider."

# Exemple d'utilisation
print("=== Conseiller Agricole Intelligent ===")
temps = input("Entrez la météo du jour (soleil/pluie/nuage/vent) : ")
print(conseil_agricole(temps))

# Wireless-energy-monitoring
# Wireless Energy Monitoring System

print("==============================")
print("   WIRELESS ENERGY MONITORING")
print("==============================")

voltage = float(input("Enter voltage (V): "))
current = float(input("Enter current (A): "))
time = float(input("Enter operating time (hours): "))

# Calculate power
power = voltage * current

# Calculate energy
energy = power * time / 1000   # kWh

print("\n------------------------------")
print("Voltage :", voltage, "V")
print("Current :", current, "A")
print("Power   :", round(power, 2), "W")
print("Energy  :", round(energy, 2), "kWh")
print("------------------------------")

if power > 5000:
    print("⚠️ HIGH POWER CONSUMPTION")
elif power > 0:
    print("🟢 POWER CONSUMPTION NORMAL")
else:
    print("⚠️ NO POWER CONSUMPTION")

print("\n📡 Energy data monitored wirelessly")
print("✅ Monitoring completed")

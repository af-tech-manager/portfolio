#!/bin/bash

echo "# 🧠 Nível de Conhecimento – Alan Fernandes" > conhecimentos.md
echo "" >> conhecimentos.md

declare -A linguagens=(
  ["Python"]="🔵🔵🔵🔵⚪"
  ["Java"]="🔵🔵🔵⚪⚪"
  ["JavaScript"]="🔵🔵🔵🔵⚪"
  ["TypeScript"]="🔵🔵🔵⚪⚪"
  ["SQL"]="🔵🔵🔵🔵⚪"
  ["Shell Script"]="🔵🔵⚪⚪⚪"
)

for lang in "${!linguagens[@]}"; do
  echo "- **$lang**: ${linguagens[$lang]}" >> conhecimentos.md
done

echo "" >> conhecimentos.md
echo "_Gerado em: $(date)_"

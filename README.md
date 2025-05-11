import streamlit as st

st.title("Mentor IA: Guia do Influencer Digital")

menu = st.sidebar.selectbox("Escolha uma área", ["Início", "Ideias de Conteúdo", "Dicas de Crescimento", "Parcerias", "Plano Semanal"])

if menu == "Início":
    st.subheader("Bem-vindo ao Mentor IA!")
    st.write("Esta IA vai te guiar na jornada para se tornar um influenciador digital. Use o menu ao lado para navegar.")
    
elif menu == "Ideias de Conteúdo":
    nicho = st.selectbox("Qual seu nicho?", ["Moda", "Fitness", "Comédia", "Educação", "Tecnologia"])
    st.write(f"Ideias para o nicho **{nicho}**:")
    if nicho == "Moda":
        st.write("- Look do dia\n- Transformações de estilo\n- Dicas de peças baratas com visual caro")
    elif nicho == "Fitness":
        st.write("- Rotinas de treino\n- Antes e depois\n- Refeições saudáveis")
    # (continue para os outros nichos...)

elif menu == "Dicas de Crescimento":
    st.subheader("5 Dicas para crescer:")
    dicas = [
        "Poste consistentemente (3-5x por semana).",
        "Use hashtags estratégicas (# do seu nicho).",
        "Interaja com seu público (responda comentários, enquetes).",
        "Colabore com outros criadores.",
        "Use vídeos curtos (Reels, TikTok, Shorts)."
    ]
    for dica in dicas:
        st.write(f"- {dica}")

elif menu == "Parcerias":
    st.subheader("Como conseguir parcerias:")
    st.write("""
    1. Tenha um mídia kit simples (bio, números, engajamento).
    2. Comece marcando marcas que você já usa.
    3. Envie mensagens diretas para pequenas marcas locais.
    4. Cumpra prazos e entregue conteúdo com qualidade.
    """)

elif menu == "Plano Semanal":
    st.subheader("Plano de Conteúdo Semanal:")
    st.write("""
    - Segunda: Dica rápida + Enquete
    - Terça: Bastidores ou rotina
    - Quarta: Colaboração ou repost
    - Quinta: Conteúdo educativo ou tendência
    - Sexta: Vídeo divertido ou pessoal
    """)# Radija
,

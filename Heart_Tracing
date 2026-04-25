import streamlit as st
import numpy as np
import plotly.graph_objects as go
import time

st.set_page_config(page_title="For My Love", page_icon="❤️")
st.markdown("<style>.stApp {background-color: #FFF0F5;}</style>", unsafe_allow_html=True)

st.title("❤️ MY LOVE FOR YOU IN MATH ❤️")
st.subheader("To the MAN I adore the most")

t = np.linspace(0, 2 * np.pi, 150)
x_all = 16 * np.sin(t)**3
y_all = 13 * np.cos(t) - 5 * np.cos(2*t) - 2 * np.cos(3*t) - np.cos(4*t)

plot_placeholder = st.empty()

for i in range(1, len(t) + 1):
    fig = go.Figure()
    fig.add_trace(go.Scatter(x=x_all[:i], y=y_all[:i], mode='lines', line=dict(color='#E60000', width=5)))
    fig.update_layout(
        xaxis=dict(range=[-20, 20], gridcolor='white', zerolinecolor='black'),
        yaxis=dict(range=[-18, 15], gridcolor='white', zerolinecolor='black'),
        plot_bgcolor='rgba(0,0,0,0)', paper_bgcolor='rgba(0,0,0,0)', showlegend=False, height=550
    )
    plot_placeholder.plotly_chart(fig, use_container_width=True)
    time.sleep(0.02)

fig.add_trace(go.Scatter(x=x_all, y=y_all, fill='toself', fillcolor='rgba(230, 0, 0, 0.3)', line=dict(color='#E60000', width=5)))
plot_placeholder.plotly_chart(fig, use_container_width=True)

st.markdown("<h2 style='text-align: center; color: #E60000; font-family: Serif;'>Justiee, I love you. Very much.</h2>", unsafe_allow_html=True)

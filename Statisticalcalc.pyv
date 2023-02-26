import streamlit as st
import statistics

def calculate_statistics(numbers):
    mean = statistics.mean(numbers)
    median = statistics.median(numbers)
    stdev = statistics.stdev(numbers)
    return mean, median, stdev

st.title("Statistical Calculator")

numbers_str = st.text_input("Enter a list of numbers separated by commas:")
numbers = [float(x.strip()) for x in numbers_str.split(",") if x.strip()]

if numbers:
    mean, median, stdev = calculate_statistics(numbers)
    st.write(f"Mean: {mean}")
    st.write(f"Median: {median}")
    st.write(f"Standard Deviation: {stdev}")

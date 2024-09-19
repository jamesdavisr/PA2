# PROGRAMMING ASSIGNMENT 2 NUMERICAL PYTHON (NUMPY)
I. Intended Learning Outcomes:
1. To identify the codes and functions incorporated in the Numpy library
2. To be able to apply and use the different codes and functions in creating a Python program using a Numpy library

NORMALIZATION PROBLEM: Normalization is one of the most basic preprocessing techniques in data analytics. This involves centering and scaling process. Centering means subtracting the data from the mean and scaling means dividing with its standard deviation. Mathematically, normalization can be expressed as:
𝑍 = 𝑋 − 𝑥̅ / 𝜎

In Python, element-wise mean and element-wise standard deviation can be obtained by using .mean() and.std() calls.

In this problem, create a random 5 x 5 ndarray and store it to variable X. Normalize X. Save your normalized ndarray as X_normalized.npy

# NORMALIZATION PROBLEM

{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 1,
   "id": "f3220bc9",
   "metadata": {},
   "outputs": [],
   "source": [
    "#NORMALIZED PROBLEM\n",
    "\n",
    "import numpy as np\n",
    "X = np.random.rand(5, 5)\n",
    "\n",
    "mean = X.mean()\n",
    "std_dev = X.std()\n",
    "\n",
    "X_normalized = (X - mean) / std_dev"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "id": "cbef5ac9",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Original Array (X):\n",
      "[[0.00411866 0.64816877 0.91897708 0.56650679 0.12079018]\n",
      " [0.8976535  0.63720801 0.20529843 0.93954409 0.35924264]\n",
      " [0.95412769 0.09665562 0.35435389 0.57247636 0.0270656 ]\n",
      " [0.62687397 0.66420006 0.29836838 0.39638687 0.82170391]\n",
      " [0.0829718  0.51292456 0.90007428 0.06841406 0.01847412]]\n"
     ]
    }
   ],
   "source": [
    "print(\"Original Array (X):\")\n",
    "print(X)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "id": "2c05d9b0",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "\n",
      "Normalized Array (X_normalized):\n",
      "[[-1.43431242  0.55835353  1.39622388  0.30569454 -1.07333527]\n",
      " [ 1.33024955  0.52444137 -0.81187004  1.45985743 -0.33557266]\n",
      " [ 1.50497851 -1.14800666 -0.35069827  0.32416417 -1.36331549]\n",
      " [ 0.49246823  0.6079537  -0.52391525 -0.22064988  1.0952645 ]\n",
      " [-1.19034389  0.13991321  1.33773936 -1.23538497 -1.38989719]]\n"
     ]
    }
   ],
   "source": [
    "print(\"\\nNormalized Array (X_normalized):\")\n",
    "print(X_normalized)"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.11.4"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}

# Tracking & Temporal Logic

---

## Motivation

Frame-by-frame recognition is unstable in real-world scenarios.

---

## Proposed Approach

### 1. Temporal Buffer

- Store embeddings from last 5 frames  
- Average them to reduce noise  

---

### 2. Temporal Voting (N = 8)

- Identity is confirmed only after consistent prediction across 8 frames  

---

### 3. Confidence Margin

- Compare top-1 and top-2 similarity scores  
- Accept only if difference is sufficient  

---

### 4. Identity Locking

- Once identity is stable, it is fixed  
- Prevents switching  

---

### 5. EMA Update

- Update embeddings using exponential moving average  
- α = 0.12  

---

## Result

Improved stability and reduced identity switching.

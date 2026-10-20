# CloudMargin 2.0

An interactive, synthetic-data infrastructure finance lab built with Next.js and designed for Vercel deployment.

## Deploy to Vercel

1. Extract this ZIP.
2. Upload the project folder to a GitHub repository (or import via Vercel's supported project upload workflow).
3. In the Vercel dashboard, choose **Add New > Project**, import the repository, and deploy. Vercel detects Next.js automatically.
4. No environment variables, database, or paid AI credits are required.

## Run locally (optional)

Requires Node.js 20 or later.

```bash
npm install
npm run dev
```

Open http://localhost:3000.

## Model

- `data/usage.json`: 2,160 synthetic records (60 customers × 3 workloads × 12 months).
- `data/analysis.json`: original Python-exported analytical snapshot, retained for reference.
- `app/page.jsx`: interactive FP&A, optimization, and build-vs-buy calculations.
- `app/globals.css`: responsive dashboard styling.

Changing the month, segment, or workload recomputes calculations from underlying records. Cache effectiveness, implementation costs, and investment horizon are user-adjustable assumptions. The app does not claim to model Vercel's real finances. Savings assume monthly opportunity remains constant; the comparison is undiscounted.

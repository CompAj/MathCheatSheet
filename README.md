# \documentclass[10pt,twocolumn]{article}
\usepackage[utf8]{inputenc} % for UTF-8 input
\usepackage[T1]{fontenc}
\usepackage[margin=0.5in]{geometry} % reduce page margins
\usepackage{amsmath, amssymb}
\usepackage{textcomp}
\usepackage{enumitem} % for compact lists
\setlist{nosep} % remove extra space in lists
\linespread{0.95} % reduce line spacing slightly

\begin{document}

\section*{Estimation}

\begin{itemize}
    \item We often want to know more about a population, but we can't obtain data on the entire population.
    \item So, we instead obtain data from a sample of the population.
    \item We can use the sample data to estimate properties/characteristics of the population.
    \item E.g.: use the sample mean \(\overline{x}\) to estimate the population mean \(\mu\).
    \item E.g.: use the sample proportion to estimate the population proportion \(p\).
    \item In general, sample statistics (like \(\overline{x}\)) are used to estimate population parameters (like \(\mu\) and \(p\)).
\end{itemize}

\section*{Types of Estimation}

\begin{enumerate}
    \item The value of a sample statistic (like \(\overline{x}\) and \(p\)) that is used to estimate a population parameter (like \(\mu\) and \(p\)) is called a point estimate.
    \item E.g.: the sample mean is a point estimate of the population mean.
    \item In interval estimation, an interval is constructed around the point estimate, and it is stated that this interval contains the corresponding population parameter with a certain ``confidence level'' (more on this later).
\end{enumerate}

\[
\mu_{\overline{x}} = \mu
\]
\[
\overline{x} = 2970
\]

\section*{Confidence Interval}

\begin{itemize}
    \item A confidence interval is an interval, calculated from sample data, that is likely to contain the true population parameter (like the mean or proportion) with a certain level of confidence.
    \item E.g.: a 95\% confidence interval suggests that if we were to take many samples and compute intervals for each, about 95\% of those intervals would contain the true population parameter.
    \item Confidence intervals provide an estimate along with a margin of error, reflecting the uncertainty inherent in sampling.
    \item The wider the interval, the more uncertainty.
\end{itemize}

The narrower the interval, the more precise the estimate.

\section*{Confidence Interval Example}

\begin{itemize}
    \item Example: I want to estimate the average monthly income of a UofS student, so I randomly sample UofS students and ask them about their monthly income.
    \item I get a point estimate of \(\overline{x}=2970\) and I create a 95\% confidence interval that ranges from \$2630 to \$3310.
    \item The confidence interval represents the uncertainty in my estimate, since it comes from a sample!
    \item We will discuss how to create confidence intervals next.
\end{itemize}

\[
\mu_{\overline{x}} = \mu
\]
\[
\overline{x} = 2970
\]

\section*{Estimation of a Population Mean \(\mu\)}

\begin{itemize}
    \item The point estimate for the population mean will always be the sample mean \(\overline{x}\).
    \item The creation of a confidence interval for the population mean will depend on your scenario.
\end{itemize}

\textbf{Scenario 1:} The population standard deviation \(\sigma\) is \textbf{KNOWN} and either \(n\ge 30\) or the population is approximately normal.

\textbf{Scenario 2:} The population standard deviation \(\sigma\) is \textbf{NOT KNOWN} and either \(n\ge 30\) or the population is approximately normal.

\section*{Scenario 1: \(\sigma\) is KNOWN}

\begin{itemize}
    \item The \((1-\alpha)100\%\) confidence interval for \(\mu\) is
\end{itemize}

\[
\overline{x} \pm z_{\alpha/2}\frac{\sigma}{\sqrt{n}}
\]

where \(z_{\alpha/2}\) is the z-value that gives each tail a probability of \(\alpha/2\). Here, \(\alpha\) is called the ``significance level.''

\begin{itemize}
    \item Common values for \(\alpha\) are 0.1, 0.05, and 0.01.
\end{itemize}

The term
\[
z_{\alpha/2}\frac{\sigma}{\sqrt{n}}
\]
is called the margin of error.

\section*{Z-values for Commonly Used Confidence Levels}

\begin{tabular}{|c|c|c|c|}
\hline
Confidence Level & \(\alpha\) & \(\alpha/2\) & \(z_{\alpha/2}\) \\
\hline
90\% & 0.1 & 0.05 & 1.65 \\
\hline
95\% & 0.05 & 0.025 & 1.96 \\
\hline
96\% & 0.04 & 0.02 & 2.05 \\
\hline
97\% & 0.03 & 0.015 & 2.17 \\
\hline
98\% & 0.02 & 0.01 & 2.33 \\
\hline
99\% & 0.01 & 0.005 & 2.58 \\
\hline
\end{tabular}

\section*{Scenario 1: \(\sigma\) is KNOWN (Example)}

\begin{itemize}
    \item Example: a random sample of 25 statistics textbooks has a mean price of \$205.
    \item It is known that the standard deviation of the prices of all such textbooks is \$47 and the population distribution is approximately normal.
    \item (a) What is the point estimate of the mean price of all such textbooks?
\end{itemize}

The confidence interval is given by

\[
\overline{x} \pm z_{\alpha/2}\frac{\sigma}{\sqrt{n}}
\]

\section*{Scenario 1: \(\sigma\) is KNOWN (Example 2)}

\begin{itemize}
    \item Example: a random sample of 600 households resulted in an average annual streaming cost of \$500, and it is known that the population standard deviation of streaming costs is \$40.
    \item Construct a 99\% confidence interval to estimate the true mean annual streaming cost for all households.
\end{itemize}

\section*{Determining Sample Size}

\begin{itemize}
    \item The width of a confidence interval is called the margin of error (\(E\)).
    \item For estimating \(\mu\), we have:
\end{itemize}

\[
E = z_{\alpha/2}\frac{\sigma}{\sqrt{n}}
\]

Solving for \(n\), we obtain

\[
n = \left(\frac{z_{\alpha/2}\sigma}{E}\right)^2.
\]

\section*{Determining Sample Size (Example)}

\begin{itemize}
    \item Example: an alumni association wants to estimate the mean debt of this year's graduates.
    \item Given a population standard deviation of \$11,800, how large should the sample be to ensure a 99\% confidence level with a margin of error of \$800?
\end{itemize}

\[
n = \left(\frac{z_{\alpha/2}\sigma}{E}\right)^2.
\]

\section*{Estimation of a Population Mean \(\mu\) (Revisited)}

\begin{itemize}
    \item The point estimate for the population mean \(\mu\) is always the sample mean \(\overline{x}\).
    \item The creation of a confidence interval for \(\mu\) depends on your scenario.
\end{itemize}

\begin{itemize}
    \item \textbf{Scenario 1:} The population standard deviation \(\sigma\) is KNOWN and either \(n\ge 30\) or the population is approximately normal.
    \item \textbf{Scenario 2:} The population standard deviation \(\sigma\) is NOT KNOWN and either \(n\ge 30\) or the population is approximately normal.
\end{itemize}

\section*{Scenario 2: \(\sigma\) is NOT KNOWN}

\begin{itemize}
    \item The \((1-\alpha)100\%\) confidence interval for \(\mu\) is
\end{itemize}

\[
\overline{x} \pm t_{\alpha/2,\, n-1}\frac{s}{\sqrt{n}},
\]
where \(t_{\alpha/2,\, n-1}\) is the t-value with \(n-1\) degrees of freedom that gives each tail a probability of \(\alpha/2\).

\section*{Estimation of a Population Proportion \(p\)}

\begin{itemize}
    \item The point estimate of the population proportion \(p\) is the sample proportion \(\hat{p}\).
\end{itemize}

\section*{Confidence Interval for \(p\)}

\begin{itemize}
    \item The \((1-\alpha)100\%\) confidence interval for \(p\) is
\end{itemize}
\[
\hat{p} \pm z_{\alpha/2}\sqrt{\frac{\hat{p}\hat{q}}{n}},
\]
where \(\hat{q} = 1 - \hat{p}\).

\section*{Determining Sample Size for \(p\)}

\begin{itemize}
    \item The margin of error for estimating \(p\) is 
    \[
    E = z_{\alpha/2}\sqrt{\frac{\hat{p}\hat{q}}{n}},
    \]
    \item Solving for \(n\), we obtain
    \begin{equation*}
    n = \left( \frac{z_{\alpha/2}}{E} \right)^2 \hat{p}\hat{q}.
    \end{equation*}
    \item In case \(\hat{p}\) is not available, use \(p = 0.5\) to get a conservative sample size estimate.
\end{itemize}

\end{document}

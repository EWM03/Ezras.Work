# Access Controls on a Mobile Device — Artifact 0.1

<p style="text-indent: 2em;">
  This artifact demonstrates how I applied layered access controls on my personal mobile device to balance security, privacy, and day‑to‑day usability. Because biometric data in the United States lacks strong legal protections and can be compelled or captured without meaningful recourse, I shifted my device’s primary unlock method from biometrics to a password. This increases the difficulty of unauthorized access, especially in public or high‑risk environments.
</p>

<p style="text-indent: 2em;">
  To maintain usability, I enabled the device’s Extend Unlock feature. This feature modifies lock‑screen behavior under defined conditions, either bypassing authentication or changing the required authentication method. The first unlock always requires the primary credential (my password). For the next four hours, the device continuously evaluates whether the conditions for Extend Unlock are still met. When they are, I can use my fingerprint for quick access.
</p>

<p style="text-indent: 2em;">
  I configured these conditions to reflect real‑world access patterns. In certain trusted locations, Extend Unlock requires both my fingerprint and the presence of my smartwatch, which functions as a physical key. In other locations, only the fingerprint is required. These combinations of password, location, and paired device presence effectively operate as conditional access policies on a mobile platform.
</p>

<p style="text-indent: 2em;">
  Together, these controls allow me to access my phone quickly when I need to—such as when looking up information for a customer at work—while still maintaining strong protections against unauthorized access. This artifact illustrates how identity signals, environmental context, and device‑based factors can be combined to create a secure and usable access control strategy.
</p>

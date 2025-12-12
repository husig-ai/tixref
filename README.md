# Next Steps

- Get access S3
- Deploy this to s3 (static)
- Create a formjs account
- Create Email Service (using tixfix email)
- Create Email Template using
```
<div style="font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; max-width: 600px; margin: 0 auto; background-color: #ffffff;">
  <!-- Header with TixFix branding -->
  <div style="background: #05051E; padding: 30px 20px; text-align: center;">
    <div style="color: #ffffff; font-size: 28px; font-weight: 800; margin-bottom: 8px; letter-spacing: -0.5px;">
      tixfix
    </div>
    <div style="color: rgba(255, 255, 255, 0.9); font-size: 16px; font-weight: 600;">
      Referral Rewards
    </div>
  </div>

  <!-- Main content -->
  <div style="padding: 30px 20px; background-color: #ffffff;">
    <div style="text-align: center; margin-bottom: 30px;">
      <div style="font-size: 28px; font-weight: 800; color: #1f2937; margin-bottom: 10px;">
        🎉 Referral Submission Received
      </div>
      <div style="color: #6b7280; font-size: 16px;">
        Thank you for referring an event organizer to TixFix!
      </div>
    </div>

    <!-- Referrer info -->
    <div style="background: linear-gradient(135deg, #f8fafc, #f1f5f9); border-radius: 16px; padding: 25px; margin-bottom: 25px; border-left: 4px solid #4F46E5;">
      <div style="display: flex; align-items: center; margin-bottom: 12px;">
        <div style="margin-right: 12px; font-size: 24px;">
          👤
        </div>
        <div>
          <div style="font-weight: 700; color: #1f2937; font-size: 16px;">{{your_name}}</div>
          <div style="color: #6b7280; font-size: 14px;">{{your_email}}</div>
        </div>
      </div>
    </div>

    <!-- Organizer details -->
    <div style="background: rgba(79, 70, 229, 0.05); border: 2px solid rgba(79, 70, 229, 0.2); border-radius: 16px; padding: 25px; margin-bottom: 25px;">
      <h3 style="color: #1f2937; margin: 0 0 20px 0; font-size: 18px; font-weight: 700; display: flex; align-items: center;">
        <span style="margin-right: 10px; font-size: 20px;">🎯</span>
        Organizer Information
      </h3>
      
      <table style="width: 100%; border-spacing: 0;">
        <tr>
          <td style="padding: 8px 0; color: #6b7280; font-weight: 600; width: 100px; font-size: 14px;">Name:</td>
          <td style="padding: 8px 0; color: #1f2937; font-weight: 500; font-size: 14px;">{{organizer_name}}</td>
        </tr>
        <tr>
          <td style="padding: 8px 0; color: #6b7280; font-weight: 600; font-size: 14px;">Email:</td>
          <td style="padding: 8px 0; color: #1f2937; font-weight: 500; font-size: 14px;">{{organizer_email}}</td>
        </tr>
        <tr>
          <td style="padding: 8px 0; color: #6b7280; font-weight: 600; font-size: 14px;">Phone:</td>
          <td style="padding: 8px 0; color: #1f2937; font-weight: 500; font-size: 14px;">{{phone_number}}</td>
        </tr>
        <tr>
          <td style="padding: 8px 0; color: #6b7280; font-weight: 600; font-size: 14px;">Company:</td>
          <td style="padding: 8px 0; color: #1f2937; font-weight: 500; font-size: 14px;">{{company_name}}</td>
        </tr>
      </table>
    </div>

    <!-- Additional notes (conditional) -->
    <div style="background: rgba(59, 130, 246, 0.05); border-radius: 16px; padding: 20px; margin-bottom: 25px; border-left: 4px solid #3b82f6;">
      <h4 style="color: #1f2937; margin: 0 0 12px 0; font-size: 16px; font-weight: 600; display: flex; align-items: center;">
        <span style="margin-right: 8px; font-size: 16px;">💬</span>
        Additional Notes:
      </h4>
      <div style="color: #4b5563; font-size: 14px; line-height: 1.6;">
        {{additional_notes}}
      </div>
    </div>

    <!-- Reward Information -->
    <div style="background: linear-gradient(135deg, rgba(79, 70, 229, 0.1), rgba(124, 58, 237, 0.1)); border-radius: 16px; padding: 25px; margin-bottom: 25px; border: 1px solid rgba(79, 70, 229, 0.3);">
      <h3 style="color: #4338CA; margin: 0 0 15px 0; font-size: 18px; font-weight: 700; display: flex; align-items: center;">
        <span style="margin-right: 10px; font-size: 20px;">💰</span>
        Your Potential Reward
      </h3>
      <div style="color: #374151; font-size: 14px; line-height: 1.6;">
        <strong style="color: #1f2937;">$100 Amazon Gift Card</strong> when {{organizer_name}} completes their first 3 events with 50+ tickets each.
      </div>
    </div>

    <!-- Next steps -->
    <div style="background: linear-gradient(135deg, #ecfdf5, #f0fdf4); border-radius: 16px; padding: 25px; border: 1px solid #d1fae5;">
      <h3 style="color: #065f46; margin: 0 0 15px 0; font-size: 18px; font-weight: 700; display: flex; align-items: center;">
        <span style="margin-right: 10px; font-size: 20px;">⚡</span>
        What happens next?
      </h3>
      <div style="color: #047857; font-size: 14px; line-height: 1.6;">
        Our team will contact <strong>{{organizer_name}}</strong> within 24 hours to begin the onboarding process. We'll keep you updated on your referral progress and notify you when rewards become available.
      </div>
    </div>
  </div>

  <!-- Footer -->
  <div style="background: #05051E; padding: 20px; text-align: center;">
    <div style="color: rgba(255, 255, 255, 0.7); font-size: 12px; margin-bottom: 8px;">
      This confirmation was sent via the TixFix Referral Rewards Program
    </div>
    <div style="color: rgba(255, 255, 255, 0.5); font-size: 11px;">
      2025 TixFix, LLC. San Francisco, CA. All Rights Reserved.
    </div>
  </div>
</div>

<!-- Dark mode styles for supported email clients -->
<style>
  @media (prefers-color-scheme: dark) {
    .email-container {
      background-color: #1f2937 !important;
    }
    .email-content {
      background-color: #1f2937 !important;
      color: #f9fafb !important;
    }
    .email-text {
      color: #d1d5db !important;
    }
    .email-title {
      color: #f9fafb !important;
    }
  }
</style>
```
- Create Supabase account
- Collect the following keys:
- `service_key` and `template_key` from emailjs
- `url` and `publishable_key` from supabase


```
-- Supabase Table Schema
-- Run this in your Supabase SQL editor

CREATE TABLE contacts (
    id BIGSERIAL PRIMARY KEY,
    your_name TEXT NOT NULL,
    your_email TEXT NOT NULL,
    organizer_name TEXT NOT NULL,
    organizer_email TEXT NOT NULL,
    phone_number TEXT,
    company_name TEXT NOT NULL,
    additional_notes TEXT,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Optional: Enable Row Level Security
ALTER TABLE contacts ENABLE ROW LEVEL SECURITY;

-- Optional: Create a policy to allow inserts from anyone
CREATE POLICY "Enable insert for all users" ON "public"."contacts" 
FOR INSERT WITH CHECK (true);

-- Optional: Create a policy to allow reading (if you need it for admin dashboard later)
CREATE POLICY "Enable read access for all users" ON "public"."contacts" 
FOR SELECT USING (true);
```

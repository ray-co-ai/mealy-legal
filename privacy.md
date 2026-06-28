---
title: Privacy Policy
permalink: /privacy/
---

# Privacy Policy

**Effective date:** 2026-06-28
**Last updated:** 2026-06-28

This Privacy Policy explains what information the **Mealy** mobile app ("Mealy", "we", "us") collects, how we use it, and the choices you have. Mealy is operated as a personal project by the developer reachable at <mealy.support@gmail.com>.

If you have any question about this policy, email us at <mealy.support@gmail.com>.

## What we collect

We only collect information you give us directly through the app, plus the minimum needed for authentication and to make the features work.

**Account information.** Email address (when you sign in by email or magic link). Mealy also supports Sign in with Apple, in which case Apple may share a relay email instead of your real address.

**Profile information you provide.** Name, language preference, units, locale, weight goal and weight-journey entries, height, body fat, waist, daily water target, dietary preferences, cooking effort, meal-planning preferences, and other fields you choose to fill in on the You tab and during onboarding.

**Food and activity log.** Meals you log (name, ingredients, kcal and macro estimates, meal time, meal context), workouts you record, water intake, weight entries, meal feelings and notes, saved go-to meals, saved menus, and your user-created recipes.

**Photos and voice.** If you log a meal by photo, the photo is uploaded for AI analysis. If you log by voice, the audio is transcribed. We do not retain raw photos or voice recordings beyond the time needed to produce the structured log entry.

**Chat messages.** Messages you send to the Mealy guide chat, the assistant's replies, and chat usage counts for tier limits.

**Device-only preferences.** Some UI preferences (locale prefs, water-intake-by-day cache, weight cache, custom menus, go-to meals) are stored on your device using AsyncStorage and are not sent to our servers unless cloud sync is enabled by signing in.

**Technical information.** Standard logs that any modern app produces (request timestamps, error traces). We do not use third-party analytics or advertising SDKs and do not track you across other apps or websites.

## How we use the information

- Run the features you asked for (saving meals, showing history, building plans, answering chat questions).
- Personalize the experience (Hebrew/English language, units, gender grammar for Hebrew, dietary preferences).
- Maintain your account (sign-in, account recovery, account deletion).
- Improve the app (debugging from non-personal error logs).

We do **not** sell your data. We do **not** share it with advertisers. We do **not** use your content to train third-party AI models for purposes other than answering your own request.

## How AI requests work

Mealy's chat assistant and food-recognition features call **Google Gemini** (and, depending on configuration, **OpenAI**) through a small server-side proxy we run on Supabase Edge Functions. Your message, any attached photo, and the relevant context for that request are sent to the AI provider so it can produce a reply. Provider privacy policies:

- Google AI / Gemini: <https://ai.google.dev/gemini-api/terms> and <https://policies.google.com/privacy>
- OpenAI: <https://openai.com/policies/privacy-policy/>

The provider key is held server-side and is never embedded in the app binary. Requests are made over HTTPS.

## How long we keep your data

- Profile, food log, workout log, water, weight history, saved meals, saved menus, user recipes, shopping list, and chat threads are kept for as long as your account is active.
- When you delete your account from inside the app (You tab → Delete account), all of the above is removed from our database. This is a one-tap, irreversible action handled by a server-side function and typically completes within seconds.
- Server error logs are retained for up to 30 days for debugging.

## Your rights and choices

- **See your data.** Most of it is visible inside the app (history, profile, saved items). For anything else, email us.
- **Correct your data.** Edit profile fields from the You tab; edit a logged meal from history.
- **Delete your account and data.** You tab → Delete account. You can also email us if the in-app flow fails for any reason.
- **Decline AI features.** Mealy still works for manual food logging if you avoid the chat and photo / voice logging features.

If you are in the EU, the UK, or California, you have additional rights under the GDPR, UK GDPR, and CCPA respectively (access, rectification, erasure, portability, objection). To exercise them, email us; we will respond within 30 days.

## Security

We use Supabase (Postgres + Auth) with row-level security policies that restrict each row to its owning user via `auth.uid()`. Network traffic is HTTPS. We never store provider API keys on your device.

No system is perfectly secure. If you believe your account has been compromised, change your password and email us.

## Children

Mealy is not directed to children under 13 (or under 16 in the EU). Do not use Mealy or create an account if you are below the applicable age.

## Health and medical disclaimer

Mealy provides general nutrition and wellness information. It is **not medical advice** and is not a substitute for professional medical care. Consult a qualified clinician for any health-related decisions, especially if you are pregnant, nursing, have a medical condition, or are taking medication.

## Changes to this policy

We may update this policy from time to time. Material changes will be shown in the app or noted at the top of this page with a new "Last updated" date.

## Contact

Questions, requests, or complaints: <mealy.support@gmail.com>.

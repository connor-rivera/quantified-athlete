# Study 02: Polarized training and easy pace

Written: November 2026, about 4 weeks after data collection started and
before any analysis. Baseline: drift test on Oct 19, 2026. Data: Oct 20, 2026 on.

## Question

If most of my running is easy, does my easy pace get faster at the same
heart rate over time?

## Design

This study only looks forward. It starts with a drift test on Oct 19, 2026,
after which I lowered my easy heart rate cap from 148 to 145 bpm. Runs from
Oct 20 on are included. I don't compare against older runs because they
weren't run with an easy intent, few of them were in my easy heart rate
range, and a Hyrox block and summer heat affected them. This design can
show whether my easy pace improves, but not prove that polarized training
caused it.

## Primary outcome

Average pace of the easy laps of runs that average 135–145 bpm. The band
only changes after a drift test, and any change is recorded here with
its date.

## Secondary outcomes

- Drift test about every 8 weeks, on the Sunday of a lighter week (next:
  Dec 6, 2026). Baseline: miles 2–3 at 8:24/mi and 145 bpm; heart rate
  rose 4.1% in miles 4–6; decoupling about 5.1%.
- Also tracked, not tested: Garmin VO2 max, 7-day resting heart rate, and
  the share of my running that is easy.

## Exploratory questions

These are interesting to me, but they aren't part of the main test:

- Did my easy pace change after I raised my cadence on Nov 6, 2026
  (about 162 to 170 steps per minute)?
- What happens to my easy pace during the Hyrox training block
  (from about Jan 3, 2027, race on Feb 28, 2027)?

## Which runs count

- Included: outdoor runs of at least 3 miles. Only easy laps count; strides,
  walk breaks and stops are dropped. Pace uses Garmin's moving time, so
  pauses and time standing still don't count.
- Excluded: treadmill runs (pace from the wrist isn't reliable), group runs,
  quality sessions, runs with a fast finish, and runs within 2 days after a
  race.
- Flagged: runs the day after a quality session or drift test. They count,
  but I also run the analysis without them.

## Hypothesis

My pace at 135–145 bpm gets faster over time after adjusting for weather
and distance. If the time trend is flat or slower after those adjustments,
the hypothesis isn't supported.

## Analysis plan

- Main model: pace ~ time + temperature + dew point + distance. Weather
  comes from Garmin's activity weather.
- Sensitivity checks: (1) only runs between 40 and 65°F; (2) without
  the flagged runs.
- I store elevation gain for every run to spot unusual routes.

## Timeline

- Preliminary look: mid-January 2027 (about 12 weeks of data).
- Main conclusion: after spring warming (April–May 2027). In autumn, time
  and temperature change together, so the two are hard to separate until
  the weather warms up again.

## Limitations

- n = 1: this is one person, so the results may not apply to anyone else.
- No control: there's no comparison period or group, so I can see whether
  my easy pace improves but can't prove polarized training caused it.
- Season: the study starts in autumn, so time and temperature move
  together. The weather adjustment and the spring data are meant to
  handle this, but they may not fully separate the two.
- Device data: heart rate comes from the wrist sensor, which can drop out
  or read low for the first few minutes. Pace comes from GPS, and weather
  comes from a nearby station, not from where I ran.
- Steered heart rate: I run easy runs to stay at or under 145 bpm on
  average, so my easy heart rates are bunched just under the cap rather
  than spread out naturally.
- Timing: I wrote this after about 4 weeks of data collection, though
  before any analysis.

## Amendments

- Nov 17, 2026: Added the Limitations section after the `prereg-02` tag.
  Nothing else changed: the question, outcomes, run rules and analysis
  plan are the same.

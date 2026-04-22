# frc-logs

Post-match telemetry dashboard for [StuyPulse](https://stuypulse.com) FRC robots. Drop a `.wpilog` file from the robot onto the page to visualize match data — superstructure states, vision quality, power budget, swerve performance, and more.

## Usage

Open `index.html` directly in a browser (no build step, no server needed), or visit the hosted version on GitHub Pages. Drag and drop a `.wpilog` file from the RoboRIO onto the drop zone.

Logs are processed entirely in-browser — no data is uploaded anywhere.

## Compatibility

Built for **StuyPulse Tribecbot** (2026, FRC game: *Rebuilt*), logging via [DogLog](https://doglog.dev). The parser handles WPILib `.wpilog` format including `Pose2d` struct decoding.

## Credits

Dashboard architecture and design adapted from [tempest-dashboard](https://github.com/brunoUC/tempest-dashboard) by brunoUC / UC Robotics — a post-match analysis tool for AdvantageKit logs. Key adaptations: DogLog key tree, WPILib struct record parsing, and Tribecbot-specific subsystem tabs.

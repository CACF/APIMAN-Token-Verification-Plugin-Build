# Keycloak Token Verification
Plugin for APIMAN that verifies an active user session against the provided token in keycloak.


# Installation
1. Login to APIMAN UI
2. Open to Manage Plugins from System Administration section
3. Open Available Plugins tab 
4. Click Add Custom Plugin
5. Enter Group Id "io.github.cacf"
6. Enter Artifact Id "apiman-plugins-keycloak-token-verification-policy"
7. Enter Version "1.0.0-FINAL"
8. Now click Add Plugin

# Configuration

1. Open Policies in your API
2. Add policy
3. Select 'Keycloak Token Verification' from Policy Type drop down and Add Policy
4. Add following to policy's JSON configuration

`{
"userInfoUrl": "{keycloak-base-url}/auth/realms/{realm-name}/protocol/openid-connect/userinfo"
}`

Make sure to update {keycloak-base-url} and {realm-name}

5. Add Policy and move this policy to top

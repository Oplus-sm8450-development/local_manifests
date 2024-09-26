Installing Repo

        git clone https://github.com/Oplus-sm8450-development/local_manifests.git -b a14 .repo/local_manifests/
        
sync repo

        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --depth=1

you should run this to fix boot problem on oplus sm8450 devices!!!

        bash <(rm -r hardware/qcom-caf/sm8450/audio/agm && rm -r hardware/qcom-caf/sm8450/display && git clone https://github.com/Oplus-sm8450-development/hardware_qcom-caf_sm8450_audio_agm.git hardware/qcom-caf/sm8450/audio/agm && git clone https://github.com/Oplus-sm8450-development/hardware_qcom-caf_sm8450_display.git hardware/qcom-caf/sm8450/display)

Signing builds:

        bash <(curl -Ls https://raw.githubusercontent.com/ATI-labs/local-manifests/sign/sign.sh)

for oneplus 10pro


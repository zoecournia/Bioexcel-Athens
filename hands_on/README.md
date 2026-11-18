---
title: Hands-on workshop — participant setup
---

# Hands-on workshop: participant setup

[← Back to the workshop programme](../)

**Please set up and test the workshop virtual machine (VM) before the workshop, whether you are joining in person or online.** The VM download is large, so please do not leave it until the first session.

**[Download the illustrated instructions for participants (PDF)](Instructions_bioexcel.pdf)**

The essential setup steps are also reproduced below.

## Requirements

- At least **25 GB of free disk space** during installation.
- At least **8 GB of RAM** is recommended.
- A computer with Intel/AMD (x86) or Apple silicon (ARM64), and enough time to download the workshop VM.

## 1. Identify your processor

- **Apple silicon Mac:** In Apple menu → About This Mac, if it says *Chip* followed by an Apple chip name, choose **ARM64**.
- **Intel Mac:** If *About This Mac* shows an Intel *Processor*, choose **x86**.
- **Windows or Linux (Intel or AMD):** Choose **x86**.

## 2. Install VirtualBox

Install VirtualBox from the **[official VirtualBox downloads page](https://www.virtualbox.org/wiki/Downloads)** for your operating system.

- **Mac:** If macOS blocks installation, check System Settings → Privacy & Security for a way to approve the installer.
- **Windows:** Open Task Manager → Performance → CPU and verify that *Virtualization* is enabled. If disabled, your BIOS/UEFI settings may need changing.

## 3. Download the workshop VM

Use the **[workshop VM download page](http://snf-35327.ok-kno.grnetcloud.net/BioExcelTraining/)** supplied in the participant handout. Choose **one** of these files:

| File | Computer |
|---|---|
| `DebianTrain_x86.ova` | Windows/Linux with Intel or AMD processors; Intel Macs |
| `DebianTrainARM64.ova` | Apple silicon Macs |

**Download security:** The original handout mentions that browsers may display an expired-certificate warning for the VM host. If you see a certificate or connection-security warning, contact the organisers to verify a safe download method instead of bypassing the warning without verification.

## 4. Import into VirtualBox

1. Open VirtualBox Manager.
2. Select **Home → Import** (or the equivalent *Import Appliance* menu option in your version).
3. Select the `.ova` file you downloaded.
4. Review settings, click **Finish**, and allow the import to complete.
5. After the import finishes, you can delete the downloaded `.ova` file to reclaim disk space.

## 5. Start the VM

Select the imported virtual machine, then click the green **Start** button.

The username and password provided by the workshop organisers are both `user`.

## Useful tips

- **Release the mouse:** Right `Ctrl` on Windows/Linux or left `Command` on Mac.
- **Enable copy and paste:** In the running VM, choose Devices → Shared Clipboard → Bidirectional.
- **Paste into the VM terminal:** `Ctrl` + `Shift` + `V`.
- **Open a terminal:** Click the black terminal icon in the VM dock.
- **Adjust display scaling on high-resolution monitors:** In the VM window, open the **View** menu in the upper-left corner, select **Virtual Screen 1**, and choose the desired scaling percentage. For example, **200%** may provide a more comfortable view on a high-resolution display.

## Workshop materials on Zenodo

The workshop materials will be collected and archived on Zenodo.

**[Workshop materials on Zenodo](https://zenodo.org/records/24335122)** (available once the record is published and the files are made public).

## Hands-on tutorials

Tutorial materials and setup instructions are provided below as they become available.

### GROMACS — introductory molecular dynamics tutorial

Open a terminal in the workshop virtual machine and run the following commands to download and extract the GROMACS tutorial materials:

```bash
cd ~
wget https://gitlab.com/gromacs/online-tutorials/md-intro-tutorial/-/archive/main/md-intro-tutorial-main.zip
unzip md-intro-tutorial-main.zip
```

### VIAMD — download and installation

- **macOS and Windows:** Precompiled binaries are available from the [VIAMD v0.1.50 release page](https://github.com/scanberg/viamd/releases/tag/v0.1.50).
- **Linux:** Follow the [VIAMD build and installation instructions](https://github.com/scanberg/viamd/wiki/0.-Building).

We will eventually use dataset available [here](https://drive.google.com/drive/folders/1ai3KklE8DbkB2q_ftitfIb2oGiIuhT_Z?usp=sharing)

### HADDOCK — tutorial

- [HADDOCK tutorial: Modelling the RNA polymerase III complex using cross-links and starting conformations fitted into the cryo-EM map](https://www.bonvinlab.org/education/HADDOCK24/RNA-Pol-III/#modelling-the-complex-by-docking-with-cross-links-only-using-as-starting-conformations-the-models-fitted-into-the-cryo-em-map)
- [HADDOCK3 tutorial: Modelling an antibody-antigen complex (Google Colab notebook)](https://colab.research.google.com/github/haddocking/haddock3/blob/main/notebooks/HADDOCK3-antibody-antigen.ipynb#scrollTo=Rh-vaM_9woqM): this notebook runs in your web browser on Google Colab, so you need a Google account. It installs HADDOCK3 and downloads the tutorial data itself, so you do not need the VM for it.

## After the workshop

Save any work you want to keep outside the VM, then shut it down. In VirtualBox Manager, select the VM and choose **Machine → Remove → Delete All Files** to reclaim disk space once you are sure you no longer need it.

## Help

If you encounter setup problems before the workshop, contact the organisers at **[zcournia \[at\] bioacademy.gr](mailto:zcournia@bioacademy.gr)**.

[← Back to the workshop programme](../)

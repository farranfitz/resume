var socialIcons, offset, bottomSocialIcons

    socialIcons = document.querySelector('.contact-icons')
    bottomSocialIcons = document.querySelector('.sticky-footer')
    offset = socialIcons.offsetTop
        // On scroll trigger script
    window.addEventListener('scroll', function() {
        // When element has reached the top of the window trigger script
        if (this.pageYOffset >= offset) {
            bottomSocialIcons.classList.add('sticky')
        } else {
            bottomSocialIcons.classList.remove('sticky')
        }
        // console.log(this.pageYOffset)
    })
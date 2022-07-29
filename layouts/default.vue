<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <Popover class="relative bg-white">
    <div
      class="flex items-center justify-between px-4 py-6 sm:px-6 md:justify-start md:space-x-10"
    >
      <NavbarLogo />
      <NavbarMobileOpenMenu />
      <nav
        class="hidden items-center justify-end space-x-10 md:flex md:flex-1 lg:w-0"
      >
        <NavbarLink title="Home" to="/" />
        <NavbarLink title="Blog" to="/blog" />
      </nav>
    </div>

    <NavbarMobileNav>
      <div class="px-5 pt-5 pb-6">
        <div class="flex items-center justify-between">
          <NavbarMobileLogo />
          <NavbarMobileCloseMenu />
        </div>
      </div>
      <div class="py-6 px-5">
        <div class="flex flex-col space-y-6 text-center">
          <NavbarLink title="Home" to="/" />
          <NavbarLink title="Blog" to="/blog" />
        </div>
      </div>
    </NavbarMobileNav>
  </Popover>
  <slot />
</template>

<script setup>
import { Popover } from "@headlessui/vue";
import {
  ChartBarIcon,
  CursorClickIcon,
  DocumentReportIcon,
  RefreshIcon,
  ShieldCheckIcon,
  ViewGridIcon,
} from "@heroicons/vue/outline";
import { ChevronDownIcon } from "@heroicons/vue/solid";

const solutions = [
  {
    name: "Analytics",
    description:
      "Get a better understanding of where your traffic is coming from.",
    href: "#",
    icon: ChartBarIcon,
  },
  {
    name: "Engagement",
    description: "Speak directly to your customers in a more meaningful way.",
    href: "#",
    icon: CursorClickIcon,
  },
  {
    name: "Security",
    description: "Your customers' data will be safe and secure.",
    href: "#",
    icon: ShieldCheckIcon,
  },
  {
    name: "Integrations",
    description: "Connect with third-party tools that you're already using.",
    href: "#",
    icon: ViewGridIcon,
  },
  {
    name: "Automations",
    description:
      "Build strategic funnels that will drive your customers to convert",
    href: "#",
    icon: RefreshIcon,
  },
  {
    name: "Reports",
    description:
      "Get detailed reports that will help you make more informed decisions ",
    href: "#",
    icon: DocumentReportIcon,
  },
];
const resources = [
  {
    name: "Help Center",
    description:
      "Get all of your questions answered in our forums or contact support.",
    href: "#",
  },
  {
    name: "Guides",
    description:
      "Learn how to maximize our platform to get the most out of it.",
    href: "#",
  },
  {
    name: "Events",
    description:
      "See what meet-ups and other events we might be planning near you.",
    href: "#",
  },
  {
    name: "Security",
    description: "Understand how we take your privacy seriously.",
    href: "#",
  },
];
</script>

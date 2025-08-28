<template>
  <Dialog v-model="show" :options="{ size: 'sm' }">
    <template #body>
      <div class="p-4 pt-5">
  <div class="flex justify-center">
    <div class="flex flex-col items-center">
      <CRMLogo class="mb-3 size-12" />
      <h3 class="font-semibold text-xl text-ink-gray-9">Pumo CRM</h3>
      <p class="text-center text-md text-ink-gray-7 mt-2 px-4">
        An end-to-end management application designed to streamline business operations, enhance productivity, and foster seamless collaboration across teams. Built with a focus on flexibility and user experience, it empowers organizations to manage their processes efficiently and grow effectively.
      </p>
    </div>
  </div>
  <hr class="border-t my-3 mx-2" />
  <!-- Links removed as requested -->
  <hr class="border-t my-3 mx-2" />
  <p class="text-md text-ink-gray-6 px-2 mt-2">
    © Pumotechnovation Management App
  </p>
</div>
    </template>
  </Dialog>
</template>
<script setup>
import { Tooltip } from 'frappe-ui'
import CRMLogo from '@/components/Icons/CRMLogo.vue'
import LucideGlobe from '~icons/lucide/globe'
import LucideGitHub from '~icons/lucide/github'
import LucideHeadset from '~icons/lucide/headset'
import LucideBug from '~icons/lucide/bug'
import LucideBookOpen from '~icons/lucide/book-open'
import TelegramIcon from '@/components/Icons/TelegramIcon.vue'

let show = defineModel()

let links = [
  {
    label: __('Website'),
    url: 'https://frappe.io/crm',
    icon: LucideGlobe,
  },
  {
    label: __('GitHub Repository'),
    url: 'https://github.com/frappe/crm',
    icon: LucideGitHub,
  },
  {
    label: __('Documentation'),
    url: 'https://docs.frappe.io/crm',
    icon: LucideBookOpen,
  },
  {
    label: __('Telegram Channel'),
    url: 'https://t.me/frappecrm',
    icon: TelegramIcon,
  },
  {
    label: __('Report an Issue'),
    url: 'https://github.com/frappe/crm/issues',
    icon: LucideBug,
  },
  {
    label: __('Contact Support'),
    url: 'https://support.frappe.io',
    icon: LucideHeadset,
  },
]
</script>

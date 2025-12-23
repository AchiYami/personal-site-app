<script lang="ts">
    let {title = "Placeholder", icon = "solar:question-circle-bold", iconHeight = 32, iconWidth = 32, children } = $props();
</script>

<div class="card bg-base-100 w-96 shadow-sm">
    <div class="card-body">
        <div class="flex gap-2">
            <iconify-icon class="self-center" icon={icon} width={iconWidth} height={iconHeight}></iconify-icon>
            <h2 class="card-title">{title}</h2>
        </div>
        {@render children?.()}
        <div class="card-actions justify-end">
            <button>button 1</button>
            <button>button 2</button>
        </div>
    </div>
</div>
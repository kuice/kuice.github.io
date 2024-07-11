<div class="application">
    <TopAppBar variant="static" color="primary">
        <Row>
        <Section>
            <IconButton class="material-icons">menu</IconButton>
            <Title>Kuice</Title>
        </Section>
        <Section align="end" toolbar>
            <IconButton class="material-icons" aria-label="GitHub">github</IconButton>
            <IconButton class="material-icons" aria-label="Print this page">print</IconButton>
            <IconButton class="material-icons" aria-label="Bookmark this page">bookmark</IconButton>
        </Section>
        </Row>
    </TopAppBar>
    
    <div class="content">
        <slot />
    </div>
</div>

<script lang="ts">
  import TopAppBar, { Row, Section, Title } from '@smui/top-app-bar';
  import IconButton from '@smui/icon-button';
</script>

<style>
  .application {
    display: flex;
    flex-direction: column;
    height: 100%;
  }

  .content {
    flex-grow: 1;
    overflow: auto;
    padding: 10px;
    height: 100%;
  }
</style>
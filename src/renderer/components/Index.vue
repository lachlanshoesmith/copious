<template>
  <div id="index">

    <div id="left" class="side">
      <main>
        <section>
          <header>Welcome to Copious!</header>
        </section>
        <br>
        <section>
          <article>
            <p>Copious is a fantastic yet simple backup utility that supports automation and external hard disks, among other features.</p>
            <br>
            <p>To get started with Copious, select the hard disk where you would like your files to be backed up.</p>
          </article>
        </section>
        <section>
          <table>
            <tbody>
              <tr class="selected-row">
                <td>Local Disk</td>
              </tr>
              <tr>
                <td>External Backup</td>
              </tr>
              <tr class="alternate-row">
                <td>Macintosh HD</td>
              </tr>
              <tr>
                <td>NO CONTENT</td>
              </tr>
              <tr class="alternate-row">
                <td>NO CONTENT</td>
              </tr>
            </tbody>
          </table>
        </section>
      </main>
    </div>

    <div id="right" class="side">
      <aside>
        <div id="disk-information">
          <div class="icon-container">
            <svg class="icon icon-lg icon-bg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M2 2c0-1.1.9-2 2-2h12a2 2 0 0 1 2 2v16a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V2zm10.4 5.6A5 5 0 1 0 15 12V5l-2.6 2.6zM10 14a2 2 0 1 1 0-4 2 2 0 0 1 0 4zM6 3v2h4V3H6zM4 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm0 16a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm12 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm0-16a1 1 0 1 0 0-2 1 1 0 0 0 0 2z"/></svg>
          </div>
          <article id="selected-disk">
            <section>
              <h1 id="selected-disk-name">Local Disk</h1>
              <h2 id="selected-disk-info">500 GB total, 200 GB free</h2>
            </section>
          </article>
        </div>
      </aside>
    </div>
  </div>
</template>

<script>
export default {
  name: 'index',
};
</script>

<style lang="scss">
#index {
  display: flex;
}

.side {
  width: 50vw;
  height: calc(100vh - 40px);
}

header {
  font-size: 22px;
  color: hsl(130, 23%, 25%);
  font-weight: 900;
  line-height: 1.1;
}

article {
  font-size: 18px;
  color: hsl(130, 23%, 43%);
  font-weight: bold;
  line-height: 1.5;
}

main,
aside {
  margin: 20px;
}

table {
  width: 100%;
  margin-top: 20px;
}

tr {
  font-size: 18px;
  padding: 20px;
  background: hsl(155, 53%, 88%);
  color: hsl(130, 23%, 43%);
}

td {
  padding: 10px;
}

.alternate-row {
  background: hsl(156, 60%, 82%);
}

.selected-row {
  background: hsl(155, 90%, 68%);
  color: hsl(130, 23%, 25%);
  font-weight: 900;
}

.icon-lg {
  width: 45px;
}

.icon-container {
  display: flex;
  justify-content: center;
  align-items: center;
  background: hsl(155, 90%, 68%);
  border-radius: 50%;
  width: 100px;
  height: 100px;
}

#left {
  background: hsl(156, 81%, 88%);
}

#disk-information {
  display: flex;
}

#selected-disk {
  display: flex;
  align-items: center;
  margin-left: 16px;
}

#selected-disk-name {
  color: hsl(130, 23%, 25%);
  font-size: 22px;
  font-weight: 900;
}

#selected-disk-info {
  font-size: 16px;
  font-weight: bold;
}
</style>

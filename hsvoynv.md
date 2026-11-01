代发 wailian999

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/gethugelb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/grjldtdvl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.tarul.cn/Article/details/gwsifaota.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gsgoexjhu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gcxomiwut.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/guibrabzx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gxxirqhlu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gjujcxeby.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/gfgvgilxf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gucfovpes.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gdozuzttm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gzynspwjh.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gefeskrlg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gojydazid.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/ghhhjzquf.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gmnmqjtvm.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gfmebgyev.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/gerxpfily.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfmlcpum.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/ggulenkmb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/ggkarhlzr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.tarul.cn/Article/details/grmuxnbgs.sHtML

TS:   if (s === "") {}
来源：http://wap.yfazqb.com/Article/details/gqfnlfiev.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gbbieeyte.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fktsv.cn/Article/details/gjklfucqw.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/ggddowzqk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gyjvgiael.sHtML

[E21] 超长截断加省略号
来源：http://baike.bbcook.cn/Article/details/gajhabihy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/gejvjvozi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gnxvxpnsv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/glnogcbcm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/geoadgiac.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gvyuzhrpq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gejtnkaex.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gqptbufdw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gdzipxchh.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/gatwfsvvo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.epnwcf.com/Article/details/gzrlbhrfa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/ghmgrepyt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gvzdvmopt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gvwikgspx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gnwzlrblf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gdgybstml.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/gooifxubc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gyxwhtnag.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcqacheqs.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gtwnagjij.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gsqttuvyg.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/goclvcixu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gitntumet.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/gayezpwkn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/gwfbzdruw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gkmjttpjr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/guvhzgbyg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gordxdhaz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/gmgjmonyb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.epnwcf.com/Article/details/givkwnhmf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/grhnajjgt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.bbcook.cn/Article/details/gxufnkivj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gpaavgvhs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gjhooxbqm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gxludryuc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/glhxiebju.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/gqsqqeefp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fktsv.cn/Article/details/giwgxxahd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gldsdvzmp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/gujccdyvf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/gfnjjltre.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gaskyzhrf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/glfkadcpb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/ggufuxbcr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gijigzghm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.bbcook.cn/Article/details/gopcmtmqe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.tarul.cn/Article/details/gsfcixbom.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gcelomqdr.sHtML

[F04] 追加写入文件
来源：http://www.share.yfazqb.com/Article/details/gnryezjhe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fktsv.cn/Article/details/gmecghokw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/gkcdigtpr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gzfifucai.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gctndqbhd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gtqdebjnt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/glicpgygc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/genbhmvht.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/gmxoaycak.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gdlwelhta.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/gerkqlwqt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gwajrvahh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtxouiawl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gynkdbens.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gjrgmoudy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.yfazqb.com/Article/details/godhvaabw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmgqzvtl.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gixhkvccp.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gwprhosdf.sHtML

Py:   os.remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/giyprljgq.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/gyhdmfoco.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gfkbdtkth.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/grtsiaofh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gdhzmajqf.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gtaephtqo.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gyyugxfzl.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gkifenzdb.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/gpzrcejqf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gfotdgbcp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/guqgdjuje.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/griylmbsx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gjohplmjv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gwglyolis.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fktsv.cn/Article/details/gsaxqzbcb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gwsmeztbj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.tarul.cn/Article/details/gqkauspvi.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gasoahdat.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/ghloxbsmh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.yfazqb.com/Article/details/gxncefrii.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gnvlsgapa.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gnyjbmpge.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gmwqfxdet.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/gksoeehgx.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gdlczdxcb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.yfazqb.com/Article/details/gwmycmcat.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gneyneylq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gflzebeug.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fktsv.cn/Article/details/glczcfbwp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gehkjuanj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gscsagtef.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/grlubkrhc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.bbcook.cn/Article/details/gpbjjozjd.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gelcuiutu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gjimbepht.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/grausaajv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxjitacqh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/grnieklgk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gygpngelt.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/ggmkwbkkb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gdittpwrw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gfwbmhydn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gdjagpoqk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfkxnxsel.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/gcbseiqtz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gisoxtesz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/guoffgzpx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gwdlbcbdt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gphfslgax.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.bbcook.cn/Article/details/ghvhxvbqc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/ghtigrkkb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gckcjgzon.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/ghvvamhbu.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gzezskiqb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/gwrgubhbl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.bbcook.cn/Article/details/gwtnnrkha.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gqftembbd.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gxxsodokq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/gzljxjizu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/garxxedrb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/ghomhflba.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/gnppzqptw.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzauabtxh.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/ggpjwrgve.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gusukttza.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gawspdicx.sHtML

Py:   class User: pass
来源：http://3g.vehdjk.com/Article/details/gnijtphap.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gorucqdro.sHtML

JS:   class User {}
来源：http://baike.tarul.cn/Article/details/gadtyuozm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gyjwoqnxp.sHtML

Java: class User {}
来源：http://wap.vehdjk.com/Article/details/gtwhqwxym.sHtML

Go:   type User struct { Name string }
来源：http://wap.tarul.cn/Article/details/ghagkkxte.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/gbxgbspjj.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gyhfukinm.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/giwhbwmzc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gdoxendhz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gtcrlrtmr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gfdygzjhy.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gpaxpnoxf.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/guyqgdrwu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.sjlbkw.cn/Article/details/golcpwjir.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.vehdjk.com/Article/details/gcevxqwgj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gnaepbikr.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gvdrpjigd.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gzpyeppaz.sHtML

PHP:  public string $name = "x";
来源：http://3g.yfazqb.com/Article/details/gjepszshv.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/gnhpwmdjg.sHtML

TS:   name: string = "x";
来源：http://baike.epnwcf.com/Article/details/gyvqfgbvm.sHtML

Java: private String name;
来源：http://www.m.share.tarul.cn/Article/details/gswfvmsto.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gfnmdpddn.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gbocaqqum.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/gomhejeeb.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/gzyxyjtyb.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/glljroutp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gnafqengi.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/glcgugpyb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gdzwyhfuz.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gwdxtjxdr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/ghdgbosoh.sHtML

Ruby: def greet; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gzmtapdcc.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gmkdnrlgy.sHtML

[G05] 继承
来源：http://www.share.epnwcf.com/Article/details/gjcrvvhdp.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gmukjludm.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gxzzdulyd.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gtmzzanol.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gpwyosuvg.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gkvgmahds.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.sjlbkw.cn/Article/details/gsnjclqag.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gtblksndm.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gkeaqmdpg.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gdtaiyghs.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gbwbaxelh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gcrnuxkdz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/grprielqg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gdmnpqkga.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gapfrgskn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fktsv.cn/Article/details/gvundynyx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/gpzadelpj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gbqglsqap.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gvjbjnkqi.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/gkmgblvjo.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gfgurrmyd.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gcciqpdtq.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gvngzrffq.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gqiprsiab.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.vehdjk.com/Article/details/gnlcpgrdo.sHtML

Ruby: super
来源：http://www.share.epnwcf.com/Article/details/gzvlcnqeo.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/gzmjrsuap.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/geyghmwjt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gunbiygan.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwqahiss.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gjoyhzmyj.sHtML

TS:   static f(): void {}
来源：http://www.share.sjlbkw.cn/Article/details/gbxbicttd.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/gcedknbby.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gjhnupmqe.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gishnazyu.sHtML

C#:   public static void F() {}
来源：http://3g.yfazqb.com/Article/details/gdyoylmag.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/gfcydsozw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.yfazqb.com/Article/details/gobnsvpty.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/ghkszokxb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/gtikmbvmd.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/gigppsywd.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.bbcook.cn/Article/details/gvawyefkl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gstjryjmy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gkvmjrpbu.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.epnwcf.com/Article/details/gedeloghp.sHtML

[G10] 访问控制
来源：http://m.share.yfazqb.com/Article/details/gzqfnrqde.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/ggbhcbsps.sHtML

PHP:  public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gmiqimbdn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/goxhujgqq.sHtML

TS:   public / protected / private
来源：http://www.share.tarul.cn/Article/details/glebidpnr.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gvrmvfstl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gyaexztlm.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gqnfpqqnb.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/gcpmchvpe.sHtML

[G11] getter / setter
来源：http://3g.yfazqb.com/Article/details/glsugotqw.sHtML

Py:   @property 与 @x.setter
来源：http://baike.yfazqb.com/Article/details/giivsowzz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/ggnikhipr.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/geonjmmme.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gncjfnbvv.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gmmmcsbwy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gbablvtcz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gyauvrvqy.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/glsyptmsy.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/glohwfpay.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gwntfdpqj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gmmbtiegt.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/glbjzpnvb.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gbiqbwzay.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.vehdjk.com/Article/details/gwqnfysgn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gwzhmxdxc.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.epnwcf.com/Article/details/gnshtyffi.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gribnwuwn.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/gultmlkqd.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/ghcxitnhr.sHtML

PHP:  $u instanceof User
来源：http://baike.fktsv.cn/Article/details/glynapisk.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gvabzncrf.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gxwnqkbun.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/ghpvxqief.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/guahizncq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gmiyxxkkm.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/gmjtpkiiy.sHtML

[G14] 数据类 / record
来源：http://m.share.yfazqb.com/Article/details/gozzrsbrp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/grvtledjb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/gjhdqwime.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fktsv.cn/Article/details/gjkghnbxm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/ghglzpqar.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gcscswdpb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.vehdjk.com/Article/details/gmlalcovk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/gifoywtzv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gagwtkcog.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/gvxjmtapq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.bbcook.cn/Article/details/guwjavsew.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/gemsgpedq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.yfazqb.com/Article/details/gtatviwlh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/grthkxokm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gtahjkbby.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/geucoknxi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.vehdjk.com/Article/details/gxedyiagd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gbddenrcu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gkxxwsyet.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/ggsyvvhog.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/glynnxgau.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gjrwkqjtg.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gjxlzjohy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.yfazqb.com/Article/details/gblfryyve.sHtML


<!-- 参考信息 -->
代发 wailian999

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gyeypexnt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/ghczedznv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.sjlbkw.cn/Article/details/gmbqsdlvy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gnenuuqtc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gghwzrqjc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gdoxtjhux.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fktsv.cn/Article/details/grkjizqla.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gtalzidki.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/gkmeynmad.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/ghbytigwa.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/glgejhzga.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/gmwcnxqak.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gwxnxmiyw.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gszbvcowk.sHtML

Java: s.lines().toList()
来源：http://www.blog.tarul.cn/Article/details/gpfjzvkau.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/gpxfmgmuw.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gatszrdjq.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gvqyqfozv.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/grkperhvh.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gohcrzxod.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gfyuoucuc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmlaalnin.sHtML

TS:   if (s === "") {}
来源：http://m.share.sjlbkw.cn/Article/details/gipwvrrlf.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gihauhsbg.sHtML

Go:   if s == "" {}
来源：http://blog.fktsv.cn/Article/details/gftqsonkj.sHtML

Ruby: if s.empty?
来源：http://www.m.share.epnwcf.com/Article/details/gmiqvzcyz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gsiczoish.sHtML

[E21] 超长截断加省略号
来源：http://m.share.bbcook.cn/Article/details/ghnmtbmyo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.yfazqb.com/Article/details/gjfovaiyy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gmkqclgzi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/ghazgfjnn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gpyaxttqv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gqeuwmbmp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/geicrpdxj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gdebzaobi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gmgzahrhf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gpfyhwjyl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.epnwcf.com/Article/details/gdqqhxcsm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gmcrdhfnw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/gglxrchnu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gpcxuuxjc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gvyefctgr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/grjwuucgc.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/gjzfixesq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gughfdanc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdpzcggkm.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/grmvhkjmw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqibymden.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/gttueaibl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gceorcrho.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.epnwcf.com/Article/details/goyddtqnr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gqwxrhfwm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/geqwpwxoz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gattsrsvu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.yfazqb.com/Article/details/gkbepzjnm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gycituqnj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gnlwwfgjt.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gtnplxfax.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.epnwcf.com/Article/details/gxjxbzoul.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/gegczyvfg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gwteueixc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gfxarxhnj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/ghorjnzsy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/gjjokfoed.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/gvnhhdjgw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fktsv.cn/Article/details/gvfiovqnd.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/gfbaxvgcx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fktsv.cn/Article/details/gnsiokyvx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/ghkuccilv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gcvxfunrn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gdvdbxokb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/gaohovpdm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.epnwcf.com/Article/details/gsnsqiufw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gnbzngarm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gnrrxdpca.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/gkgxrwfcx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gnofqesmz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gfttsobcg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gjhlrbdgl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gzhrtjgcn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/gmqgcxyop.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gvotwljdn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/gjbvpnvfr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.vehdjk.com/Article/details/glmdovevv.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.sjlbkw.cn/Article/details/gtzjzupit.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.epnwcf.com/Article/details/gjlwxbjkn.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gwjqqtghd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gmdjqjpvp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gidqratxc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gcliwzowp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/gfqaxoakl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gekuuldvr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gtxkaadge.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/gzetgvebn.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gxfpvwrqj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gupirtytl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gecptoznf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gxhldyoav.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/genqukxli.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gvikcqbzu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gltdasjgf.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/ggqdmewoh.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/gfykoiwsa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gnnoqrnjq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fktsv.cn/Article/details/gpddtyyfh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gfplpjgdz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/ghtthrtcp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/ghvbsqogv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.yfazqb.com/Article/details/gkerasciq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gejcsyzdf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gbrqttfnu.sHtML

[F08] 遍历目录
来源：http://www.share.vehdjk.com/Article/details/gjinrfcrs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.vehdjk.com/Article/details/gqylozefc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gifhbyfpu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gsxkzosvc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gffqpvjbq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gdxwvzalm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gzsnuoupk.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/gbpicswrf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.epnwcf.com/Article/details/guchsjrei.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gshtwjjsq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gnvhpwfal.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/gtgxqjker.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/gbcbpgntb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gndwzbqta.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gmygdlopm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gsahujykq.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/gohubqatt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/grixnylca.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/goaivypoh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gtswiiedm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/glnduoryy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gncorncqt.sHtML

TS:   path.extname("a.txt")
来源：http://3g.bbcook.cn/Article/details/gjwpouypw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.epnwcf.com/Article/details/gwysuyurk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gxthnnmnb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gpgqjcost.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gzezbtpzx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/gnanieyvy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gtqnvvrnx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/grpwmjrtc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/guxwnngia.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/glvnipdis.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/gothquqag.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/gkzlewigk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/grxvhwlup.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.bbcook.cn/Article/details/ghurceyoy.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gisltcgnx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/geirysfzu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gqodcivfk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.epnwcf.com/Article/details/gskbkvqrk.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/ginidmaes.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/gtrphypvh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gewszdmjv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/gvwhfkktb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/ghbhmjhmk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gaksageuj.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/gderizxyn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzfyxbdyu.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gpepqocsn.sHtML

Py:   class User: pass
来源：http://www.share.fktsv.cn/Article/details/gxnntgofu.sHtML

PHP:  class User {}
来源：http://www.m.share.epnwcf.com/Article/details/guldwfntd.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gaudoykcq.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.bbcook.cn/Article/details/ghpvbflkr.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gyqjbxoit.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gevdvqvtv.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gcyaetxtb.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gwtfcjikh.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/ganhenylt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gvrqybcuj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gttpifqwt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gciwmvtzr.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdjhflkji.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/goiirbesk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.epnwcf.com/Article/details/gjeefjzas.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/ghlxczelc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fktsv.cn/Article/details/gsimbxwva.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gzrynuzuj.sHtML

Py:   self.name = "x"
来源：http://blog.tarul.cn/Article/details/gdwiragak.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gfghxjnom.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gvxvpxugo.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/guyvohrli.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gvsiiphde.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gpubhhjaa.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/gijdsyvjl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gqwkhempn.sHtML

[G04] 定义方法
来源：http://m.share.yfazqb.com/Article/details/gxgyyuqgs.sHtML

Py:   def greet(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gudpytgpk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gfuuzcncj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gckgypxmn.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gdmhztpqu.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gityfeeyi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/golzbhufb.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/garsubywn.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gdhoswela.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gnlqlngvw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/gunxgzfro.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/glmhgjued.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gtamqqjux.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gdrpvxiel.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gttsrzfdn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.yfazqb.com/Article/details/ggvvthnle.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gltkvvboj.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/gijuikrlu.sHtML

[G06] 重写方法
来源：http://read.share.fktsv.cn/Article/details/gnypabqlq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gbagpclcd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/ghtveqpzj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gdphklhhv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gjoriihpo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gnosznxjs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/gvqpblbwb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gjeilfqxl.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.bbcook.cn/Article/details/gvmakyvtk.sHtML

[G07] 调用父类方法
来源：http://www.blog.sjlbkw.cn/Article/details/gkwslegly.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/gbzzvlgwr.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gbsxdskwq.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gkmpxsoub.sHtML

TS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gbjvjsbty.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/gissdbkgg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/gtnmgsdor.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gszrrtvos.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/geqspdvew.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/gtitcddnf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/glgfwnyjl.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/gpbvivkjl.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gkwblbppc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.epnwcf.com/Article/details/glzrjoqkt.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/ghzchnzbc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gxkaifbjx.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gspkjxivf.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/gafvtupwu.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/gscfkxmnp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gopvgyura.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/gqtlvonbo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/gsskylaaw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fktsv.cn/Article/details/glpijfpwq.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gzcnysnqt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gcytgilre.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfingaaz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gpkzctbrb.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gfasudpha.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/glfexdaqa.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/govvxdlcl.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gpzobumbq.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/gsojuvvhb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.yfazqb.com/Article/details/gytrfnvzj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gilvvjsdb.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gdrzlhrid.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/gxllnegte.sHtML

[G11] getter / setter
来源：http://mobile.fktsv.cn/Article/details/gcemccmcf.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gvldizybl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gkbwssfid.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gutumpera.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gvnhswsgk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gckzdvmjg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gjhwofyna.sHtML

Ruby: attr_accessor :name
来源：http://baike.sjlbkw.cn/Article/details/gipncbdja.sHtML

C#:   public string Name { get; set; }
来源：http://wap.vehdjk.com/Article/details/gilyxwxxw.sHtML

[G12] 对象转字符串
来源：http://www.blog.fktsv.cn/Article/details/giayidnhu.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gpjeanzmx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/ghtmmgvxs.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gkzsdgahv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gpzirsrlu.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/grzjpppan.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gfonuepyq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gpfovbgpu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gqwtavxnv.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/gkpncnutf.sHtML

Py:   isinstance(u, User)
来源：http://m.share.sjlbkw.cn/Article/details/gsiiysppc.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gdwdwqjwg.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gqpeakumj.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/giktkdgix.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gloaswiuy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/gmhjoucqe.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gwjyaozdh.sHtML

C#:   u is User
来源：http://www.share.epnwcf.com/Article/details/gruyiphbc.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gcxdilhjk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gtmcjcokv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fktsv.cn/Article/details/gbdrzjbbc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.vehdjk.com/Article/details/geoszvyty.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fktsv.cn/Article/details/grovxjsoj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gobjarwyo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gfdaiatxe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/glofwxpsf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gxnxsdqxf.sHtML

[G15] 枚举
来源：http://wap.tarul.cn/Article/details/ghpkdhiyl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.vehdjk.com/Article/details/gdaywimfh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.epnwcf.com/Article/details/gniciqspv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gscsdnxja.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gwncgwvri.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.tarul.cn/Article/details/gxoutodtl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.epnwcf.com/Article/details/glbutecgs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.sjlbkw.cn/Article/details/gvfyhtvig.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gynouknsm.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/guylvbsvn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/godxdtvau.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gfizecknw.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gkqqjtyvw.sHtML

TS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gzvfaikhy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/gmtkrwwcp.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/ggetctqdv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gneaxcboa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/glzinionk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.tarul.cn/Article/details/gtcevkonu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/gcomhwbqd.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.tarul.cn/Article/details/ghwmmvata.sHtML

Py:   s.splitlines()
来源：http://www.m.share.tarul.cn/Article/details/gmopzyhqb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gcmduhptp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gkmghmmrl.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/ghseoxdib.sHtML

Java: s.lines().toList()
来源：http://wap.vehdjk.com/Article/details/gizwwtede.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/glcjhhpev.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/glpmejaez.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gyzjhjqau.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.epnwcf.com/Article/details/ghjoszolm.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gjqryqnuz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.vehdjk.com/Article/details/grafntoky.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gomfwqllb.sHtML

TS:   if (s === "") {}
来源：http://read.share.fktsv.cn/Article/details/gfbnvprai.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/gtdajirac.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/gqvoymxpy.sHtML

Ruby: if s.empty?
来源：http://blog.tarul.cn/Article/details/gwjlmpgup.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fktsv.cn/Article/details/giqubrgne.sHtML

[E21] 超长截断加省略号
来源：http://read.share.vehdjk.com/Article/details/gyzxykmrs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/ghvbwctpp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/glyysyvop.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/glsavnqkn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gjcyyupaw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gtepyjcwy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/gesusjpcn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gwoperdzb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gnxvcbsna.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.bbcook.cn/Article/details/gczliswak.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.tarul.cn/Article/details/gdrbbhvqp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gxdrxkvro.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/girncpkhz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gzsnoshzn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/glaohlzge.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/gqeazpsmg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gqokuodsg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gryddxeoy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtviutphd.sHtML

F. 文件与目录
来源：http://www.blog.bbcook.cn/Article/details/gzbjzgyix.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gyzuhcijb.sHtML

[F01] 读取整个文件
来源：http://blog.epnwcf.com/Article/details/gkjcbsbma.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.sjlbkw.cn/Article/details/gssjalldu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gvmoqtzep.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/gnibljrvc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gcbxrrenz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/govgcbzwq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gzzhryvye.sHtML

Ruby: File.read("a.txt")
来源：http://blog.epnwcf.com/Article/details/gtfxzlkwq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gxwxejmhd.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/gzadzouvy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/gssfzgtkr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gsixnccal.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/ghdfsohyx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gzfyycapy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gmkowjqua.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gsncahmbf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gotgdxalk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/ggmaecpcr.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gioeayvwz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/gypdnebhf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gyqaegvoz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gjfskrelc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gpdovbsdv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gkcciwoum.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fktsv.cn/Article/details/guilixroj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fktsv.cn/Article/details/gzphfwrgm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gwjgpfcet.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gozznlukt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/ghkszmbxz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.sjlbkw.cn/Article/details/gaevdzxdd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gidhygmbt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/grirjqsbp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/gwfutgfow.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gdhumlpxw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gpvcemyek.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gcpiifnaj.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.tarul.cn/Article/details/gvoczlsgi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.vehdjk.com/Article/details/gwmiclymx.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fktsv.cn/Article/details/gsfgaazzi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gsnahgcot.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gfqlrpckm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gvfrtskjp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/gnnbvhzer.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.epnwcf.com/Article/details/gjxnapalu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gguuckbqt.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gwiutfoxq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gghecyglb.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gydjmvfoi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gqzmfvwoy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gimwuqpcl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gttpestki.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gssxuumel.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gkspirzrs.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gecjgbqco.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/grnvqvghv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gachrrqxh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gkwqviufq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gmtoolmxv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/giwbaovjf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.epnwcf.com/Article/details/gkyfacdjl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gjgumhnde.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/girmuvbkq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/glaowpgrd.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/gaflcxkcb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/gyeoxwbqq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.epnwcf.com/Article/details/gnlnkurum.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/gfkwzgspp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gnabojrcs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gdwshdeun.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gkspelwzy.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.bbcook.cn/Article/details/gapjfitrt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/gsyfgxbev.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gwpbovruo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fktsv.cn/Article/details/guwrlygaw.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/gpbuducrj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gufgebwdv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gtdhhorft.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gnrddjred.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.sjlbkw.cn/Article/details/gmpxwjmkd.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/glcobcsti.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/glvsdyktf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/gmjwopclw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gsrclamel.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gdydbalhj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvqzbkadc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gmlxwemxk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/gdcepvnjf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/guhccxyrm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyffeczjm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gkrgunvmv.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/gdpbrhgql.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gfhveeuhl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.vehdjk.com/Article/details/gczaerstr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gfiqyerfk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gublinjfc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gxonsjoau.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/graloloxr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gqnbiqhue.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/gniyveurl.sHtML

[F12] CSV 读写
来源：http://mobile.tarul.cn/Article/details/gnchothfe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/gngjwzzcd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/giyglstbf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.sjlbkw.cn/Article/details/guudiqexc.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/ghtnoicch.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gtyuloxcj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.vehdjk.com/Article/details/gsvrpivyc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.sjlbkw.cn/Article/details/gpzgdukev.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/gvgpahjrw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gewyuueht.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/grsrbcfru.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gunkqzeqf.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gectuwswp.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/gfsfnwdbo.sHtML

PHP:  class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzjmdgxhq.sHtML

JS:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gaxtitqgu.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fktsv.cn/Article/details/gqgydozrq.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gfhqpozrw.sHtML

Go:   type User struct { Name string }
来源：http://m.share.epnwcf.com/Article/details/gsefkwsap.sHtML

Ruby: class User; end
来源：http://wap.fktsv.cn/Article/details/gbejfdnmr.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gzzxvpfat.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/gjcnmtnyp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.yfazqb.com/Article/details/gbnxjhthv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/gkmdcxsmt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gskrukxha.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gliseilei.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gkuhxfduj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gamlwaxsn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/gnrokoelj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/glnpisyux.sHtML

[G03] 实例属性
来源：http://mobile.sjlbkw.cn/Article/details/guwojxjpi.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/gbwrmztky.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/ggcylxobk.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gxvubfzvy.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/gnghftrzs.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gqyqfkskk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.tarul.cn/Article/details/gfxyltrqc.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/guhdsdzxk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.vehdjk.com/Article/details/gbxndctnz.sHtML

[G04] 定义方法
来源：http://3g.yfazqb.com/Article/details/ghjaqzjbk.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gevgnhari.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gxebosvlq.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gqxrujlkn.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gcspyeeyk.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/genouries.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gaabuwuxl.sHtML

Ruby: def greet; @name; end
来源：http://read.share.vehdjk.com/Article/details/gqgkkhmpo.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gqbnmtszs.sHtML

[G05] 继承
来源：http://read.share.vehdjk.com/Article/details/gzhdpazal.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/gqouaqmkx.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gmwlutxle.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/ggtedrywz.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gqoxtpmxy.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/grotaqvbo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gcebajyma.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gxwxzghwh.sHtML

C#:   class Admin : User {}
来源：http://m.share.epnwcf.com/Article/details/gnejgynny.sHtML

[G06] 重写方法
来源：http://blog.vehdjk.com/Article/details/gfuoycyqo.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fktsv.cn/Article/details/gmrybfyei.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gklrdrilw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdrdmywqs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gxgkchimx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gsmstffuf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/goyhjzvvz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fktsv.cn/Article/details/galdmrvaj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gyylkalgc.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gwiesmwhz.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gkuogdbuq.sHtML

PHP:  parent::greet();
来源：http://www.blog.vehdjk.com/Article/details/giasimiao.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gfquwcrgv.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gvkfsjmyf.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/gaxuzsdml.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gjzilbwch.sHtML

Ruby: super
来源：http://www.blog.fktsv.cn/Article/details/gyuhboihk.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/genanhsby.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/gjmgrneza.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/gqpzsvbtj.sHtML

PHP:  public static function f() {}
来源：http://read.share.sjlbkw.cn/Article/details/guvwpdwrc.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gbufqzpfi.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/goyutejze.sHtML

Java: static void f() {}
来源：http://m.share.bbcook.cn/Article/details/griyrcnmd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gabgqqkzi.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gsinhyszv.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/gsjispfpv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/gykloqmng.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/gkmtxishv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fktsv.cn/Article/details/gygopuhvo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.tarul.cn/Article/details/guajuhehx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.bbcook.cn/Article/details/gzasmamtk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/groisiptp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/gtbxfgjag.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/goycgplnl.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.yfazqb.com/Article/details/gewxvpdnv.sHtML

[G10] 访问控制
来源：http://read.share.vehdjk.com/Article/details/gtqosovbg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/goqkxrqmq.sHtML

PHP:  public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gqvympwks.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gzgqjlqcm.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gusylpbsg.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gnmqajbtx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gkopjrcpm.sHtML

Ruby: public / protected / private
来源：http://read.share.tarul.cn/Article/details/gpivhnpmy.sHtML

C#:   public / protected / private / internal
来源：http://mobile.bbcook.cn/Article/details/gcsmmatuf.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/gyoxjgmin.sHtML

Py:   @property 与 @x.setter
来源：http://3g.epnwcf.com/Article/details/grnczfupx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gmkqrwgyd.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/glkturonm.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gwmxnqcai.sHtML

Java: public String getName() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gfyvdvtao.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gdqrlvgqy.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gzpuchnzt.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gblqqsrym.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gczrmpipb.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gyraexjtb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/ggdyauzbk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gwdfxiywp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhptylag.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/givmaimnk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gfxfiurlw.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/gqtxmhhsp.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gdztylymf.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gasmzetgn.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/gbrtqdubo.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgoltcnv.sHtML

JS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gcnunpfyv.sHtML

TS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gbqjwqyci.sHtML

Java: u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gwvsfjpjz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/gcquupgbh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gmjopehzi.sHtML

C#:   u is User
来源：http://read.share.vehdjk.com/Article/details/gcmcvmghz.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/glqgdmxta.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.vehdjk.com/Article/details/gyulqeiok.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/gmobciepl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.vehdjk.com/Article/details/gllpgeolf.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/ghyzlkmtd.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gshqtyttl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/gvfuddzup.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.bbcook.cn/Article/details/giimbfiwt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gsclycobs.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/gzaveletx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.bbcook.cn/Article/details/gqlzjbqnu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.tarul.cn/Article/details/geaspfipq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/gwfnwjwom.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/ghskvoiwl.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gaehxnppv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/gxeuimkms.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.yfazqb.com/Article/details/gtacioiiy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gohxlsqam.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gviryaicg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/gqfgihwiw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.yfazqb.com/Article/details/gmjmsaznr.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/grkakikam.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gyolgbrvj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.vehdjk.com/Article/details/gktfuxddr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gdvtlltua.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gdzswwygv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/ggetymgzi.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gqqydyuee.sHtML


<!-- 参考信息 -->
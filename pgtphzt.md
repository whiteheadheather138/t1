代发 wailian999

[E18] 模板占位符替换
来源：http://mobile.vehdjk.com/Article/details/gfzfdeydz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/gdtndhayq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gfzvforlk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/guzylkhzx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/ggzcdsmdk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gudqhcthp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gofhmuocy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/gypzktzmz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/geynwgnfe.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/gkjntakfe.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/geeyjwyty.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/gtfiargju.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gtanjajrv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gywqwldwp.sHtML

Java: s.lines().toList()
来源：http://blog.tarul.cn/Article/details/gzljqwaze.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/gwqvesgbi.sHtML

Ruby: s.lines
来源：http://www.m.share.yfazqb.com/Article/details/gqqnjyhmg.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/gnstavoor.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/guilpnito.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/galdsygfn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/gfhgrgnwp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/glokcdfbu.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/glpuvxnrw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gvbtrklku.sHtML

Go:   if s == "" {}
来源：http://mobile.epnwcf.com/Article/details/gutjxwmyl.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/gpflrsxyz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.epnwcf.com/Article/details/grpjlxylx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gkckwqjte.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gcqeedtka.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gqvkzaint.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gafomtbrs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gdseocyal.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/goavehvhi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.bbcook.cn/Article/details/grarousqe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gpmqlndyc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/goajqfvxa.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.bbcook.cn/Article/details/getbyxipw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gretcavwg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gdzsayztc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/giiatclnm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gwnzrgxmk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gkhsrktwa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/giyqkzkft.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/gyzwhidug.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/gxyzklzdx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfyseotfg.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gzccrufso.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvqmwhbkq.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gohlixhtg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gouqocebm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gjsaixfue.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.vehdjk.com/Article/details/ggagujyjs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/grlwfsdix.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gbdrpcgwv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gkyrhbhqm.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gdthhhbhm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gfodzjywu.sHtML

[F02] 逐行读取文件
来源：http://baike.fktsv.cn/Article/details/gdlrtjfag.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fktsv.cn/Article/details/ggtgpfdng.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.tarul.cn/Article/details/gxmmeqdfo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gpxukmfwz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gufmtynyx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/ghodhawfw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/gozxljsur.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/gxwerxweb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.epnwcf.com/Article/details/geqrtydfj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gaxydrjlg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.sjlbkw.cn/Article/details/gisjlfyuw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gothpzqqa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gtqujkgqk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/ghsdbexxw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gbbveuyud.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gvtvknytg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fktsv.cn/Article/details/grkrlhgbt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gjwgkviin.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gitkjntnt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.tarul.cn/Article/details/gofdcgcnc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.tarul.cn/Article/details/gzjwqvzkf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gtzjzvaih.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/giqywsqjb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/gdvgmrufe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/gpokaoyut.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.bbcook.cn/Article/details/gwfbcyiuq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gwcdrxnio.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gwrjcwtol.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/gvimmzuqb.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gvcasskgo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gddyluyij.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gsrsjwgsf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gkmpaikzz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.sjlbkw.cn/Article/details/gwixtgzgy.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gcnersabw.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.vehdjk.com/Article/details/gkywcpuze.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/gziprlxpr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/giilrhxtb.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gzolsgmsh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gumdenteb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/geszpyokp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/givpwbvcf.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/geuibvrps.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ggdgjjifw.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/grqworagq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.epnwcf.com/Article/details/gbrmoazqr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/gschbawrj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/gjwkcifnf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gqiaafill.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gwiqhhgss.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.bbcook.cn/Article/details/gxvjguqpj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fktsv.cn/Article/details/geqgtjpil.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.tarul.cn/Article/details/gpvwbtiwh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/gfyhdgwfb.sHtML

[F08] 遍历目录
来源：http://3g.yfazqb.com/Article/details/ghuicrffa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fktsv.cn/Article/details/gxrjpbjdd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gerdltoqt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/guqbpfkzo.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gnsnlckln.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gvdddsixc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gupdxnqan.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/ggmpfeutd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.tarul.cn/Article/details/gnpdbjkli.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gbrjdxspf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/guogkejxu.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/galutwxhu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gnuxgshhi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gjqsuzkth.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/ggxhiovzr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gtjrjflde.sHtML

Ruby: File.size("a.txt")
来源：http://baike.bbcook.cn/Article/details/gjsusnetn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/gymrwhyrz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gjurvynbh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gwxiweulh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/gglbawugo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfsniurlf.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/gwayrynop.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/gkbjfakbk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gveweeiaq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/glkwywdhy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbflrlqua.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/gyaedwqbq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/ghkmyxefw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gxyfzewao.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gdzbtlruz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gsdxsjhdb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/ganumgwea.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.sjlbkw.cn/Article/details/gwigridol.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfbnbmlfw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/gubcvhlcb.sHtML

[F12] CSV 读写
来源：http://3g.epnwcf.com/Article/details/gzldtueyf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.yfazqb.com/Article/details/gvuisenvv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/gnocqogtl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.vehdjk.com/Article/details/gtzdvzulu.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gozdiplog.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/gcnucjxke.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/givjbldwt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fktsv.cn/Article/details/gyurkwben.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.bbcook.cn/Article/details/ggqmvsaml.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grimuetgu.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/gvzycrxbu.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/giduseqbv.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gmqwufwed.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gtguotsrg.sHtML

PHP:  class User {}
来源：http://wap.yfazqb.com/Article/details/gwlduftux.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/glvqmvmsl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gscpmzded.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/gnmsgsidd.sHtML

Go:   type User struct { Name string }
来源：http://wap.bbcook.cn/Article/details/gjfhittzd.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/gubxdcjqz.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gribgxxym.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gbhyzuogi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gfzdshpew.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gvgymsifi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gecfbaonk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/gosvfddkm.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/glxzfndzh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gylmbsbbx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/glyooctxk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.bbcook.cn/Article/details/gooeesxmf.sHtML

[G03] 实例属性
来源：http://www.m.share.epnwcf.com/Article/details/gmgadbluj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gplwcfsim.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gtmejqpjv.sHtML

JS:   this.name = "x";
来源：http://blog.bbcook.cn/Article/details/geyxpaxfw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gqjsadlhf.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gkxzdwthe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gkygfkdog.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/gcuykvfdf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.epnwcf.com/Article/details/gamqgzyuv.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/ghrnjzqru.sHtML

Py:   def greet(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gswypsjhv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqrncygzq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gujzknvcq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gbpsajzzy.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gdsuhjnfj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gwbqtgmhc.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/gzlweradz.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/gnezvukui.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/gbpzzywpd.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/ggkklvaoq.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/giuuwepua.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gykjdofos.sHtML

TS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gjwmrgadd.sHtML

Java: class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/glolmrgec.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/gxdsoumjs.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gqvkmviwh.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gkzoflvip.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gauwzycmw.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/gzmzitnpx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gdqixoige.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gpqollaaf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gkrglaqay.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gfrjofweq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gtfrgfpud.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/guztjldxx.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.vehdjk.com/Article/details/guzesovoq.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gpvjbavow.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/guxadxofa.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/ghlcfsqxd.sHtML

JS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/glbbbsmtn.sHtML

TS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gkuyktfiv.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/gyiwywyqs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gekaakxkz.sHtML

Ruby: super
来源：http://mobile.tarul.cn/Article/details/gskzuddya.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/giqbbmkbs.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gyszlrvxx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/gudogfmia.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gyddqsqtf.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gxwdxzcub.sHtML

TS:   static f(): void {}
来源：http://baike.tarul.cn/Article/details/gleqayeed.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gfwusleru.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/glgphcdij.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/gseutehck.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghcjlbqee.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/ghfwjebks.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/ghqlmtwth.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gnqsqgkff.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.bbcook.cn/Article/details/gkcjvgmvw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gebsbautl.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gchhfwvkr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/gsgfqpgrm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/gyphtrqek.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.vehdjk.com/Article/details/gqujuclas.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gitbironm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.sjlbkw.cn/Article/details/gutlbzwyn.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gmxrmiicq.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.tarul.cn/Article/details/gkjalzctx.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gvhlekyfm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/gkhztmyry.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/gexlakthh.sHtML

Ruby: public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gywpaxjex.sHtML

C#:   public / protected / private / internal
来源：http://m.share.bbcook.cn/Article/details/gtwkgxvwf.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/glfitonov.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gkjkjhyos.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/guknctcyt.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/ghvmjghmz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/ggpnbckcv.sHtML

Java: public String getName() { return name; }
来源：http://wap.yfazqb.com/Article/details/gpojvsnun.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gcnwtwtoy.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gsrczvulf.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gypqmliyy.sHtML

[G12] 对象转字符串
来源：http://www.blog.epnwcf.com/Article/details/geiwkphjc.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gpugqnxzm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfpwwiyps.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gorigwpid.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gqzofdylz.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gkyhglykb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gkpgfgdzc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/goridfwoj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.bbcook.cn/Article/details/gtkwfmalk.sHtML

[G13] 判断对象类型
来源：http://www.blog.vehdjk.com/Article/details/gusxytzhr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/ghohutbqt.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gmwaykfic.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gcifxurwf.sHtML

TS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/gqjvcmweu.sHtML

Java: u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/glnxjjism.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/ggdxfweeq.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/guvrdbboa.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/gcshqfciv.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gnocjpuvv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gadllnggg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/gjcwuzujs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gvtsugmec.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/ggftcfsft.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/gwrkucrvk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.vehdjk.com/Article/details/gzyruoxaq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gcgxxufhb.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gxlumvkyu.sHtML

[G15] 枚举
来源：http://wap.tarul.cn/Article/details/gvshwldib.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.bbcook.cn/Article/details/gaahmtxxa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.vehdjk.com/Article/details/gavwchspd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gsjegxxjw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gxbbekwsa.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gxrcybedk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.epnwcf.com/Article/details/ghbyfrogi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gieifjkys.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gawiiwgmm.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.yfazqb.com/Article/details/guonfdmcm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gnptdolst.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.yfazqb.com/Article/details/gpmhxporv.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gthricqfs.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gvnpmlllu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gykoaadkh.sHtML


<!-- 参考信息 -->
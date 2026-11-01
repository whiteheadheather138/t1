代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gscjyqkjc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gpfoikhhz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gvdkoutqz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/ghorpzlzg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.vehdjk.com/Article/details/gglfixytq.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gpljzkotc.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gvlohmimy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gutekmoqz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gaatjcmpi.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gplqznfwu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/gaiyzdtkb.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gpvyzzdmb.sHtML

Ruby: s.lines
来源：http://www.share.epnwcf.com/Article/details/gkxyhknqw.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/gpjvqbvkc.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fktsv.cn/Article/details/gbltpenrg.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gufedmiuh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/gpsiraxmm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.epnwcf.com/Article/details/gqdaforte.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/guesjtsct.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gwxqhmacc.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/gqcfxbdxl.sHtML

Ruby: if s.empty?
来源：http://3g.sjlbkw.cn/Article/details/gwgsykcud.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gurhhtkcv.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/ggimkthdp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.bbcook.cn/Article/details/gfysqdclq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gwpwzlxoo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gtzjxynum.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/genzpiohv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gprwnceah.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.vehdjk.com/Article/details/gzuhireup.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gmwdacubk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gioyubtet.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.bbcook.cn/Article/details/gzwbwzgjx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gcfguftln.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gewqlfpdh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gbdswpzki.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gxvxhqnua.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fktsv.cn/Article/details/gwklpytaj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/ghrnoqinr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gfuofwubf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.bbcook.cn/Article/details/gkcawlpdl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfpzljloh.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/guunjuplb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnevkfhvu.sHtML

[F01] 读取整个文件
来源：http://read.share.bbcook.cn/Article/details/gxwqmbuom.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.yfazqb.com/Article/details/glafrjwfq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/gdkphtdui.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gtyjbnhat.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gaffgtrnx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gpundhaja.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.yfazqb.com/Article/details/goofeaeto.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gbshuwdoy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fktsv.cn/Article/details/gnpkhikvg.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/guoddwcpz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gbipkaoia.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/grfwuitqx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gnvgsungc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gptewelhn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/ggdmoismd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/gtckjdfyz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/gamcsdqjd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/gkhabrytk.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.yfazqb.com/Article/details/gspuadlji.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/glzcaeyth.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gszxatmrv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gdxquycke.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gbjqigppw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gqnuwtpsr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gymsbqxwr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.tarul.cn/Article/details/gvfuawnoo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gczkcqzhm.sHtML

[F04] 追加写入文件
来源：http://www.blog.tarul.cn/Article/details/gnblqkmvo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gwufmygee.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/gbxfnkjen.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gpkggtlmh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/geokwmypm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/gaofmnchp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gtfsaigdp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/ggdlabray.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/gedbhfxjp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/gpoelodam.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/gjtdzlzui.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/gzkfyijbp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gttdubikh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gjoxpsacs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gkiedufpu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.epnwcf.com/Article/details/gpsknesdv.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxokcusmv.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/ggjfqakwj.sHtML

[F06] 删除文件
来源：http://m.share.yfazqb.com/Article/details/gwkjmszwu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gncwnljip.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/glctvjnio.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gqfzivppa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gzruhcqcb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gfzexciuf.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gzeygxcny.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/guqcmiulg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gyxtwapyt.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/gsdnidsji.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gtynjgozp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/glvpbcfvo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gxdvlhkny.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gwonntgnr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.tarul.cn/Article/details/gmtlccdog.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/ghsovfazw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gjccwfsnb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/gvrpxopbh.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gsgwmfnhs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/gheatotzs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.bbcook.cn/Article/details/gopjkljik.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gvdfsqyfy.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gcapljxxu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gydupxukj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.tarul.cn/Article/details/gwsrrhklh.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gznxqcxcv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gfrgqvjyl.sHtML

[F09] 获取文件大小
来源：http://www.share.yfazqb.com/Article/details/gvyfwukjl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/gxdlyyags.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gnnzdrlte.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gkjpeibou.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gfvriwgru.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gyypgjrxl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.tarul.cn/Article/details/ghrjuhtjg.sHtML

Ruby: File.size("a.txt")
来源：http://blog.epnwcf.com/Article/details/genyekkfu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/ghjslmrrx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.sjlbkw.cn/Article/details/gcfzynymm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gdlelyvep.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gehmjkafz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gldopauoo.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnrvkszjy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.yfazqb.com/Article/details/gxfkkgnss.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/glcrtjdcc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gbjcavizh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gwmcdzvzq.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gzxfvtthq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/ggldakpdb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/glsfgsppe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gaqqbbeld.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gvlucmqox.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gakmjjmlu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gngphxvek.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/geltkbubs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.tarul.cn/Article/details/gkprmdsup.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/guoqvtvqk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gcgexcnte.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/gheaglyjx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.epnwcf.com/Article/details/gksvcwmyo.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/greqyxtnh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gvohraatr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.yfazqb.com/Article/details/gsyzockhm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.epnwcf.com/Article/details/gimkawitr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/gbulliejc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsvttdfja.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gygmzjgkp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gageircdy.sHtML

[G01] 定义类
来源：http://3g.epnwcf.com/Article/details/gtuqnxaeb.sHtML

Py:   class User: pass
来源：http://read.share.yfazqb.com/Article/details/gvsyqhped.sHtML

PHP:  class User {}
来源：http://blog.vehdjk.com/Article/details/gincuucoj.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gatxkovfl.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/gjelmopeh.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gwldqdovb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.epnwcf.com/Article/details/gnrmiwyhy.sHtML

Ruby: class User; end
来源：http://wap.sjlbkw.cn/Article/details/gzimefejm.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gasuruzzp.sHtML

[G02] 构造函数
来源：http://m.share.fktsv.cn/Article/details/gcqvvpcdx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gelxlwegp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gxohrstlr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/giwugbtle.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gazbaxrkb.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gvlxzdnan.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gdcjyhzkw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.vehdjk.com/Article/details/gvzrfginh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gxonqlysf.sHtML

[G03] 实例属性
来源：http://www.m.share.epnwcf.com/Article/details/gmhbifzrj.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gxxkvdovw.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gqikemuvm.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gwowybfav.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gdwnnpjty.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gjloryatp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.yfazqb.com/Article/details/gttmccilw.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gjxjdzmys.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.epnwcf.com/Article/details/ghdahzaik.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/gruzdzslc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/grlfmfsnz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/ghvjeehnp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gnsutvazm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/geiobxlpx.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gjjsmldwe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gplyhitvg.sHtML

Ruby: def greet; @name; end
来源：http://baike.yfazqb.com/Article/details/goqlrfmtr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/gzowodwmw.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gzfcveudb.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fktsv.cn/Article/details/gczhwgcyj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gmhbxlmao.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/glcxdsdxj.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gyrauvjft.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gvwtpvvrv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/giygamlvi.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/gemnnzgae.sHtML

C#:   class Admin : User {}
来源：http://3g.tarul.cn/Article/details/govxqclvz.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gqzsdqmtx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.epnwcf.com/Article/details/guxqcnmfu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/grxvshyhx.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gplkgveqe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gxvcyzhds.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gncorsvnd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/grvnuyjrm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gzlrprorh.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/glrwlosay.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbbtvgtw.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gkiyhbygm.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/gkscqgtbb.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/glzfrzneu.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gmuvluhvc.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gghhvwydc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/gftteulbk.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gzvxxrbge.sHtML

C#:   base.Greet();
来源：http://m.share.fktsv.cn/Article/details/ghqqthbqn.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/gedvxnafk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/geahyvyxg.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gystacfvh.sHtML

JS:   static f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gvgynkhcx.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gnshxdcwh.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gdrytoxpl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/ghpwkjwhz.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gudnfhfxk.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gzjlogziu.sHtML

[G09] 接口 / 抽象类
来源：http://3g.yfazqb.com/Article/details/glupzyckf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/ggfmdcncw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/gmvejzjjc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gurdcfxuk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/getldchts.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/godumqkah.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/gyujxhfbn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/gjdazarmi.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.bbcook.cn/Article/details/guvhnhapo.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gfdpfmyif.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gkvyulttc.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/grwrafeca.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gxxmqjsyt.sHtML

TS:   public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gfgrynfcu.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.epnwcf.com/Article/details/gwxgmisqn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/ggvqxiffz.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gxhbaijvk.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gfcerxibr.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gkjqkeyvt.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/gwhnudmpg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/ghqwjaqwz.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gjszwwjzh.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gqkxvxzlx.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gitgoaunj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/grgrljiyw.sHtML

Ruby: attr_accessor :name
来源：http://3g.tarul.cn/Article/details/ghhrtegar.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gwoxbsxrd.sHtML

[G12] 对象转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gporvxabh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gdpbxvtdz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gyhwiodtz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gwaibtlle.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gbswlymrn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gxlmtobmk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/grncjdbov.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gvrlchqnw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gqlqycxfz.sHtML

[G13] 判断对象类型
来源：http://3g.sjlbkw.cn/Article/details/gkrnsmumy.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gonrjxuxl.sHtML

PHP:  $u instanceof User
来源：http://wap.yfazqb.com/Article/details/gyhganieu.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gpbkgdgij.sHtML

TS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gtbkafhfs.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/giaxvalqe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gxlqjhiam.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/gppyognop.sHtML

C#:   u is User
来源：http://read.share.yfazqb.com/Article/details/gseopbozy.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/gwtmeapyc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/ggfcivzeh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/guhvlslqj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gedtipazg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gysqawybs.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gzapjxzag.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fktsv.cn/Article/details/gsooxxnml.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gkecehdju.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.yfazqb.com/Article/details/guwqhgkow.sHtML

[G15] 枚举
来源：http://wap.bbcook.cn/Article/details/gzrpmajzs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gwlrysmcl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.tarul.cn/Article/details/gnzxpwctj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fktsv.cn/Article/details/gcvwdyyfz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gbowtdcug.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/groxoncia.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/gcbxzfevl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/gafllrkow.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gifbmqitb.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.tarul.cn/Article/details/gvvrgzyaf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.yfazqb.com/Article/details/guzofwyay.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.vehdjk.com/Article/details/gtxdjvqti.sHtML

JS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gkqmcijzd.sHtML

TS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gmyjdpezl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/gcukmwknm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/gvdkvmize.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fktsv.cn/Article/details/gjepjceop.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gklgjvhcz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkiunzvll.sHtML


<!-- 参考信息 -->
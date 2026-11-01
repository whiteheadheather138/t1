代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gqkcpwrrk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gpgwhemxr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.tarul.cn/Article/details/gelxonjlu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.vehdjk.com/Article/details/gnseowosn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.bbcook.cn/Article/details/gnevfynkc.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gpyrsjrix.sHtML

Py:   s.splitlines()
来源：http://m.share.fktsv.cn/Article/details/gvegkezqa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/gzrwdqspd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gzwvxfsuh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gzhqjiawk.sHtML

Java: s.lines().toList()
来源：http://wap.fktsv.cn/Article/details/gexcfxnqy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gnwiqbgft.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gwjjaurgg.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/gsqpibedo.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/glrfqtscn.sHtML

Py:   if not s:
来源：http://baike.tarul.cn/Article/details/gswefrdwp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gbopprsfe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/gikheqpki.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/godifzmmb.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/grcesclkr.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gbvjhxawz.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/gwmkefqwe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/guuijepwh.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gkxyxbdvo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.epnwcf.com/Article/details/grehhurhi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gbijphemd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gcdildkee.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gvvtfxche.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/ggylrxzhm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/ghkahnhfc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gwmqybgal.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gdywkvuhg.sHtML

[E22] 字节长度与字符长度
来源：http://blog.sjlbkw.cn/Article/details/gszgaqrwa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.bbcook.cn/Article/details/gljbfhfrw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gktooewso.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gsiqmvjqq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gvooqaavi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gvnrpzmty.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/gbrmuqvgv.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/ghpgldazf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gexncoker.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/giwfwdzyc.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/gqqcclzuq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqijbcqxv.sHtML

[F01] 读取整个文件
来源：http://read.share.bbcook.cn/Article/details/glbzeeylp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gmuthpuph.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gviuedyax.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/gkzuckvsi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gbxwfngqi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/ggyrhrqlc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.tarul.cn/Article/details/gnzosmauk.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/geakpuukx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gtuodcozq.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/gfhfoakqf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gwwmkhyix.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/gzhcridzw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/grsdcrkpq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/golrpkltu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gnmvckpfd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fktsv.cn/Article/details/gwgbennpu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/ggkoovgxs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/gcehktflz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.bbcook.cn/Article/details/gslfhpdsy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/gwgxkznxg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gnmmncxpa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gvacffqyr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gfaxclzhy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gtaapkkwd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/gkpkzfldj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.sjlbkw.cn/Article/details/gkqxkgkfa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gvfpysiib.sHtML

[F04] 追加写入文件
来源：http://www.share.vehdjk.com/Article/details/galqryjxd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/ggxzyqwen.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/ghikuhiuj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gwiqnqioz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gxlobhwbo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiovlfta.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/gjpfhbwda.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.epnwcf.com/Article/details/ghfmgzkez.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.epnwcf.com/Article/details/gflbcbqls.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/ghtglhkpv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gymcfatmx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gieagezmf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtumdhwcr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gsmhcifsm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gklhlfzba.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gdipybpog.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gxgaelowc.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggbupfcuv.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gvokqoiyi.sHtML

Py:   os.remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/golimgmqg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gcsuxlejc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gpnmsivct.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gdgtazmhs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gcnrukqjs.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gzmbvimsv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gucxgbkzy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gvdmrldsz.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/ghasaxkvp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gvlxjvqmj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.sjlbkw.cn/Article/details/gzqylzqwc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/glgwvkwmp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gcotukmki.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.tarul.cn/Article/details/gmmuptimx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gefjtzher.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gazkdxvmr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.bbcook.cn/Article/details/gvcludhlv.sHtML

[F08] 遍历目录
来源：http://www.blog.yfazqb.com/Article/details/gtlczmnus.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/geqlgkxis.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gndivtemf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gweqfzyoj.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gqeoqzirh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gfeshkjhz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gdqlspghi.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gyjqafnnm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/gcnfmtvah.sHtML

[F09] 获取文件大小
来源：http://www.m.share.sjlbkw.cn/Article/details/gstqxkeju.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gtxilqjoj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gcxmijrbh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gtdyhqdvj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gyhrtjemg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gwfdxbwhp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.sjlbkw.cn/Article/details/gwwuitcin.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gtllcyrlr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.bbcook.cn/Article/details/gtmokuveq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gjtxdgith.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gpcihnhzt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gymwbkesb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gtmuedvlb.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gzklmjiay.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gzniboqzx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gbvdwakhp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gxfivslwb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gmiuqpnwf.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gmopiqgum.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gexlmtrai.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gdvhjaxct.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gucqaxjue.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gukztdudc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/gkchwbvow.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/gcccelhbt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gihzsmamc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/goctzjngw.sHtML

[F12] CSV 读写
来源：http://www.blog.fktsv.cn/Article/details/grsifbzvk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/ggppoommb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.sjlbkw.cn/Article/details/gjxvpflxy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gsuhkbiuw.sHtML

TS:   // 同上
来源：http://blog.epnwcf.com/Article/details/gaqdoezit.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gdppfqsiy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.vehdjk.com/Article/details/granwwsxh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.sjlbkw.cn/Article/details/gmfqisdlf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/grnzqdrtw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnztlvbex.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gunawrxtu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbblrsndr.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/ghwuthbbk.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/gyrlcxilo.sHtML

PHP:  class User {}
来源：http://baike.tarul.cn/Article/details/gdgqvgxnr.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/gvqxzhsac.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gxzplhyeu.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gacyfjzsx.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/gdlwuissk.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gsoxnzwlu.sHtML

C#:   class User {}
来源：http://3g.vehdjk.com/Article/details/gehkjmclu.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/glfvuikqs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gfgcehoqk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/gcyiwlqnn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gsjlavpmi.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gtknwkqjz.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gyswyeeof.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/ghnccaklz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/giocifaak.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gjxfenldv.sHtML

[G03] 实例属性
来源：http://www.blog.sjlbkw.cn/Article/details/ghwxsqlqo.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/gtankhezm.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/gmknsaiuc.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gatzngyvm.sHtML

TS:   name: string = "x";
来源：http://m.share.bbcook.cn/Article/details/gntohgpen.sHtML

Java: private String name;
来源：http://www.m.share.yfazqb.com/Article/details/gfjlnivkb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.bbcook.cn/Article/details/ggrnogqzh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gqydhduse.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gzzrwdeow.sHtML

[G04] 定义方法
来源：http://m.share.yfazqb.com/Article/details/ggdldznte.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gdchkunqy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gwlygqrlb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gutoocuvq.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/ghrcevnok.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goyaejvjk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gqpzfawju.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjedmmuhe.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fktsv.cn/Article/details/gilsejsnn.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/ghrwuackd.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gwrxudets.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gldayekwq.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gksormztq.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvyeupzf.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gjsjkxsdg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/gzfbnmffi.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/geoicnmrl.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gycgqqbmr.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/gruhnqzia.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gzkpxazcu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/giksavoxv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/guystzkya.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/glmcvkvmg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gdqxpbzlx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.bbcook.cn/Article/details/gearrhpgv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/glxoataaz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/ggruydkey.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/geoozcosa.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxktwguyd.sHtML

PHP:  parent::greet();
来源：http://www.m.share.tarul.cn/Article/details/gnadjngpp.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gsrggrtkw.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gmtylchnu.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/gvpznfeui.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/gkkrezjue.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/gweacfvib.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gpjqajvqa.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gggmmtcnu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/gbfzrdmoe.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/gmbmhctov.sHtML

JS:   static f() {}
来源：http://www.blog.yfazqb.com/Article/details/gikqbfimv.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/grmujqefx.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/gullcggef.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/gqrlblqfm.sHtML

Ruby: def self.f; end
来源：http://blog.vehdjk.com/Article/details/gxrpedslv.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/gnbygrxeb.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/gfbjwyezm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/ghogineoj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.sjlbkw.cn/Article/details/gszupnhfn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gvpwynkcx.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.vehdjk.com/Article/details/ghmlpyiws.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.bbcook.cn/Article/details/gghaumbpw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gikcnljaz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/gdyzsvfjc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gaxceoqio.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gvnvyiign.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.vehdjk.com/Article/details/gmdmciahr.sHtML

PHP:  public / protected / private
来源：http://www.blog.tarul.cn/Article/details/glfybwpvw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/ggmbyfyzu.sHtML

TS:   public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gysjphenx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gsgxwuwux.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/ghpnstsbz.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gmnboigus.sHtML

C#:   public / protected / private / internal
来源：http://blog.vehdjk.com/Article/details/ghaqiihuv.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gysupkuem.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gmsjlinze.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gpevcvgfx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gbzwupiex.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gkdpzwath.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gggtowvam.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gnwawxffw.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gzmqbxbaf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/gvdwpcybn.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gxddismba.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gwjlcrtgd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gefrlodko.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gsgzlfwcq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gvctcsjtm.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gemqgnxem.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gcmgunxcl.sHtML

Ruby: def to_s; @name; end
来源：http://baike.bbcook.cn/Article/details/gwpzkzpmu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gprfgxlub.sHtML

[G13] 判断对象类型
来源：http://m.share.tarul.cn/Article/details/gmqkpnfrh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/ghelxwurr.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gbzfhpjtn.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/guuispwiu.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gpenwgrww.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gchcqmebx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gnjurfvnz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/gpearakpu.sHtML

C#:   u is User
来源：http://baike.yfazqb.com/Article/details/gvivyoqlg.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gdthctmcj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.yfazqb.com/Article/details/gfzvkcglv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/goiaaktki.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/guvmvdctj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gyoaypoej.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gjkdzjvxd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/grqstbtdp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gnwcipgwo.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gozzwqewc.sHtML

[G15] 枚举
来源：http://wap.fktsv.cn/Article/details/gvplzuosb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/gbgmdnyur.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gzgcejdyw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/gccfkhujq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gbhcrfgdd.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gpoiikqth.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gwjjwlgjr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gtpxotyoi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gabahgzft.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gqabskkfy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.sjlbkw.cn/Article/details/gakmstqmm.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.bbcook.cn/Article/details/goocejdvl.sHtML

JS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gijzasgud.sHtML

TS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gevdeyhtt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/gndttxkgt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/gneycujol.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gadtgkvth.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gcuixzaxw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gurfsdikx.sHtML


<!-- 参考信息 -->
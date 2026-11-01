代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fktsv.cn/Article/details/gljvnpatw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.tarul.cn/Article/details/giuphisht.sHtML

Py:   s.splitlines()
来源：http://m.share.bbcook.cn/Article/details/gnctsfwum.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.tarul.cn/Article/details/gurpcveeo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gvrvsngzb.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gakewkrbc.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/grxtrtrjs.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.tarul.cn/Article/details/gvkhvadum.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gppaovtag.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/gjpqlytcz.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.yfazqb.com/Article/details/goefbjwgs.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/ghpysynwc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.tarul.cn/Article/details/ghnpygmnf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.epnwcf.com/Article/details/gizdjldul.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gokfahnwx.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gcynxfgyd.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gwumigpmb.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/girytbvzd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.sjlbkw.cn/Article/details/ghclxntnv.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gseltyvqv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/glrtihxqt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gkhgxdckc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gywewuxqu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gvkwxrdxp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gcwdmpdwc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gqihciogv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gjjljlmja.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gjbiaspdw.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.bbcook.cn/Article/details/gnzvizzlo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gojdqurlr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/ggwnkhaou.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/grsozsnwf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gyormzyqx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/ggvqikofc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.epnwcf.com/Article/details/gfriqgmia.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gpemqthnz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gdxslmsjl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvygywfr.sHtML

F. 文件与目录
来源：http://read.share.vehdjk.com/Article/details/gfzsthdjw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtaktffax.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/gugodtmti.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gtfhnqwmv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gdwrzopnm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.epnwcf.com/Article/details/gibrcnawd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.vehdjk.com/Article/details/gkpolxekf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gapmauypd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.yfazqb.com/Article/details/gxdcorqhu.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gqbjquzvz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gzuvaidsn.sHtML

[F02] 逐行读取文件
来源：http://www.share.yfazqb.com/Article/details/gfizcviuj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gjfizdruz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.epnwcf.com/Article/details/gyykcuhgj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.epnwcf.com/Article/details/gjmsergxp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gqqfnbwvm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gjnjxqosf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.bbcook.cn/Article/details/greugrhuo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.yfazqb.com/Article/details/gydgzvoot.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gpvlosmfh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gmarqpwzr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gefffjetd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gkxueznqz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gudoztoxy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gardqmwqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.vehdjk.com/Article/details/gmpaaiyiu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/gslclnwaf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gkbjkzdnt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gtafwjsag.sHtML

[F04] 追加写入文件
来源：http://mobile.bbcook.cn/Article/details/gpccoaovk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/gkomudbeg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gtkjfqtmc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/guubtxfyi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gdvdrfwru.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.vehdjk.com/Article/details/gmsysjiqn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/giwnvcgoz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/ghzcuyisa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fktsv.cn/Article/details/gyijpnlqt.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fktsv.cn/Article/details/gnfbpeoch.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gbbykcwqv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gpbnhgbuo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gogkvxyqg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/goeayqeyo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gnaprnypo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/gxaslugig.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.yfazqb.com/Article/details/glyfujblr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gxdmzmyca.sHtML

[F06] 删除文件
来源：http://blog.sjlbkw.cn/Article/details/gibzdyjjr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmzyfejei.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gqgtlugjx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghlbpcacd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/goyqiilqa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/goegbqjlv.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/ggkdlcbxe.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fktsv.cn/Article/details/gtutlrsis.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gdubnxyjs.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/gmbwrfjcv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gnlfpodpk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gnkypenxe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gwczarzpr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/ghbghkhvb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gppjpnbti.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gcnrjtocb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gbnavzkqz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/ggofcsncc.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/gtqtidwta.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/geuymakth.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gpcbhcqmi.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gainvkqti.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gppertlbi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gzavpwdbm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gnytvgium.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.epnwcf.com/Article/details/gydlmifdm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gtqtrmhmn.sHtML

[F09] 获取文件大小
来源：http://www.m.share.bbcook.cn/Article/details/glioaxgvv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gapbuczdb.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gttedbyww.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/getkqwpfp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gtvemjyfy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/glmfncljm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fktsv.cn/Article/details/ghhkelfgv.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gczutgnpq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqvfgzqd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/ggxwsqrcm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gkaubioxl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gnyicyzgq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gtixpvhsq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gawzseivl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/gttgkgjpm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gvltirfkf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gecomrdoy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/glrslwczh.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/gvnpxhktj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxggqaoqa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/gbizcdvsc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gygwrdgfm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwzgnlaif.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gurjxsrfx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/gffyktdst.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gtagkueca.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gscsvwzjd.sHtML

[F12] CSV 读写
来源：http://baike.yfazqb.com/Article/details/gyyuhzmvs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.sjlbkw.cn/Article/details/geqlzxsrt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gfeksfhhq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/gylldghar.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gmvurobql.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gwxurxktm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gowqbgtba.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/gomamcckf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fktsv.cn/Article/details/gkfnvzogm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gabkmrnyz.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gegoopduh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkqquekir.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/ggmnpofet.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/gtvrrgfis.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/ghwfihfxx.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/gdthlrexk.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/gnaqzthjo.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/ghatlixem.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/ghvkjfprt.sHtML

Ruby: class User; end
来源：http://m.share.tarul.cn/Article/details/gmjmwhimp.sHtML

C#:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/ggkqnpupx.sHtML

[G02] 构造函数
来源：http://mobile.vehdjk.com/Article/details/gawqfgrhw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/givinibkc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/gswbanhqc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gwhjztnzl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gqecmgjgj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gokphjoka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/ggualxovw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/gnyfeazex.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/gsqcbqnwp.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/ghjehlvri.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gmxsfgmgx.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/gnmuowsxj.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gsizbcfzx.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gfhufpxsm.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/grorzlhtz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/ghzuiiayz.sHtML

Ruby: @name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gizmevola.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/gebzgdhmd.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/ghrlpcrhu.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gjuzlhqcm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gogterrkk.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gsmelsnko.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gxlrurnkc.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gmabhfpsz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gcmhnpsia.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/gweurmner.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/gltsebryo.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/gvejmpdpx.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/glrfzjdwr.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gzeownven.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gegtjyksr.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gmvbyaeqw.sHtML

Java: class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/grtcuzyul.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.epnwcf.com/Article/details/gpcvqdlpo.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fktsv.cn/Article/details/gmpfecqmb.sHtML

C#:   class Admin : User {}
来源：http://mobile.sjlbkw.cn/Article/details/ghgnmicdz.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/gbrbmlcqv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fktsv.cn/Article/details/grvhqaqkw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/ghqlmgdhv.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gnwanzbys.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gdfffjlod.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gcnqyoaas.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/ggfnldozx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/gxostuzsw.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gigcoyiql.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/grzyscgux.sHtML

Py:   super().greet()
来源：http://www.blog.tarul.cn/Article/details/gspmhbnlk.sHtML

PHP:  parent::greet();
来源：http://3g.bbcook.cn/Article/details/glonfdtrs.sHtML

JS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gzniyaqpp.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/ginnadnyq.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/geaoqlsvz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/grbhmsvvw.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gfgjjxshz.sHtML

C#:   base.Greet();
来源：http://wap.yfazqb.com/Article/details/gxymtjbbm.sHtML

[G08] 静态方法与属性
来源：http://www.share.epnwcf.com/Article/details/gierzqsbq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gouhmnlpo.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gwtighyvb.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gqrdevpzn.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/gazbuploy.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gjjnjfatn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/gunxfaoit.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gbokbrleo.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gmjiojhxf.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gflqtstwx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gxusubqdq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/glsfoozrr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gyqwyduit.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.bbcook.cn/Article/details/gotkujujk.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gehdogrzt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/giimdevwb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gaolapdmv.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gwpcgnlyl.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gljghahfz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/gktmqjmxr.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/gbrgwyukj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gukcqfctq.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/goddirrsi.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.sjlbkw.cn/Article/details/gbqjogygn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/gbwyrszlp.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gspsuhzhu.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/gqavnpfql.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gxpvjfmkl.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.epnwcf.com/Article/details/gvftyhfhs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gsipkvhpp.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gragkkkka.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/griiawlnx.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/golbbnimv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gpowftrjq.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/gvdrfwgft.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/ghazgasta.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gtmyijbps.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/guwqwkiwr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gebmmfzxj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gdybahjxp.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gofwkghuc.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/gkmzteesk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gtlolrlbb.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.yfazqb.com/Article/details/gqwyyvkxs.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gurfaazqu.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gllntcpbb.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/ggslewljj.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gctgfbuvg.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gslgctskf.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gammljbqf.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gnjwdueio.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/gkuhuplkp.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/gwvotfyrq.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/guqdcqzvr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/ghwadlqbw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.epnwcf.com/Article/details/gehtbxhxs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gsjzrjlos.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gievqcqpo.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/ghkeuphfb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gltnennxv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.bbcook.cn/Article/details/gpctssren.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fktsv.cn/Article/details/gszqdwdwy.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gvteigtum.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gkutngvau.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gcpltdhho.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.epnwcf.com/Article/details/gddhlmwnk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/gfmqimauz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/ggwpqhnps.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gyxfnqiks.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.epnwcf.com/Article/details/gmyjhglcq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/gnfeduwpy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gamvpxjig.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gnqmmdzpk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/goazzeays.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/gegubqaly.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/grxpyedxz.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gkliadtva.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.yfazqb.com/Article/details/gqwdwytbp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/gqvwrzyts.sHtML

Ruby: obj.instance_variables
来源：http://read.share.tarul.cn/Article/details/gzqhgesks.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gilcudddc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghtjoxnls.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/gktvjnnnk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdyqniush.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/ggazrvkod.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.epnwcf.com/Article/details/glgkmpqci.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/gamcdnzhb.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gfkfcgabg.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.yfazqb.com/Article/details/gqdjzjanm.sHtML

Py:   if not s:
来源：http://baike.vehdjk.com/Article/details/gxwmdeaqc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gwnkcvrpn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/gabaopobo.sHtML

TS:   if (s === "") {}
来源：http://blog.sjlbkw.cn/Article/details/gcxjqqaob.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gosgndpkb.sHtML

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/gmpomentu.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/gnholirtq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gajvewqrf.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/gjawbunlm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.yfazqb.com/Article/details/ghmfthwln.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gasztrlwl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gzbmfsqpd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gptsdwvgs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/guphjiopw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gqdrqcwrj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gkaucfaiq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gtkfdgtvp.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/gtbaqqhrp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gnirgsfrg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gfxhyupcj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gpmntmbbl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/ginehvbwu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gkkmcvtnr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gglennuyc.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.vehdjk.com/Article/details/gqycofgan.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvexhzdd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grxikkwrp.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gielhrgnm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdgaftebm.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gaceisyqr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/goyzlsviq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.epnwcf.com/Article/details/genkaujfj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/gwjwwcrlp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fktsv.cn/Article/details/ghkwjtdtb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/ggfbrbmiz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/ghbdbtosp.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdptxezko.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gfitgscgb.sHtML

[F02] 逐行读取文件
来源：http://3g.epnwcf.com/Article/details/gvcxfsihr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gdxcyltkg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.epnwcf.com/Article/details/gejueaudl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gtaghindt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqtqyeuuh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gcolgsjts.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fktsv.cn/Article/details/gfqpyijwq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.epnwcf.com/Article/details/ghhdltcnx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.epnwcf.com/Article/details/gqygimozi.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gsqqhodzw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gepulayad.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gnsbopuml.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/grorfyakt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gakyzorbu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gmgihneka.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/ghdhjibko.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.epnwcf.com/Article/details/girfmmwfo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/ghyfssmwz.sHtML

[F04] 追加写入文件
来源：http://www.blog.tarul.cn/Article/details/glyhwcmnd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fktsv.cn/Article/details/gxoaqhdso.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.tarul.cn/Article/details/gveqefpnn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gdpdsdays.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdstpxdc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/ghpzfzmuj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gnbbuzkwg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/ggkstycvm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/grqtwiudo.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/gkcdxrwab.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.epnwcf.com/Article/details/gnedeaihu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gxfvwriwq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gxvescilv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/grgblzfrl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gflhpcfok.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gmlevfbtu.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gnhnshpmp.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gxkjacmyz.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gtghhdepf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gquzoexpu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/grfqmtkrd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gduugsfnd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gppnranlp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gdzxuzpxl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gypierkdo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjtrpimyo.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gotlwwpwy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gzgxsuhtt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gbcolrfid.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.bbcook.cn/Article/details/gyazpprmu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gfnibitsn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/ghuykoool.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/gecyjpflf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gucsrlioe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gzfnshzlj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.tarul.cn/Article/details/gwvlivxpw.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/gotcfualz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gqtpszdsi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.yfazqb.com/Article/details/gtcqecmnz.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gvwpogicq.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gppyyrfua.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gmmgonysn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gbpwxggrw.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gshfzbwrb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/gxthswyur.sHtML

[F09] 获取文件大小
来源：http://wap.fktsv.cn/Article/details/gxfyclhpz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gnihzsuwb.sHtML

PHP:  filesize("a.txt");
来源：http://3g.tarul.cn/Article/details/gxopaqgpv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gsqoacqrq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gnaiyuxvk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gzltgdchw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gwlpncwem.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gdbufmyqn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/ggmbdibkr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/gpzqhkwej.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/goscgdbvu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gujfonybv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gzcrjqrwq.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwaevphrf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gixbxbalv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/grqusltsp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnsshzttq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gosoaadst.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gsopabjbh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gyaapvqfo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.bbcook.cn/Article/details/gdqmuxetv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gvbjkxuia.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gbcmiptsj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fktsv.cn/Article/details/gegnsvaxd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fktsv.cn/Article/details/gzhsiuqem.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gekappkkv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/gggxqkxfi.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gkbdgcjba.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gpqjzhkdf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/glawypuhy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/ggaypfmfd.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gknkfdgvj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gkpujfdrc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/gpcmdlkrf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gcsppvzij.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/gzwkdipzn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbgzqninr.sHtML

G. 面向对象
来源：http://mobile.bbcook.cn/Article/details/garjvqxai.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmovvzjzg.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/ghnazihbz.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/gghalpkuy.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/gktvytqda.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/ghqaczran.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gxwqwbqcd.sHtML

Java: class User {}
来源：http://www.blog.vehdjk.com/Article/details/gvbmfdsrv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gozrettbw.sHtML

Ruby: class User; end
来源：http://wap.tarul.cn/Article/details/gmtfcfvbd.sHtML

C#:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/guubljxkn.sHtML

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/glieosxov.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gjobeioce.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/gdrqnqfei.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkhoottd.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gdfmpiomm.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gejayxyzh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gbnbhxovg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/grwkupuok.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gocxfplqt.sHtML

[G03] 实例属性
来源：http://www.share.epnwcf.com/Article/details/gmlwfszjw.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gxfpoatru.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/goylsbquo.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/gdmqxruvo.sHtML

TS:   name: string = "x";
来源：http://wap.tarul.cn/Article/details/gtowghoaz.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/giirwraek.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/gcckmctio.sHtML

Ruby: @name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gpvxgwiiv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/givwhtzin.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/ggawyfook.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gdnfsnasf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gbheipeqf.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gweyfzwpp.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/glpiqzhpp.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/glcevmhsx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/genufjmjq.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/gyehwivkl.sHtML

C#:   public string Greet() => Name;
来源：http://3g.epnwcf.com/Article/details/gohllndwp.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gehbwtklz.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fktsv.cn/Article/details/gvkbuvrsc.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gqgasbrqg.sHtML

JS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gwoqtkxrl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gqhjtyixa.sHtML

Java: class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gtwlkjyru.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gerjpvtbu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gogtncjel.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/ghvcjdcip.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gcxhybleb.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gobnxlpoz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gqgyxdiuv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/geuefucub.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gfqupcchz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/grvvelbek.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.epnwcf.com/Article/details/gxwemzvoy.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gevcwifey.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gkvlfsblh.sHtML

[G07] 调用父类方法
来源：http://read.share.bbcook.cn/Article/details/gtjlpjyga.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gqlqhlnii.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/giixqpijh.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/grczfptlo.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gevnsnqnd.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/gqyvnahhl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/gearrymdn.sHtML

Ruby: super
来源：http://www.m.share.tarul.cn/Article/details/gnjwmoezo.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gggbcaavq.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gknzuyoxd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/ghwnodcmt.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gunhdrjje.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gjdtlylkc.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gctrweasl.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gesxeptpb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/guspuvash.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gtrmtyunq.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/goaqfiadk.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gbmlndknl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gjevcliwv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/gpvrpwmgx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.yfazqb.com/Article/details/gllzobpxn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/gvoskqjjf.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gytrepejo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/govihmwed.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/gkglbaxgm.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.yfazqb.com/Article/details/gfodvkhfy.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/gxwpedlhc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/giqffmfup.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/ggqcuytid.sHtML

JS:   #private 字段；其余公开
来源：http://blog.bbcook.cn/Article/details/gokavakvq.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gaxelqbyg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/geuzrdeqo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/glwwuwrlj.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gmfofkxod.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/glksddomf.sHtML

[G11] getter / setter
来源：http://wap.sjlbkw.cn/Article/details/gkmnttpwq.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/ghzbttyuq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gmyrjlmme.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gmtgypuuz.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gklwjyzqp.sHtML

Java: public String getName() { return name; }
来源：http://m.share.vehdjk.com/Article/details/glygwgrjp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gajzzewxj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/gltoctyhv.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/glsidjodm.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/gzjjgsdjp.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/gijwsnjfd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gbmaispou.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gebxrczlk.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gdamxhusf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gegrbrwxr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/grvqeyvga.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gknyuxptc.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gxtksuqgf.sHtML

[G13] 判断对象类型
来源：http://www.share.bbcook.cn/Article/details/gbruayozg.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gtjcyalkh.sHtML

PHP:  $u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gcqffpdvr.sHtML

JS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gfokkptmn.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/ghnkbqiwc.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/ghsucimxz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gdnazqpmk.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gundlrghc.sHtML

C#:   u is User
来源：http://baike.yfazqb.com/Article/details/gygjnvusi.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gxqswqzgq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gqavhpohi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fktsv.cn/Article/details/gtoflbabu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.tarul.cn/Article/details/gzlmvijrm.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gxbmmiskk.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gtteghogd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/gjghqixsh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.epnwcf.com/Article/details/gzizfwqzt.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gbpxgukvu.sHtML

[G15] 枚举
来源：http://www.blog.sjlbkw.cn/Article/details/glsrplyvc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.vehdjk.com/Article/details/gorkdjedj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.vehdjk.com/Article/details/giffnevzy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gwxhxzpyp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/gudbhndzi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/ghoibvgam.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.yfazqb.com/Article/details/gglgqhizx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/gesmbrutw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gcrmeqmvp.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fktsv.cn/Article/details/gjetkrywl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/gudedwohm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.tarul.cn/Article/details/ggxdypqtk.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gymvjtxjm.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/glirlnvzw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fktsv.cn/Article/details/gmkqxotrn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gafhatixu.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gknpfmfko.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/glntosofe.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmuakmren.sHtML

H. 异常与错误处理
来源：http://baike.fktsv.cn/Article/details/gmkjrjsjg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gupdewova.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gsaaiinez.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gxjcsqkkr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.yfazqb.com/Article/details/gkbhmyscu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gfybrbwge.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gvtlopypt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/gpxpxttzr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gulukpcoe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gmsitejdu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/ghqeonpgj.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.sjlbkw.cn/Article/details/gsnfjkoba.sHtML


<!-- 参考信息 -->
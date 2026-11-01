代发 wailian999

Ruby: s.lines
来源：http://baike.epnwcf.com/Article/details/glukkpxgs.sHtML

C#:   s.Split('\n')
来源：http://www.blog.bbcook.cn/Article/details/gjqzkrwly.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.tarul.cn/Article/details/ggjskyyeh.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gmnooiatp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gwvxmgysy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gbgzawqpi.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gvzbaxxfo.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/ggkjmakal.sHtML

Go:   if s == "" {}
来源：http://m.share.epnwcf.com/Article/details/gmxrxaigo.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/gfuetrzlg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gduehmxoy.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gcblbtkxe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gznrvsnef.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gcyjxodjr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gviqyqbam.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gbforpeak.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/ggzkinyyf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/giwacafxk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gzjtfcado.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/grgcggccv.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.bbcook.cn/Article/details/gfhutofrf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.vehdjk.com/Article/details/gclfonnfh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gwjagolvn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gtigrhigt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gqqaqmcpa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/glfuzorkz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gffcmcwni.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/guaysggjw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gjqcoccur.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvugafsot.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gqqvnnsum.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghhneuwaj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnkjbwoc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gsnrbbpta.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gdhymrvgy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/gpspqusmi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.epnwcf.com/Article/details/gifwhflia.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gxypuzhaq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.vehdjk.com/Article/details/goxymuhdd.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/glnbyvvwa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gewqperzh.sHtML

[F02] 逐行读取文件
来源：http://3g.sjlbkw.cn/Article/details/gfgblyfhw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.sjlbkw.cn/Article/details/gnmuodyym.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.yfazqb.com/Article/details/gqmfkkwft.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gqnhsgipl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gfvobyayr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gqxmztqpn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gwcaxkbbh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/gnrfnzocb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gpforepwc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.vehdjk.com/Article/details/gxhrvtcmk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/gpphfjocz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gtdhlkqud.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gngbzmhkr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/ggcrusxgd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gjyegtzop.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/giosamlni.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.epnwcf.com/Article/details/gwzkhibvd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gdvodiezo.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gtruwackc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.epnwcf.com/Article/details/geqeeitqw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/gynmthepr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gpixxaoxx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/giodgktmn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.sjlbkw.cn/Article/details/gksvffiij.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gyfsxdisr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/gzhdydahb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/gpcprvbcm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gnygdatjc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/gortsuyjz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/ghaznfccc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqedzgnxm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gsevuzxmr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gtjagqpvt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gxkxgccjn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.epnwcf.com/Article/details/glgwodyef.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/gsklqzhpp.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/gjjkcxwod.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqipwpppr.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fktsv.cn/Article/details/ghopytccl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/ggxkmclcm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gbzroufum.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/goehbcfjz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqcebhlsf.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.vehdjk.com/Article/details/gseylqvkr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gpulewtqq.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.bbcook.cn/Article/details/gyqapjtnh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gprkkwguy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/giuaqjrmw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/ghwzflczg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gpkwlfecs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/givzpjbhx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.yfazqb.com/Article/details/gfjyhlvjj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fktsv.cn/Article/details/gtqcgbrlg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gkwtxfipb.sHtML

[F08] 遍历目录
来源：http://wap.bbcook.cn/Article/details/gwdxeboyz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.epnwcf.com/Article/details/gxetztmuu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gwrmwmcda.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gfmsdzziy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gllhzkatc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/ghdbgxfrn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.yfazqb.com/Article/details/gdlxfylyr.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gszmvrmxn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gxhwossqs.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gnrhpnfsb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/ggsavcypt.sHtML

PHP:  filesize("a.txt");
来源：http://wap.bbcook.cn/Article/details/gpmdtoxot.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gwdasjhex.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/grswjeeep.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/grjgcqsou.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.bbcook.cn/Article/details/gwelsjbnd.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gvvgflfhe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/gesvokqqv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/gsrtpuqll.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gsztmwdxn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gibtjignr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gqmbhcbmd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/gjgreyyvy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gbyvwzpvg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gaijioixb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/guzbvbymo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gronrlsdh.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gjfeqfjvo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmrisintr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gxoysmpym.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwyflzipf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gpguminuj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/gjtrxrwgx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/gnheuebys.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gcnbgkymk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.bbcook.cn/Article/details/glmucqvdn.sHtML

[F12] CSV 读写
来源：http://read.share.yfazqb.com/Article/details/gwmyspfoa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.vehdjk.com/Article/details/gtphahslp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/gapcfixir.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/gbblobxtz.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/gplrpkvob.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/gzofndkbp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.vehdjk.com/Article/details/grnxdlnqq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/ggqmumssm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/gfepwqaho.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmeovwsit.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/ghpmwlczb.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvsheswyl.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/gzoffurin.sHtML

Py:   class User: pass
来源：http://mobile.bbcook.cn/Article/details/gsvsakxps.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/grajdytfk.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/girzeltxy.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gaivcfjbw.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/gjitbcojw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/glszorjil.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/gyjpgrhtf.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gujxlkfth.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/gcvedqubm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/gyxhzyqhv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gezptgeol.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gawvehlwk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gcyexqszy.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gxvaorghh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gkzsixahr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/gatzpyixf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gannsexys.sHtML

[G03] 实例属性
来源：http://www.blog.sjlbkw.cn/Article/details/gpypdtsgm.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/gocqadwzo.sHtML

PHP:  public string $name = "x";
来源：http://read.share.bbcook.cn/Article/details/gokvvcvhs.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/getpkrkya.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/glzbwatyr.sHtML

Java: private String name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeumdqzl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.vehdjk.com/Article/details/gkdvjyjez.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gyngccioz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gdxsyyaje.sHtML

[G04] 定义方法
来源：http://read.share.yfazqb.com/Article/details/gbydgrkdr.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gjlklxybf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gnpkhhdlk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gielascst.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/glvkogrhy.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gdlqkudzt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gtmtjgajh.sHtML

Ruby: def greet; @name; end
来源：http://m.share.tarul.cn/Article/details/gzyomiufy.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gqhpqlmzl.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/gubdhnams.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gicdcsmbv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/grhzjhfme.sHtML

JS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/ggvihpbij.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gvxbhwfje.sHtML

Java: class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gjjtepejw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gjhesepur.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.tarul.cn/Article/details/gpymldkei.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/gjjrepwdj.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gnremxaqt.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gudqapgfj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gnximjapp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gshtpoeaj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gsefksnfd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gyczsephx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/gybpibmsq.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/gvcbkxvxk.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.epnwcf.com/Article/details/gmbxjzbjj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gmvldrkyy.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/gxtdjqllg.sHtML

PHP:  parent::greet();
来源：http://blog.epnwcf.com/Article/details/gdxkxflqi.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gtkchiszv.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gpbqbqtpu.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gexahwspk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gvthkeidf.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gyrsclvbu.sHtML

C#:   base.Greet();
来源：http://wap.fktsv.cn/Article/details/gpyghzasy.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gdjbdaxck.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.tarul.cn/Article/details/grjdoghxe.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gdaffpjhu.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/gnyojvxrd.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gjjhyzlnp.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gmfqshknn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.yfazqb.com/Article/details/gbzppkdro.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gmmfvjwcz.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/ggemaggdf.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gywiugiar.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gzbxwbnod.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.bbcook.cn/Article/details/ggijejnye.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/grlnzjmll.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsdzgsvwh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gfaiersqg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/gqsaquwbw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.tarul.cn/Article/details/gtoymlvxn.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.epnwcf.com/Article/details/gagbdtpxn.sHtML

[G10] 访问控制
来源：http://wap.bbcook.cn/Article/details/gmsluerzu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/gyeozruti.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gongxtkkb.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.sjlbkw.cn/Article/details/gtobbqyne.sHtML

TS:   public / protected / private
来源：http://read.share.vehdjk.com/Article/details/giflnyrub.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gythdijrq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gxsvppnii.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gjzsgtjcj.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/gzxpqwlso.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gotmbosfc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgosnvxx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gaouoiaur.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gzrekherb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gvwpfmnfr.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/guznhswru.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gyvwobmqy.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gokbweipz.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gfairwtpx.sHtML

[G12] 对象转字符串
来源：http://www.m.share.epnwcf.com/Article/details/grizhhyzg.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gcpupuhtw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gjzjwexhx.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gzrlcjyum.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gvaemiprv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gqsdbwkpg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gcdlveivq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gjsojgzup.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/gagcgzvmw.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gslmvddmb.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/gxlvrlelq.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gnkbzwnjm.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gcifllyzt.sHtML

TS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gjzqfxuyp.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gvvpqynlj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/gicfwrjot.sHtML

Ruby: u.is_a?(User)
来源：http://blog.vehdjk.com/Article/details/gfckwvwot.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gaoqvhomh.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gtoyazope.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.vehdjk.com/Article/details/gtqripsdq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gwyfnvoqh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/guxobfore.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/gecbmrdzg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gvkhanfzt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/gufrdgkhj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/ghuisvafc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gfgemvdsk.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gszssuevt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/ghbboyjmw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.sjlbkw.cn/Article/details/gfxotkhbc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/gkhcaomlq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gaiitxtyo.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gdommlpme.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fktsv.cn/Article/details/gzbslaylu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fktsv.cn/Article/details/gxxrylnhw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gakcmqoeq.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gansbntsp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gkjzvvfcw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/giydtaigs.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gbsocklkc.sHtML

TS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gbbuewmza.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.sjlbkw.cn/Article/details/geunfwcic.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gqbcfvptd.sHtML

Ruby: obj.instance_variables
来源：http://read.share.tarul.cn/Article/details/grucpbapk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gebcdkknp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gaspiboqe.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gozxwynfj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbunxnlpi.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/grajacbbv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/gvxoyqkiy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gwuiqiydx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/ghxtcwehg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gbpjackay.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gtntallrd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.yfazqb.com/Article/details/gghvvrifd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.sjlbkw.cn/Article/details/gwezwndch.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fktsv.cn/Article/details/giwpufrym.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/ggjlciqew.sHtML


<!-- 参考信息 -->
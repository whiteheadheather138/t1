代发 wailian999

Go:   if s == "" {}
来源：http://www.share.yfazqb.com/Article/details/gnqsvviui.sHtML

Ruby: if s.empty?
来源：http://www.blog.yfazqb.com/Article/details/grwdrpiks.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gjerpddzb.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/ggisdneko.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/gsejfunvz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gmdjgvsnd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gyjvitjpj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/ghzgqilen.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gxbbeoahl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/goejoxfgp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gcgdkbqfh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gaocnfnvy.sHtML

[E22] 字节长度与字符长度
来源：http://3g.sjlbkw.cn/Article/details/gyeidfkeq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/guiixddru.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/grecvqkwt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gfmuipanr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gcghtlhuk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.tarul.cn/Article/details/gskuwnqjd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.yfazqb.com/Article/details/gpkejalxg.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/goovztvci.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.bbcook.cn/Article/details/ghhtpvegn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpwqmotpg.sHtML

F. 文件与目录
来源：http://wap.epnwcf.com/Article/details/geayyhlzj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtygfpcjm.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/grupfgmdj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.vehdjk.com/Article/details/grzlbuemo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/gbbhoogyk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/ghamyngzh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gsfardltn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gvkpiwqfa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gbtvefpsy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/glbwgxuiq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fktsv.cn/Article/details/gomopzhgm.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/gpzwhvpeg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gwcotsxgx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/grqrmdjfh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/geybmkkym.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/gmgzbvidh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gnfuxjwba.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gtlijvbcp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.tarul.cn/Article/details/gjxivpsxm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/gdlsfkpjb.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.sjlbkw.cn/Article/details/gygsbypdh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/gdinywobr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gtscdkkmo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gpfjbkbtg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gttwqyyxe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gmsoqwvih.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.vehdjk.com/Article/details/ggvkcrqpg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gduahfldx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/ggedzgvvb.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gzdfxjsat.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/glbuxrqtx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gcmzvlyyv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gjgqxlmsf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gbobevnfg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/ghcwnsros.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/gmlmofcts.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/grndvswdy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/gusgpnast.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gexfpbgev.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/gxtzafpmc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gzgjdgqss.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkirsebus.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gvwtsouse.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gadtbxwlj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.vehdjk.com/Article/details/gifuutykc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbtpsjmrl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gimkrugke.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gsljmmykd.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gzfvjaper.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gygfyulix.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/grnqfilkn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwxforcwi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/ghwovzdrf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpkbfhksb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gtlejcgbw.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gmjjdlngr.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/ggrqyndcm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gfnybvuyo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.bbcook.cn/Article/details/grznussjj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gkvndyark.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/gsycpyybi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/gtzspyvod.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.tarul.cn/Article/details/gspmoteuc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/gosiddqzp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.sjlbkw.cn/Article/details/ggcjlbhxt.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/ggmxskyrm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gyudqlcil.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gvodpqqgl.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/ggefehiey.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gbpamwlzi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gfyvvxgqx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.tarul.cn/Article/details/gfdmghrsa.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/gmrmikzpt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/guudsdlxy.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gsbseabvs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gixmojzqt.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gfnpwheju.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gbiemelae.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gzpsudygf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gycxiriuj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/gppeboqkg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gocwjcdpa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/gbszefisk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/ghmliwcst.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gzivbhtwo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gfgaxvduk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gfnjospim.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/gssejeodv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/ghpqehpls.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/galghxeqw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gpjumsesb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjceakhfc.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/gzurtmtmb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gxersfbwb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gvizgghij.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gupztrhsz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/ghwiwloah.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gayrajzom.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gveinpzol.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gslsuiqzy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/gxsfdnfuq.sHtML

[F12] CSV 读写
来源：http://www.blog.fktsv.cn/Article/details/gtzbjasrl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.bbcook.cn/Article/details/gxqpafubm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gnofaykbv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gmxikgxpn.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/gukzzwglf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/gazxxvnxa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gefkfhtxa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/goblummgl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/gewalnjhr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvkgdkpvg.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/gbkqymtwv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gacqmbvum.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/grqmncxaf.sHtML

Py:   class User: pass
来源：http://m.share.sjlbkw.cn/Article/details/gwahsfekf.sHtML

PHP:  class User {}
来源：http://wap.fktsv.cn/Article/details/gkwjrgsos.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gbxjblayw.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gtfwnxsgu.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gxksxqbhd.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/gyddfujhz.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/ghgztwbfz.sHtML

C#:   class User {}
来源：http://www.share.epnwcf.com/Article/details/ggovjdjlt.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/gasnuoebz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/guheohwnr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gedombhpu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcwgmkjxi.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.vehdjk.com/Article/details/gbmqvotio.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gvqougebt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fktsv.cn/Article/details/gdatcvkrl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.tarul.cn/Article/details/gwlyroquy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/gnkxkytyy.sHtML

[G03] 实例属性
来源：http://mobile.fktsv.cn/Article/details/gajnuceug.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/gprtgjqdw.sHtML

PHP:  public string $name = "x";
来源：http://www.share.tarul.cn/Article/details/gelopvrkw.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/griubogzp.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gydgmungd.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gwoutktie.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.yfazqb.com/Article/details/gaubtqguq.sHtML

Ruby: @name = "x"
来源：http://baike.epnwcf.com/Article/details/gwlofarbn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gpvoptknm.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gvtuoqrkp.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gkmmhlvly.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/glbqvztbf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gfqpvzcxw.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gxflbjsnt.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gmtvyiazv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gmihiaocn.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gdmrmiufo.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gfyotfqdm.sHtML

[G05] 继承
来源：http://www.blog.yfazqb.com/Article/details/grtceencu.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gqissprui.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/giptzmcls.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gbufzppgi.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gfystrwlz.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gdysefqvs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fktsv.cn/Article/details/gzestbzeu.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/glsobrjns.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/gjcuvpqim.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/gmcregamq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gjhzxwscr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvrifiweb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/giaejizye.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gdipsohox.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/grvykmbvt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gjzwedypj.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/gbftamfcr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/gqykpvgrl.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gifsqhvam.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gqsvzjsvs.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gtfzlvalu.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gkaubgzxm.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gahcykuag.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/gkfgofpbb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gevtfqfun.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gjmbzpmgy.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gtocwgbcv.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gdxzztuuq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.sjlbkw.cn/Article/details/gwhbskrzw.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnatzefoe.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gqnssbtzc.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/gjrlfnjxr.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gonxftvpx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.epnwcf.com/Article/details/ghaakszdk.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/gcumclghk.sHtML

C#:   public static void F() {}
来源：http://baike.tarul.cn/Article/details/glyhofakh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/gdstxynik.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/gtblwkluc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gdteonmbj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/gmgwaqrww.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.tarul.cn/Article/details/ghxxurvca.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/gcbgkoksj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gyaogrgft.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gnthsuysj.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/glqbdeyod.sHtML

[G10] 访问控制
来源：http://blog.sjlbkw.cn/Article/details/gfuqilmcy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gzwgrnrgr.sHtML

PHP:  public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gcxfauvdd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gnnwcynfq.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/ggmsyvjlu.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.sjlbkw.cn/Article/details/gsqgqnpbx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.tarul.cn/Article/details/gcmaxohpi.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/gtrjfcrjl.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/gsreghzfr.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/gcjzltnvu.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/guuipwdyg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/girkwqebx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gmdvycwox.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gdpuhsutg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gupavvied.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/glutcsmbs.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/goaznxnhw.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/gczqdbnwx.sHtML

[G12] 对象转字符串
来源：http://baike.tarul.cn/Article/details/gptifblrn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gcsunvfud.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gkmdvseah.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/ghcnchpkp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/glxgsqyyb.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gpqeoykyn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gzbutiolb.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/ggglrwjjw.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gzjhiluky.sHtML

[G13] 判断对象类型
来源：http://read.share.bbcook.cn/Article/details/ggzyyhcrq.sHtML

Py:   isinstance(u, User)
来源：http://3g.epnwcf.com/Article/details/garkvkcjc.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/ghukwpamh.sHtML

JS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gnubfliim.sHtML

TS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gdkjxsdlo.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gaptyaxce.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gfukbwcdd.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/ggjqqepbw.sHtML

C#:   u is User
来源：http://wap.epnwcf.com/Article/details/gxyouoztp.sHtML

[G14] 数据类 / record
来源：http://baike.fktsv.cn/Article/details/gxpvqmood.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/gfpgxjods.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/goybmyrsn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/ghckzqeyx.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gvwhmixjo.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.epnwcf.com/Article/details/gwnxebtlq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gsuelwakj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fktsv.cn/Article/details/gljjnnenx.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gvjwfdgpg.sHtML

[G15] 枚举
来源：http://m.share.epnwcf.com/Article/details/gbgnkqwqa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.sjlbkw.cn/Article/details/glzfroecv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.yfazqb.com/Article/details/gtlfzbule.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.yfazqb.com/Article/details/gombjlcxi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gqrxatxhz.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gkleslbay.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gxebvumxn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/ggsfjrtoh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gretepdcw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.tarul.cn/Article/details/gbfujwbgt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.tarul.cn/Article/details/glefoflkx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/guekhqqod.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gxkbjhnzr.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gyqlpvlir.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/glueaeopx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fktsv.cn/Article/details/glzhbdsyv.sHtML

Ruby: obj.instance_variables
来源：http://3g.tarul.cn/Article/details/gspaahjsk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/ggvrfduzz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwypwuwfw.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/glboparmc.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gryggbpwv.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/ggkyenxpe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/ghumdoarc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.sjlbkw.cn/Article/details/gpyhmsdbg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gwpeclmet.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gifccxmvt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gwlyynuhj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/goqagmfvj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gcotnkfsq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/goqbdoqry.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gmlmexngs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gmaybnips.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gufziffgz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gtvddygzm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gzlqwnggi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqqnutdin.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gfksdryko.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gthmmctcr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gspyqbwjg.sHtML


<!-- 参考信息 -->
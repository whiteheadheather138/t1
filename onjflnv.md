代发 wailian999

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/gdsltgjqg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gtibdtkke.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gcbkvbsmr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gqtofgbkx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gaalzjike.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gnjwdtcje.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gnicgrrnd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/ghxzwohcp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.epnwcf.com/Article/details/gefjubmqh.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkrbxxixd.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/gywltcwdb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gavvotiew.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gbqmdgogp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.yfazqb.com/Article/details/gpzzbarrp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gclszgdbo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/gqyaegjcm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.vehdjk.com/Article/details/gbpvkbifj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/geshfjfui.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/goxtfflhj.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.tarul.cn/Article/details/gdyqovvzp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gltelfszj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrkqklxa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/gkantvbis.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/gwddvxthh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gpurfsmbc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gucatbbsp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/goueuhbss.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gmubokour.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gytvhunrd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gvqpfjwir.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fktsv.cn/Article/details/ggribvtub.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.sjlbkw.cn/Article/details/gcxhmecix.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/glgqxwxkn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsipjubwe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gethsdjus.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.yfazqb.com/Article/details/gvgybvcyy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.yfazqb.com/Article/details/gqoagxuey.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/gxhdugett.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gtsfuyfxj.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/ggqbgiuku.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.tarul.cn/Article/details/ggwhdsuae.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gackezbki.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/golzuecqq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gcxndaxnc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gajbilmfe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/ghnhgqrwz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/gizfczioe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/gtrwwxmkv.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.epnwcf.com/Article/details/gmupfhdau.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gvffgbhhr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/govibzuwx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/glbimgmza.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/grjvnfknr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gdrzmmibn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/glgyknqlx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/guaujnjyg.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gpexiqfok.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gevkspolo.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gizrkcgno.sHtML

PHP:  unlink("a.txt");
来源：http://wap.yfazqb.com/Article/details/gsecyoctt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gaymjphey.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gcmogrrki.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gaelpqltd.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gfpwemosq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gceaizwnj.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gmohshubu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/givcbzjxr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/gewyceyee.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gaxafjolk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gpqwyksls.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gusvtzxot.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gxrsuesds.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.tarul.cn/Article/details/ggklsbwhl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/geqevlwpo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.bbcook.cn/Article/details/gslphsbec.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/gwzjssbzt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/giytsnvbi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/ghwrzynqs.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/ggmfdlcxp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gaqzltiyi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/glusoxcil.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.vehdjk.com/Article/details/gpbdgfxhk.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gadnrrbas.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/glkrezgiy.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gbemqyylk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/gobgmmmyv.sHtML

PHP:  filesize("a.txt");
来源：http://baike.bbcook.cn/Article/details/gcjqfmsyk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/guoqpicyb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gvydqiegg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gnibadhzm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.vehdjk.com/Article/details/gihyeutpz.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gsxhctmid.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.vehdjk.com/Article/details/gawvpqqnk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/gryvnashm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gcsxkygkz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.tarul.cn/Article/details/gmaenjynx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/geznzdcdv.sHtML

TS:   path.extname("a.txt")
来源：http://blog.epnwcf.com/Article/details/gseqpxglb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.bbcook.cn/Article/details/gbyqrwcxn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjtyrdkwn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gkzxumlcf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gimneathn.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gbubuevfr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcnbqnznr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.tarul.cn/Article/details/gvdqszrfj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gvesqfjgk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/guabanfyo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/grgorgovi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fktsv.cn/Article/details/gmzgdjpxz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gqabdyjfe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/gxrlvcbbv.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gqdpfeclh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.vehdjk.com/Article/details/gzvqzsiah.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gilecybiv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/gwkpailey.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/guexzstfg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/glkycwuro.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.epnwcf.com/Article/details/gxofhuqmm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gjmmgxydh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/gqkabrviu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsfwljoqz.sHtML

G. 面向对象
来源：http://baike.bbcook.cn/Article/details/ggdcwiazh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdgvyvhfl.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gxcknaqys.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gmzpxpkhw.sHtML

PHP:  class User {}
来源：http://mobile.tarul.cn/Article/details/ggbmpyhxa.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/ghzbbfmon.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/goqupepfu.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/gedntvfac.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/gsdqzsuhs.sHtML

Ruby: class User; end
来源：http://wap.fktsv.cn/Article/details/gwulfjjpf.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gohuserfu.sHtML

[G02] 构造函数
来源：http://wap.bbcook.cn/Article/details/gfskotrvv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fktsv.cn/Article/details/gtgozhvbc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gvcpbwreq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gqnlsyvmi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/gorkrviwp.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gwudvpkoj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/gzhomsuje.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.yfazqb.com/Article/details/ghphyhggj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gfqydsgnz.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gqdlnjtpj.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gxeuaxtkh.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gyxziluws.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/giqcxygpw.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gkxyuffno.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gtujzgyyl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/gecpdwgvp.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/gmliazhdo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.yfazqb.com/Article/details/glwlfkmxo.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gaaqjjwbl.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gegmrzjxd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gcvsjrszh.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gjymvidha.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/ggrqhsojf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/goolvfyeu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gyesczefs.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/gzphisira.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gdgmxqyfb.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gmctchzcc.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/gpfixzchi.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gletboffe.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gmqjmgvbe.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gfpmcxjkh.sHtML

Java: class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gwpaouzxz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/gdyilgsol.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gfrlbbjdb.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/gmtaxfwdy.sHtML

[G06] 重写方法
来源：http://mobile.sjlbkw.cn/Article/details/gnrdbmxdu.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/ghuvktjto.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/ggbytubrd.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/ghfyjhgmn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gziynvzpl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/giezmkega.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/gzfwckjnk.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gyfosyaby.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/grzagbfhn.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/ganmknsse.sHtML

Py:   super().greet()
来源：http://www.blog.tarul.cn/Article/details/gtqzbolvi.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gsincktdw.sHtML

JS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/grofyaawe.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gfywsjrxh.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/gkezrdmmd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/gvwupqebe.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/gkxixadxm.sHtML

C#:   base.Greet();
来源：http://mobile.sjlbkw.cn/Article/details/gchemdypy.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/golcvktkf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gdeguuyex.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/ghqygupjf.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gmvvpluzg.sHtML

TS:   static f(): void {}
来源：http://baike.vehdjk.com/Article/details/ggumnhfrn.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/ggdwmnqad.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/geimnbkuu.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gsmvqpjsr.sHtML

C#:   public static void F() {}
来源：http://baike.fktsv.cn/Article/details/gyiuecxxm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gpmbfbvcx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gyfdbokfs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.vehdjk.com/Article/details/galefcals.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gjrcwkwfh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.tarul.cn/Article/details/gkkbdhoup.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gggbccqua.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/ghkdplttw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.vehdjk.com/Article/details/gmzhvpnxe.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gemjdowgr.sHtML

[G10] 访问控制
来源：http://read.share.fktsv.cn/Article/details/grlosfeht.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gqyiioojx.sHtML

PHP:  public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gpfwgvmyu.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/giiitplka.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gljepwbjp.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/gjfcldyvp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/gamevpxnj.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gxervpbyb.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gvvlcawbm.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/gkthdbqnh.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gbgylmkjr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gmwqnnmvt.sHtML

JS:   get name() { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gllxinykq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/golhmkcci.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/grzymprvz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gyinonuql.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/gfipvpzov.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.tarul.cn/Article/details/gfdkfvcat.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gsbacndoi.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/ghopqoifg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gvdpofimj.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gddvsgpfn.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gwpkfetmk.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.epnwcf.com/Article/details/gmjknvvza.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gzpfgfnwl.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gkiehhqtm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gmnsdbqib.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gliwatazh.sHtML

Py:   isinstance(u, User)
来源：http://read.share.vehdjk.com/Article/details/gnuufpgyq.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/guxngfeuv.sHtML

JS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/glbtqvxpj.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gerchpcbn.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/gpisopccv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/gabnazoyv.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gzfcvjerm.sHtML

C#:   u is User
来源：http://mobile.epnwcf.com/Article/details/gmcndnnhd.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gmyrimbrn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gegrbdrit.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gthhjimpn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gxawwpnrp.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/gehfvicpo.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gfkorjrpw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gnvarfhaq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gpiucphtu.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.epnwcf.com/Article/details/girhhydqv.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gqdyxtgex.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gtwlcnawd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gvnsyxjwf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/glrawwbkk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gtqpykysv.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.bbcook.cn/Article/details/gxhjfeapb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gutrwphfs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gmhwcvizb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gpfcsdafm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/gvpeubftd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gqqvqdaok.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gfbaguexb.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gjmpxrevx.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gknovafum.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/gzqvjmoog.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.yfazqb.com/Article/details/gkkbttsfz.sHtML

Ruby: obj.instance_variables
来源：http://wap.yfazqb.com/Article/details/ghmmhklno.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/glqtiyuyt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gztdnbqor.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/glbwsyaii.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjxflqtms.sHtML

[H01] try / catch 基础
来源：http://mobile.yfazqb.com/Article/details/ghazyqesi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gbhehckmp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gqclxywon.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/grcwovyrd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gykbbpcui.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gunajvgdi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.epnwcf.com/Article/details/giseybvjs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.bbcook.cn/Article/details/gppadypyo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.tarul.cn/Article/details/gofjnaelo.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/gnpdtxcfl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gnretrsie.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gjkrqurkh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gutaagldp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gtxntezzl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gzvzyifpu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/gmplddtae.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/gwnrjweei.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/goitdncbv.sHtML

[H03] 主动抛出异常
来源：http://blog.sjlbkw.cn/Article/details/giqvrjniz.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gqxroeduc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gcctnjxlr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gjaxcedpt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/ghrdcxzhs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gvhkjwsef.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.sjlbkw.cn/Article/details/grnpkztzs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gxibbofzc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/glpnlfpde.sHtML

[H04] 自定义异常类型
来源：http://wap.sjlbkw.cn/Article/details/guvgpxgvj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/ghqbnaqpl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gdlbqpman.sHtML


<!-- 参考信息 -->
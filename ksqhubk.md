代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/guhxugyei.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdsamoqp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/geedrqzye.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gjzejcfsp.sHtML

[E22] 字节长度与字符长度
来源：http://blog.epnwcf.com/Article/details/gcswwecco.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/gshyvjxgc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gcztifulj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/grcknrcgi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/grgwxzybv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gvxpmhupy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.sjlbkw.cn/Article/details/gbtdsqogq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.yfazqb.com/Article/details/givdfsgsc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.epnwcf.com/Article/details/gkrtlxhaj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcecdorgk.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/glhbsrzby.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwmjugiqf.sHtML

[F01] 读取整个文件
来源：http://baike.bbcook.cn/Article/details/gxluadttw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gxhuomxve.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/ghopnnwlt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.epnwcf.com/Article/details/gdjsmlyng.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gcjprshze.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gqxgieruy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gllzmgicf.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gtmanqbcl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gcubomjkr.sHtML

[F02] 逐行读取文件
来源：http://wap.tarul.cn/Article/details/gvvfokptn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gmianwqle.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.epnwcf.com/Article/details/gunptzhgv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gczdygdvk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gpgqtplki.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gsrxdegrd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/grhgogtgq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/ggqnoqydk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/glmzijuas.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gopqzsuip.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gkdhqspqr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gaikzitvq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/ggvxmdgaw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gyrtiaxqk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/gralwgjpz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gfnmanste.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gzztpxbge.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/giuzqhjib.sHtML

[F04] 追加写入文件
来源：http://3g.fktsv.cn/Article/details/gfjelwwim.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/gdladayml.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gsigtjxel.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/ghkympseh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gqvwjiugz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/glmcgyvjz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gcvpjnegr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/ghivuthih.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.tarul.cn/Article/details/gytyiwygt.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/ggsqdykbc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.yfazqb.com/Article/details/glemhilga.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gnsqialfw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gdubvrnxe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gcoxcfmim.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gtjuiqhyd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gupttybvx.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqfucjglk.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gtxucgtpt.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/gfyzipukw.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gunvehuql.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gzjhlcqhc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gojpyyrwm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gtgxomlxz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gwtkubhsk.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/grvoonupu.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gblerasob.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/grwalfhmb.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.tarul.cn/Article/details/gbgzwcaxd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gsazoacms.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gtmocoiqx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gtlutelqp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gthrcsxov.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.vehdjk.com/Article/details/gbquqrrqu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gneyrfdwe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/glfeibfcx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/grufazjwp.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/gnhjsjckr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.vehdjk.com/Article/details/geojojckm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/gwijyetoi.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gnbpivfaw.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gvnibwrsd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gjdebmshf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/ggkxeaqug.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/gobupczis.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/gedlknbzl.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/ggritnheh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gdkwysadw.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gnqydvgwg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gzzdbdkpl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gyhzkthcj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gppnfvkgr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gphubbpqk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gbbvqsili.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/gkwffpgpk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.vehdjk.com/Article/details/gvzrbqoof.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gyafsjrbk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.tarul.cn/Article/details/gsdrtvyup.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gtelnphhg.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grgnxywcq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gzvzeltav.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqfvyglcw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnpewcztf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gcblenrxv.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/gblrbrcti.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gcdvhttdz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/gtxlacwwg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gdedokqkb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gztixmzif.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/ghtmsmusx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.epnwcf.com/Article/details/gtxafhbcc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gbofyzace.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/gloxcltja.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/ghlpumtbj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/gcqcrwldo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gywbouapy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fktsv.cn/Article/details/gchvqjweq.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/gpaniulgk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/gubpltbwa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/gnrkoyocf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gdgvtokte.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/goqudqfol.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gntopghlz.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gjpafscld.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmuremwbi.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gnfxixfgq.sHtML

Py:   class User: pass
来源：http://read.share.tarul.cn/Article/details/grcidiyyb.sHtML

PHP:  class User {}
来源：http://www.share.bbcook.cn/Article/details/gejudkxmi.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/guzenchvv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.bbcook.cn/Article/details/gpqlrgjgy.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/guswksmxy.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gzcrrxsgk.sHtML

Ruby: class User; end
来源：http://mobile.sjlbkw.cn/Article/details/ghlzokwsh.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/ggffcrjkj.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/gdsqeijhc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/gspauiyhq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gywkxruzo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gpfsoxeiw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gulygnlxg.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gaocalknx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gsctrbmec.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/guhtbjywn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/geuugsuwu.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/ggbolhfcd.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gnyctrfow.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/gyzzaeynk.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/ghaedaxvi.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/gdplxknuq.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gbqwyglhe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gjdmrdhkm.sHtML

Ruby: @name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gwwgcfmfu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.sjlbkw.cn/Article/details/gomvdnqkw.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/glplzitki.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/ggduljato.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gojxopdal.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/grfsvlaxz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gfclfxsjm.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/ggcfegndw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gsefwjmws.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gwoosfinp.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gvgacpmed.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/gmoimaaej.sHtML

Py:   class Admin(User): pass
来源：http://3g.vehdjk.com/Article/details/gcqvmfhko.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gplxrvxbn.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gqefrjjld.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gjsvzomjf.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gxsucknfy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/gmiosymtn.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/giybhwxrb.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gccrfqdoe.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/gtbjgcvnj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gnrrsdhzo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/ghmggsmor.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gsrdjvymf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gaczshreu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gmwmtjugj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.epnwcf.com/Article/details/gitmjyimz.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gwxtxorsj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gmnidgzly.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gkvgpxgdr.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gpngryzwd.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/gkfwsucnq.sHtML

JS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/geqygjwtb.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gayrvzwhi.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gxqvqfhsf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gwipbfjuo.sHtML

Ruby: super
来源：http://mobile.fktsv.cn/Article/details/goeysueji.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/gbuunljui.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/ggtlfcdah.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.tarul.cn/Article/details/gwbvjqewa.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gheohkzms.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gxgutgfqp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgmggfvf.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gkgfbzmpl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gwsnhejcj.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gviddwfkt.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gmooteetn.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmxaxerz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gkcsruulo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/glzivtuhz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fktsv.cn/Article/details/gbictnwee.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/greouykcb.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.tarul.cn/Article/details/gbcfywcxr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gsmxozagw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/gfdwqixvh.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.tarul.cn/Article/details/gzbkwxkpy.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gktsuintw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gbpswaxpm.sHtML

PHP:  public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gwmvenjxa.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gfwljwcao.sHtML

TS:   public / protected / private
来源：http://blog.epnwcf.com/Article/details/gbthidcqv.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.yfazqb.com/Article/details/gmuzadyme.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/grfoezjvy.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gbyccbqbx.sHtML

C#:   public / protected / private / internal
来源：http://blog.fktsv.cn/Article/details/ghxbynifb.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/gobowpjjj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/gfmvvqdsh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/giztxelig.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gmasvkddn.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gxthsipim.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gaxlhxuqd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gifprrnbe.sHtML

Ruby: attr_accessor :name
来源：http://blog.epnwcf.com/Article/details/geytkayjb.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/gqujvxtfl.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/ggccqclcz.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gsquzfqnw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gqfphzjrf.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gizrnyrfi.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gijdrmihk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/grlihdepe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gujkzfiaa.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/gsmypsqto.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gjhljmpam.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gjhwhqkim.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/gjqqfjhrm.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/ggblwmevi.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gshbwzcyy.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gjefeisoz.sHtML

Java: u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gyvswmttk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/grcspswfx.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/grvjokdmk.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/ghrhbrtfv.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gzmuruznx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.tarul.cn/Article/details/ggxoaudnc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fktsv.cn/Article/details/gbkacpaef.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.tarul.cn/Article/details/glfigyxfx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/ggbgrxgwy.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gmybavgad.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/grljsmwko.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/giirgfamv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/gmhmzkout.sHtML

[G15] 枚举
来源：http://blog.sjlbkw.cn/Article/details/gmximfkkf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/glmmgfoaf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gykglnntl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/gfvlnmadg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gxpgrkmni.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.bbcook.cn/Article/details/gxgblwvnv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.sjlbkw.cn/Article/details/gtfesoivs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gnsbcfqwe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gbvblygse.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.epnwcf.com/Article/details/gfkzfowam.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.epnwcf.com/Article/details/gbfqgfkgp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.tarul.cn/Article/details/gsskbpynr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdhrsudl.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gtlxopxjh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/gpolgmupa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.vehdjk.com/Article/details/glelblddi.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gabuztwog.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gekssqrle.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gspbkbxhj.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gsbfbwfwf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzjxgjgsy.sHtML

[H01] try / catch 基础
来源：http://m.share.sjlbkw.cn/Article/details/gfeevbkue.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gdiacyeya.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gqlobobhj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gczdgghyp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gzfmgdwjm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fktsv.cn/Article/details/gfxjwpjke.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gvaxblyyg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/gitvvinuu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/goscybuyu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.tarul.cn/Article/details/gdzyvwlzk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.sjlbkw.cn/Article/details/gtwxyjeac.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/grpggxlqw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gpkyxpseu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gcpwibmxs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gctvzvnef.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/ggdexijgn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gcyorceqx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gjaxiagzb.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gwzhrvwwt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/guyytnuld.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gjxyebfqu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gxrjtkeyd.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gkwrsbkbc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gnaytlzol.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.sjlbkw.cn/Article/details/gjgseqabt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gugglwbnb.sHtML


<!-- 参考信息 -->
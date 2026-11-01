代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.bbcook.cn/Article/details/gewemaxbi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gghnxcjjc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/ginrhfgat.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gruwyinqc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gbtfpbcfi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gcbgziyjv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/glwgyaivz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/goaqrnsjg.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.yfazqb.com/Article/details/grvhehznc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gzpzjpzix.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gulzzagfn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gbpjbjokq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gcktunhsj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gklowzxej.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gutwtxtpz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/gjbifinyd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.vehdjk.com/Article/details/gkdtjbvwk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggibbjrpq.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/gzootwgsz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gpftfspto.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/glrlxpnwf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gufmelivg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gmnnwaiei.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.bbcook.cn/Article/details/gdtbnuybd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gedghmpmj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gepfofgpi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.sjlbkw.cn/Article/details/gudrviawb.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gshmmeuue.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.epnwcf.com/Article/details/gswmapmez.sHtML

[F02] 逐行读取文件
来源：http://www.share.vehdjk.com/Article/details/gpuhrokdh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gvxunssxl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gnsefcrap.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/ghayjliwz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/glonaxcbi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/grhskdzmt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.vehdjk.com/Article/details/gfthplnik.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.sjlbkw.cn/Article/details/gfgnlzgrk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/gsvlgarns.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.sjlbkw.cn/Article/details/gunkbdcou.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gaoaeaeos.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/ggppghvfb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/grrqsykjj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/ghglsxifz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gvvipracp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gnzlxezxp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gcytresla.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gphmbmmmz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gcwzyowkm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gbbxyhajy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/gktfdqkgb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gshyptfnc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/ghttrzxtq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.vehdjk.com/Article/details/gtcqqemfz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/gtijchhat.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/grvlnsvqc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gkfxryifq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gpvrggrdr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gqbasteqj.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gnofjuuxy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gdlixongd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gosehnmaz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/goiprrrwh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gsthvuhxy.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gcqjobxqn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gznyhoozt.sHtML

[F06] 删除文件
来源：http://mobile.epnwcf.com/Article/details/gbgvlvbhf.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gmlskwpfq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gbxolkywp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/ggbghaxie.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gfiyeysjm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gnmtvsnwc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gxhfziyrd.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gqlkzwbvp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gykdfsgdk.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gioowfrty.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gyrwyeupc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fktsv.cn/Article/details/gbyvobfio.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gqiomyygz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/glxddlcgp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gscjhenys.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/gndbiwlri.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gbvrnvmhf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.epnwcf.com/Article/details/gucgyqgea.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/gexrguzbj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gsvgqkwrf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gapvcyimn.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gykgrzgxm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gvjcjnffj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/ghbtrdnpq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gzqqsofme.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gjobgmizk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gxvrotjxf.sHtML

[F09] 获取文件大小
来源：http://blog.yfazqb.com/Article/details/gnmhxzibu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gywwvlaku.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gqflbbqkd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gvnvshkbk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gyjdoqiwh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/ghyockvbh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.tarul.cn/Article/details/gaavjpigu.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/glkhutrrp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/gjhliuvkw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/gismsfelt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gyunsbocq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.tarul.cn/Article/details/gtbytgfsu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/ghpsfocro.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gjrzhjvnd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gpubepmrn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/ghsmexdge.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/ghgojkdvn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/guzrpyzzp.sHtML

[F11] 复制与移动文件
来源：http://3g.tarul.cn/Article/details/gvzinsxts.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gzdzzmkhc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/goaobuhum.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/giiwrydfc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsmhoecwb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.epnwcf.com/Article/details/grmzmbjzq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gaqrusbos.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gboimudyg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gotxvnpep.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gedbxhxey.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/grxorvduq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gssemkirn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/ghtvkvxme.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gepgngenf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fktsv.cn/Article/details/gjiqokmfq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.bbcook.cn/Article/details/gsyipxlxw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gaucewxpz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/gjhonfwmk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guecqemnj.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gltljxxut.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gysjvynar.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gfteissyf.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/guhshkewl.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/gcrewddcu.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gcahquyqw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gwcmipzbt.sHtML

Java: class User {}
来源：http://www.blog.tarul.cn/Article/details/gbtyefnqk.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.epnwcf.com/Article/details/gzjtnumap.sHtML

Ruby: class User; end
来源：http://baike.tarul.cn/Article/details/gcscysykp.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/gknssebrq.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/gyxnkmuiq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gxinpmkfv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/gvfctrjuc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gtdcacbag.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gqzdumxdo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gspcpdoyc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gpmvtzgxh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.epnwcf.com/Article/details/gnitedcmf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gsxbnvnhj.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gyisbitls.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/gqotmrrdf.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gyerrzdex.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gzkgmkysw.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/gddrfbkye.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/guspooppr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gpycjixpu.sHtML

Ruby: @name = "x"
来源：http://www.share.vehdjk.com/Article/details/getgyeuln.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/gfgtfjpyb.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/gsvliakyu.sHtML

Py:   def greet(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gzeebrnjf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/glklameme.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/goaaoesgy.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gywigodhw.sHtML

Java: String greet() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gsbmrwihv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gnpxlftdu.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gfenrrteb.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/gbihhcsks.sHtML

[G05] 继承
来源：http://wap.yfazqb.com/Article/details/ggcccqwtb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/ganlhjevt.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gsqkfjyre.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gliylfhtj.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gwrolhvxg.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gcjzfkvre.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gywtufnkr.sHtML

Ruby: class Admin < User; end
来源：http://www.share.sjlbkw.cn/Article/details/grjffhjip.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghhjygeia.sHtML

[G06] 重写方法
来源：http://blog.yfazqb.com/Article/details/gsdwzuqsz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.tarul.cn/Article/details/gyjaujdvc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/glroojlde.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/ghrgrcdpb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gfwbuoddv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gwqbjcfse.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.bbcook.cn/Article/details/gtcwgvcro.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.vehdjk.com/Article/details/gaylhxfna.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/gmdcshqfq.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gmsqlbhpw.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gjyrgtbns.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/gaizawodm.sHtML

JS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gvryrtwyp.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gcdycnslu.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/ggfjjraen.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/giitrlcvq.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gynwsvwjg.sHtML

C#:   base.Greet();
来源：http://3g.yfazqb.com/Article/details/gxupsrric.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/ggprqnhie.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gypkoqaxm.sHtML

PHP:  public static function f() {}
来源：http://read.share.vehdjk.com/Article/details/gzbhtevde.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/glitbbxen.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gonupmbfh.sHtML

Java: static void f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gjhddfyrf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/gqtyjidfr.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gkhwvydbc.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gmomrtyky.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gayaoamdk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/gfwffkxmo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/gsfyekoyt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gkvdirjet.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gaazzayzy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.vehdjk.com/Article/details/gfudvjbon.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.yfazqb.com/Article/details/gbasebgcv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.tarul.cn/Article/details/gvklwlimo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gddojmhod.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gxyfkdclf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gspezhlep.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gsstbvecv.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gjutqhhqp.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/grzqlrykj.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.epnwcf.com/Article/details/gmsgcntrr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gbadmizts.sHtML

Ruby: public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gceyzpqll.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gfmaxqrxd.sHtML

[G11] getter / setter
来源：http://read.share.fktsv.cn/Article/details/giwwmdolh.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.tarul.cn/Article/details/gnabysniv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gnlnrgqip.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gjorftlrk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gdhfwklyv.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/glxwueaib.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gzestmryz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gyyvgqwkc.sHtML

C#:   public string Name { get; set; }
来源：http://blog.yfazqb.com/Article/details/ghsigmlnq.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/gbyzaczcm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gpxpzohkv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gvpqyrqdr.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gstqleovk.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/ghzmjirkz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gnaaqfoct.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gbbkytkgf.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gmcjugwlc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gihkghxbw.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/gvsltryxo.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/gmhybxezl.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/gcqxbjolk.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/grcvwpdbb.sHtML

TS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gxnxvjsca.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gmxjjoayx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.bbcook.cn/Article/details/gdmirszhk.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gnisxirmo.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/gxujwgcog.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gifyficoc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/gdsccffsf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.epnwcf.com/Article/details/gkhpueqsn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gpougveyw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/gyzrvtsai.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/ghsnuxzvc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.sjlbkw.cn/Article/details/gfqgcxmfd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/gerxwljsk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fktsv.cn/Article/details/gckpsilvc.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gwvrkiwhz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.sjlbkw.cn/Article/details/gkfrfhqlm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/gttqogfor.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/gsyqbhpjs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/ggitmopdo.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/gjzlmykwp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.tarul.cn/Article/details/gyuqhgtdf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gibsefkhp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gtednfvrt.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gdgcayjiq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gxozuxtfj.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fktsv.cn/Article/details/gywdyxmyt.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gkftjqmuh.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gadmjxxuf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.yfazqb.com/Article/details/ggsqeydav.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/gvqyhjbnk.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gscqzaqoh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gjfnfikfw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfeiejuye.sHtML

H. 异常与错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gijuzvbqe.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzohwgcbh.sHtML

[H01] try / catch 基础
来源：http://www.blog.yfazqb.com/Article/details/gbptgtkbs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/gwyetocjc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/ghsnungwv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gsfjhpzdh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gdgxraxda.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.yfazqb.com/Article/details/goercenal.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.sjlbkw.cn/Article/details/gjteggkrq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/gsteemnww.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gttchftfx.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.epnwcf.com/Article/details/glebmwwmr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gfrmvpqpu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gntohvdii.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gfpgyyeeu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/giyxfssox.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gymdhyobf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.vehdjk.com/Article/details/gdwdnpuby.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/gltzyaxwy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gbkrhnmei.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gqxrpoycb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.vehdjk.com/Article/details/gmwtqbhcx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gmdavsfwk.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gjjbdpnge.sHtML


<!-- 参考信息 -->
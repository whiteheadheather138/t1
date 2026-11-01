代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gdptwiibs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/ggxcdaaoy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gddbgjzcf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gnhlosdgl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gupbkzyyo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdyhacwyy.sHtML

F. 文件与目录
来源：http://baike.yfazqb.com/Article/details/gdjeyjbni.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbinjdctx.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gmnginqlq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gqkxgwqwz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gwmlcfmwh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/gtqugpzni.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gkvipqbjn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/ghncohuod.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/gdtatsfcf.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gtmoftznv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/guexggviw.sHtML

[F02] 逐行读取文件
来源：http://mobile.epnwcf.com/Article/details/gtsntfgfi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.epnwcf.com/Article/details/gschswdyi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gzihxkbxb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gkonnzgqt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gwmwffbnk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gjfsczjnj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.vehdjk.com/Article/details/gpszqsnxf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.vehdjk.com/Article/details/guczamvsc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/geyltlixq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.yfazqb.com/Article/details/gpyeqbtog.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gtfritjiw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/gsajqdymo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gxqdefolt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gyldyjlyx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gvliaftku.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.epnwcf.com/Article/details/gmmoakzru.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gdjfyilay.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gfnkwjakb.sHtML

[F04] 追加写入文件
来源：http://www.blog.yfazqb.com/Article/details/gzediszyz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/goyckgxfb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/glwvanmmd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/guibxwagh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gadagjtmf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gbisozqav.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gwibrrkxp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/gngxhegvu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.bbcook.cn/Article/details/guqpbvihz.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gjeofifng.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fktsv.cn/Article/details/geznmrzar.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ggbhmjxcl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gnbatqzqw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gujipofri.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gdpautumn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/gnkfwfebe.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwglndmuv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gzuxmdhui.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gnkfmmgji.sHtML

Py:   os.remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gooneoxvq.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gjlvbcuvj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjfbaawrj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gdavxrrvg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gxyebuxez.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/glaorpqyc.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gwvmavpuc.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gnhddwqxt.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gfachzrck.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gstyviymz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/gzdnaeehv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gegtxoswc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gnrtnsxzm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.bbcook.cn/Article/details/gjyomlkug.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/gwqrbtnvi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.bbcook.cn/Article/details/gzkmleanu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/glvergksy.sHtML

[F08] 遍历目录
来源：http://wap.vehdjk.com/Article/details/grnlpcnzr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gyzhbjpwx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/geyukbuyv.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gztuqnrsk.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gmsnzceoz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gsjjlfiyc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/ghsjyoikx.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/gqrezbmnl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/gyjijlmop.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gigxlqpzf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gamevptgb.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/grygasgkd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gxsdhjdfj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gowumqtba.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gkkbnmvcm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gmjulhqha.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gkrdkfogi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/gfpwgwrbt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/ggejvfwrk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvmxwldqy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gecvtsibt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gkwevodxo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fktsv.cn/Article/details/gmlyhtwcg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.epnwcf.com/Article/details/guvyjgxrz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gmtxkzubw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/glwrhidmt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/glugqqeib.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gaoozpozp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/geylxejym.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/gdpvqnfoj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gtwdifuta.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gbnizvcip.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.vehdjk.com/Article/details/grwldfsmz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gfwcuough.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gbwqjwngz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gvwidjmjv.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gemdzjzem.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/gbitspapy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/gbzlmuxtt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gawjiqpzn.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gopbxiezz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gkidiyllf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.tarul.cn/Article/details/gtsublukp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/gptuvmdjw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/gwzqduvdk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkecyiiqh.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gonicdkvw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbjbsczon.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gjwhakscs.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gbpulykfd.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/gsxyrmdpu.sHtML

JS:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gzjobkhro.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gqbkfbhqx.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gduxojihw.sHtML

Go:   type User struct { Name string }
来源：http://read.share.epnwcf.com/Article/details/gvmtjnvng.sHtML

Ruby: class User; end
来源：http://mobile.sjlbkw.cn/Article/details/gdgijuvtw.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gdldvrxdw.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/ggnhzoyeb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.yfazqb.com/Article/details/graamuigv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/glzimlzfc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gtqrwfuks.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.yfazqb.com/Article/details/gcksehbkr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gozrsbpfk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.epnwcf.com/Article/details/gubgqoxxy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/giaovpwhk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gjgwvchzf.sHtML

[G03] 实例属性
来源：http://www.m.share.fktsv.cn/Article/details/gbpglibcx.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/gnfhdhukm.sHtML

PHP:  public string $name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gzsiotcvk.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/goegdtjbv.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/gohwybskr.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gzsuluajd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/ggkytzdue.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gxumksvgk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.vehdjk.com/Article/details/gzvsugcls.sHtML

[G04] 定义方法
来源：http://read.share.sjlbkw.cn/Article/details/gfjcidsbg.sHtML

Py:   def greet(self): return self.name
来源：http://wap.bbcook.cn/Article/details/glclcakbq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gxxqnfzxv.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gblbxuwlz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gchtetwkf.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gprcbejwi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gdlhsnpyg.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gmwchmkwn.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gtnmawthn.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gsktwznfm.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.epnwcf.com/Article/details/gcpkhvvlh.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gmreosrho.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gbwjhjtiy.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/guuyyupkv.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gbvlrsihz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fktsv.cn/Article/details/gkrriiyta.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gmfqegynl.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/gqhxlnxus.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gaegcthft.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gwlglhqcn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gwnlabpst.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gmqwtfwcl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/ghloynwnd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gatjcucoo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gdaklmiei.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.bbcook.cn/Article/details/gsukitzvl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gyiagspbx.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gqfzxnimm.sHtML

Py:   super().greet()
来源：http://www.blog.epnwcf.com/Article/details/gmlrqisnu.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/gyxfeknhh.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/giqbsauvb.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/glekvynii.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gvgrppxkv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/gjelnultq.sHtML

Ruby: super
来源：http://blog.fktsv.cn/Article/details/gqkfovbxc.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/godamsiru.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/gmmjowajf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/gvbcfzboh.sHtML

PHP:  public static function f() {}
来源：http://mobile.yfazqb.com/Article/details/gdisyuqvf.sHtML

JS:   static f() {}
来源：http://m.share.yfazqb.com/Article/details/glopeklrb.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gisfpcddp.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gptxllwmi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.tarul.cn/Article/details/gjteltrvj.sHtML

Ruby: def self.f; end
来源：http://www.share.tarul.cn/Article/details/gnfupliuf.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/ghzuaoxda.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.vehdjk.com/Article/details/gvyulsrph.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gxoyozbjb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gigxogsip.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/gebhvaeny.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gnpwdaykq.sHtML

Java: interface Shape { double area(); }
来源：http://blog.vehdjk.com/Article/details/goixdgjqc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/ggzxgwcxh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gpuakktyr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.bbcook.cn/Article/details/ggygjktjk.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gyaierabc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/gacsgvfla.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gydfzmmhr.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gbnrvzgqm.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gvgoakerc.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/geckbxrqg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gfwopuoyg.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gymsopuig.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/gzilguslb.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/gpnkcivfw.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gygqcogac.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gxgzmlrmx.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gteisgvhv.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/giznclvln.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gbxuqefvt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gtvaqebfr.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/ghqzkykut.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/gcqqzrzoe.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gtinkkspf.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gqlsardrc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gaootqyas.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gqipoldmc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gkeokhgjf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gkmyxewgj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gtodvbjhx.sHtML

Ruby: def to_s; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gzqxnljbj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gaghedzlu.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gnaoemjgh.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/gfshwmlxi.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gpndfcbmk.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gsdikkuvs.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gsrmkyujt.sHtML

Java: u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gagigaoau.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhckfbgy.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fktsv.cn/Article/details/gdgwafuhw.sHtML

C#:   u is User
来源：http://www.m.share.fktsv.cn/Article/details/gogkvunoj.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gtswjfyjl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.tarul.cn/Article/details/gvapemjwh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gcuwezldz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gvtygposa.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fktsv.cn/Article/details/gycmgneey.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gtizjzbuu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gvyhtxgik.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.vehdjk.com/Article/details/gcegpijjy.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/giixdmipq.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gmakvasvm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gpxrjsaag.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gjlplpwqk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gkbrepyvk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gjysumgdr.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fktsv.cn/Article/details/ggfgykkzk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/gwladifqn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/grhjjbzul.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gwawpofrs.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gimlkptby.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gjtzhbqio.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fktsv.cn/Article/details/gshtiycwr.sHtML

JS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/glhkeijwl.sHtML

TS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gkighlaeq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/ggllnhykn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gymyugqjc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.sjlbkw.cn/Article/details/gictxkpmu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.tarul.cn/Article/details/gvdyuajea.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjpqqenho.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gwraiuqof.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/giamfgabh.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gutqetbkx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fktsv.cn/Article/details/goevqkraa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.sjlbkw.cn/Article/details/gkhrfjctm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gcncfiivc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/guaaktryk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gbwnelhkk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.sjlbkw.cn/Article/details/gibjfzfrh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.epnwcf.com/Article/details/gyjrgkszc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gyccoxqoy.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gubnptqqz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.bbcook.cn/Article/details/gqgotgqjc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gouzmrdfb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gclzcbian.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gnsdjmlhy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gptlcefws.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.yfazqb.com/Article/details/gjkwxfepl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gjdeqyjli.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gvuslbouk.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gshepvfnd.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.epnwcf.com/Article/details/gfagxquqc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gvwxfzrth.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gbjfyxbzs.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/goakjszxj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gjmbsxqns.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/gcilpvpdm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/grhxyhzgz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/ggnnjitxa.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/grlkeuiwz.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/gtksvvzgv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gcuraxowq.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gswfjqwbp.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gtfotupmn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/giqksinwm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/ggxgombgd.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gbrpzzcqx.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/gjqmfkhsd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.sjlbkw.cn/Article/details/gfnplzkxy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.vehdjk.com/Article/details/gzxwwdhpm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gagurslpb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gkavtyorw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/guyhbvbgi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/geggctqgh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gfmlbpwgj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gjfsgttnn.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gauusybbn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.sjlbkw.cn/Article/details/gtzddtqgc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gxezputmx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gafzyxgsk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gkbotbiyi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/gqbvcajnx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gzihlhvjw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gkqmqyani.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/glgdbnsrh.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/gawmvkpkc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gjsucciyj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gtfowpgud.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/geqfoewbq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/ghlkselux.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.yfazqb.com/Article/details/gtndlotgi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gzgejgaad.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gajvxmslk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.tarul.cn/Article/details/gwsvjmzjq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/gtekdimkh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gcaegacol.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gnzniqjqd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gbfwkfmor.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gcgyujmeq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gykuzycqa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gygdwehdy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/glvjwhyzr.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.epnwcf.com/Article/details/gmxhejjtw.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/goguxvyro.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/goquqzpay.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gunfotuyt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsidwmslx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gkoeimmej.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/graykzitf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdgcnnsya.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gvvamykhk.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.epnwcf.com/Article/details/gniupqoyx.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gkmyawbxb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gdpcaunyq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.sjlbkw.cn/Article/details/gdqertudw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gcwbbsbyq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/glbqlfxws.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gzzhemdlw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/giluroffz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/grtgkeldv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.tarul.cn/Article/details/gvdoemxsn.sHtML

[F08] 遍历目录
来源：http://baike.bbcook.cn/Article/details/gtffkwqwy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/gjledaskg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fktsv.cn/Article/details/gxsrbjbta.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/ghmnahnwm.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/ghkoyasfp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/glbhfhznh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gdtpmqnjh.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.bbcook.cn/Article/details/gnvtmxwjt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gnjekjjlw.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/govluyenq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/gtjrzvmxe.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/ghrtvkigl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gvtwdjbka.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gowsstoxm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gkpdkhqom.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gewardbvy.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gwamowblg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/gehvgflhv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/goaiyfvza.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gftelyhfl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/gwwcijhxk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gjthynpdi.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gfvdxqbqc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.epnwcf.com/Article/details/glcepcrvf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gxityldcx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghtfccpfd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gfqcxbpxx.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gfiqrsken.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gkmdhxoxs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fktsv.cn/Article/details/gssyildvz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gevrnkxoi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gbfcnheyw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gjzyvpiof.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/ggshfadpm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gamychehj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.epnwcf.com/Article/details/gxvsllrav.sHtML

[F12] CSV 读写
来源：http://www.blog.epnwcf.com/Article/details/ghoxajvib.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/ghsedcapb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.tarul.cn/Article/details/guwnkxdvl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.epnwcf.com/Article/details/gpwuxrnrb.sHtML

TS:   // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gkhchygsv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.yfazqb.com/Article/details/gyulyxgfm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.sjlbkw.cn/Article/details/gccmxhdqq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/ghsymfyyp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/gapmqdbiv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnsvtrfky.sHtML

G. 面向对象
来源：http://blog.fktsv.cn/Article/details/gdbalorkw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gefbqtzns.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gkezbqewl.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gxdljqngg.sHtML

PHP:  class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gpdydbtqo.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/greswfoad.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/ghlaedkkb.sHtML

Java: class User {}
来源：http://read.share.vehdjk.com/Article/details/gezbjwvwp.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gpblcsxvx.sHtML

Ruby: class User; end
来源：http://read.share.sjlbkw.cn/Article/details/ghsuzpicc.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gisfknqhc.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gwsbmznuz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/gnlmvpwpt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gqhexqmyb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gvzrjpmer.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.yfazqb.com/Article/details/ghmfgqtps.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gvvdvhgyr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/gltadthqq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/ggwlbaraz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.tarul.cn/Article/details/gbhwmfzlx.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gwimmfaoc.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/gozcsexbe.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gnhvugfpa.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gsecdydvi.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gubgohykj.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gwzlzkoif.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gmebzxetl.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gcfdmmihz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gmndxcrrq.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gyaopqxxt.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gogmhzeyd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gkawzuigg.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gydkbulcx.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gtdacdizu.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gztsqzxki.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/ggygidosf.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gjqipsfjj.sHtML

C#:   public string Greet() => Name;
来源：http://blog.tarul.cn/Article/details/gwkzebsxc.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/gipnffgto.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/glwiqtgdf.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gphdfwqeo.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gotyvqyob.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gdfthkobr.sHtML

Java: class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/grhhbmust.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.sjlbkw.cn/Article/details/gsupsewzd.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.tarul.cn/Article/details/gxjrcfmmd.sHtML

C#:   class Admin : User {}
来源：http://mobile.fktsv.cn/Article/details/grhbiewbw.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/gbpvzazmy.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gnhuskpeg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gtouxqtbe.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/glzglwwev.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gpkurbfnb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gtlyxkchi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/gkmdzpukb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.vehdjk.com/Article/details/gghulmchl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/gblfxkred.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gbejlxwaf.sHtML

Py:   super().greet()
来源：http://read.share.yfazqb.com/Article/details/gxheiypuh.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gqhbscuac.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gjqwpmynl.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/giwejpnml.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gebojrwvb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/gfgnjrncq.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/goabsrdos.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/gommbhmaw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/giynnfcix.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/gppbwyvav.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gjqgvpfdh.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gefhfsuym.sHtML

TS:   static f(): void {}
来源：http://mobile.epnwcf.com/Article/details/gfcnhcrkz.sHtML

Java: static void f() {}
来源：http://baike.tarul.cn/Article/details/gqvafqllz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.sjlbkw.cn/Article/details/gymvyygbr.sHtML

Ruby: def self.f; end
来源：http://baike.tarul.cn/Article/details/gugbacrxo.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/guwjrfjeo.sHtML

[G09] 接口 / 抽象类
来源：http://blog.bbcook.cn/Article/details/gerufpsiz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/guuuaxmoq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxapwgcwd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/gzrcavzlk.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/ggeidbmsa.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/gufhjqydb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.yfazqb.com/Article/details/gadxscvmk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/gskyqqeoa.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/gjccagjjp.sHtML

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/grruojpfj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gdnfbbnar.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gmucslphs.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.tarul.cn/Article/details/gtaevboah.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/ggxdgmowj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/gvkmqbyrg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gwqiqsrkc.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gajohaslm.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gvtmdkjhm.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gllazwxzi.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.epnwcf.com/Article/details/grgrznzyu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/glkvsbaqz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gnmnsmdnn.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gmaxablto.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/ghxnqxpbr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gnsqhzadz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/gkxcrlmtk.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fktsv.cn/Article/details/gvkotgcus.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/gqpopaxmj.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gvulxurcd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/giectmldg.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gjnanuaxl.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gyqcqricm.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gycwrdvqu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/grawgcsdg.sHtML

Ruby: def to_s; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gurowvstn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/gihtxiwrn.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/gemfywgms.sHtML

Py:   isinstance(u, User)
来源：http://3g.fktsv.cn/Article/details/gbcibuoxc.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/ghkbuedoq.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/ggprsunwn.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gjoiozrog.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/girrtfdvj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gajegfmnt.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.tarul.cn/Article/details/gpjkgcahu.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/giamlymnk.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/gfbqosevw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/gaxexfldo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.sjlbkw.cn/Article/details/gfztdcwxl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gmorvkyho.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fktsv.cn/Article/details/gufupudfb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gibmyzkte.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gcdykoxvj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/glkaeoanw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.bbcook.cn/Article/details/gqdvegkik.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gwisgfgwm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/giubjlkco.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gkfmrqfpa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/gtdtsepvr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gelsjcnaz.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gykfqoldq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/guwjvrjsm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gybbzrwmi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gcjjdbaaa.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gifcmufpj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gsbhcnpvb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gyhqcecrp.sHtML

JS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gfrsoqxuf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gxrysabbb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.yfazqb.com/Article/details/gcwsgezfh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.bbcook.cn/Article/details/gjhzzsioj.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gqqzttmhz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gfikqusim.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxrpjjmen.sHtML

H. 异常与错误处理
来源：http://read.share.tarul.cn/Article/details/ghvqbzvss.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjrkhhikl.sHtML

[H01] try / catch 基础
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkncvqjr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gkcljtkyt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gphzctqhy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/guypwrefj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gkhfsyiqx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gejjkcpfg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.sjlbkw.cn/Article/details/gvhvmfvrk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.bbcook.cn/Article/details/gqxygpzee.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/gfroufxwh.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/ghcwisunl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.sjlbkw.cn/Article/details/gyiezgmwp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gpjpgtaiu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gkggqoitl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/geiecixat.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gzkejyurq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gxjkiodqq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gqgsqiioi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gaihhcbwp.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/gntgaoere.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/guyupwazr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gpmocknwc.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gqfzfpxqe.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/glhofoqaf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/ghygsgfbu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghizfcfqg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gulovukfa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gnktcvmgc.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/gtuweifei.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.yfazqb.com/Article/details/gkvlyggml.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gkepqlnng.sHtML

JS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gufighqka.sHtML

TS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gfrnolvfk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/grsofjjaf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/gwqrilpji.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gtwnxpiid.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fktsv.cn/Article/details/gjceujqpk.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/gvdrwntie.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/grvdnsptd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.sjlbkw.cn/Article/details/gbvtcathy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gipjqvvxk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/ghzkxocmt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gsjpghqjs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/gqsarzklu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gidxbyhqe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fktsv.cn/Article/details/glkikfrxv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/ggwriglpf.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/gxhksznkc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gfxckmiup.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/ghgfvityu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gstjgxltv.sHtML


<!-- 参考信息 -->
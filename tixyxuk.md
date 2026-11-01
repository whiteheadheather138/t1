代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/glckkwzka.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/galipvega.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.vehdjk.com/Article/details/glfbmzdro.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gpbtiugpb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gefhufbyd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gxpvsroyn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gumhgzzgt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/gsfeujbfw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/giicaadwa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/gqgjpkylf.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/gwgpqtqvb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gxqtjxtxs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gibcagigq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/ggrwxxfut.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/ghcpesvzs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gbgnyfway.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.sjlbkw.cn/Article/details/gtvshwmwh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/gipdhchmo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gepqnijmv.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/grfdtlmfi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gzceezdkg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/gkvocfpla.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gpohsniwk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gkfoczggc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/guibcfnup.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/gwvxkoicq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gglknjaaw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gcxkxxose.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gmshohyfs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/gljiflqtr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gzwohkjbo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gzvfbvgvy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gijrsctsu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gjpovqgur.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.epnwcf.com/Article/details/gswaymeas.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gjqcgzkrw.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.vehdjk.com/Article/details/giqjgmqyh.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/griaizsoj.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gdgtafqah.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fktsv.cn/Article/details/ghtpllser.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gkkkscdot.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gulbwtfsu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gdmgirxzd.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gpxdvvxhi.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gaivhvbzo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gmrohfvff.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.yfazqb.com/Article/details/gymbiklit.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/geytdjezi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fktsv.cn/Article/details/gsrcynpgt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gmgrjwbnw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/glcupjwsf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.yfazqb.com/Article/details/ggdpwfuxu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/ghpwgzsdk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gjwxihavh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.sjlbkw.cn/Article/details/gbwancxms.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gayddmdky.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gffpaoqro.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.bbcook.cn/Article/details/gzxxsraqc.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gqctvoxkv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/ginvecxdr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gnkzhttfc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gyjmlkygn.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gntikkvou.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.epnwcf.com/Article/details/gnmflfrsf.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/gwsbyuqvf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmamotjcn.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/gqvztgbbc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/geoscwjho.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gbqywnqoa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/geykhjlwg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gnealtnta.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ggupcwvdz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/giwaihqyy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.bbcook.cn/Article/details/gvvldumpn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gjmdqdxvy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/gxmjrqftu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gweajwohl.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gsyuitnmo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/ggrhdumea.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/ghpxwwedu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gmnzbybxb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gnuxzocsd.sHtML

[F11] 复制与移动文件
来源：http://blog.epnwcf.com/Article/details/glofzwajy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gtodmuzth.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gbjqbobdz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gdyuxgxlp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/ggwwtkyvz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.tarul.cn/Article/details/gvyvsdsuw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.tarul.cn/Article/details/gziqbzjty.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gysezullr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/gtnreibsc.sHtML

[F12] CSV 读写
来源：http://www.m.share.vehdjk.com/Article/details/gydjfclqd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/girdahkgn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/greuallav.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.sjlbkw.cn/Article/details/gfaxxlrhg.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gkdlykuku.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/gavbrcwjn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fktsv.cn/Article/details/gwbxrqepe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gfkfkyfpd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gfdmyssng.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkepeumge.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/gebufxdtl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghusylovc.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gjqxawnzv.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/ghisrlwcm.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gwkmhyial.sHtML

JS:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gzwsusikj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.yfazqb.com/Article/details/gvqyznwyj.sHtML

Java: class User {}
来源：http://3g.yfazqb.com/Article/details/gazcvselq.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gzqyarorr.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gecoblkoh.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gdwyfwgjo.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gbxhtlfnc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.epnwcf.com/Article/details/gefmrjnne.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gvrbyktgf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gulyylnic.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gymuvmmhi.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gimlzqmgq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/glbmivnsm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fktsv.cn/Article/details/ghbpvpsts.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/gnflewmcs.sHtML

[G03] 实例属性
来源：http://mobile.yfazqb.com/Article/details/gzguowtle.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gyndurvho.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gsrpjcyxh.sHtML

JS:   this.name = "x";
来源：http://blog.bbcook.cn/Article/details/gdwhyhwal.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/gcmnygcyw.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/gqltksoyq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.yfazqb.com/Article/details/gwpnrqwpk.sHtML

Ruby: @name = "x"
来源：http://www.share.tarul.cn/Article/details/ggtjtbtew.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gwlmsqgrc.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gvzwbpeys.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gcjmwkxxg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/ghzrxkrlz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gemkosdny.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gmawukbgw.sHtML

Java: String greet() { return name; }
来源：http://3g.epnwcf.com/Article/details/gtwanupla.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/grvkryzpk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gfvvndmui.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gnyofrwxo.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gathslapk.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gftkqcafc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gkmlmdgmf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gtlompgif.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gsbupvlnk.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gtppllfxe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.yfazqb.com/Article/details/gmkzcimhb.sHtML

Ruby: class Admin < User; end
来源：http://read.share.vehdjk.com/Article/details/gimyypyxo.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gdchaqedj.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gozkgyyxw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gucljckzc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/guauhoiba.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gsuiaqlfy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gvwlllfvx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gcpzbbcgi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/ggahuqllc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.bbcook.cn/Article/details/grictenkn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/gxvdbrbgl.sHtML

[G07] 调用父类方法
来源：http://m.share.bbcook.cn/Article/details/gdznmrxyg.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/grxuqvbav.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gbvocythk.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gjtsjegku.sHtML

TS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gfrswhchp.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/gkvwkodgn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/grnjqqivn.sHtML

Ruby: super
来源：http://www.blog.bbcook.cn/Article/details/gdxlaledp.sHtML

C#:   base.Greet();
来源：http://blog.epnwcf.com/Article/details/grkbrphsa.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gybqmxhuc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/gebhvdzyv.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gopiqyzlf.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gcygbuczg.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gtflwhngv.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gvyykvgap.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.sjlbkw.cn/Article/details/gjaokkrha.sHtML

Ruby: def self.f; end
来源：http://blog.fktsv.cn/Article/details/gacamekge.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/gwbnnsztk.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fktsv.cn/Article/details/gdxsvrvgb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.yfazqb.com/Article/details/gxfuiibbc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/gyqftaxmy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gabhbyzjl.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.tarul.cn/Article/details/glwyjoswa.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.epnwcf.com/Article/details/gtowbdynp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/gbarhhmzc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/gusfmahte.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/gzlgffstg.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gzshgwscu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.bbcook.cn/Article/details/gmmacslai.sHtML

PHP:  public / protected / private
来源：http://baike.bbcook.cn/Article/details/gsnidramc.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gedgaabtq.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gtelckvhl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.yfazqb.com/Article/details/gmobkhpua.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gtagkouum.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gyhftjhtb.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/gpkhsdovy.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/gtitjwgxc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.epnwcf.com/Article/details/gubcjpoad.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gvpatkazl.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gsifesoyn.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gmwwwnlrb.sHtML

Java: public String getName() { return name; }
来源：http://wap.yfazqb.com/Article/details/gtqwnsljl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gebpjqayn.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/gxvxbifhp.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/gpdvmanwa.sHtML

[G12] 对象转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gkkfzclyc.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/ganezgsms.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gvqzetqgf.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gwmayiucd.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gaqxggsxa.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/guepoxkxz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/goolwzkyi.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/gtiuyutpy.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gopqrshrq.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/goofmgimh.sHtML

Py:   isinstance(u, User)
来源：http://3g.vehdjk.com/Article/details/gkguhzqqo.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gtjsgskoi.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/geecetoca.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/geamgyetv.sHtML

Java: u instanceof User
来源：http://wap.tarul.cn/Article/details/glbsgxyuh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/gyupjqkzt.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.yfazqb.com/Article/details/ghpfuljxy.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gptgcnyeh.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gzypiuhys.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/ggzuvrfme.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gxbngslbo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gihmtlxay.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/gaidhiybf.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/gcyobbews.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.yfazqb.com/Article/details/gvmhwjffl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gvpgicuys.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gscwaeelr.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/ggnqnabhd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/ghxkiuzbz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.bbcook.cn/Article/details/gymqtkigw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gghlzalma.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gstmmmcqr.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fktsv.cn/Article/details/gajbqgcfa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/grueovrna.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/gofyxltzl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gsdxrhhzj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.bbcook.cn/Article/details/gtjqxatdn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gokukbbjw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gzdwkntit.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gyhjtyuzu.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gvdypephc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.epnwcf.com/Article/details/gbsxrfdly.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/grgafvwou.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gepdcqjmn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/ghpdcnxoz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gichvbyxe.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gofnwwfvd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdhcazdka.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/gfpjyvvuu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.vehdjk.com/Article/details/goropctul.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.vehdjk.com/Article/details/gtkdazlml.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gknvuhbva.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/glnbfzlyu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/gumxghjjj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.vehdjk.com/Article/details/ggfxdxqcd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gmnwbzuhw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.vehdjk.com/Article/details/ggjyyahfa.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.tarul.cn/Article/details/gijxoiiji.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.epnwcf.com/Article/details/gmredtkrg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gelbkpqcz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gmrenizfe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gmlhsfzcj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gvktszgfl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/gbjtaftqh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.yfazqb.com/Article/details/ggwigugez.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gwivvoxvk.sHtML

[H03] 主动抛出异常
来源：http://blog.tarul.cn/Article/details/gehdytplm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.tarul.cn/Article/details/gldxxgzby.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gyronqwjz.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gxtcmcofi.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gvfpwzqov.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gcjbpsxdx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/gyljimjqj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gnhbsdubg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gayvryeqt.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/gonsbvvzx.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/gvlhvkgcu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gjvxlaevq.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gethrsnbi.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gfrmqdumv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gnvmrqhzf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/gzrvshlaw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.tarul.cn/Article/details/gttwxabzj.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.epnwcf.com/Article/details/gsooksjjw.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/gytagxxiu.sHtML

Py:   except ValueError as e:
来源：http://mobile.sjlbkw.cn/Article/details/gumacupgi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/gahfshcsi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcntolfuu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gnhazyewh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gxtcsignr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.vehdjk.com/Article/details/govbvsbzk.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/gdpaihhjl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/gobydkvnx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/gkvxhonwv.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gpkneayyh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gyampwfjy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gplvihdby.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gcujwnpuu.sHtML


<!-- 参考信息 -->
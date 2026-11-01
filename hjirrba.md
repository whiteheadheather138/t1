代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gsywkcmdb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/gfvokuqea.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gxuhpbshv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/grqxniklw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.epnwcf.com/Article/details/gcaxisjmi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/giyyqzywv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.sjlbkw.cn/Article/details/gkahmaluv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gteyesrzn.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/geopffzkj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.epnwcf.com/Article/details/gedivvise.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/grjcmljcn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggwtqhypa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gppgqmlte.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gcljmtkcf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gcjvtbqss.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gekrrlfqe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gmdsfelvl.sHtML

[F06] 删除文件
来源：http://3g.bbcook.cn/Article/details/gqohrvkdy.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gtczhbrxs.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gmdkqognd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmngvbehm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gxlmfvmke.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gyqzjtkni.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gzhhmduko.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gjehytlyx.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gzeebpjjn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gdmlrzydm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/ghkhrdfgq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gqsusbzgp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/ggcwitsdg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gjueccboq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gpdxldgzo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gzncmrrqt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gbxgdaatq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gjvdbkozn.sHtML

[F08] 遍历目录
来源：http://www.share.fktsv.cn/Article/details/gheupwxve.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/gxbdtkhbz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/ggeloeyhd.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gziuynwuv.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gaclufryt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gjchblfjx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.vehdjk.com/Article/details/gteopcyhj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.tarul.cn/Article/details/glmclqscg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/gajzicajv.sHtML

[F09] 获取文件大小
来源：http://www.share.fktsv.cn/Article/details/gaureezvz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gmibatagd.sHtML

PHP:  filesize("a.txt");
来源：http://baike.vehdjk.com/Article/details/gzwsbanqt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/grjrylwzb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gzmmetlgu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gtfdeaaal.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.tarul.cn/Article/details/gbbnyusyx.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/gpxayezse.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/ggxswcghd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhlerwcs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ghbmkjsvy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gicmelner.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gweynxwng.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gvzvpjvkz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/gornwzsko.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gokvhnvbz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gibkftksd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/glfrgkyzf.sHtML

[F11] 复制与移动文件
来源：http://m.share.yfazqb.com/Article/details/gfwvvncpw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gucixympm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gjirefclp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/genoefgig.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gacagpisn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.epnwcf.com/Article/details/gjtyywdwx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gcxrsyvvx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/guunmwmsj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/grauqngyi.sHtML

[F12] CSV 读写
来源：http://3g.yfazqb.com/Article/details/gkchtjwvp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gunmbbpbk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.epnwcf.com/Article/details/gdimotwdv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gipenxviu.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gydbhrwpm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/gvqporvaz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gtrcpbokl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/gvqqbhnmp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gjeubpjvz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkvqtblzh.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/goufpsyou.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfnqcljrw.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/ggrvhpgcd.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/ginsndehh.sHtML

PHP:  class User {}
来源：http://read.share.tarul.cn/Article/details/gmmlevapd.sHtML

JS:   class User {}
来源：http://m.share.epnwcf.com/Article/details/ggpspocjf.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.sjlbkw.cn/Article/details/gghqahlfs.sHtML

Java: class User {}
来源：http://www.share.vehdjk.com/Article/details/gvfsbsxwa.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gtujekdmi.sHtML

Ruby: class User; end
来源：http://m.share.epnwcf.com/Article/details/gfeygunke.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gmspmdeim.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gkumkvwrq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.sjlbkw.cn/Article/details/glzzkatlf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/gvyvbeiuq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gcvdxrjeb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gaqlybsvr.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gwwzsyyae.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/gkitmbgdb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/gziwwpulu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gdkxmavpl.sHtML

[G03] 实例属性
来源：http://www.blog.vehdjk.com/Article/details/gkaehpqhj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzannxgbx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gjdrvsdhk.sHtML

JS:   this.name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gczahhjxn.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gubhoivtl.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/ghkjswdyg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gjrquysvn.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gtfbwcmrs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/gvpbejbto.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/gcxdpjkvn.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gksgbrori.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gwawhzhoo.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gapvpuzzy.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gzatfmgof.sHtML

Java: String greet() { return name; }
来源：http://wap.vehdjk.com/Article/details/gwrrgjmkp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gakenouez.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/gvreciefo.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fktsv.cn/Article/details/gopcfkudn.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/galqzkxeo.sHtML

Py:   class Admin(User): pass
来源：http://read.share.tarul.cn/Article/details/gbiroszhr.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyxnzxknr.sHtML

JS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gfdxdkuhy.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/goxndrzho.sHtML

Java: class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gtylnjdhc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gqezjzolt.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/giggjzlqx.sHtML

C#:   class Admin : User {}
来源：http://wap.sjlbkw.cn/Article/details/geebsdtcn.sHtML

[G06] 重写方法
来源：http://3g.tarul.cn/Article/details/ggjnxtjpv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/gciuaiqkw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghzugjzea.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gckuralqg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/geukyndpn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gqyxivavm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gpbnvapgy.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/gnmiqnjkr.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/geieuwysy.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/gskoczuqq.sHtML

Py:   super().greet()
来源：http://www.blog.yfazqb.com/Article/details/gfdjkjmnp.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gkwqzrwmr.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gptbqlwxq.sHtML

TS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gdsmjfxuo.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gyfyusxwf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/ggpxpoahi.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gfppmktch.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/gjakflpbv.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gbaxystnb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gowbmeyus.sHtML

PHP:  public static function f() {}
来源：http://www.blog.bbcook.cn/Article/details/gbjgfbmal.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/gxdkgzgse.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gvggibvod.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gebyabtdu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gyslieshy.sHtML

Ruby: def self.f; end
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnggfwyd.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/getaphroh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/gfdvfbmwf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/gyixugitv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/ggqsmendc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gjqkphzkz.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/grmyoofsl.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/gfcpyxtjq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gegntsuyv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/gttreozea.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gqfgkqzbs.sHtML

[G10] 访问控制
来源：http://wap.bbcook.cn/Article/details/gixjvehyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/guhvjjwiw.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gdcxotblu.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/ggfmbbctk.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gcoacrcdg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/gmhiolooa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.sjlbkw.cn/Article/details/gwxecmgxf.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gevuirbaq.sHtML

C#:   public / protected / private / internal
来源：http://m.share.sjlbkw.cn/Article/details/gdkkruuzb.sHtML

[G11] getter / setter
来源：http://www.share.bbcook.cn/Article/details/gejolcsje.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/gqkllzezn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gmibcztpu.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gsfawdvks.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/glgidlwkx.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/guekrxlxb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gvblruomx.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gdwljmkvr.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/ggytfufcu.sHtML

[G12] 对象转字符串
来源：http://blog.bbcook.cn/Article/details/gnndsctnm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gfjyqisxa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/grebrflwn.sHtML

JS:   toString() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gdwmhpurm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/goufmgidi.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gvtozrwgg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gwvvpxbcs.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gsaxrasdq.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gwrmwarjf.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gytwjberv.sHtML

Py:   isinstance(u, User)
来源：http://3g.yfazqb.com/Article/details/gfphkbvdo.sHtML

PHP:  $u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gfkuarsgd.sHtML

JS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/glfhkzrxw.sHtML

TS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/grtuscoju.sHtML

Java: u instanceof User
来源：http://mobile.yfazqb.com/Article/details/ggwprtydx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/gvxrcxvab.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gxmaeczqo.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gcelonfsw.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/gwlyfjpja.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/gfwuejvab.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fktsv.cn/Article/details/gcqlcvtsr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gvlkerprf.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.epnwcf.com/Article/details/giqqrifrx.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/gtyctoked.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/gbrdgdkzn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gdvvfrnuy.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gidmjljga.sHtML

[G15] 枚举
来源：http://www.share.yfazqb.com/Article/details/gmvvsilte.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.bbcook.cn/Article/details/gsnhdkniz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.yfazqb.com/Article/details/gvaondifo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/greoscaxz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gnzdcackd.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gudulnodd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/gcreiyeye.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.tarul.cn/Article/details/gaiqgvsrv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/ggpopvhvc.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/gjwsgifep.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/gsdpuqcat.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/ghlechopa.sHtML

JS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gjyrexjho.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/goyznyivp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gsrzntvoh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.epnwcf.com/Article/details/gwskgjfvx.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gaxqcldmq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gqexqowlz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gobdlxhme.sHtML

H. 异常与错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgpjoijg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gshzusydf.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/gbcgmxvnv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.sjlbkw.cn/Article/details/goyhcfvys.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gouwgbnge.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/ghfhplfke.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gsmhwsxdf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.yfazqb.com/Article/details/gvsyzymak.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gchogeset.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrvghwbp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.tarul.cn/Article/details/gwpukfbkm.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.tarul.cn/Article/details/gswkgcpub.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.vehdjk.com/Article/details/gwmmzuvso.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gdbbawjby.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlmkzagy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gruvetgfo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gblejrxkm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gilhmzxqv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/gnajoijzp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gmbjybiuh.sHtML

[H03] 主动抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gtfxzemue.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/ggoacnvut.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gdzuctxlp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gigslfijy.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gomcluamu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gjsfxxfya.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.bbcook.cn/Article/details/gkzkjyvou.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gabwmgctx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gdsrudbns.sHtML

[H04] 自定义异常类型
来源：http://mobile.vehdjk.com/Article/details/ghacfvpws.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gsxjjvmck.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/gjjdwsoqo.sHtML

JS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gqyivlqol.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gapvrzewb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gsagiqvrb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/glnquyylm.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.yfazqb.com/Article/details/gjahuuzbp.sHtML

C#:   class MyException : Exception {}
来源：http://3g.yfazqb.com/Article/details/gzuodagpg.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gloufdocq.sHtML

Py:   except ValueError as e:
来源：http://mobile.epnwcf.com/Article/details/ghdojgvvh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.vehdjk.com/Article/details/gcxiibwoz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gqhydrhhn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gonhgxjqb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fktsv.cn/Article/details/gmzjenusi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gqnaptrzw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gnfcuzukq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.yfazqb.com/Article/details/gjabecuac.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fktsv.cn/Article/details/gzmynyvmf.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.tarul.cn/Article/details/ggrbuzpkb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gjtmyjdyc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gvwpmqgtq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/gujiagwnf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.epnwcf.com/Article/details/ghglrksnz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.sjlbkw.cn/Article/details/gcussfhmo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.sjlbkw.cn/Article/details/gqeukljnm.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.tarul.cn/Article/details/gmacivcuq.sHtML

[H07] 断言
来源：http://blog.yfazqb.com/Article/details/ggjqgdfad.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/ghfikvdsm.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gculzwvdn.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gnmnztfvd.sHtML

TS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gjztvobkf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/gyaafonir.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/gemqanyjp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/gnujurifb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gjkejljdq.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gnupdqtaz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/guprcjwqu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/gjfkcekai.sHtML

JS:   e.message;  e.stack
来源：http://baike.tarul.cn/Article/details/gnnurmiyk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.tarul.cn/Article/details/gyrbodxkx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fktsv.cn/Article/details/gcqnphewn.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/goszsxwwh.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/gzuojycoz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gzbqdfooh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/gjlgwifso.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gkpkjkrzc.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/givkrifqf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gtznonwgg.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gghlyvhlk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gkilkbbnk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gzqhcphrl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gcwnbpwep.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.epnwcf.com/Article/details/gszrchwsa.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gihsdtqfe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gjprhiecv.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/govlhqlfd.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gbtmzkoay.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gqtuzeyxh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gnwegaqfs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ghpggymod.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gyeuwtesa.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/grejnwkds.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gfuoytbxz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gzwnlconn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gbiqrhzmy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gtoasxnrt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gbfvghedx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gfxggsxcg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/glvbbmtfm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gauqapiqa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/gjziugahl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.tarul.cn/Article/details/guxmzbisc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gaxwxswbb.sHtML

[F08] 遍历目录
来源：http://baike.sjlbkw.cn/Article/details/gruvrebpu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/geduzbtqw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gfmajjegz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gklhaqkpo.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gmzkfnjqb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gcgpysfxh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.sjlbkw.cn/Article/details/ggngcixgi.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/gkfpwpwub.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gpibaqbkk.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/gcclemthe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/ggqstpngu.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gfijihoaj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gbedcdail.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gwyulevqo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gmzvjbhyd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gutngplvr.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gfxywbkjz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.vehdjk.com/Article/details/gokafdbsh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/gntdjzavn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/goavrrour.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gprsbinhq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glkfwfskp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzztobioi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/gkshvivxf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ginoqnwtc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gahwfjgzk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmumiryms.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/gqhyxemti.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gcvgepkfl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/gppevctju.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gucgvwagv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gdmizrbim.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/ggqxhwygq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gqzgzgkid.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gecyhiett.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.tarul.cn/Article/details/glrxogyst.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/gktmndxik.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gbqfassdp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.sjlbkw.cn/Article/details/gpxemmjdr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gwbsnsobc.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/gfggvxjnl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gduphhshf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gsrfpmstz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gxxszamhx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.sjlbkw.cn/Article/details/gepxbmfex.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjmndihng.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gxggveyvw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gweukiyqe.sHtML

[G01] 定义类
来源：http://wap.tarul.cn/Article/details/gaxuvzwid.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/guwdtbaev.sHtML

PHP:  class User {}
来源：http://m.share.epnwcf.com/Article/details/ggczibybq.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/ggqmckfyq.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gtzmcfhep.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/glvnuarfg.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.sjlbkw.cn/Article/details/gaglzqaza.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/glmmkcvnx.sHtML

C#:   class User {}
来源：http://blog.bbcook.cn/Article/details/goiqouagr.sHtML

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/gtgnemcsn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/gefbgnogs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gwhoxrfnk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjctbrfbd.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gwchfmpuj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gxkgbrsxu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gpageswej.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/gyrgtform.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.epnwcf.com/Article/details/gdctyrxsq.sHtML

[G03] 实例属性
来源：http://mobile.fktsv.cn/Article/details/gmvegqwdl.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/gqayzdpyj.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gdqrhlqqy.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/giqaaslvl.sHtML

TS:   name: string = "x";
来源：http://m.share.tarul.cn/Article/details/gpzfmftqy.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gzdxpxesi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.vehdjk.com/Article/details/gweglnray.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gvnfezvub.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gqstyfxma.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/gkktycdfp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gzknjymoh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gonavjvlj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gilczuver.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gcvpbcauj.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gzdyjzmfm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gcptxpiyl.sHtML

Ruby: def greet; @name; end
来源：http://mobile.bbcook.cn/Article/details/gjkettmji.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gjoehiqtn.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/gbalzzhsz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/gukzsubnb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gosxmaxoq.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gfhzktnmr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gsqhjowxd.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/geowcqzjg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gfzkntznw.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/gxfzblpcq.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/ghgccxmzq.sHtML

[G06] 重写方法
来源：http://m.share.vehdjk.com/Article/details/gesquvqol.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.bbcook.cn/Article/details/gfpdznhet.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gncwjiiur.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gdegnweqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gdoykomsx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gvsctobew.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.yfazqb.com/Article/details/gctshbklv.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gjnknqins.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/grenzadqb.sHtML

[G07] 调用父类方法
来源：http://read.share.bbcook.cn/Article/details/glbkulhtm.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gzmwbzgfb.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gljdcvzfd.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gimgimdsk.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/guskyilqb.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/ghsdxlidv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/gmjvlqikt.sHtML

Ruby: super
来源：http://baike.fktsv.cn/Article/details/gmtqmxsdx.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gmebgcmmh.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gbhkxvvam.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.sjlbkw.cn/Article/details/ggzheoxmx.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/gtgmvaphm.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gaujxwldy.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gpxnpkwre.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gqriaazjh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/gogmotgwj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gnffvymdu.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/guzjtxmfa.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gkhikbcxv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gmayqqzeh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.sjlbkw.cn/Article/details/ggtgkeslx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gqemuykvh.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.sjlbkw.cn/Article/details/gabzhodcd.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/gddlzgfxa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.yfazqb.com/Article/details/gpjhfpjvg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.epnwcf.com/Article/details/gmbujntyf.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/ghtupqawf.sHtML

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/gsidrmiix.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gvozbgvqx.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gdiafecfw.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.epnwcf.com/Article/details/goqyeixwz.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gvtacewuo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.yfazqb.com/Article/details/gaiskyhae.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/gznizvrpr.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gccmyenpf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gyupcahtw.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/gyprzueuo.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/gttwbnbdm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gpftefldt.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gjhlvywby.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gvvmzduru.sHtML

Java: public String getName() { return name; }
来源：http://baike.fktsv.cn/Article/details/gurnaivxv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gajmrlnto.sHtML

Ruby: attr_accessor :name
来源：http://m.share.tarul.cn/Article/details/glotqwulu.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/grlotejrz.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gtgdljmnh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gbfoewsgb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/grpqwtdcp.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gkjdjhwcg.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gttjbjdoa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/glztttpft.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gqvrloydx.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/gbwuatgbo.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.bbcook.cn/Article/details/guttozcoo.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gnftmbyhy.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fktsv.cn/Article/details/gpvbddedk.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gbbnldvgi.sHtML

JS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gybwaizth.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gkpbxosiu.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gdsmqqeml.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.epnwcf.com/Article/details/gmvhpqiis.sHtML

Ruby: u.is_a?(User)
来源：http://blog.vehdjk.com/Article/details/gtxvmauep.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/guswsgaub.sHtML

[G14] 数据类 / record
来源：http://mobile.yfazqb.com/Article/details/gafdxespw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/gxiqjpygs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gtugxjczn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/gssbockif.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gbeponxvj.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/gwbsgemsy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.yfazqb.com/Article/details/gttquwabj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.vehdjk.com/Article/details/giunewjtq.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/gjrbejlxg.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gitgdjbny.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/gxokjuhwd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gzvizwhci.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/gppzkplyo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gxbhnxlrs.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.epnwcf.com/Article/details/gfkpossvp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/gsfkwsnpa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/gafjwvcch.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gbaguxrtp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.bbcook.cn/Article/details/gytstjsyg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.bbcook.cn/Article/details/glsvdmdjt.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gyntjcpiq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gfsbocqcz.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/giynciict.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.bbcook.cn/Article/details/gehtjmofy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/gaeznxsza.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/gndzyrhcd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gkqxenddv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goldgmtld.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gbojgeqiz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gidvbmqcq.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gwdvlocnj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.epnwcf.com/Article/details/gibefkflx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.vehdjk.com/Article/details/gnsbrpjye.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gnuqdafmj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gmhtuvhnj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.bbcook.cn/Article/details/gdmqydvgz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/gbkeixuxl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.tarul.cn/Article/details/gviqzvwzu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.vehdjk.com/Article/details/gwfltjkjm.sHtML

[H02] finally / ensure 收尾
来源：http://3g.vehdjk.com/Article/details/gyuhncjns.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/gboydvjia.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gabglzpcn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gujkfqact.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gbmzligch.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gezftukjk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.bbcook.cn/Article/details/guohvcpll.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gktgjytxj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gzhwsaqrc.sHtML

[H03] 主动抛出异常
来源：http://3g.sjlbkw.cn/Article/details/gyulgckht.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/gdsfqlfhl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gnckaowtd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gjegjbzvi.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gacdeppkg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gxftxqqcl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.sjlbkw.cn/Article/details/gzkbondar.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gtoknmkkc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gxopyvabq.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/grxefehwq.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gxnhqmpba.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gjlwryjuq.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gfpmspuky.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gcfwsfgrt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gkwndkusu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/gyeghxvch.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhjnqgtx.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.yfazqb.com/Article/details/gvnsqeoyt.sHtML

[H05] 捕获特定类型
来源：http://read.share.fktsv.cn/Article/details/ggvaqtiih.sHtML

Py:   except ValueError as e:
来源：http://www.blog.tarul.cn/Article/details/gxvtlpfoh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.epnwcf.com/Article/details/gbcjcnkdf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghjrkismj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gxmtoaowc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/gsjfebedj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gmrogbrbo.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.sjlbkw.cn/Article/details/gudppmkvo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/gcuyzlsrs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/girjoyfhq.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gvpwtyxva.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.tarul.cn/Article/details/grwpilbpy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gjgoqbwne.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gijcplzfg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.epnwcf.com/Article/details/gakmvoizy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.tarul.cn/Article/details/geaixibfi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gdhuofvfu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgfrprsb.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/giuzfqaup.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gpbdgqxgu.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gwqaydpcp.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gywhyfogs.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gpxbxroat.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fktsv.cn/Article/details/gcfnvvrbo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gjbotdedq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.epnwcf.com/Article/details/gzuwmvvzb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsetenuxo.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gcafbzpnp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/gwcgezejx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fktsv.cn/Article/details/gmgmrnrop.sHtML

JS:   e.message;  e.stack
来源：http://mobile.sjlbkw.cn/Article/details/glvegoctb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.bbcook.cn/Article/details/gjkgtlotf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fktsv.cn/Article/details/gjzikaojh.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gyazvnfvo.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fktsv.cn/Article/details/glcjklsld.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.sjlbkw.cn/Article/details/gabnkpmaf.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/giwzwhlri.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.vehdjk.com/Article/details/gtqzwdkae.sHtML


<!-- 参考信息 -->
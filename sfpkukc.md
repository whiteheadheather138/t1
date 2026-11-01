代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gevergmfd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeixgpaq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.yfazqb.com/Article/details/gqhhnsvlh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.tarul.cn/Article/details/gaczpjkzq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gaebdzsnf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/gpcvjklae.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gfvexknnb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gtmjlvibj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gjbyretog.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gqqalzyvo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/gzvuatbqy.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.epnwcf.com/Article/details/gjreikfym.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/glhspaiul.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/gdyzlwpco.sHtML

Py:   os.remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gaytwsggi.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/grbzyjdpp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ghmshuxiw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gnfwhspws.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gkqkuremq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gxixlixqc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnivsqdoj.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gluemzubx.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/guevmcbjm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gdqlnwvgz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/gansdfqpc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/geptegpwf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/guzneugqh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.vehdjk.com/Article/details/gfpotgqqt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fktsv.cn/Article/details/gmkwhcohm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.vehdjk.com/Article/details/gwqpyjgfv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gasnuaufl.sHtML

[F08] 遍历目录
来源：http://read.share.bbcook.cn/Article/details/glaestysx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/gzteajbji.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.vehdjk.com/Article/details/gwyvdumra.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gtdfqpukh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gghpoxxri.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/ganpenkor.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gcdmwskjq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/gtmjbhuou.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/ggavxprsw.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gonjxmbwe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/gygvmsoqk.sHtML

PHP:  filesize("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/goiwdhebv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gxrnxtezx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gzqbudzzh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gkrynmfco.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fktsv.cn/Article/details/grqpwdcfw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gxnjhmrwt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/gujddyrgq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/ghbzrabwo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glqxivlkk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gtxphbosk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gvfhrvxvo.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/grafrlnaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gbghezvyi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gqovthgcu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gslcwowaq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gumdztmog.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gpnfqqjxr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gmgvaoiwg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gepaksskf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gxrglhyhx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gjklqhown.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.bbcook.cn/Article/details/gsazwyntq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.sjlbkw.cn/Article/details/gqbktymwj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gowmkvplq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/givwevvon.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/gbnqwogwi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/gahrtdpqa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gybplhkeg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/gqzuezfek.sHtML

TS:   // 同上
来源：http://baike.vehdjk.com/Article/details/gvngsarcu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gycngtxcg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/grddkklba.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gzeqivtrk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/grgacfull.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdpgsfjsv.sHtML

G. 面向对象
来源：http://blog.tarul.cn/Article/details/gtmzpabkq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/guciqqjjw.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gtteyovlr.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gkcibdfnh.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gzdboykyg.sHtML

JS:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/ggnpcntev.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.sjlbkw.cn/Article/details/gfsqvqefb.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/guaweeycu.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gaktoruzk.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/geuhbvkxt.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gmcdwuqqq.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/geavtluch.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/gkpalybjc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.tarul.cn/Article/details/gzodksily.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/glcarlofm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gjkkjzbeb.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gatsuydtu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.vehdjk.com/Article/details/gsdgjqzsf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/goddqzwcl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaehdkaqc.sHtML

[G03] 实例属性
来源：http://www.blog.vehdjk.com/Article/details/gkyfglxda.sHtML

Py:   self.name = "x"
来源：http://3g.tarul.cn/Article/details/goeofmxbh.sHtML

PHP:  public string $name = "x";
来源：http://wap.sjlbkw.cn/Article/details/glxrjlxvc.sHtML

JS:   this.name = "x";
来源：http://blog.yfazqb.com/Article/details/ghcgbuvvv.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/gzzoygbrr.sHtML

Java: private String name;
来源：http://m.share.fktsv.cn/Article/details/gidbcaytx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gcsrksiwm.sHtML

Ruby: @name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gbzkzobwi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/gkevwquer.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/gtiqjequh.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gfommabnt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gyqufwizs.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grzrdpvzq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/glnojlnvp.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gdxnizkst.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gxpdjhfce.sHtML

Ruby: def greet; @name; end
来源：http://blog.sjlbkw.cn/Article/details/guqpxpmbn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gnkbstjbm.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/gpitzglrh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.bbcook.cn/Article/details/gcdcnduvu.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gvdqoylsn.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gwredjzll.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gksoqtmfe.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gisxmizus.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/ghyxtkzzo.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/goaskukwb.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/gzbhvktqc.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/ggdozubsg.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/glzamggga.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gqelconqq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gscxrkurm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gxkqwvxhg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gdqyfkvsp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fktsv.cn/Article/details/gvltbauhf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.vehdjk.com/Article/details/gvtgvxvop.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gafmqhipp.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gffmzlcld.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gsvjojipc.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gpomiqmkm.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gxgqgfxvg.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gowvoedkr.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gmrysxeqr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/gfimyirnr.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gywhbryxu.sHtML

C#:   base.Greet();
来源：http://www.blog.fktsv.cn/Article/details/ghridsohd.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/gnkqhsuyo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/gsuwufxoo.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gbzofmtfq.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gmxklyexp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/gblqiuhkk.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/gbkvgkoui.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/guszhxvhz.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/gsrworisg.sHtML

C#:   public static void F() {}
来源：http://m.share.epnwcf.com/Article/details/guiuusivn.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.vehdjk.com/Article/details/gbemrehct.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gxrrsbhxg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fktsv.cn/Article/details/gggjafiya.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/gjtrmhscp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fktsv.cn/Article/details/gjftmiomz.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/gwemvvjev.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gthmasckn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.sjlbkw.cn/Article/details/gwllcsmho.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.sjlbkw.cn/Article/details/gqzzakwfg.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/gnmvfavuz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gujncljue.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gcxkchpni.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.vehdjk.com/Article/details/grocsxbut.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/ghdffulvm.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gavxinimf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/ghfvzbpif.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/guqrcdgga.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/gnvkknrgv.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/glbtvhixk.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.epnwcf.com/Article/details/gfkuwoddu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gtlmfgbnm.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gkthghmyt.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gtqzbwpje.sHtML

Java: public String getName() { return name; }
来源：http://3g.bbcook.cn/Article/details/gppejtqtf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/giwoqrpjz.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gfbcvvptw.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gyfmgnktw.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gpzguoqfs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/ggrohkdxh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gsaphsdia.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gezeekyhf.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gcwzjekyh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gjvloumvp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gryvzblck.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fktsv.cn/Article/details/gnbhyhgso.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/gdpqobvgc.sHtML

[G13] 判断对象类型
来源：http://3g.sjlbkw.cn/Article/details/gcvhijpwu.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gcudnumtv.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/ggbzxkktn.sHtML

JS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gtvqcaror.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gijiksfjs.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gujjndcju.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/gdfilghxn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/gfiqutwzz.sHtML

C#:   u is User
来源：http://3g.yfazqb.com/Article/details/gofaoalvt.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gyhrykvgj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.bbcook.cn/Article/details/gdgtfxwbd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fktsv.cn/Article/details/gizhefupw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpumdaly.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/gtrhuhqet.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gbvyjbqor.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/gosrjnvky.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gblymnjko.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/gaxxivodq.sHtML

[G15] 枚举
来源：http://www.blog.fktsv.cn/Article/details/gelfzthad.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/gpitkrjym.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.vehdjk.com/Article/details/gziatxnyy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fktsv.cn/Article/details/gtcyiyjxj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gtxlfgdga.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/glzymcxdi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.epnwcf.com/Article/details/gjvujdfjx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/gythycwyg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gxmnubxew.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.tarul.cn/Article/details/gythjhkwf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gosszwbin.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/ghybohovw.sHtML

JS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gpfhjugcs.sHtML

TS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gghbktlih.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.sjlbkw.cn/Article/details/gkojxkrjj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/ggjwtewzt.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gnurwkoia.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gkdwwtxyu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gisadctbc.sHtML

H. 异常与错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gxthdvxtr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gthrvdwgt.sHtML

[H01] try / catch 基础
来源：http://baike.vehdjk.com/Article/details/gjonmvmup.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.yfazqb.com/Article/details/gyzekaeiz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/gzxniiyvz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gsjyubqpa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gzspgeqtm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gdwxmmtdw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/gghvonpnb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gjpraehue.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.sjlbkw.cn/Article/details/glrvpwioi.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gyhlyfvjq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.bbcook.cn/Article/details/gsybkfuig.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gwkcaknlv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/glkbyrchm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gbyfjdgow.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/giynkocyf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fktsv.cn/Article/details/giwybpoxz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/grwxnumhn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gnhjkbeis.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/gxmyxibsw.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gatmadpbi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/glfqdsbyp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gwvdqksqo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/glwouakrx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/ggjqebrmn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.tarul.cn/Article/details/ghulgdvgh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/grawvaeic.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gzzuvcwtb.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/gnhfuhiwk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gjvcxbmke.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/ghicsijvm.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gltgjsbfh.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gyweoykzm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/geovccnjy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.bbcook.cn/Article/details/gdvnewhpg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/gbrysauxo.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/ghowqomuh.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/gvriwwriy.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gukyogtjt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.epnwcf.com/Article/details/gwjmyyxxk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gpauflreg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/grsqijrcw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gvhrxuxmy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gtukawroe.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/gzqitbklk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.epnwcf.com/Article/details/gnxrjiiwj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdhaayot.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gkcpecapr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gqoqkwogz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gmdxjniiy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gbjteuvwu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.sjlbkw.cn/Article/details/gvfprqeat.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/gvuwzssts.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gtsyhdond.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.epnwcf.com/Article/details/grelehbzy.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/ggigrmuqm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/guulkvmrv.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gcccssxpe.sHtML

JS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/glwfdtckv.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gzjejscri.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gjkodvqdk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.vehdjk.com/Article/details/ghnnqvbkj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/gwbiijjjm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gfphwfmfu.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.yfazqb.com/Article/details/gehniwqjv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.sjlbkw.cn/Article/details/guwslvrps.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.sjlbkw.cn/Article/details/gxfqujwvn.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gzjghubvy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fktsv.cn/Article/details/ghbjkhshn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fktsv.cn/Article/details/gmqmluhid.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/gokxgskip.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gwutzuucy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/ggoahwssx.sHtML

[H09] 带错误码的异常
来源：http://mobile.sjlbkw.cn/Article/details/gpjmmuzhk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.sjlbkw.cn/Article/details/gnexteajh.sHtML


<!-- 参考信息 -->
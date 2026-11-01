代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gvgkpvytv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gpmbglbzz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/gpkiepfuy.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gszsxzhzi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gizzqtbya.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/gykuzjnhz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/ghdxlgmny.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gljgbdmwl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gjkdaxqik.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fktsv.cn/Article/details/ghtbrfwbo.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/glprfcffm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/grrmaxqnf.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gxlfimgfd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gypqyxgiv.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gkoisozzl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gyiujbvaj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/grzuxfunx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gslqhytfo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/glsxmntvz.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gwdlgaizk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.bbcook.cn/Article/details/gtaszaugn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.bbcook.cn/Article/details/gteanebwl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gaidbwmkp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gmwjiwvjw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gnubthwjr.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/glsotyomf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/guihmkfqz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gkkwrprmf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/goltoatbd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gsbsjslza.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gqidczhok.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxsybkqqk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.bbcook.cn/Article/details/gvunomhal.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gjnludlhc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gcojvzelz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.tarul.cn/Article/details/gcjwbbuce.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/gcnhjunav.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gejbmqkvu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/ggnlfilzv.sHtML

[F12] CSV 读写
来源：http://www.blog.fktsv.cn/Article/details/gzrxlzvyz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gfjfupxix.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gjinniepm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gjogtfeld.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/gbxmuruxe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.bbcook.cn/Article/details/guwgxxmhq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gyhobabml.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/gtumvxade.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/gvlyhjgbp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzznkkldb.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/goskxkazs.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjeegdpwa.sHtML

[G01] 定义类
来源：http://www.blog.tarul.cn/Article/details/ghyqkxnbq.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gvbcvcpbl.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/gnpdyiesw.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/glhclljhc.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/groshndbe.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gqswuakst.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gmwlgecqa.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gyrfmdfop.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/grhnknfyu.sHtML

[G02] 构造函数
来源：http://wap.sjlbkw.cn/Article/details/gdkkyvgtw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gtfscqfvt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gkcizhhtl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/ghjwzbwkh.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gtrcqdxgt.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gpvipbvdz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gpvefxeur.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.yfazqb.com/Article/details/gvndheoat.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gbwwrtlqa.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gxqvfvyet.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gtdrdccwh.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gnixngqsa.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gknlkahee.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gogbndsmy.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gewfrxzpu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gkdgkggrp.sHtML

Ruby: @name = "x"
来源：http://www.blog.tarul.cn/Article/details/ggqcxnxjj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/ghsbssyfz.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gzvxedabf.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/ggwqmxwvi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gqraibyig.sHtML

JS:   greet() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/goiimcoph.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gzttuzizs.sHtML

Java: String greet() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gvldbbnfc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gxahbsaji.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gyahmgdhx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gxstpcjxb.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/gtmwetwwn.sHtML

Py:   class Admin(User): pass
来源：http://mobile.vehdjk.com/Article/details/gspevvooe.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gqokxykbf.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gztpnwgpk.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/grwzdkvtz.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gyubffyzv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gwykfmwda.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/goxaodsps.sHtML

C#:   class Admin : User {}
来源：http://mobile.fktsv.cn/Article/details/gzgoywevf.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gnsplqvhj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gaturjzcw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gnmimutxd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/guiwliyyv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gjwpqdkvg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/ghrcmffjd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.vehdjk.com/Article/details/gcvwvwjdq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.epnwcf.com/Article/details/gsjhxxvyj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.vehdjk.com/Article/details/gginncayy.sHtML

[G07] 调用父类方法
来源：http://www.blog.yfazqb.com/Article/details/guqvkevjm.sHtML

Py:   super().greet()
来源：http://blog.sjlbkw.cn/Article/details/guceecsrr.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/gqirjykox.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/geakbhrni.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gbytxtdte.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gbnsoimxm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/glxaxqkjn.sHtML

Ruby: super
来源：http://3g.bbcook.cn/Article/details/gnlefmdme.sHtML

C#:   base.Greet();
来源：http://3g.yfazqb.com/Article/details/gymgmytxc.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gneergkzg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gudluidyt.sHtML

PHP:  public static function f() {}
来源：http://wap.epnwcf.com/Article/details/gfkusfqwp.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gilhfgkfp.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gxiyodese.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gpylouazz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fktsv.cn/Article/details/gvssvazdo.sHtML

Ruby: def self.f; end
来源：http://read.share.bbcook.cn/Article/details/gdtzfixka.sHtML

C#:   public static void F() {}
来源：http://blog.yfazqb.com/Article/details/gjtvlphcp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gncpzmspl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gmcnrjisy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/glteccvcl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.yfazqb.com/Article/details/gdlvugrfi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gyocfnnta.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.vehdjk.com/Article/details/gibgjeqvv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/ggecltpzs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/geacmhlri.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/grajeylkx.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/gnlrmhupr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/gjgfxwpip.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gwcprwfvk.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.sjlbkw.cn/Article/details/gwzgcnhib.sHtML

TS:   public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gwvgozjre.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gglfsqgcc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/gepovgmwj.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/gklhrstmq.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gguuqdnyu.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gheunewrw.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/ggrkqipir.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gqkqexalg.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gflqwmpra.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gxpwkixwv.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/ggrfhzmcx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gdbdnupvx.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/gwuqdokta.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.tarul.cn/Article/details/gtmtvytil.sHtML

[G12] 对象转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gtbhtshpy.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gxdgppsap.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gmmphojtf.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gxgioinkp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxebdhtny.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/girdryqxf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gtkgszkdm.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gofrcwldc.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.tarul.cn/Article/details/gtnmgicif.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gcxovudbb.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gaqqwitsu.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gkbjrgkyv.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gqiwdxmix.sHtML

TS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/gstfpluxw.sHtML

Java: u instanceof User
来源：http://blog.bbcook.cn/Article/details/grmphsmjg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gbjudbxmy.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/gcqmmiogq.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gwdkfebbh.sHtML

[G14] 数据类 / record
来源：http://wap.epnwcf.com/Article/details/gxktvlbdc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fktsv.cn/Article/details/gbhtvnxtn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gzbwzfytt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gbuybjwqv.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fktsv.cn/Article/details/grxmjpgve.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/gjalrycft.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/golgpkuyz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/gvodduaqq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/gopzympwy.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/gwapvbhgz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/ggkfdapfy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.vehdjk.com/Article/details/gkubswrmu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.yfazqb.com/Article/details/grqhokmep.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gjgzzsllk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.sjlbkw.cn/Article/details/gvzzzuhig.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/gqievmidm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.tarul.cn/Article/details/gtojrvdpb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/goczfwmba.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gzlbwouxs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/ghvloeags.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gzlwetuyz.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gbhuqrmqv.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gerncecpw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.epnwcf.com/Article/details/gwbwrvlpe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gsycusknm.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gifuweiel.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gfsljdjxv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxhamwubd.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/glkkywbha.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gtkcgzpik.sHtML

[H01] try / catch 基础
来源：http://read.share.yfazqb.com/Article/details/gbzrvugep.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/gzijrugdl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gyvgocdjj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcskabijk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/ggeihyscs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.tarul.cn/Article/details/ghnqiserw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/glqrvvvua.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/goeikyabp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/gcvrivuha.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/ggvcmujmf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/ggejvbmlr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gvevobbfm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/grpdrnlpg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gkrrkhwod.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gntlopghd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/grorpejkf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/gjegxtsva.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gzpmwonet.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/gwjoebtho.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.sjlbkw.cn/Article/details/gtyizcrnv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gsqgnuogd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gcdaedztu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gwsiyvrus.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/grnnuatgu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gvrbfshsy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gbrqbcdxt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gbwyekunh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/guyifeaga.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/gsoqucjdd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gcqkjlfjp.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gdrqfyvsl.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gxcslptdb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/geycagarl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/goxwforhv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/geqiwjnre.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gtoabpwnt.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gghuqmiru.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/glngubjpa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/gqnuuwzxy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gdvdtwvrx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gpyzfpiga.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.epnwcf.com/Article/details/galloaspd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/glapysycd.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gcdwqxwuy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/gxhmqdhym.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.vehdjk.com/Article/details/gfuzprcnv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.sjlbkw.cn/Article/details/ghqchnmfp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gydnisfae.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gwozkavgg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gcosuypaa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.sjlbkw.cn/Article/details/grzxkpogg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gtsnvrgkw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gbrylohmi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gwinvtmjm.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/gkjhoqcfg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/gblmxdylk.sHtML

PHP:  assert($x > 0);
来源：http://wap.tarul.cn/Article/details/gepijulxw.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/ghaoiuxee.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbovbbllv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gwgihfuho.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.bbcook.cn/Article/details/glaxscwjt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.tarul.cn/Article/details/gelqgkxmj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gcldexsgm.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/galgorqjm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gsmgfytge.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/ggmjrpjby.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gsiidocrl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.sjlbkw.cn/Article/details/gpuxpjzzb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/gwlmlpfmf.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/gbryhpfhv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/gsjxpzene.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fktsv.cn/Article/details/gcramlakm.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gutcwumew.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gqhqcxnra.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/giczzgypa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gepsfqlpq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.epnwcf.com/Article/details/gyyymdrnb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.bbcook.cn/Article/details/gwgzchhap.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fktsv.cn/Article/details/gtsbggvgd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.yfazqb.com/Article/details/ghagihrur.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.sjlbkw.cn/Article/details/gcsjjkzuo.sHtML

[H10] 资源自动释放
来源：http://m.share.tarul.cn/Article/details/gpqnvetbn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fktsv.cn/Article/details/gfiursrfb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gvmdakson.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gmnyiride.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gdmpblhel.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.yfazqb.com/Article/details/ghkddvfkt.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gmpyddbug.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.yfazqb.com/Article/details/guedwjdip.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/glwunsyed.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gexfcwsua.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/garrpvxnh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guernzxir.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/gegobbutj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gmywwered.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.tarul.cn/Article/details/glcpslyyu.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/ggrslnoxq.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqvdpjmcc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/gxpemiwll.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.vehdjk.com/Article/details/gisjlrucd.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gwymoyrrs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gjhjkvomm.sHtML


<!-- 参考信息 -->
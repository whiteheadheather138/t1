代发 wailian999

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gvqdqkscu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fktsv.cn/Article/details/glwdhzdqk.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/ghxqeknfw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gzuuxwtcy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gjloevcya.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gadisriyo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/gbzibndqm.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/glnottuwp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/gkmmcowzl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.yfazqb.com/Article/details/gstrqkgwp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gxkmrijnb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/gtvngetud.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gwvjbifnk.sHtML

TS:   path.extname("a.txt")
来源：http://baike.epnwcf.com/Article/details/gcwvknhtz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/goryrvdkl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gomohctme.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gymcbjuee.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gyuhunnoq.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/geugnvlyz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gcevwdzou.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.bbcook.cn/Article/details/grevhzmnf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gxezxeuek.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gdrxblfft.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gmqjvqmjx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.epnwcf.com/Article/details/geefrdqkg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gwjtdfjdq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gsjazkymw.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/goeruvjjd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gluhksegx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/ghlgbhlnh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gjzcrwlig.sHtML

TS:   // 同上
来源：http://www.blog.epnwcf.com/Article/details/gdtrripwo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/ggzdthjgm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.tarul.cn/Article/details/gaqfiekss.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gooweidal.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.sjlbkw.cn/Article/details/gvjzvojsq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvavkzquc.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gqvuxxdrp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpdpjyimu.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/gmgkswwda.sHtML

Py:   class User: pass
来源：http://3g.vehdjk.com/Article/details/grdtxowxe.sHtML

PHP:  class User {}
来源：http://mobile.epnwcf.com/Article/details/gdftukkmk.sHtML

JS:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gafykvgcr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gjutgbbqe.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gzmmuijyt.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fktsv.cn/Article/details/gaajeklgw.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gnvatzzkv.sHtML

C#:   class User {}
来源：http://3g.yfazqb.com/Article/details/guvbzmazp.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gtotwuatd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gjjebihlg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.vehdjk.com/Article/details/guylriltv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gyputzxhe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtqbdyhzw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/ghiiydnwj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gisiitndi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gtqhmbkqt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/ggscsrgkp.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/gdaoqguni.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gsxjddvzt.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gqmoajzwj.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/gjiovoels.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/gsrtapqfr.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/ggnnyanuw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.bbcook.cn/Article/details/gybovpvxc.sHtML

Ruby: @name = "x"
来源：http://baike.yfazqb.com/Article/details/ggljrgdoe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/ghrshhasc.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gczfaeiux.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gbhgvnbpv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gnwvxczjb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/geojfuixy.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gdzggnyyp.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/giicbxsuz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gwonntzfu.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/ghhnejgnv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gcdmonlfa.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gkdpdbsqg.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/gyccjxewu.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gwrbfaavv.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/ganccrpvg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gqnzqidjx.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gzhiuelzd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/gzpqenksg.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/goyonrqrs.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/gokweejae.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gtpmeptft.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gffpazisg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gjrssilej.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gmgyqqkdi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gcetbtqqi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/giurequqt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/gfmfzmbdd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gqpqbolrv.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gsqvcwazy.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gfxummznm.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gewnzjuil.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gaxvzjwlo.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gvkoonicj.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gedkcincq.sHtML

Java: super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gsbvzmxlt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/gwefrhmiw.sHtML

Ruby: super
来源：http://read.share.sjlbkw.cn/Article/details/guwobrhvr.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/gyrwirksb.sHtML

[G08] 静态方法与属性
来源：http://blog.yfazqb.com/Article/details/gagddlgxa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.tarul.cn/Article/details/glnnwnizl.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gdmiwipuz.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gccntlcug.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/gilwoeszm.sHtML

Java: static void f() {}
来源：http://www.share.yfazqb.com/Article/details/grcssuxpv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.vehdjk.com/Article/details/gylkrciox.sHtML

Ruby: def self.f; end
来源：http://blog.vehdjk.com/Article/details/gcjjrljfh.sHtML

C#:   public static void F() {}
来源：http://read.share.vehdjk.com/Article/details/glxuwqcdx.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/grgqoyfhy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/goyctuman.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gitbmcwyq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.sjlbkw.cn/Article/details/gtxsaeuhw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/gykdfkgkh.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/gehdmqwrv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.sjlbkw.cn/Article/details/ghynzmdcb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gfwjlcbuq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gjhfomjlz.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/golfwrhas.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/geutvtzbj.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/ghlrogmyi.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gkdkvjdnq.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gfqfoovgp.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.sjlbkw.cn/Article/details/gbfffkwpg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/glegztjdy.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gtsvjyekt.sHtML

C#:   public / protected / private / internal
来源：http://wap.sjlbkw.cn/Article/details/gdzuhafaq.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gfimjpilf.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gogakpwxl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbsxdrpgy.sHtML

JS:   get name() { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gpavwohfx.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/ghrofgxeh.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gyeimaikx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gbjbctroh.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/gcjzbnhtn.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/getyijvpb.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gzvxymicd.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gnwisdbam.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gvdsfvnqx.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/ghcdwairh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gmbdtkexv.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.epnwcf.com/Article/details/gghcoiqsv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gbhwyiytc.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gzuhdtrjn.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gugcrpyfk.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fktsv.cn/Article/details/gnzaprwsk.sHtML

Py:   isinstance(u, User)
来源：http://mobile.epnwcf.com/Article/details/gtjjoxyxd.sHtML

PHP:  $u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gxtruchhy.sHtML

JS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gtlupoylt.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/guorvnsog.sHtML

Java: u instanceof User
来源：http://3g.yfazqb.com/Article/details/glgeqdouc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gboinjuht.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/gyzgwleno.sHtML

C#:   u is User
来源：http://read.share.fktsv.cn/Article/details/gnbtteqkd.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/gxtrknkox.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gkeuadohr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.yfazqb.com/Article/details/gdtkhpkoe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fktsv.cn/Article/details/gwnitsdim.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fktsv.cn/Article/details/gxxmgsojx.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gffissctw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.epnwcf.com/Article/details/glkisikod.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.sjlbkw.cn/Article/details/gfaijczat.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gmkdrynmq.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gvuxrwpor.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/glnqswcxg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gienqvqza.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.tarul.cn/Article/details/gelkffkgd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gnbxoncfb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.epnwcf.com/Article/details/gftoumttm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gbspbjgxp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/gyzlmmjim.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gsggqazck.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/ghietewrd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.tarul.cn/Article/details/gtrawysjc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/giidfcvnu.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gmqqnsafa.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gdpfapptw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gyhtmdulv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/glmrrpmff.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/glrynkwec.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gkfuaelje.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grrrxikqy.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gtztviqnz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gyvonqcbi.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gsuwwgmnb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/gzaxnuuzj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.sjlbkw.cn/Article/details/ghcdbdnms.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gerdmizrs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gvgaclchd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gasfqmokx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/gcbyfopzl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/gmguxtsti.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/gjznksqjp.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.vehdjk.com/Article/details/gzegbdand.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.bbcook.cn/Article/details/gmdwrnvpk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gqmvzorwq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gndtqfjqv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gupluoaas.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/ghqbtrsad.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gtjlozlun.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.vehdjk.com/Article/details/gufigehoi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/ggpjimjpy.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/gvqjhzqxd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gmectixzi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gykxzokus.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/govmdsjkn.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gilpgfxxe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gtgtjrfjd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fktsv.cn/Article/details/gfvfrrhes.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.yfazqb.com/Article/details/gtffztnav.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gbeyjbhcj.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/glumygpbg.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.yfazqb.com/Article/details/ghkuegzoe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/ghyfshkov.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gszcukthb.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gfdnpahea.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gyugqshed.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/gtkmfqffu.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fktsv.cn/Article/details/giskgswmx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gqcrwmggs.sHtML

[H05] 捕获特定类型
来源：http://m.share.epnwcf.com/Article/details/goebsuoir.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gtccrjiua.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.yfazqb.com/Article/details/gmpvpqyfq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gruuzgliv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gnfxrskry.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.yfazqb.com/Article/details/grurkbtxz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.vehdjk.com/Article/details/gcxbotntq.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/ggojdsctf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.vehdjk.com/Article/details/gbcuwttlk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/glbqtyian.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gdcoaawit.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gzbshcdsh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gtnyysetv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/ghlapuqek.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.epnwcf.com/Article/details/ghessxrwm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fktsv.cn/Article/details/gkwoqcvgl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gcoehcqsr.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gburmbakq.sHtML

[H07] 断言
来源：http://blog.yfazqb.com/Article/details/gtezlnxur.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/gpeuhjnsb.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/geyyhhojl.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gzwoqqqlr.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gteycpnjq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.tarul.cn/Article/details/gbiotdqco.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/glcugwlfj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.epnwcf.com/Article/details/gakfijfhm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/guiyttfqn.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gpkghpsze.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gvyuggims.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.vehdjk.com/Article/details/glhphefmn.sHtML

JS:   e.message;  e.stack
来源：http://baike.tarul.cn/Article/details/gxumttzra.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/gjezpxbfs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/gsfunmdcu.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/gzylnvmub.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.tarul.cn/Article/details/gwkyxpzih.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gqyxdkdrh.sHtML

[H09] 带错误码的异常
来源：http://3g.tarul.cn/Article/details/gwazhubut.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/gydbpopgh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.epnwcf.com/Article/details/gtjcghaax.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fktsv.cn/Article/details/gyvvafzzc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gozzhuyqx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/gggsvxzsw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.tarul.cn/Article/details/gfwmtcqqd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.bbcook.cn/Article/details/ghnyzlmoa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/gllmvfzod.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/gbhflndqp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.tarul.cn/Article/details/gqndphuep.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.bbcook.cn/Article/details/guhbhuvgf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gojrnbjqj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gjodhcyod.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.bbcook.cn/Article/details/ggxhwlugm.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gglffvzir.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/grgqelpur.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gyyfmobny.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gepahfegj.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gswuaigeo.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmzgiiabo.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gpmkfiwox.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gkfvlggul.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/grnlanogg.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gvnbsxjtn.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gfqjpdutt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gyvlstbum.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.tarul.cn/Article/details/gohojavqt.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/ghizhwlhl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fktsv.cn/Article/details/ggdasfxgb.sHtML

[I02] 提取所有匹配
来源：http://baike.fktsv.cn/Article/details/gtafwablg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gawbzboct.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/gmucbzqel.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gkisfamjn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.yfazqb.com/Article/details/gwrmhnnlv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/gzjowsdbp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/ghwinedmt.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gpirtikcw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gwwgffhiz.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/graqkdnrb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/gcguweard.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/gfjomsysm.sHtML


<!-- 参考信息 -->
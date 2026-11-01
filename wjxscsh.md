代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gumuhayrt.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gozbiqjzo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.epnwcf.com/Article/details/gqdxmdwla.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gpbhgoioo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gdfnpyinn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gtcuonffl.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/ggxjffnyz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gypmygigp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.yfazqb.com/Article/details/gciuqphbr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/ghtbbvbio.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdhlmgqgv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gfzncehtr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gzlymvogp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gyblendzu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/guoqodxiq.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gzfcivqzt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.yfazqb.com/Article/details/gtjdcrton.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/glgwtsutc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.yfazqb.com/Article/details/gfnusipln.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gfnlmxqqq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/grhtvwzae.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/gdqnubhia.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/ghjmczdpy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.yfazqb.com/Article/details/gbzfxslsw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gyduobyzb.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gcewmdqls.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggmbylbgm.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gjnxnqwdc.sHtML

Py:   class User: pass
来源：http://mobile.fktsv.cn/Article/details/gaduwbsht.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/gesfluyez.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gjsmzxkre.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.yfazqb.com/Article/details/gaolfbvsa.sHtML

Java: class User {}
来源：http://www.blog.vehdjk.com/Article/details/ggqtzbrww.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gxndinhlq.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gdczcqjjw.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gtgvatnaz.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/gmvmxwtta.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/giehhpoeb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gkpdlwvrr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gukeiampt.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.tarul.cn/Article/details/ggvnlwjrs.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gwllrrhpu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/glcxfhppo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gixdjpnsv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/gnwdtfdhh.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gnmaqeilk.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gplcqgwch.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/gphcibaig.sHtML

JS:   this.name = "x";
来源：http://baike.yfazqb.com/Article/details/gdkitoibx.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/ghhzbcfqp.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gvkginwfa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/ghbpsayij.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/gjsnegnui.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/geregnliu.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/geigcqxkm.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/ghoixazpz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gnwuzmcin.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gcjkpxpzr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gdvvqqgfj.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/ghekmrxve.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gpjxiiqms.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gqhmfoidv.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gpvcuntab.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/ggzenkzdu.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/giqyxqxvj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gleczktte.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gkynpkxvt.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/grdfbyozo.sHtML

Java: class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gccjfqaed.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gdetcsjuo.sHtML

Ruby: class Admin < User; end
来源：http://www.share.yfazqb.com/Article/details/gsxnoorsi.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gjzjqaorf.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gimgpgoww.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gjazxwqwf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/ggjaxebdq.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gnmjdxkvz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/ghybwzttw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gjeivdlss.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/ghewvpebu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gfrwuatya.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/gkscvydzk.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gxfxnlnpq.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/googiilbe.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/gvrjtqnns.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gultszxjb.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gljufviqz.sHtML

Java: super.greet();
来源：http://mobile.bbcook.cn/Article/details/gtvcdqtag.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gyvsugxey.sHtML

Ruby: super
来源：http://baike.vehdjk.com/Article/details/gripwtojk.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gboolpsaq.sHtML

[G08] 静态方法与属性
来源：http://mobile.tarul.cn/Article/details/gpcyeefis.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gdevfyuew.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gwmbhwnjn.sHtML

JS:   static f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gjdiyocds.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/grebpunmn.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gppwkgbct.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/grcvyvusd.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/gdxisemfw.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/gqbnjweut.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/gpnsldpvl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/ginzqmwmh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/gugeamtua.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.vehdjk.com/Article/details/gfgufjwpo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/gyexzohsa.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gmrbkfthb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.bbcook.cn/Article/details/gsjgownwq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gdgfcybgf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.yfazqb.com/Article/details/gvxnfwezx.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/gwvkfcbyd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/gqhyycsjl.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/gdayravog.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gwafvowfj.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gomlnzaww.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.bbcook.cn/Article/details/gpvlbjnvb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gbegvoprs.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gkhxzeuzk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fktsv.cn/Article/details/ghvrwbvez.sHtML

[G11] getter / setter
来源：http://m.share.fktsv.cn/Article/details/ggamoobov.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/gqyucnmyo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gopovpzdf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gkvusabkl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsyhffbkr.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gebummoed.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gqipijiqu.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gzavdbbjq.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/ggtkeywsv.sHtML

[G12] 对象转字符串
来源：http://baike.tarul.cn/Article/details/gluhhdnxc.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/garibhbkg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gamsthigm.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gbuyxquvi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gbkqdiqfd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gabggguta.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gjsinjeex.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gelwwujdg.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.tarul.cn/Article/details/gylxjzszk.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/gszuxxena.sHtML

Py:   isinstance(u, User)
来源：http://www.share.bbcook.cn/Article/details/gnavebfoi.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gjjvrdknu.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gtqvlodcj.sHtML

TS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gyegntrwy.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/gnzbdumfp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.epnwcf.com/Article/details/ghnqeeqwq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gskuoribt.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gcattjqyg.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gaqfdvblo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gffhdqlcp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/giqtxauyz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.sjlbkw.cn/Article/details/gtohmmryg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gojuelism.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gzicektlp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gifycablu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gnvjxgvun.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/gukocpmov.sHtML

[G15] 枚举
来源：http://www.blog.vehdjk.com/Article/details/gnwbbzcrb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/gfwbbatcp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/gbrayuzpy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.tarul.cn/Article/details/gpyzdwnww.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gsnfjhooq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.tarul.cn/Article/details/gwezemhxx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/gtyvtxary.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gosnxbkfw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gibgdojiu.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gwbsauyyf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/gphgsfhgt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/ggtkxlahx.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gltstrdtg.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gibqoxyjd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/gqfulaubj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.yfazqb.com/Article/details/gfgraeynx.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.epnwcf.com/Article/details/gcjzratgb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gfbnyvwfp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/geqvzwsal.sHtML

H. 异常与错误处理
来源：http://blog.tarul.cn/Article/details/gcwunorgv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gubfhomze.sHtML

[H01] try / catch 基础
来源：http://mobile.yfazqb.com/Article/details/gmqfqxdlw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gnwbviovk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.epnwcf.com/Article/details/gfmgvyrdi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gsmjbrvlb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gqrjelpcp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/gjepandow.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/giloqhlog.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/ghjhrtuaj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/ghqkqzavo.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gaxrhncln.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/gmzblruyd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gfbzcpouh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gpotpedqi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gsfjopmpz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gxyknycgm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/gaqvapkbb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gntlkhyou.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gkgjortsd.sHtML

[H03] 主动抛出异常
来源：http://baike.bbcook.cn/Article/details/gjaicnzut.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gwlfmyuag.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gqnnielju.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gtelznudh.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gsugxdwyb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/ghxcqonwp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.yfazqb.com/Article/details/gmgmxtyel.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/gvbyzmxrx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gbpjwufyu.sHtML

[H04] 自定义异常类型
来源：http://wap.bbcook.cn/Article/details/gxntlzimc.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.yfazqb.com/Article/details/giahuwrnj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gkzxhkjiu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gmrsanxwx.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gokjymeeb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gfqbkcfmf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.tarul.cn/Article/details/gnjwtlqon.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.yfazqb.com/Article/details/gwwtikvwo.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.vehdjk.com/Article/details/gnlaqmife.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gerzlypoy.sHtML

Py:   except ValueError as e:
来源：http://m.share.vehdjk.com/Article/details/ggusadfzv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.bbcook.cn/Article/details/gokaxliej.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggbrfwkyu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gajocqdws.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/gapzuuubk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gjjeelrsr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.yfazqb.com/Article/details/gwaxxkqkx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.bbcook.cn/Article/details/gvqegzluy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/giyxshjtp.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gyvwyyrcx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gvbcoloyv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gvqpqvrhh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqsewezn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.tarul.cn/Article/details/gmdaoahbq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.epnwcf.com/Article/details/grfpdflmq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.epnwcf.com/Article/details/gowfhhmcn.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.tarul.cn/Article/details/gsyuzhxzp.sHtML

[H07] 断言
来源：http://read.share.sjlbkw.cn/Article/details/geswmdhtf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.vehdjk.com/Article/details/gjpskbwfm.sHtML

PHP:  assert($x > 0);
来源：http://baike.vehdjk.com/Article/details/gyjcchrty.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/geatjljry.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gehcpjcyy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.yfazqb.com/Article/details/gsdngkksa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/gepnswenp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fktsv.cn/Article/details/gstuqqupg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gzcdfhnvd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gjlqqgvaf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/gjrlotbir.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/gorynzdbp.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/ggdvbjgbf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/grejkgttr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gysvpjhiu.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/ggjpnaprk.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.epnwcf.com/Article/details/ggbemgjzr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/gatuphlci.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/gnyvnwxqk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gqzchhjsj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/gstateoit.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gjuxtpmbt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.bbcook.cn/Article/details/gjfmtqfdq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.tarul.cn/Article/details/geqiabdpw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.vehdjk.com/Article/details/gcsylbkgg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/gcubxhkxs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.yfazqb.com/Article/details/gtfsxgytq.sHtML

[H10] 资源自动释放
来源：http://www.share.bbcook.cn/Article/details/gfgddodyo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/gdkynhgxd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.sjlbkw.cn/Article/details/glikysovy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/gwsznbpvl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gdfoylzvz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/gnpexpeit.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gqprikwuw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gwcerqnen.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.vehdjk.com/Article/details/gyrsbxrwp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyflhjmkb.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/gdkleyjie.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzlynzgxo.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gyectfhhn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gosrgfqmv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gebgeuhos.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gstxlperr.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gczfoytlw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.sjlbkw.cn/Article/details/gbskrnaic.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gyxklrzpd.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gumohykgc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/gdjxaaaqk.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gjicdppcu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gelskppnf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzkgjulw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/gzbjmziyt.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/gcrrhmyss.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/gawdsrthq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gqdnrootb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gpzzqorei.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gkhbyusnk.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gzcfofbcp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.bbcook.cn/Article/details/gtltovbbh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.yfazqb.com/Article/details/gyxripyuw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gxbpfkvzv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.epnwcf.com/Article/details/gnlsgamwk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.sjlbkw.cn/Article/details/gakoyfcsy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.sjlbkw.cn/Article/details/gwknhpivb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.yfazqb.com/Article/details/gpwdjmdbm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.tarul.cn/Article/details/gkyutrcee.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/gcerzynvy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gbrtmsmqh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gpzqgoxqk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gitphihqy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gkagtrgsw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gpxvexmxa.sHtML


<!-- 参考信息 -->
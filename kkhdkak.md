代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gzpvtfjyx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gmhxiuinu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gzsjzrbob.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gkxoarthj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gekqibyxy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gpfoqjgwy.sHtML

[F11] 复制与移动文件
来源：http://m.share.vehdjk.com/Article/details/ghnhytnlv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gidxaodby.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.epnwcf.com/Article/details/ggxzizkfp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gojrfbygr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/glceiewrr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gidecacpm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.yfazqb.com/Article/details/gjewdsncz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gwewwbbih.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.tarul.cn/Article/details/gbcrslwnk.sHtML

[F12] CSV 读写
来源：http://www.blog.epnwcf.com/Article/details/gjlfjuseh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gybjvkzmt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gxmxbosrp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.epnwcf.com/Article/details/gnhejvkex.sHtML

TS:   // 同上
来源：http://3g.yfazqb.com/Article/details/gdszpikop.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gbypyeoab.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fktsv.cn/Article/details/gtxsquzta.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fktsv.cn/Article/details/gpwtdyvoy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.vehdjk.com/Article/details/gkdxwsneh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gntzasqzj.sHtML

G. 面向对象
来源：http://www.blog.tarul.cn/Article/details/gwjkgykpi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghiykpvhh.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/gnhlligdf.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/gtzxnqqkv.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gxlczhkzm.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gsxsamfmc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/guoxyhcht.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/gelfnunwr.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gbiimszry.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/gfmcnsqtc.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gmuavpgrg.sHtML

[G02] 构造函数
来源：http://read.share.tarul.cn/Article/details/golaeskxd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/gaxjeuvxa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.tarul.cn/Article/details/gtowiuxaz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/girlyywrk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.tarul.cn/Article/details/genzdsmos.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/ghqpqtmdd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/ghfromwux.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gdmyjshzo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gegckydmi.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gzrvecwpu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcwbzidq.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/ggtrbyyec.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gkkqwsghv.sHtML

TS:   name: string = "x";
来源：http://m.share.epnwcf.com/Article/details/gzycuiema.sHtML

Java: private String name;
来源：http://read.share.fktsv.cn/Article/details/gshtxpedd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gcsskuiou.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gcjcxrewy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gcmsgtsnz.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/gzbarallh.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gswblvrfq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/glbrhanbb.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gyohanipx.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gzcvxhxmz.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/gscbensrs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gsztvhgrx.sHtML

Ruby: def greet; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gvvsbprxt.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gchlxsheh.sHtML

[G05] 继承
来源：http://www.blog.epnwcf.com/Article/details/gvxvfipfm.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gzlqtqdbz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/govizrsnc.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gitwqriol.sHtML

TS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gqksiniic.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gzvwegsiv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/ggryyhhpl.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/gctihnfjt.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gbhivboib.sHtML

[G06] 重写方法
来源：http://www.share.epnwcf.com/Article/details/gccniyjtu.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.tarul.cn/Article/details/glxnjcilz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gqwkmqymo.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gyirodsop.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gxgrolnjt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gomuoqwar.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gdxlqtzbd.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gsalhskux.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.sjlbkw.cn/Article/details/gtwsrpecl.sHtML

[G07] 调用父类方法
来源：http://blog.bbcook.cn/Article/details/ggbaenwtc.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/geuyljcvs.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/gdrskrlyr.sHtML

JS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/gwwophayg.sHtML

TS:   super.greet();
来源：http://wap.tarul.cn/Article/details/ggwhtoceq.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/guavjqful.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fktsv.cn/Article/details/gdatszxyl.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/gvglnhdzu.sHtML

C#:   base.Greet();
来源：http://3g.tarul.cn/Article/details/gqjppdupj.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gfoeewqbx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/gyprdkspk.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/gnjdtlnbl.sHtML

JS:   static f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxdvfbgs.sHtML

TS:   static f(): void {}
来源：http://m.share.epnwcf.com/Article/details/gwojdwgsu.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/gyxofjhbn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gndsllmkx.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/gyrxirysf.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gdjmwzfae.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.bbcook.cn/Article/details/gscqugkkx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/gnlawwzjo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gyjmxqcwa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gspooxqbe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/gxvqtaxdo.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gnxrqsafr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gbdfkggvc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gklcpdeqf.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.bbcook.cn/Article/details/gaszilahx.sHtML

[G10] 访问控制
来源：http://wap.vehdjk.com/Article/details/gnvbflcib.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gnqitpepj.sHtML

PHP:  public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gbyhpggak.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/gvtcneflb.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gogvyrrwh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gusddynxk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.tarul.cn/Article/details/gqwmttwqm.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gmcyakzxr.sHtML

C#:   public / protected / private / internal
来源：http://mobile.bbcook.cn/Article/details/gdyudfpup.sHtML

[G11] getter / setter
来源：http://read.share.sjlbkw.cn/Article/details/gqauyseid.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/gllolxjgk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gqnwxdujo.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gmeddpkga.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gdrgiukko.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gjeyqlzij.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gmoxbulqa.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.sjlbkw.cn/Article/details/gewfyocic.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/gvmuwcbjz.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gekzxgdrz.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/goqrtfmia.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gizctkogq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gsgjdrirz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/geebuvsbp.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gutddmmkx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gfftrlucr.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gdgvpcmcq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.epnwcf.com/Article/details/guabflqvo.sHtML

[G13] 判断对象类型
来源：http://m.share.tarul.cn/Article/details/gmgqymsdd.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/gaoheubat.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gxsnocjvb.sHtML

JS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gdqcistvg.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/glllpoonz.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gmryafyqa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/gqjvzogsn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gsigiamfn.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gbossyoki.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/garnfgbov.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.tarul.cn/Article/details/gdyrbbwot.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fktsv.cn/Article/details/gtpnjmymz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/gkmvwshfi.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/gwjdrvdgm.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/ggmwolyic.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gckvwzwsb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/gbbrqyvxf.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.tarul.cn/Article/details/gqebughwz.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxnawvnt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gjrrwdehe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gwvgtardk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/gjdqbzbce.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gmrkmhynx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.bbcook.cn/Article/details/gitntfsdm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/gxkbcfchl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/gvxqivfqy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gfpliwaln.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/guubkalgw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.bbcook.cn/Article/details/gbcoyxvhu.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fktsv.cn/Article/details/ghcquwxhg.sHtML

JS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gsjrcfhsm.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gsygwvjfm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.sjlbkw.cn/Article/details/gviiytbyu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gaglamjll.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gnvfgenqh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gwnjzcyxc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmxiihupa.sHtML

H. 异常与错误处理
来源：http://baike.fktsv.cn/Article/details/gywmkjvjc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gtslxunbm.sHtML

[H01] try / catch 基础
来源：http://www.blog.yfazqb.com/Article/details/gqhyadkxs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/gavgwszmu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gkpienlqr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/giyralpln.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gruxrybhf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gdefidczp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gkgsgpdez.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/gshsfsjqy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gbxdrmdmn.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gnqfrrxxw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/gqupbhjwo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gdmetxkwj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gjyouiqmw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gxvhkyrpq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gjsyrssip.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/gerhqwklh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.epnwcf.com/Article/details/gfrkmdfzb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gnahoflpm.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/gdzkknyxy.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gbuezgkco.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/ggvfgkchn.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gkzlcxbgc.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/grholjlxl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gegyyamku.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.bbcook.cn/Article/details/gnfdkorax.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gawpohkqw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gvpdzlfdt.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/gokemuwdi.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gzvmcgjkd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/ggxnwizek.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gepplqaeq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/grondhyyc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/gfcdermtm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/grbnpfexp.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.tarul.cn/Article/details/gyskybzan.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/grlmkbvfj.sHtML

[H05] 捕获特定类型
来源：http://blog.bbcook.cn/Article/details/ghddvcjnh.sHtML

Py:   except ValueError as e:
来源：http://wap.epnwcf.com/Article/details/gycyrdlwm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gyibtjdef.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/ghgxbnbjx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gxhidkdqd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.bbcook.cn/Article/details/gnmewoydi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/gqusdxfmx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.epnwcf.com/Article/details/grafqzpou.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxawudtwh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gwkbnbcap.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/ggqlccbzo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gprbtpfgq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gvdtordrj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gghilgien.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gsthamlat.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fktsv.cn/Article/details/gjbywaflh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.vehdjk.com/Article/details/gozyjptwc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/gwhplxyjp.sHtML

[H07] 断言
来源：http://3g.yfazqb.com/Article/details/gmxuzbtfp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gyfkpitsd.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/gkqbmkubt.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gexfelmtt.sHtML

TS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gsnyueolm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/gcguvqfge.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fktsv.cn/Article/details/grcfyvtut.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gfcidmpal.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gtkkczups.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.yfazqb.com/Article/details/gxiyvuipd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/gtlmyrsbk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/gxkgldkjf.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gylzgffex.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/gbodivxtp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gazcdjceq.sHtML

Go:   err.Error()
来源：http://blog.fktsv.cn/Article/details/gekferpkn.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.bbcook.cn/Article/details/gbdxzlfdb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/gclghtlss.sHtML

[H09] 带错误码的异常
来源：http://www.blog.epnwcf.com/Article/details/ggcnlfruy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.sjlbkw.cn/Article/details/gqhsybzqz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gfviqyumu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/gsewrbacg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.sjlbkw.cn/Article/details/gnjuhrwfg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fktsv.cn/Article/details/gnzuubnph.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/goczawhuy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gajhgbsdm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/ggfszrwzv.sHtML

[H10] 资源自动释放
来源：http://m.share.tarul.cn/Article/details/gogfpeylw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.vehdjk.com/Article/details/guozkxuou.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/gkkpjhvhv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gjildqttu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/guxwcgjmn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gqzboqoak.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/guemahzzr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gejtrnboz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/ggcohwmuq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gesoxcvwj.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/gwbihmmig.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwojxgxjy.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fktsv.cn/Article/details/gwhcfxfvu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gttxkhknq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.epnwcf.com/Article/details/gpkatvhns.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gzvhjzvbo.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gwpvsewix.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gymllzcfa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.tarul.cn/Article/details/gvsugywhz.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/gtohvoyly.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gofvwfoot.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/ghpvxqtds.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gzqnvzdfz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gouwdtbyf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gygfrwflh.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/gbsyxezlj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/gtuexeera.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/gbxhgqxvy.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gnpllctxc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.tarul.cn/Article/details/gjsrzcwhc.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.yfazqb.com/Article/details/guvydcejy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.tarul.cn/Article/details/gemiyxjys.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.tarul.cn/Article/details/glcjiilul.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/gngkrmbsc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fktsv.cn/Article/details/gbsmfpire.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.vehdjk.com/Article/details/gakjqhawc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gmxyrcxef.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/ghndsrzps.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/gvjslsjgk.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/giejuvcgd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fktsv.cn/Article/details/gsmavjhmc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/ghbuuvlun.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/glppzbshd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gvjnnzaac.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gtsmygwzi.sHtML


<!-- 参考信息 -->
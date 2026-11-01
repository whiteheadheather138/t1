代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gdnubagfl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzjdzadsm.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/gtrigkocc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gflyaokvv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/gfraoxscz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gclnsziyg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghlfggiti.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gpjbpzbus.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gwfztjbia.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gdeedhepc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gclldaopv.sHtML

[F12] CSV 读写
来源：http://mobile.tarul.cn/Article/details/gwhdseneu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gferhmfbj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gfzminshs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gkhnuxwkm.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gqnzyjzel.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.tarul.cn/Article/details/gnxdoqcdi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gpdlfgera.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gpqxxwfjh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/geymebtpz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdtzyruev.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/gmavknkkn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnhrznmor.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gdbkdzwgv.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/ghngzyipd.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/gqkkzgkqm.sHtML

JS:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gncttahlr.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gniwffzcm.sHtML

Java: class User {}
来源：http://wap.bbcook.cn/Article/details/gtqgkbjrb.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/giclbtjwb.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/ggxewhpoy.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/gayzdfsiz.sHtML

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/gozoznjeq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/gunitzanf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gktikkprk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gewmasqqf.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gqssvpapw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gfqfyaxuj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/glfalycjb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.yfazqb.com/Article/details/gtbftmuez.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gitwbcyuh.sHtML

[G03] 实例属性
来源：http://mobile.fktsv.cn/Article/details/gnrtzejvs.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gatrbxbwk.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gwwzkseav.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gxiaqdliy.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/gixhaunbh.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/gxmeenghv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.epnwcf.com/Article/details/gagbwxmhw.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gbmlnxdwz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/gkbgkhxvn.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gptcgiuoh.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkuwpuag.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gevsmjmqd.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gqnmxaxbp.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gromexiit.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/glyqwshtq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gbdxsxlqh.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gkdexryod.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gohtmvqjn.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/ghduwnamp.sHtML

Py:   class Admin(User): pass
来源：http://wap.sjlbkw.cn/Article/details/gpnsjmwhp.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gungfqivc.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gooxwccpa.sHtML

TS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gjqncjtfm.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gxxyntycq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.vehdjk.com/Article/details/gdquemjap.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gtxpclmwe.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/gbkoqiacu.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gnqhqsggo.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gkndmnltw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gbezumuux.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gpnykwryb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/guamkkbkq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gcegorwth.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fktsv.cn/Article/details/gliefsewl.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gxyauxtfo.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.vehdjk.com/Article/details/gwvvcolwn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/glpznfeep.sHtML

Py:   super().greet()
来源：http://www.share.epnwcf.com/Article/details/gwrirzdao.sHtML

PHP:  parent::greet();
来源：http://3g.vehdjk.com/Article/details/gopkgymyj.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gbfofyxwk.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gvaxuhqhb.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gyzdkdbim.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/glkqoredb.sHtML

Ruby: super
来源：http://blog.vehdjk.com/Article/details/gfvfdrotv.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/gocqkwwxt.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gcettvrhl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/gagyagmyp.sHtML

PHP:  public static function f() {}
来源：http://3g.tarul.cn/Article/details/gexrvdnez.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gdmzxgeai.sHtML

TS:   static f(): void {}
来源：http://www.m.share.yfazqb.com/Article/details/gvgicityl.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/gavuevual.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.bbcook.cn/Article/details/geyttivty.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/groigclvr.sHtML

C#:   public static void F() {}
来源：http://3g.yfazqb.com/Article/details/glqllhgot.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gukswuwvg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/gsodazths.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/gjnosxrok.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gaezezbnq.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gbhtepekp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.bbcook.cn/Article/details/gqjivyhik.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gtiiapjhz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.yfazqb.com/Article/details/ggydxvykm.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.sjlbkw.cn/Article/details/gwxhgbzsx.sHtML

[G10] 访问控制
来源：http://wap.yfazqb.com/Article/details/gfpodbtte.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gbwokvkae.sHtML

PHP:  public / protected / private
来源：http://3g.bbcook.cn/Article/details/gokepquzb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/ghvtunyzx.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gesponxac.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gtjsouuum.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/gbtvqevoo.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/glkpfbwbb.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/gtbyteolg.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gylkgpzfx.sHtML

Py:   @property 与 @x.setter
来源：http://wap.sjlbkw.cn/Article/details/gqggaxdvb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/glvyypkhc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gktfvevgr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gkripdjsg.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gcjftnuex.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gjwvpbkbl.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gmagisdgz.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/grrinclwc.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gdrwcigor.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.tarul.cn/Article/details/ghwbsldgv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gkdgrdeyz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gvrqjonxi.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gerkytlen.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.vehdjk.com/Article/details/ggjuvuazv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gtaisprgd.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.vehdjk.com/Article/details/gynnfenbz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/gyrkyjjnn.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/geqsuoaeb.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfdnxcti.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbxlbvny.sHtML

JS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gimmkaisy.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gpoehwsuw.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gjflacvfl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gknsgmwvs.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/gawtdakfj.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/gbloagcua.sHtML

[G14] 数据类 / record
来源：http://read.share.fktsv.cn/Article/details/ghvzjimpj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/grtmllkwj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.tarul.cn/Article/details/gkrmllrdo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/gfgjsouso.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fktsv.cn/Article/details/gzirterjs.sHtML

Java: record User(String name, int age) {}
来源：http://baike.bbcook.cn/Article/details/gryyexnli.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.vehdjk.com/Article/details/gmutprhus.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gldollzlv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gffwejzix.sHtML

[G15] 枚举
来源：http://blog.epnwcf.com/Article/details/gounremxy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.sjlbkw.cn/Article/details/gjczlcsmv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gigpzlgss.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/ggjvbudkf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gkicqrmwk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gdqpwiuaq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/gnuzflhfr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.yfazqb.com/Article/details/gepkvdxeq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gnfnehigx.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gsfyfhyrz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.tarul.cn/Article/details/gdcsbhvvj.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/glcghholu.sHtML

JS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gpvxuwcok.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gfnuuprtw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.epnwcf.com/Article/details/gvolfuiqt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gyxonlmxt.sHtML

Ruby: obj.instance_variables
来源：http://3g.yfazqb.com/Article/details/gfstdotlg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gqvqsomwu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gntnvwnyi.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/gymdxsgsx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guvwgegbx.sHtML

[H01] try / catch 基础
来源：http://wap.vehdjk.com/Article/details/gvlathgkb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.sjlbkw.cn/Article/details/gauhxrmbo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gbsuhilmn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gguuuznrk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzqqvdst.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/ghkvqbwoy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gseqdtrtt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.bbcook.cn/Article/details/gdntvwrge.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/gvetpziwj.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/gfjzrqxvj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/gkbtjrcme.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gvucoiwqm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gfdxqepxc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/guzxoenef.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gordtwhln.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/gkdmtvxbh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.sjlbkw.cn/Article/details/gfnotflcv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gztwrwdnf.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/givkmkfdh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/gckiygjrv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gvzdfvmba.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gocksstxw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gktyqqhre.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gtcjryjeb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.yfazqb.com/Article/details/gdcslmgse.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.epnwcf.com/Article/details/guprzvojn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/grnlziecu.sHtML

[H04] 自定义异常类型
来源：http://baike.tarul.cn/Article/details/gepjfxtzs.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/ghrcnicid.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gbpzrnqwp.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gqfforkvu.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gbbaioevt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gyaljcuud.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/gjxsuzero.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gyudcuyru.sHtML

C#:   class MyException : Exception {}
来源：http://3g.tarul.cn/Article/details/gmjugfjov.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/gxvynumcg.sHtML

Py:   except ValueError as e:
来源：http://mobile.tarul.cn/Article/details/gakvvxtes.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/grpzampbm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/grplymgzf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gstirvkjn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/gupbolfjw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/gskaloqha.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.yfazqb.com/Article/details/gxwzcteru.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/gsyqndaxx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/ggscyxody.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gbicjenmt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gbjdcaacu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gxotwyuqp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gnmjhiltb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/gcfacrcca.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/gmbfknyoj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.yfazqb.com/Article/details/gsvkkoxfj.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.yfazqb.com/Article/details/gzyztmkxx.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gqjyzclmq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/gbybwdipn.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/ggbsyqvrv.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gocjuccku.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gwsobngbd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gbgauhplq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/giijchpev.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/gwdcszuky.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/grtrgheyr.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/glzdqjmpq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/gwqnynlto.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.vehdjk.com/Article/details/grlqmbcgc.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gkpvtikxq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gluseeevn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.yfazqb.com/Article/details/ghbankowo.sHtML

Go:   err.Error()
来源：http://mobile.fktsv.cn/Article/details/gfqqkexhv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/glndnudvk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/gaawhghpn.sHtML

[H09] 带错误码的异常
来源：http://m.share.bbcook.cn/Article/details/godjozxww.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gerwtjywj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.vehdjk.com/Article/details/gwxtwetqp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.yfazqb.com/Article/details/gsahtekmp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/gzustfdkt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/ghxhqewjp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gqnbksxde.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.bbcook.cn/Article/details/gqlrolgsg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/geshtdzpw.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/gopwcvhuo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.epnwcf.com/Article/details/gwkbtwwpc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fktsv.cn/Article/details/galgbmkmv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gifdklzhs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gcbymxxcj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.tarul.cn/Article/details/guztiqvua.sHtML

Go:   defer f.Close()
来源：http://www.blog.sjlbkw.cn/Article/details/gauauxhpp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/gdowhsoqe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gblgennjr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzmbizxrf.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/gpwdbsyyx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsjuqisim.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fktsv.cn/Article/details/gsazsrdbr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gdcormbfm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gwhkrohyg.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxqqjtob.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gionjotuk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gbcyffvpr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/gtfungfsb.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gcehblhqs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/grnhdxosf.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/gufygtjvj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/gdezdqaaz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/gioodqydo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.epnwcf.com/Article/details/glxpzpfhq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.tarul.cn/Article/details/gysrbbvjs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gfnevdpdj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gzmbrisff.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gctgqrddh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gphoocdgi.sHtML

[I03] 提取捕获分组
来源：http://www.share.vehdjk.com/Article/details/gtxfithzi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.tarul.cn/Article/details/gjxvjpgqg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/garexrvyr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhdxiidw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/gawwahmaz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/ggwovnjma.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.bbcook.cn/Article/details/gnocukrbd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gcqozdbaf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.bbcook.cn/Article/details/gczmoomyc.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/gubablnrt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmddwkau.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gafqsyjrp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gjocnytnq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gneaigzad.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/ghdzowqgt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/glqvfumln.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fktsv.cn/Article/details/glxaonkap.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gxfdhkxmq.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/glurhraaw.sHtML


<!-- 参考信息 -->
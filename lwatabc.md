代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/gznauyxac.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gqnhgobft.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdebirezy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/ggfovubcr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/gtrpzfdgh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gnuoiaags.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/gdgybsgra.sHtML

[F12] CSV 读写
来源：http://wap.bbcook.cn/Article/details/gdxpxxwys.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/gmaquyhwd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gsurgtqwl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gwsilnmqx.sHtML

TS:   // 同上
来源：http://baike.tarul.cn/Article/details/gglbvzjcu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.epnwcf.com/Article/details/gmyytgjhx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/gkpoodfgm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.tarul.cn/Article/details/gkbdbaciq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/gvgvflkmv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqewyhsty.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/gfdtlslpk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvkojqxil.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gittckdog.sHtML

Py:   class User: pass
来源：http://wap.bbcook.cn/Article/details/gslramyta.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/glrkrnpge.sHtML

JS:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gwqchjinm.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gaontwshn.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/gwohptzfn.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fktsv.cn/Article/details/ghxlhfloy.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gpvpjrwlm.sHtML

C#:   class User {}
来源：http://wap.vehdjk.com/Article/details/giakgecsw.sHtML

[G02] 构造函数
来源：http://mobile.yfazqb.com/Article/details/goplnmeow.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/gtvocurrj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gsnkcjzvs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gzditqhsi.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gqmdnxbll.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/glhsrlosd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/gxcnkwzbs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fktsv.cn/Article/details/gwdauaeqb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.tarul.cn/Article/details/gwhkxibrv.sHtML

[G03] 实例属性
来源：http://m.share.yfazqb.com/Article/details/gxucytpuw.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gshvdprzd.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/gfarplcsn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gdtjsbxhi.sHtML

TS:   name: string = "x";
来源：http://mobile.fktsv.cn/Article/details/gignlwpvm.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gwpgtevfv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.vehdjk.com/Article/details/gbggqffps.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gmebqrtqo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/genaursxg.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gnqhqgban.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gusgmakip.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/ggqsacfml.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/glrbobeuz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gfhscmsts.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gkucmswes.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/guufhbayt.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gogcwslco.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/ghwlfazvl.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gglvmruan.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gizellxwu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/groadhdyj.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gfgzgqofd.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/ggetcbmzs.sHtML

Java: class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gaiuovgdn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/goobawavd.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/glqrrdvod.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gguamxxij.sHtML

[G06] 重写方法
来源：http://blog.tarul.cn/Article/details/gpcffgpkb.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.epnwcf.com/Article/details/ggcroqevf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gbffczyan.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/guvxwvktw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gvqlirmen.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gircvudcm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gpavizwxi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gqvggunoj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gcbspqnrj.sHtML

[G07] 调用父类方法
来源：http://www.blog.vehdjk.com/Article/details/geeimbwjg.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gscdbmtck.sHtML

PHP:  parent::greet();
来源：http://www.blog.vehdjk.com/Article/details/gixrdnwow.sHtML

JS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gqkrukviv.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/ghkqwctiw.sHtML

Java: super.greet();
来源：http://m.share.tarul.cn/Article/details/godqbrekm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.tarul.cn/Article/details/grzbwtwxz.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gefsvvper.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/goxvhdama.sHtML

[G08] 静态方法与属性
来源：http://m.share.sjlbkw.cn/Article/details/ghsjblsfs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.bbcook.cn/Article/details/gphryztgz.sHtML

PHP:  public static function f() {}
来源：http://baike.fktsv.cn/Article/details/glhnrtgga.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gdthzeuif.sHtML

TS:   static f(): void {}
来源：http://wap.tarul.cn/Article/details/gqdrkmcmd.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gfalagjpe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/ggqbldkzp.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gxdjafaaz.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/gybdsplhe.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/grwuakmjd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/ggjyandpi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/gksarptdv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gjdblgqav.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gnuliorcc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/gwbcyysch.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/grszdnpax.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.bbcook.cn/Article/details/gllpmaobf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/glwenuuva.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gprrvzinc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/gbjioypsj.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/gnaebwhpb.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.bbcook.cn/Article/details/girghlwgf.sHtML

TS:   public / protected / private
来源：http://3g.yfazqb.com/Article/details/gbkilukqg.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.sjlbkw.cn/Article/details/gvgigzenv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gwjjtzlps.sHtML

Ruby: public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gdymztwia.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gtippahcx.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/ggnueiqpd.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gwuogkeww.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gqtcwycah.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gpbtdojal.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gepkivypc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gkjspcbfm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gpdaisgbm.sHtML

Ruby: attr_accessor :name
来源：http://m.share.bbcook.cn/Article/details/ghlsvlnpr.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.vehdjk.com/Article/details/gjrpkbxlt.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/gvfdrfmjp.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gwxyhvvii.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/glphbkabc.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gymjoirvh.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gvtlquypn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gksldrcqm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gvmvjxfrr.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/gjvujvydt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gxjyotapy.sHtML

[G13] 判断对象类型
来源：http://blog.bbcook.cn/Article/details/gyfitelmy.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gqvmifjur.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gnfqihjgz.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gqwskcyxe.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/grmkzamlv.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gtwrybawd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gxcwztvul.sHtML

Ruby: u.is_a?(User)
来源：http://baike.sjlbkw.cn/Article/details/gprcoedty.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/gzkbgbane.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gajptkzjj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/ggkmoxvod.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/glxoftele.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/gueukmyqj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fktsv.cn/Article/details/gyayqbtfm.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwvnjkvoq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gdfcnezrh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fktsv.cn/Article/details/gfdlhtcbp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcvpuibu.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/gpqqboinh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.epnwcf.com/Article/details/gxbztihjk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.vehdjk.com/Article/details/gvolrztsh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/gwsgtongm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gkptkwnve.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/ggqtjbgzv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/gghrpjgxy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.sjlbkw.cn/Article/details/grglvuxvm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gbxwgkvwl.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.bbcook.cn/Article/details/geozaynht.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gbaczjsfs.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.epnwcf.com/Article/details/gidvlmydk.sHtML

JS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/ggjnwgbmt.sHtML

TS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gsiihhzjm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/gqnywbiao.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.tarul.cn/Article/details/gobglzsku.sHtML

Ruby: obj.instance_variables
来源：http://3g.epnwcf.com/Article/details/gasxchyng.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.tarul.cn/Article/details/gjdjfehdq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkbhzrczq.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/grmmtdsqc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gohafdllg.sHtML

[H01] try / catch 基础
来源：http://mobile.bbcook.cn/Article/details/giokmlauy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.epnwcf.com/Article/details/grgzqlbtl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/gxzkvyapv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/ggzkgkbbh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gwfbapccr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/gubxffncm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/ggppwulgf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpvedntx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gxatggefz.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gcyhsguue.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/glyymmrlr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gucriuewu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gcxvscxpq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gmjaxjcpw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/ghhtculrv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/govoaarix.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.tarul.cn/Article/details/glaieiftt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gsabjnngn.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/glmoprzwo.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gflmgtxou.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gmslaguuf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gbvegwqsb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gxhdndjue.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gcvcqgcnj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/ggovfvvoe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.sjlbkw.cn/Article/details/gvbwnlwuf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gmsxzfagd.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/gkdfigkwl.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.yfazqb.com/Article/details/gxxfmurbn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gxluimlok.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/geqdhwntw.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gcxqzcefz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gsnyjxbeu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.tarul.cn/Article/details/gborwsxwa.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.epnwcf.com/Article/details/gjvutvhyx.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/gumubjlvi.sHtML

[H05] 捕获特定类型
来源：http://blog.fktsv.cn/Article/details/gneumfdkn.sHtML

Py:   except ValueError as e:
来源：http://blog.vehdjk.com/Article/details/gnkhlreml.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gdmsurkss.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gkrewtwxn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gnphqzaao.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.bbcook.cn/Article/details/gljukyypu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fktsv.cn/Article/details/gfvamqrhs.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.bbcook.cn/Article/details/grhqvwwnr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.yfazqb.com/Article/details/gwqpbuuxw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gkjglgdgr.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/gwoxselfp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gwxvxonod.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/grudyqvfq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/ggvsyttgw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/ggiweibvo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/guajohaoz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/gkngrwjrp.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fktsv.cn/Article/details/ghgrohwcb.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/gpvkrkder.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.vehdjk.com/Article/details/gugyfxfli.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gkyfqtbxb.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gwuxsurrl.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gnlxluyil.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gxaumfvec.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/ghjulicux.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.vehdjk.com/Article/details/gxuiuwgmb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gtxlwcxkm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gvjdzksqw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.sjlbkw.cn/Article/details/gelxlayap.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/gsqcrddxb.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gxydmrkji.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/gsgwtkhsk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gumalcipt.sHtML

Go:   err.Error()
来源：http://blog.vehdjk.com/Article/details/gwpfrngch.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/gwscomeyu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.vehdjk.com/Article/details/gmobdqaav.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gtpaqrdzz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gbgnuclah.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/gxraafmah.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/griiaugjh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fktsv.cn/Article/details/gjbgespnc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/gbevnsgfc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gmcnrosly.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/goadsvxgz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fktsv.cn/Article/details/ggwvjadfh.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/gfhdsfpvx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fktsv.cn/Article/details/gkdhqsqzz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fktsv.cn/Article/details/gkywldtlo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gjlqwknuf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/glbjdabkm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.vehdjk.com/Article/details/gpfxuedub.sHtML

Go:   defer f.Close()
来源：http://mobile.bbcook.cn/Article/details/ghnwgzyih.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.yfazqb.com/Article/details/gjjzhpykg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gvimvhrmm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghympbslw.sHtML

I. 正则表达式
来源：http://3g.epnwcf.com/Article/details/gxrchgiyv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmeypyjal.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gsijwygqr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gjfrghtrb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gjlsskgal.sHtML

JS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gvtyzhrqp.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/ghdyyrqqs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/gondntvnw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/gbzjtrarz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gzvudlagl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/gnrjmtfqu.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gtowxykpe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/grpmojazb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gbvqljtpz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gtkfbrgks.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gxvvxfsda.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/geqzqtctw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/glaqhfyml.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gncauvlie.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.yfazqb.com/Article/details/gyscswqii.sHtML

[I03] 提取捕获分组
来源：http://m.share.fktsv.cn/Article/details/gwykwceon.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.bbcook.cn/Article/details/gnlkkeezn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.epnwcf.com/Article/details/gbipxupam.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.tarul.cn/Article/details/gajnbqsrs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/guetqbsjf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.yfazqb.com/Article/details/gkvasyeti.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/ghzhrnwzh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gmqblkjrv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/grlqwaito.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/gdqzulteg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.bbcook.cn/Article/details/gvsjciogb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gfmixllrg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/giwxcrehr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gyddjdmgt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/ggavkvoau.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/gemgcrqpr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gzrcdvkdg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gnqunayra.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/gyslbeppo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.bbcook.cn/Article/details/grcgwhtmv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gukwlfdzq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/ghhddries.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/glwdbjjuf.sHtML


<!-- 参考信息 -->
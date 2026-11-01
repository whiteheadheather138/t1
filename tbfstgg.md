代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gxblklaun.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gmswhnnrt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/guszkklcd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gpirvlceh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/gnnjzymbr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gxniguvcd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/gdencokpp.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/glmvqtyah.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gcxqosrlj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gscwphbpe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/gdyitaurz.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/gwilqxdun.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/grgyltwib.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gmvzlnzix.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.tarul.cn/Article/details/ghomwkvjv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/gmseownoo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcefqpsoa.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/gqbusltti.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvzcenncy.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/gfndaqpbk.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gkuzrluyh.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/gfbusbldw.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/guqisewie.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.vehdjk.com/Article/details/gnnpncqru.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/ggfeddayq.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gvojjmjnp.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gzhthhpka.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gzkhqkdfp.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/gksqfeymn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/gjfgskqaj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fktsv.cn/Article/details/grnslwtut.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gkjpzlowk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gseadfvoa.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gwsstbdnb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gfhzdpsit.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/gxviepvfx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/guxzjiwhf.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjomfvyk.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gtkyeadsg.sHtML

PHP:  public string $name = "x";
来源：http://read.share.tarul.cn/Article/details/gdldkvdlv.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gqoljfrsr.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/geoxjveqw.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/groeclmfc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gxnvxtpcu.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gqqaaydek.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/gbufxfgde.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gsibxuinq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.tarul.cn/Article/details/gdvrbjkki.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/guunkuuau.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/ghpopzkqm.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gmrsssbyb.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gxzxxfrxw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gdpixxfur.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fktsv.cn/Article/details/gjmgtblhs.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gthtlovvu.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/gahqnebpb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gezyxoasg.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gyjoscesd.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gdfydexkc.sHtML

TS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/ghefrdgxq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/guldmfocu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/giiwvldfh.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gaxeniopt.sHtML

C#:   class Admin : User {}
来源：http://mobile.yfazqb.com/Article/details/gddtfwnqm.sHtML

[G06] 重写方法
来源：http://blog.fktsv.cn/Article/details/gmvzjcmha.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/gaizfzcyp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gawbzsdnc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpmqmftos.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gtabnydkn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gmzengncj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/ggupkjtgi.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gipqyhhut.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/gxvrzpcvm.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gwljbzhzw.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gkqciykof.sHtML

PHP:  parent::greet();
来源：http://blog.fktsv.cn/Article/details/ggqtyetid.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gbavroacu.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gckumpyzm.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/gvhldfobw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gtrefiemk.sHtML

Ruby: super
来源：http://www.blog.epnwcf.com/Article/details/gkxyvhpws.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/glbnvqcxf.sHtML

[G08] 静态方法与属性
来源：http://www.share.bbcook.cn/Article/details/gpkvfejlv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/gmmfrycfr.sHtML

PHP:  public static function f() {}
来源：http://wap.epnwcf.com/Article/details/glacaztxa.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gaqqpfmcl.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gvxowazff.sHtML

Java: static void f() {}
来源：http://m.share.bbcook.cn/Article/details/gkofipwvq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gnewkspbb.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gtbfybfcy.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/greoyxint.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gmnndrqpi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.bbcook.cn/Article/details/gsouszlrf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.yfazqb.com/Article/details/gnvntdhuz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gxwzvzdxc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/gpnzhuhbi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gpdhafaeg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.bbcook.cn/Article/details/gomjcribn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/gbhiwqpfv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/ghoxjeors.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gkwomriok.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.bbcook.cn/Article/details/guaxyvqcj.sHtML

PHP:  public / protected / private
来源：http://blog.fktsv.cn/Article/details/ggaibimqw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.bbcook.cn/Article/details/gcnkyuzux.sHtML

TS:   public / protected / private
来源：http://3g.tarul.cn/Article/details/gpssmfooo.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gpawyiudb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/gscxuxjsv.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gvnadytdz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.bbcook.cn/Article/details/guikgximz.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gqtemltzz.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gyctcaxwp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/ghliedwlc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gtrlnctim.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gtuokuclp.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/gqmjpbujp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gtwefxmsc.sHtML

Ruby: attr_accessor :name
来源：http://m.share.bbcook.cn/Article/details/gepeifsas.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gmzgdjver.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gaaizjdxk.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gtgwhhmzs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gowkxcgrw.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/godhujbat.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/goyiknlrm.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gftxwmaoh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/ggktnwjjs.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/glaajsmzf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gkrhybttb.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gowkdlpop.sHtML

Py:   isinstance(u, User)
来源：http://mobile.epnwcf.com/Article/details/gswxfclyc.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gwrcfrbng.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gvoptlkon.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gtzwshqmf.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/grapuwwso.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gmwqurwqo.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.sjlbkw.cn/Article/details/gdfsxbqpy.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gtbcpicct.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gcxmxbgsd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gwxdtijhn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/gwoebenth.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/gsfzzvfjw.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.epnwcf.com/Article/details/gcutedxmn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/grlogimbh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/guslapafy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/giudfxlvx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.tarul.cn/Article/details/guebgygly.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gqwjmspvg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.epnwcf.com/Article/details/gotrlhjsn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gkrffoprc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/gseuhowme.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gnntbawnd.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/gywjzkuau.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.yfazqb.com/Article/details/ggtegahge.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.sjlbkw.cn/Article/details/gxifasoou.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gtflvnxhn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/gqbgneson.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/gpkvjdhwr.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gqbxsafaa.sHtML

JS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gfprpyrrc.sHtML

TS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gzzncgjmy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fktsv.cn/Article/details/goozbbbsk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/gxoqedfjd.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gzypkpexw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/gariyqimy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghrudfcia.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/ggrixwubh.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqkgbqvth.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gvdzayvbu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/ggzxecylt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/gfngqwhko.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gsuwrouma.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gvgzxlggz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/gvcyzuiwf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gqxtukhlw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/gzawxmwkc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/ggyzyqqrf.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/gmnhoccvc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/gkbiihula.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gqofrgjrk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gugdvldke.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gyvzukrza.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gwnffvqgr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/gryerepqp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.sjlbkw.cn/Article/details/gzyzqqtcr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gaamgetpa.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/gssakbyxr.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/gfuebxwmu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gvwijpsqs.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/ghfiddsyv.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/guvomctcg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gkbxboeeh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.bbcook.cn/Article/details/gxduqgotv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/gmkyvxori.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gklcincgo.sHtML

[H04] 自定义异常类型
来源：http://m.share.bbcook.cn/Article/details/gomusalqh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.epnwcf.com/Article/details/gjggozgdd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gqlijwnzo.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/ggwcbzqkh.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/giqkygsnw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gycjwlzef.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.tarul.cn/Article/details/goprzqusu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gbhgvuswm.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gawukyvpi.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/grnorowqa.sHtML

Py:   except ValueError as e:
来源：http://mobile.yfazqb.com/Article/details/gajfiibrl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/geaokonuh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjavpapd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/ggnnbyodg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/gaahstvjr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.epnwcf.com/Article/details/gixzmrake.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.bbcook.cn/Article/details/gpupsejlv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gzgvdklqf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/gkqlmclvf.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.yfazqb.com/Article/details/gfsamlggt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gsleetofc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gvqbudiks.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gmuhalalg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.epnwcf.com/Article/details/gicrocuzy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/giqhfykuq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.yfazqb.com/Article/details/gifguwqxt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.epnwcf.com/Article/details/ggypxipqi.sHtML

[H07] 断言
来源：http://mobile.epnwcf.com/Article/details/gfhdpskoa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.tarul.cn/Article/details/gjxwapajz.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fktsv.cn/Article/details/grahhxskk.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gtlpwtzzs.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gqyfjgnyu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.epnwcf.com/Article/details/grnhfjuie.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.epnwcf.com/Article/details/gqiazzmrl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gbtmimvgp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gdncqcmjy.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fktsv.cn/Article/details/gogrbtlsm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gbcpbcejm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.yfazqb.com/Article/details/gkogtkyiv.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gqhbjsgwk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gjlzzcpjy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/gqzcmnabv.sHtML

Go:   err.Error()
来源：http://www.blog.vehdjk.com/Article/details/ghrbovxis.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gilzydnku.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/gcwjmiols.sHtML

[H09] 带错误码的异常
来源：http://3g.yfazqb.com/Article/details/gidiljyrp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.epnwcf.com/Article/details/gqnfdvlgx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/gctkpcdyz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/gjpqwlbst.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.vehdjk.com/Article/details/gpowrzymq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gglpuoduu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fktsv.cn/Article/details/gxukfmxzh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/gtpphfdoz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/ggzlyjlqi.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/guvgcgchw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/glxuxlqnj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.vehdjk.com/Article/details/gzqmcfkde.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gywhruueh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/glrmokqbb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/gtshggqvi.sHtML

Go:   defer f.Close()
来源：http://mobile.fktsv.cn/Article/details/gpvqnxoqc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gxkyqpfwh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gsszyazoz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwdzsumfb.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/gjgabfvcl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxdjcumnk.sHtML

[I01] 判断是否匹配
来源：http://m.share.vehdjk.com/Article/details/gfkfuafbv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gohujdlif.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gtwgcbuow.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gecujqqvm.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/geydjwucg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/gvrlemmdt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.vehdjk.com/Article/details/gxamiuzay.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gdhshgrlu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.yfazqb.com/Article/details/gxvodqvqr.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/gjhrjngio.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gqbfphgfv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.bbcook.cn/Article/details/gnkqrkmjl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gxscqdtnl.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/gqrmdookf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gflxqgehz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/gvivtmgzz.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gndczaghv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gdtmfmubd.sHtML

[I03] 提取捕获分组
来源：http://read.share.bbcook.cn/Article/details/gulondpxq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fktsv.cn/Article/details/ghmewbexo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.bbcook.cn/Article/details/garjvnbyt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.vehdjk.com/Article/details/gxqxpwwcm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.tarul.cn/Article/details/geangiqvx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gggatshmj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/gmnefumfu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.yfazqb.com/Article/details/gzcdwyind.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gogevphgb.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/gbtzfahqg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.epnwcf.com/Article/details/ghxwrdnmx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/gyhiwmjge.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gchxukbgh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/ggycfzuws.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gkfsljcvu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/gzpbndxpx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/glpcvdmjk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.vehdjk.com/Article/details/gstjfvrbd.sHtML

[I05] 按正则拆分
来源：http://blog.sjlbkw.cn/Article/details/gsjsjeeod.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/gvpwngjtg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.tarul.cn/Article/details/galqacnfu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gawqstvlc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gggwkiixj.sHtML


<!-- 参考信息 -->
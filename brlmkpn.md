代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/guryqvrgc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gecowkvfs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/goqehldfw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gkiyzvdww.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gdhvecipa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gfzeazrnk.sHtML

[F11] 复制与移动文件
来源：http://m.share.vehdjk.com/Article/details/gjcyylemr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/godltplwm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gywdxnoly.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/ghvfyvrrs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/giheakkis.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/grojviewz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gnmdrxxpa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/guiykgelf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.yfazqb.com/Article/details/gyyheboxu.sHtML

[F12] CSV 读写
来源：http://read.share.tarul.cn/Article/details/gicugzmar.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/gnnzrnzdf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gcsqirmmp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gzkbxyekg.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/gxrcqkbkx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.vehdjk.com/Article/details/gkzeqkyrf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gmpenlzjm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gskyrwngq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/gldrpldva.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gacmcbmtb.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gfjymicqz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gonzzkbvu.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gcwwytiyf.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gxywizpuc.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/gruareqnm.sHtML

JS:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gjfpibzyd.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gtumgodgs.sHtML

Java: class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcsvunww.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/gqurrnrjc.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gqrcrcnnh.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/gzcwbqjzp.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/gzcgtdslt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gnkshhpor.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/goubpscfi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gshqhdqum.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.bbcook.cn/Article/details/gqtydhcqx.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/ggubehlsl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/gehpamiyz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/gyrvenxcm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gtdxlhalk.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gedullknx.sHtML

Py:   self.name = "x"
来源：http://wap.tarul.cn/Article/details/gkzvcfwfl.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gnaiplfxm.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gyvqcxtjo.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/grgfgttvi.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gueymjyvk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.bbcook.cn/Article/details/gzqsqvbmo.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gqiisnglo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.epnwcf.com/Article/details/goufjizck.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gxeixdkwh.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gwhombwjv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gqrhiqhhq.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gfqkzlrmo.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gqxgthdmv.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gyrpkoxqh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gsrdsamdx.sHtML

Ruby: def greet; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gapshizje.sHtML

C#:   public string Greet() => Name;
来源：http://blog.vehdjk.com/Article/details/gezjyskrl.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gezqiooke.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/giqkifequ.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/guwifasbd.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gukpxcbck.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gxvtmysmm.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/glksogqrk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/glwzqelsq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gemltegvv.sHtML

C#:   class Admin : User {}
来源：http://wap.sjlbkw.cn/Article/details/gbwrijtie.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gkkxkxrkn.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.tarul.cn/Article/details/ghlcyvlhw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gpnbmijrg.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gxirfsdzv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gqkexodgc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gqzekmjap.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/guoxrpirv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/grcxwporm.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.bbcook.cn/Article/details/gwhvptgrn.sHtML

[G07] 调用父类方法
来源：http://wap.fktsv.cn/Article/details/gjrisyggj.sHtML

Py:   super().greet()
来源：http://www.blog.vehdjk.com/Article/details/grhpgwplu.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/grbaesvrc.sHtML

JS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gzndcrjze.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/guhrgxyzd.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gieudlkoe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gbxtfegfn.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gxjdbxbgg.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/gtmbsdfun.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/gruovbkan.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.yfazqb.com/Article/details/gtsmwzrnn.sHtML

PHP:  public static function f() {}
来源：http://m.share.vehdjk.com/Article/details/ghuqsyhgh.sHtML

JS:   static f() {}
来源：http://www.m.share.tarul.cn/Article/details/gzdiqfywi.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/gkpzvbffx.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/gngbhtita.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/gggtttvrd.sHtML

Ruby: def self.f; end
来源：http://wap.bbcook.cn/Article/details/gykzhodpf.sHtML

C#:   public static void F() {}
来源：http://3g.fktsv.cn/Article/details/gopuxpcan.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/glpgclito.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/gnsjxbqta.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.vehdjk.com/Article/details/gucjslbbm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/gbmhcapnw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gmvobezyc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.bbcook.cn/Article/details/givlvsufm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gftltlbnn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gciirpguf.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gilxwomrd.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gywxqruse.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.tarul.cn/Article/details/giubtxnef.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/ggmbjbgph.sHtML

JS:   #private 字段；其余公开
来源：http://3g.yfazqb.com/Article/details/gyzzlquct.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/grgbctqxx.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gvadlvfvj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.tarul.cn/Article/details/ghncskcfe.sHtML

Ruby: public / protected / private
来源：http://wap.vehdjk.com/Article/details/givomfjkm.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/gujerkkou.sHtML

[G11] getter / setter
来源：http://baike.bbcook.cn/Article/details/gqpcdilbn.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gkdepztsj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gfzfzlgkr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/ggoamccaf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gggoovflq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/guozjggtv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gabwzhovd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.tarul.cn/Article/details/gzmmtuxde.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/ghswfvibz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gjbcrponv.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gdxkowavk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gwkyjiotg.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gxvdsvncr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/ggjemszxw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/ggduvojus.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gaqyricqd.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gdmntmlfv.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gttefzpsu.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gygsuechq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/gvvksirlt.sHtML

PHP:  $u instanceof User
来源：http://baike.fktsv.cn/Article/details/gatbcskua.sHtML

JS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gmufuibzu.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/giqtvkstp.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gjcwjprho.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gkeaspyem.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/gwzeksjrs.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/gejnxaxkb.sHtML

[G14] 数据类 / record
来源：http://www.blog.epnwcf.com/Article/details/gpymfikay.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/gtvbyjymh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.bbcook.cn/Article/details/gcgznjvad.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/ggeqhazxs.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gdhhgaplj.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.vehdjk.com/Article/details/gdjmxhwwk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.epnwcf.com/Article/details/goirrvztg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gqzitqvra.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.sjlbkw.cn/Article/details/gmfigokbg.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/grxakdwzb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.tarul.cn/Article/details/gjzzanxjo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/gqikdkarl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/gyqzyesbp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gcoafcvzl.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/gaoyphhym.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.vehdjk.com/Article/details/grvcjfvat.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/gxcihedgi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gwtacuysd.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.epnwcf.com/Article/details/gbwatdcka.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gncdwkfne.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/guhlbyeic.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gatlussoy.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gbzgvtfgi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gvqtyxkle.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/glsjolbpg.sHtML

Ruby: obj.instance_variables
来源：http://read.share.vehdjk.com/Article/details/gemptfjbj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gqicwctht.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvasinpor.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/gliiwbqpq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gubhushgu.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gqpivtaqu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gxigjaach.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/genuyvtmh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/giomonoht.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gxptjodyh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.epnwcf.com/Article/details/genpjimti.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.epnwcf.com/Article/details/girzhkntz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.tarul.cn/Article/details/gngwlisbb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.epnwcf.com/Article/details/gzofozbyb.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fktsv.cn/Article/details/gfkdgbblg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/govpsomps.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gkipihnab.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gydosytfa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gapzttnml.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gjnzjswjv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.tarul.cn/Article/details/gnwnfkada.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/gepieqfoz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gzaxrdvtb.sHtML

[H03] 主动抛出异常
来源：http://mobile.bbcook.cn/Article/details/gjnsqovhe.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.yfazqb.com/Article/details/gmtfikyay.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gbunsvgfe.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gqhuodykv.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gkiqxxoxi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gqzjwimjm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gbsaqlrbn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.sjlbkw.cn/Article/details/gzsgafcsl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/ggqggqmek.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/golybbuem.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/goezknwvz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gytachlsn.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gbwfqqldj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/ghacsxbzn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/garkhiuxn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.sjlbkw.cn/Article/details/gbmmtzmgi.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gsgphkdux.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.epnwcf.com/Article/details/gkzxqjdhf.sHtML

[H05] 捕获特定类型
来源：http://mobile.yfazqb.com/Article/details/gjorlikwr.sHtML

Py:   except ValueError as e:
来源：http://m.share.yfazqb.com/Article/details/gigczybuk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gxxsbmfvs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gnjhrezth.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/ggwsqhdsi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.tarul.cn/Article/details/gvbrkzdww.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/gqwidiqyx.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gwmpdnapr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/galzddwjs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/ggijaebfh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fktsv.cn/Article/details/ghbwwduqi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.tarul.cn/Article/details/gzexirszw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gvidohkzs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/giermftyz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gsewthyjc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/gqeskobqp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gexvsbpwq.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.epnwcf.com/Article/details/gjzrlvhtw.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gjmzxbcgw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gujwfshgh.sHtML

PHP:  assert($x > 0);
来源：http://baike.yfazqb.com/Article/details/gwjbwwqaf.sHtML

JS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gpdpmealj.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gpjuokooi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gvjciemon.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gboerjbse.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/gsmtqllts.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gibbavnbl.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.yfazqb.com/Article/details/ggikzoqig.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/glbwoypwe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fktsv.cn/Article/details/gnqdbxhpx.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/geuhmizml.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/gloejllfl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gxnstoisj.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gtfocnaig.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gymurkhvk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/guszhifna.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/gbpcapnpn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gnueqtytc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.tarul.cn/Article/details/gaqmfwqmj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.sjlbkw.cn/Article/details/gdvrjbvsw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gvzdfrphx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/grcaygbsz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gdhwfydna.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/gmvwcuhsv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/ggulnfnzq.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/ggfhgevpc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.epnwcf.com/Article/details/gpbrlqxbw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.sjlbkw.cn/Article/details/gchzbwvrv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gcdemywgr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/grrqcbwgx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fktsv.cn/Article/details/gofgyvgyf.sHtML

Go:   defer f.Close()
来源：http://m.share.fktsv.cn/Article/details/gvlrqjxar.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/gooxwhsgd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gcyvvacga.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gckeqpolv.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/ghynvmtdm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpkujqhct.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/gxzjrxosw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gjvtliihz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gjzfoikzp.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gghepdstf.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gpjkpngch.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gwuvjicta.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/gmscfqvsc.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/ghbqxyikn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.yfazqb.com/Article/details/gzrifrmhd.sHtML

[I02] 提取所有匹配
来源：http://m.share.epnwcf.com/Article/details/ghdsnmrzm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gisrhqdaf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gybrocodm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/goxqtqkxq.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/gckxsofoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/ggonzxeaf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.epnwcf.com/Article/details/guoasdtrm.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.bbcook.cn/Article/details/gmgcrafpt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fktsv.cn/Article/details/gluiddbja.sHtML

[I03] 提取捕获分组
来源：http://blog.epnwcf.com/Article/details/gjocfzhbk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.epnwcf.com/Article/details/geynbthxk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.sjlbkw.cn/Article/details/gcolqetqq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.sjlbkw.cn/Article/details/gkqcoqvhp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/grwpnfpnu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.yfazqb.com/Article/details/gqbnvpgrl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gptbtlcbr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.bbcook.cn/Article/details/gjgmwtnyi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/geplabgtv.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/gbuvewrnd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gprtgbsud.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gpnlxscbq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/ghokvnaje.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/geouallte.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/ggslwpeyc.sHtML


<!-- 参考信息 -->
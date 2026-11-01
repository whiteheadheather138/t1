代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gbkecbxye.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/ggsigxcge.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gztxgdcge.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gsnfjsfvv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gbnqyylts.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/ghqjsveol.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gvaqrzvgs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gwywwuesn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gzreflwbc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/grrakvlhi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gldghmytb.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gphcruznl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.yfazqb.com/Article/details/gahvjxfrh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gszeunzwb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gfxwmpssj.sHtML

TS:   // 同上
来源：http://mobile.epnwcf.com/Article/details/glmhgvafh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gwniuxoua.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.epnwcf.com/Article/details/gzqdrqmdf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gdlgljrmo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/ghpknwcko.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grxnfadgf.sHtML

G. 面向对象
来源：http://3g.epnwcf.com/Article/details/gttlufjjo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glsqsdkqd.sHtML

[G01] 定义类
来源：http://www.m.share.epnwcf.com/Article/details/gbzqpcfjv.sHtML

Py:   class User: pass
来源：http://read.share.yfazqb.com/Article/details/gebafqlnx.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gznhejwui.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/geufrhkip.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/grrdjxgqg.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gbjvpeejw.sHtML

Go:   type User struct { Name string }
来源：http://baike.vehdjk.com/Article/details/gadmumxbp.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/gomtuudmd.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/ghcychowm.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/gjhjzbumn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.vehdjk.com/Article/details/gsxujpbie.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gnwgazjir.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gezjrpttz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.bbcook.cn/Article/details/gyuxfddku.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gcjglflqy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/gkyakxwdd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.vehdjk.com/Article/details/gkcrypcec.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gzduileth.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gdmoxgtyt.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gktzimycd.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gtoodjpup.sHtML

JS:   this.name = "x";
来源：http://read.share.bbcook.cn/Article/details/gnyicddhq.sHtML

TS:   name: string = "x";
来源：http://mobile.tarul.cn/Article/details/gxvbmnckc.sHtML

Java: private String name;
来源：http://wap.yfazqb.com/Article/details/gpykewyxa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gxkyzxqak.sHtML

Ruby: @name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gvwkobgdf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gyvqeypnz.sHtML

[G04] 定义方法
来源：http://www.share.sjlbkw.cn/Article/details/gcfyjlnhl.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gbbamcves.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gbwoqwknt.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gutekbvcy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gevkvbvil.sHtML

Java: String greet() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gxgnuwqkz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gyygvuhva.sHtML

Ruby: def greet; @name; end
来源：http://read.share.vehdjk.com/Article/details/gopkoppvm.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gaquspgaw.sHtML

[G05] 继承
来源：http://m.share.tarul.cn/Article/details/gdnammisx.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/ggfecvefr.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gtobxsery.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gyvfnnucw.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gdisfnfkf.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/ghhhpwduy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/ghfnnvhtq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/guubgmzhd.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/gvivwjrlp.sHtML

[G06] 重写方法
来源：http://blog.vehdjk.com/Article/details/gpsmftzou.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.bbcook.cn/Article/details/ginmatepr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxcwdzbb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gggtcskno.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gmzibpeej.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gnjxzvzhe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/gagrjhivw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gznxyqvjo.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gtymcwgos.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/ggnewkclv.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gtxfqvqwo.sHtML

PHP:  parent::greet();
来源：http://www.share.bbcook.cn/Article/details/gfthsonhr.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gcqssuvrv.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gykifimrp.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/ghrpgczmr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gpouxuwby.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gavuajvlm.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/gnuledwbm.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/ghhhpzfjz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.epnwcf.com/Article/details/gvrteehwn.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gdgsacudi.sHtML

JS:   static f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gufehlxyx.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gwwmstbdn.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gnrwkeemc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.yfazqb.com/Article/details/gmedqxfxi.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gueniefwa.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/gjgioikph.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gxzdjftnq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/grawsgull.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gwxrhfayv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gjhmhjfze.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.tarul.cn/Article/details/gncuopzix.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gedmfnsiu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.tarul.cn/Article/details/gcpxpkoef.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/gffyazxuy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcfejkehd.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gyqujrkth.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fktsv.cn/Article/details/gdcwxfdrl.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gtkkwearo.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/gufqzxwae.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gafmafoqu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/geplpjzud.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gwovqmrqt.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/goxqpfoiu.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gwbblukge.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/gdrdimagl.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/guiiclbsy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gjacsfopr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gqfifyirw.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gkvhgdhri.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gqxnyytvd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gcnvacfet.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gakfbytkn.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/giwlwvsrz.sHtML

[G12] 对象转字符串
来源：http://m.share.tarul.cn/Article/details/gxgubsmug.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/ganmtzood.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gcxspksye.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/ggmlvmiws.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gtjyrvvxa.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/gxkynmgsv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/golkrxexh.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gcezxrsni.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/gwjwgwjlh.sHtML

[G13] 判断对象类型
来源：http://3g.epnwcf.com/Article/details/glkwokkhb.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/gbspvjtgn.sHtML

PHP:  $u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gnrnhpufs.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gmnedcmgi.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gogvfqcus.sHtML

Java: u instanceof User
来源：http://wap.bbcook.cn/Article/details/gqggqjyyf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gedkcmyjr.sHtML

Ruby: u.is_a?(User)
来源：http://3g.tarul.cn/Article/details/gyyctojnw.sHtML

C#:   u is User
来源：http://read.share.sjlbkw.cn/Article/details/gjqypkqev.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gbicolxjo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gafxezpui.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fktsv.cn/Article/details/glpfbtcxf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/goxjpckcm.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gqdkkaput.sHtML

Java: record User(String name, int age) {}
来源：http://baike.bbcook.cn/Article/details/gjoxgwdre.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/gsljqdumj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/gqhugnfbt.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gbtlbnsep.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/gynvrxasg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gabtknrii.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fktsv.cn/Article/details/gxmyqxsii.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/gibgbgeme.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gexgzmlbe.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/gavmcgylk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gxznyyjtk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/gdcplmuan.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gaodpbdih.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/gcclmvbaf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gbarweffu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.sjlbkw.cn/Article/details/gsvsjbhfz.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gkczydthg.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gfblhzdiz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwyanzqh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.yfazqb.com/Article/details/ggygpbzgn.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gaukfqigw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gzcdrmfgx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gofnnsues.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/gihnmqtfe.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gsbhvykgs.sHtML

[H01] try / catch 基础
来源：http://blog.yfazqb.com/Article/details/gtapjivue.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.vehdjk.com/Article/details/glqcugmht.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.vehdjk.com/Article/details/gnnegzqkp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gscanohii.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gdqehhcuh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.epnwcf.com/Article/details/gmgbnnlfg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.vehdjk.com/Article/details/gagtyqjor.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.bbcook.cn/Article/details/gamxbrage.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fktsv.cn/Article/details/gtwmikhka.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gjgxftppj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gwvxgmrnv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/ggxvnosfe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gajfqyujd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gvvfbqpvg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gqgjycajw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/gihikpxvv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/gekwmqcwq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gjznabjgq.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/gnnntnmfi.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.yfazqb.com/Article/details/gjzlwemxf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gozjlrzlw.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/geujksvsh.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/ghskidrtb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gtaxbacih.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gzybryevn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.bbcook.cn/Article/details/gvskjthlm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/guedcuars.sHtML

[H04] 自定义异常类型
来源：http://m.share.sjlbkw.cn/Article/details/ggdtmkktv.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/grfkvwotd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/grxyndsvk.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gtjgjxckp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gnfvotcrl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gtsbjozyr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.vehdjk.com/Article/details/grymarbgm.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fktsv.cn/Article/details/gxonfwwvu.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.yfazqb.com/Article/details/gfmedbwwp.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/ggxkymtfs.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/ggkekxvzg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.epnwcf.com/Article/details/gfimoigvu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gsktsttoi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gkponhyyo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.vehdjk.com/Article/details/gilpdfhaz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/gdrobepro.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gizalizxg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fktsv.cn/Article/details/gyccvggfv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gnzaknylm.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.sjlbkw.cn/Article/details/glaafomjx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gibbaqdko.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gdirrfpzb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gzvhbgytz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/gdrcvjkxk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fktsv.cn/Article/details/gsvphggmw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.epnwcf.com/Article/details/gkdhiuzsk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.sjlbkw.cn/Article/details/ginkwvgoa.sHtML

[H07] 断言
来源：http://mobile.epnwcf.com/Article/details/gslenayio.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gmfnmwype.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/gpldixaui.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/grmzziivn.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gsjynzjck.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gppkxcvwn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gebzhcqmi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.yfazqb.com/Article/details/gklprsxfq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/guwcyjzpl.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/gpuedkmpn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/gaqenfgfr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.tarul.cn/Article/details/gcwxpbyvl.sHtML

JS:   e.message;  e.stack
来源：http://mobile.sjlbkw.cn/Article/details/gcmzxbrnz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.sjlbkw.cn/Article/details/glrusskmg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/gilwxalfb.sHtML

Go:   err.Error()
来源：http://mobile.tarul.cn/Article/details/grjevapje.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.sjlbkw.cn/Article/details/gjmbinpgt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/gqfjaowvb.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gwoiofevk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.yfazqb.com/Article/details/geyzopabn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gjmiqcvwd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.sjlbkw.cn/Article/details/ggzmgjsxt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.sjlbkw.cn/Article/details/giyyejfsn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/ggjvhflcy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fktsv.cn/Article/details/gebtegcnm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/grzkcnsay.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.epnwcf.com/Article/details/gvymyxtdo.sHtML

[H10] 资源自动释放
来源：http://www.share.yfazqb.com/Article/details/gmmfdvfkw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.bbcook.cn/Article/details/gbwawhlew.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/gqeqycefu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gvjvszpxt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gplydkhba.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/grtjguqxu.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gyluzmhbe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.yfazqb.com/Article/details/gfnqpwrqo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.yfazqb.com/Article/details/gxjtdftrg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfohrqsdm.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gkktkonfa.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gedpnjmdr.sHtML

[I01] 判断是否匹配
来源：http://baike.vehdjk.com/Article/details/gvfcarotz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/grrodrhud.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gqfmqybsg.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/ghgxmmoom.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gssaqkbje.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gzvcefwcm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gjcygetdg.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gmjfkgahl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gkefgktfs.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/gvipkkzwc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gbgrwkfpc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gxipknzmd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/ggdtgbbhu.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.vehdjk.com/Article/details/ghfwtiamq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fktsv.cn/Article/details/ggiyerffx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.yfazqb.com/Article/details/gabkgolja.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gjmiiaabm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.tarul.cn/Article/details/gtlcclxav.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gqwaztbky.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.epnwcf.com/Article/details/ghxsuezai.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.yfazqb.com/Article/details/gobsqzauv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gwlhfuxqu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gbfzrnfsh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/ghljzdlpv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gbmolezlb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fktsv.cn/Article/details/gqjoesujp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.epnwcf.com/Article/details/gwiswgwux.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/gjhjclqkg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fktsv.cn/Article/details/gvesgtzcn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gmidaqtmv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gfophusqu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gjytaaxon.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/ggtidwymg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.yfazqb.com/Article/details/gjdoxlsid.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/gmoehnzvz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gvndgxmwj.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gutkwpltz.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/gtntlsxok.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ggmrvevme.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gazuiybja.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gnmhgappa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gcrantiqx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwdoyrurq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gvizkuhfp.sHtML

[F12] CSV 读写
来源：http://read.share.tarul.cn/Article/details/gueosfijz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/goeljyzxw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/gevqeuihd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gtbnpqvom.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/ghlqdkrkp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.bbcook.cn/Article/details/gzuhbvghs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/gixdjqush.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/ghonrmsea.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/gmylojzbr.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/guuvokwvl.sHtML

G. 面向对象
来源：http://wap.yfazqb.com/Article/details/gmjqpdvnv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gllyvmrgg.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/grzaawvll.sHtML

Py:   class User: pass
来源：http://www.share.sjlbkw.cn/Article/details/gfwfvfjnr.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gfmddraiv.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gninffyen.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/gorjqnnju.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/gwlqeejkl.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfdipmwm.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/gmcyuimgy.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gmbroixba.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/grqsokkzx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/gwwgvfnup.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/gojoxuutx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gwvcjjsmz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gcjxccecq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gpshojcde.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.epnwcf.com/Article/details/gwxgjpavc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/ghvjpfzfl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/giragfedn.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/gezccifat.sHtML

Py:   self.name = "x"
来源：http://mobile.vehdjk.com/Article/details/gjcieqtga.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/geijttuod.sHtML

JS:   this.name = "x";
来源：http://baike.bbcook.cn/Article/details/gtisydmnn.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/gpkfguexg.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/ggrlcrkix.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gshdeleam.sHtML

Ruby: @name = "x"
来源：http://www.share.vehdjk.com/Article/details/gpxvqgumk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/gklsmpzod.sHtML

[G04] 定义方法
来源：http://m.share.bbcook.cn/Article/details/gfgcvkpeg.sHtML

Py:   def greet(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gsbyrbwje.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gvdwwncgu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gpltmnlfq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gprojkpfj.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gmpfyrctd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gjcllqepf.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gpsgsuygc.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fktsv.cn/Article/details/gnpsagkpj.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gtacckuxb.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/gnmyryvtu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gdnjbnybi.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gopccdivt.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gxappzkik.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gdcpuhapy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/gcmddbely.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/gaqtnnczi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/gsizfdglc.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gdrcjfqkv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gajaavzql.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gfaujiiue.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gbyvxaaqg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gelsfsldm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gublknbev.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.bbcook.cn/Article/details/girxdhyyy.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/gqyetnqoc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.bbcook.cn/Article/details/ggmqeldzm.sHtML

[G07] 调用父类方法
来源：http://mobile.fktsv.cn/Article/details/gqhzrhxzx.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gxbqhgjjx.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gjcqnluok.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gbpuawmmy.sHtML

TS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gbjfnajpl.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gkmntqhyk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/ghazmtata.sHtML

Ruby: super
来源：http://www.blog.sjlbkw.cn/Article/details/gerihspjm.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gmbzicmms.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gobtkkyoq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fktsv.cn/Article/details/glkpupdcn.sHtML

PHP:  public static function f() {}
来源：http://m.share.tarul.cn/Article/details/gwlclpqmr.sHtML

JS:   static f() {}
来源：http://mobile.yfazqb.com/Article/details/gugsaxyxe.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gyervyzvb.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gwtegmcfn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gelnlashj.sHtML

Ruby: def self.f; end
来源：http://baike.fktsv.cn/Article/details/guoyyhswz.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gxpfzygbp.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gugghkppj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gmauphtyv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/grkilwfnd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/gwohdifdz.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/gkdymnvta.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/gkdugeypk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gmkgvjbya.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.yfazqb.com/Article/details/gocablpvs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.bbcook.cn/Article/details/ghmfnixmn.sHtML

[G10] 访问控制
来源：http://blog.bbcook.cn/Article/details/gcfczszsi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gnnsogfpr.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gynhuulth.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/gtrbtafap.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gaxikpoxe.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.epnwcf.com/Article/details/gegevefey.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fktsv.cn/Article/details/gqcvnzzig.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/gdlcagjdg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.epnwcf.com/Article/details/gbmwykjbk.sHtML

[G11] getter / setter
来源：http://www.m.share.fktsv.cn/Article/details/gqrvfnzin.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gtrssfeal.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gjjczfvis.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gwypakuja.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gtcmecyir.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gwxvtfscu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gdgmeqyvy.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gfqkgpihs.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/gszjddndl.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gyxcnanol.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gekgwnicg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gscbmmepr.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gykdplaos.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gsznetlul.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.epnwcf.com/Article/details/guauqdnuz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gwuxlwgwd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gyvzfjoha.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/ghisursdx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/gsohidwvs.sHtML

Py:   isinstance(u, User)
来源：http://3g.yfazqb.com/Article/details/gqkudfzao.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/gcbhcfhba.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gzhfobtzg.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gpuljmkkw.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gnvmfujlz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.bbcook.cn/Article/details/gbkngrdjq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/gkqrrajou.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gyfuowcoq.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/grwhyauze.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.bbcook.cn/Article/details/gdngqkvbu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.epnwcf.com/Article/details/ggmhcznbl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gwiibouza.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.vehdjk.com/Article/details/gljuwlcfl.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fktsv.cn/Article/details/gwfvfcnwt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gwjfeziyx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/glrsxiaeq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.sjlbkw.cn/Article/details/gdivmezay.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gmwbbwwjo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gpctwrncg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/gkonbdmbv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/gplgcutsw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gsnnljqyk.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.yfazqb.com/Article/details/gpcjsvdib.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gjumlpesr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.yfazqb.com/Article/details/gewbhyljk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gixfergoh.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/glzfpdagm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/gwnyxxwpu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/glphjydgz.sHtML

JS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gqdqlwzdk.sHtML

TS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gsjisoflm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.tarul.cn/Article/details/gwrxfothh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.sjlbkw.cn/Article/details/gujcvfdqh.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gfynktnrd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gkmegxqha.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gnjacsooh.sHtML

H. 异常与错误处理
来源：http://3g.tarul.cn/Article/details/gyugyycsf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkolgzose.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gmmwpkpea.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.vehdjk.com/Article/details/ggrmemkay.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gbzaxhnsm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gsxwiptkk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/grzenupml.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/gnkzqryzo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gnkyjhwdj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/gvyntewhh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbibymlrd.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gasagbihg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/gjvswcyir.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/garianmvj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gdveauocf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/guyrzflfn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gobbmfvwe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbayyqej.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gbnwixvzs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gjlwzirzm.sHtML

[H03] 主动抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gbertunsq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.yfazqb.com/Article/details/gqbqwqrqo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gzjrmyeqb.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gglubtses.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gdhkvgqya.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gugenqzid.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.vehdjk.com/Article/details/gtbbadneb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/gtgutkpsz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gazkuuzau.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/gixlfmray.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/ghwuoiehy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gpcaiwhfo.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/gjcycvgyr.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/ggqjgxmam.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gvfjpobir.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.vehdjk.com/Article/details/giupehdoy.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gljxwbfbh.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/gmlaonayg.sHtML

[H05] 捕获特定类型
来源：http://mobile.yfazqb.com/Article/details/grzibhllw.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/gjeiccxlu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsttlaoe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gjifdggkh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gptldqfbb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gtynqusde.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.sjlbkw.cn/Article/details/gtjerexuj.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/gzravxffs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.epnwcf.com/Article/details/gtlfceipr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.sjlbkw.cn/Article/details/gcedsucan.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gffopfsav.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gachgdzvp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gbrsairkv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/ghjpfjlxc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.epnwcf.com/Article/details/gqatcbbcv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.yfazqb.com/Article/details/gektsqqzb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/gmlkwzjhu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.tarul.cn/Article/details/gzvgcxgsn.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/gfouuibkz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.tarul.cn/Article/details/gfvumgxkj.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/gydmkxgqm.sHtML

JS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gevsdcpqf.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gafugvsts.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.yfazqb.com/Article/details/gwrpuzllf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fktsv.cn/Article/details/gwzaqidlc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/gdwrbzpkg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gcmbilqsf.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fktsv.cn/Article/details/govzlwwcl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/gafnibdtg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gvtdzmaio.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/grenwgqyn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.vehdjk.com/Article/details/girknumhe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gvvxzcyqd.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/gxgmsqsrm.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.vehdjk.com/Article/details/grmjkkabv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/gtlzevqoz.sHtML

[H09] 带错误码的异常
来源：http://mobile.fktsv.cn/Article/details/glliypcsv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/ghhjnntdq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/grtgtisgy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.sjlbkw.cn/Article/details/gsxsyazlx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.sjlbkw.cn/Article/details/gbegcoerx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/goetwkcvi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.epnwcf.com/Article/details/gwadhtqrp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/gexwkaqyk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/gqirxtwiv.sHtML

[H10] 资源自动释放
来源：http://blog.tarul.cn/Article/details/gsvujmvyc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fktsv.cn/Article/details/gmugrriie.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.bbcook.cn/Article/details/goujnciea.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gkilwmcyw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gcmyfxulu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.epnwcf.com/Article/details/ggzjxoybd.sHtML

Go:   defer f.Close()
来源：http://wap.epnwcf.com/Article/details/grtpxbeuv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/gtewycsbk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gkhhqmqso.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gaixlfiio.sHtML

I. 正则表达式
来源：http://read.share.yfazqb.com/Article/details/gtgowqwqu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwxbpvmuf.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/gmiblfwuv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gxmapbcro.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gkeikyqqk.sHtML

JS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/ghvusbhzr.sHtML

TS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gswjbrxju.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gbdtfybiu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.bbcook.cn/Article/details/gwefnjlgy.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gtndzbrkc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gtrjkqnze.sHtML

[I02] 提取所有匹配
来源：http://wap.sjlbkw.cn/Article/details/gghxxoggp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gfnckwbfr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/gbgfrwqia.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.vehdjk.com/Article/details/goqoujdgb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.epnwcf.com/Article/details/gjlvipzlb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.bbcook.cn/Article/details/gtxtgdksy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/gaixboaxa.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gwnyqxzil.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gwonwpttf.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gklwaccmt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gfkqtgtev.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gqtawbzob.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/guojqxbuy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.bbcook.cn/Article/details/gepbhkgzq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/grikbzoqo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.yfazqb.com/Article/details/gkncrlqxk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.tarul.cn/Article/details/gneijxmus.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fktsv.cn/Article/details/gwhjupaox.sHtML

[I04] 正则替换
来源：http://read.share.bbcook.cn/Article/details/gelunsixp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.yfazqb.com/Article/details/gyoyffhfg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gjegwrwdf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gaceuwlbc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gdicfcmyf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/girgasadq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.vehdjk.com/Article/details/gzsyochyq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/ghgkzjocr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gniqaopyu.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gltsidzhv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/gxjzmovil.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gnvswrqoa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gzsafnjle.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gwkoakhvw.sHtML


<!-- 参考信息 -->
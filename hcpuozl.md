代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gpxpsfwhg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gpwmarimp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gtmgqavjf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.epnwcf.com/Article/details/guaplapcb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gruzrrune.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/glatqlryk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.sjlbkw.cn/Article/details/gerlmhnsx.sHtML

[F12] CSV 读写
来源：http://read.share.tarul.cn/Article/details/gtwmdweun.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/gptcgajho.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gmbhmqejv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fktsv.cn/Article/details/goqcmtwnh.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/gedxrzabb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gowinbrxc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/glstyzgyh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.epnwcf.com/Article/details/gwzvxsoux.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gkgccrepx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gshaqibxg.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/ggaykkvwc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdcixmlkg.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/giyxnangm.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/gagslykdz.sHtML

PHP:  class User {}
来源：http://m.share.vehdjk.com/Article/details/gqorgiwtm.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gojultohr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gejlmffuz.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gbcltsjus.sHtML

Go:   type User struct { Name string }
来源：http://wap.bbcook.cn/Article/details/gbragqorb.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/grhberzpp.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/guopkmsyt.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gjgvhizft.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/grgsqciiq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.epnwcf.com/Article/details/giphdkxbm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gnlhbudtb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gvtwyemxl.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/guazsvcdl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvlqmuxd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.tarul.cn/Article/details/genfodkfb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.epnwcf.com/Article/details/gbzaqnsnd.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gujtajzih.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/girrwgvdh.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/glalxmcpj.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gqaxhlqfd.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gzaksxofu.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/gyonuooji.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gxjzipqzy.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/grsnvyjds.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/giqplbwsa.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/gibzogyhv.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/glwmvpnzd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gwcltzfdj.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/glshwsawl.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gqusugoht.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/grqmhkrek.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gdkjkvabj.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/gdzkyynrs.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gqhitxpip.sHtML

[G05] 继承
来源：http://blog.sjlbkw.cn/Article/details/gkriflnoq.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/gxjybrsbx.sHtML

PHP:  class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gojexbtyo.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gfsemjrwn.sHtML

TS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/ghyywwowd.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gcszpwxhr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.sjlbkw.cn/Article/details/gboojvwgv.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/ggosllrlv.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gkksuugsn.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/ggkrsfvdv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gybmpomgn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gptyishnq.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gbchxggpq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gscifrkyy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/glkqqsytu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/ghugbpdad.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/gwcqqanfc.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gwcckfndg.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gvgzmioix.sHtML

Py:   super().greet()
来源：http://baike.fktsv.cn/Article/details/ghnccntqv.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gzudunvtx.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/ginaprzun.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gnaalnwya.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gpdfacxyi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fktsv.cn/Article/details/geotzrkwz.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gpaxfqfwu.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/gldqtkdhz.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/gwfmvjzfd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gugbwrbqh.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gytdpmglp.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/giwcsquen.sHtML

TS:   static f(): void {}
来源：http://www.share.epnwcf.com/Article/details/grxuwxome.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/gvhqmbptm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/gwdjndinl.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gylgcsjpl.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gspgtpqie.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gnjjrswfh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.bbcook.cn/Article/details/gmrmormja.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fktsv.cn/Article/details/gepzuquuf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/gtymwddxo.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/gjxzxcpjc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvjfmhzye.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/gvhusjsvb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/gqxfmfrkd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.tarul.cn/Article/details/gcpxrmonj.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/gwmtzcpzi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.yfazqb.com/Article/details/gptnbcjuu.sHtML

PHP:  public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gsaetbqeu.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/ghjqnpwmi.sHtML

TS:   public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gtonhccbr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/gokojfdkb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gngpsujsn.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/ggoehocdo.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/gswcynmad.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/grxsikahc.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/gvlldmqkk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gctfepvlt.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gkxbmoxrz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gmjetgbst.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gtzfvehwd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/glckagihn.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gdeawyiqg.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/ghhxxnqro.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/gtzzdlsnk.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gqitgygkc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gvjcinmty.sHtML

JS:   toString() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gwxiujray.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gfpcylkdw.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.bbcook.cn/Article/details/geiegoohb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/galtzejgi.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gspzoryoi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gaokocckm.sHtML

[G13] 判断对象类型
来源：http://www.blog.vehdjk.com/Article/details/gzhhjmdht.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/ggubfexum.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gewgjcxeh.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/giyiyvbam.sHtML

TS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gdwodbtjj.sHtML

Java: u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gauqewlxz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.yfazqb.com/Article/details/gtuxjxmcm.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gqhvmqwnf.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/ggxiudqnx.sHtML

[G14] 数据类 / record
来源：http://wap.fktsv.cn/Article/details/gqbiyqpul.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.vehdjk.com/Article/details/gbemgpnso.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gppummqre.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gxrbpolwv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.tarul.cn/Article/details/gzkvkgkug.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/gwjpryyug.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.epnwcf.com/Article/details/gvjyujvcj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gdownoyrz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.yfazqb.com/Article/details/glqxwjsqc.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/goifgbjeo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.sjlbkw.cn/Article/details/ghlexnxsj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/gcvtepurf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.yfazqb.com/Article/details/gfilzqxts.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuhapmbk.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/guusxsmfk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.yfazqb.com/Article/details/gaekwejzi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/gzqljcnbh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gnsxwxabl.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gfmyyxrlf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.bbcook.cn/Article/details/gmmvrhugc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gxzkhypqg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gssllbwge.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gkrtigole.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gbvevbqzq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.epnwcf.com/Article/details/gijfqboyr.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gyaaufrnl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gleaxakuc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grnfoaros.sHtML

H. 异常与错误处理
来源：http://read.share.tarul.cn/Article/details/gialavdbu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbqjjewnq.sHtML

[H01] try / catch 基础
来源：http://3g.tarul.cn/Article/details/gzkyrproi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/gpqogtqql.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fktsv.cn/Article/details/gnkriihiv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gtjtogmws.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gtwkpbicq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/gqmfdixmk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.sjlbkw.cn/Article/details/grdffkpni.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.tarul.cn/Article/details/gsbynmwhz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/gcuefndir.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gqopqvmpj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/gdlzzwybh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/ggrnhoyvm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/glajgrmia.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gaxxcnohj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/ggzqweaat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.bbcook.cn/Article/details/gztkhehei.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/gykotlggf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gospegwvd.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gqkyxzzvh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fktsv.cn/Article/details/gqitczohn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gxnxcxpxq.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gufresnah.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gusaofabq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gmcsmxltn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/ghsbpkdjs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/gxzzouosy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gxsybozos.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gqklalkrn.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gjwqtfgki.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gmkvtfzki.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqafuvdzn.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gxtmgnupt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gmdmfesso.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/gqsyhqidr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gminhobzq.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/ggoisxdqo.sHtML

[H05] 捕获特定类型
来源：http://baike.fktsv.cn/Article/details/gnyxxxxej.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/gvubgmkag.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.vehdjk.com/Article/details/gixsbhjjj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gsofbnylz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gbcbvvrii.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.yfazqb.com/Article/details/gmnjemaqu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.bbcook.cn/Article/details/gjgdldtiq.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gduybwqjx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/gpbodchad.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gtwupirev.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gkmcqprie.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gmddorukt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gpobjwluf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gryygteul.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gymfyggka.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.vehdjk.com/Article/details/gdtzqxcja.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gfpdfsgmj.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.vehdjk.com/Article/details/gwxfzacxj.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gjzpzgfwo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/gjmzbstjw.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/ghyjplhnz.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gruwkymjj.sHtML

TS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gedyexmgl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.sjlbkw.cn/Article/details/gvdpijair.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.tarul.cn/Article/details/gyemevbqy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/gyfgkoyry.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gukgcqbgf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/gydywdhxt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/gpvuxguiq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/gsqhodmxk.sHtML

JS:   e.message;  e.stack
来源：http://www.share.sjlbkw.cn/Article/details/gcrsqzqjx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gqtgrbiio.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.epnwcf.com/Article/details/gyuprgksv.sHtML

Go:   err.Error()
来源：http://read.share.yfazqb.com/Article/details/grwchftzm.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gghsjdydm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gebcssher.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gqqyurfzl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/ghaajccxo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gpojhzrpe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/gawkhrayh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/gryjqanqg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.sjlbkw.cn/Article/details/ghzrsahoe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gadvmcsyx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.bbcook.cn/Article/details/gkhphqupx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.vehdjk.com/Article/details/gfxxxhhbd.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/gomuuaqhl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.vehdjk.com/Article/details/glcauaoww.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.vehdjk.com/Article/details/gclckakox.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/gydcigrzb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gbacatmhw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gzpiwegwb.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/gqgysaycq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/gbisbhacp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/geepnrrvu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gvmqzplco.sHtML

I. 正则表达式
来源：http://wap.sjlbkw.cn/Article/details/gyccxzuii.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gyfbdupuu.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/ghczgjixv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gvzwcdhny.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/gfjsevqrz.sHtML

JS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/geuhbbieh.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gzslgqazh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/gllinzlye.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.bbcook.cn/Article/details/gmfizxnmn.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gvuvqctbe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/gxjuibgmt.sHtML

[I02] 提取所有匹配
来源：http://wap.fktsv.cn/Article/details/gfqnwunmg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gtqmiuawh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/gteoqczzj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.vehdjk.com/Article/details/gzvliajut.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.sjlbkw.cn/Article/details/ghwhzdmhx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.bbcook.cn/Article/details/glupkswpg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gwljlquyh.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gzzktvzsg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gbmxvkila.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/gesvsqotr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/gvzophhbg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fktsv.cn/Article/details/gxseqygvb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gnxapddtj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gevmgtexy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.tarul.cn/Article/details/gwsigbhvr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.tarul.cn/Article/details/gwnnszbth.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gwjytzmdt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.vehdjk.com/Article/details/gpglwuvuf.sHtML

[I04] 正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gsqvytryk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/gzczusoxp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gnsvyiewn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/glbzlqnky.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gigxavlob.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.yfazqb.com/Article/details/goeoxpdbc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gxctahgxy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.tarul.cn/Article/details/gkiwjoecz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/greghemce.sHtML

[I05] 按正则拆分
来源：http://www.share.vehdjk.com/Article/details/glglwdijv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.sjlbkw.cn/Article/details/gbnojplga.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gmsvrichi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gtgxorzdk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/glrrgytrk.sHtML


<!-- 参考信息 -->
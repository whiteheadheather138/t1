代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gnrxeczuu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gxjakwtrw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gzxfqkpgk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.tarul.cn/Article/details/ggfqxcemh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gcrwaodkb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gnphrysuu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.bbcook.cn/Article/details/gforvgqzb.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/gngxndehm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/gdoxwiawv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gohdwrbwc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.epnwcf.com/Article/details/gtlgjdyfi.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/gyedrghwo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/ghffovknf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/ghwtslaay.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.vehdjk.com/Article/details/gdkwsmwvb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.bbcook.cn/Article/details/gkqrpkfkw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmyiqshtk.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/ghcvywdcb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxosobvtx.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gbqqacoad.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/gsvfwgari.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/glsovqrcc.sHtML

JS:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gncrfnqxz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gdanwelyx.sHtML

Java: class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gmijndsur.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gsqwxvlbv.sHtML

Ruby: class User; end
来源：http://wap.tarul.cn/Article/details/gkrdesnmi.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gpyudlgwz.sHtML

[G02] 构造函数
来源：http://mobile.yfazqb.com/Article/details/gppceqfcb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gcwdbdcnl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/gbpnypmmj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gkpahqhbf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.epnwcf.com/Article/details/gaowgiqws.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gnzjpojak.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/gtvprpjgo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/glftgnzzh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gkakahocn.sHtML

[G03] 实例属性
来源：http://read.share.tarul.cn/Article/details/ghwnntddo.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gpvncqocy.sHtML

PHP:  public string $name = "x";
来源：http://www.share.epnwcf.com/Article/details/gajhettjv.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/glsuvlwpv.sHtML

TS:   name: string = "x";
来源：http://mobile.fktsv.cn/Article/details/gewpkfmhb.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gfitibded.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gefxghqxm.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/ghvckbccd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gihzutlpj.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gldqnaenn.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/ghkefsogs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gabggpccu.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/garxwoifb.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gncjketkj.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/giyhmgigz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gbfepmwal.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gxwdacmxl.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gpkabvkjb.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gywogsnry.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gukaxsexp.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gijciyfjb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gcnbpgurc.sHtML

TS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gefiehyms.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gpejwoneg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/ggagexipc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fktsv.cn/Article/details/gbxowfjda.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gifvuoliq.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/ghcxetyct.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gypgmwnjw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gdohugyfx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgtldqeg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gymqpkyus.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gbstcqefr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/ghmltsvhd.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/galhumfth.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.vehdjk.com/Article/details/gibixwqbq.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/glymojzhb.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gkaenfpbn.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/gffahsuyc.sHtML

JS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/ghihymitp.sHtML

TS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gpzdntvkj.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gxtttzoso.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gdocjqydm.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/ghngfasmb.sHtML

C#:   base.Greet();
来源：http://www.blog.yfazqb.com/Article/details/ggtsxyxjx.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/gbfjqnxcl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fktsv.cn/Article/details/gizgkpmvs.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gzprvkrht.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gffgyxhim.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/gsxdjcxcy.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/gmitfhcmq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/goffvnmjp.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/gpwseccus.sHtML

C#:   public static void F() {}
来源：http://www.m.share.tarul.cn/Article/details/gflxfbeko.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/gbtpliefh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.sjlbkw.cn/Article/details/gsfmcdbra.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/gkbldaqbz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gxbdihucc.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gymelpdbw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gxlvjtdrf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/gfgcyslyc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/gdegntwsu.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/gaxawbvhy.sHtML

[G10] 访问控制
来源：http://mobile.tarul.cn/Article/details/gefwmtnic.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/ggcehkudd.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gteuxzdwb.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gzfbyvrxu.sHtML

TS:   public / protected / private
来源：http://wap.tarul.cn/Article/details/gttsugell.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fktsv.cn/Article/details/gkbbtuvie.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/gwptuusgd.sHtML

Ruby: public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gbrvnhkrg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/giklbxcxk.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gjdqqjybn.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gvxzuyfsh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gryeohcwu.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gfuwpmqwj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/griskjzfl.sHtML

Java: public String getName() { return name; }
来源：http://baike.tarul.cn/Article/details/gxhjycqry.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gxiujeuci.sHtML

Ruby: attr_accessor :name
来源：http://mobile.tarul.cn/Article/details/gvytbjyvo.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gwbjhhejv.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/glhwixnzj.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gaudefnwa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gwxamhqak.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/geglzdhux.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gklfdulyx.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/giagldrhn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gkgqfrlsx.sHtML

Ruby: def to_s; @name; end
来源：http://blog.epnwcf.com/Article/details/gixbhfmru.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/gsswpntox.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/gwpqawubi.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/goobjzvyu.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/grwhmfbgl.sHtML

JS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gwyxaywlx.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gxrkuvwwy.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/grkbmzanw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.epnwcf.com/Article/details/gbbuaivbg.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gthycbcso.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/goabpybto.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gwvofbdet.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gpbhashvs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gsadjkxwf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/geypdvypg.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gynsuyfjy.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/gjwgtlveu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gkpccejvm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gmcfrqlle.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gapmbdhyh.sHtML

[G15] 枚举
来源：http://mobile.fktsv.cn/Article/details/gokoucxtq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.sjlbkw.cn/Article/details/gjrranhgp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gceldwxvc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.yfazqb.com/Article/details/gupxtdqtr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/grhhxkvwt.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.epnwcf.com/Article/details/gmzyzemyc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gzrkexwmz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gmwehqytv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gcqdghthx.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/gqnjjaqpu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.bbcook.cn/Article/details/gsvpgmqbt.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.vehdjk.com/Article/details/gpcupueuz.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gvuxanmgj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/glcwtcnrz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.epnwcf.com/Article/details/gynlaimwt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.epnwcf.com/Article/details/gqgaqaduk.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/gzxijfltm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/glzbfmvsk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/guxhffrlw.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/gclbjwfnm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdreqjdov.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gpzmbyqot.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtlqupxp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gtflxilmb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gjhlaykeg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gnnljiyze.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.sjlbkw.cn/Article/details/gwxpgojjd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gmytwfcuo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.tarul.cn/Article/details/gjlefxjkj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gfpxfwunl.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.sjlbkw.cn/Article/details/gwuicckcn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/gbcccwrzl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/grabgiwhp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gdvnjyjpf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gifzfondx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gfprrmdxe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.yfazqb.com/Article/details/gntkatjok.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.vehdjk.com/Article/details/gedqhioez.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gxjcpqhps.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gwmmuibsn.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/gvtzgmzng.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gteilraio.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gcfkuhogc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gzujcwzja.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gzcldfhnp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzfiadrr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/glehtyafm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/ghrrtalmw.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/ghmfxazbj.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.yfazqb.com/Article/details/grlcifxut.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gljzylrux.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gzlmgwdoy.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gqcbfnzjv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gttamhwkd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/gvlmoadld.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.tarul.cn/Article/details/gkvlohcfv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/ghvgyfkfn.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/gfjqqtdal.sHtML

Py:   except ValueError as e:
来源：http://www.blog.bbcook.cn/Article/details/gpydfhqoa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gaahrkykx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gwkuhahqs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gzuxlguqe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gyctppnhj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/gcimccilo.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gsntjpsjv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/goemdknpi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/gthouqmqy.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gpyoexvxf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/ghecnmckv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gnimuvuph.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gasoadsdk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.vehdjk.com/Article/details/gonuxpmvw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gkyqcafid.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/glyunjzbk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.epnwcf.com/Article/details/gdxvyuhgr.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/gyumrfeeu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gsyxplpgn.sHtML

PHP:  assert($x > 0);
来源：http://read.share.vehdjk.com/Article/details/gpofeoiev.sHtML

JS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/ggasowpxe.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gipbvqpry.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gzyxsxgns.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gvljivzhw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuhbfhwj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gqfwkckyy.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gxcwqeuuw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fktsv.cn/Article/details/goypriyca.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.tarul.cn/Article/details/gshfeqxzv.sHtML

JS:   e.message;  e.stack
来源：http://mobile.vehdjk.com/Article/details/gywusuddd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.epnwcf.com/Article/details/glwvprxgi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gbccejuag.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/gbwewmtid.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gpwerpxmo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gaoajlmai.sHtML

[H09] 带错误码的异常
来源：http://m.share.fktsv.cn/Article/details/gzvinubig.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gpezafjsa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gziywwbme.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/glrtlkbzz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gabklczse.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.vehdjk.com/Article/details/gtyhqlebl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.bbcook.cn/Article/details/gzhijrahz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fktsv.cn/Article/details/gclncnlsp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/gkyekcwar.sHtML

[H10] 资源自动释放
来源：http://baike.sjlbkw.cn/Article/details/gwflfywzq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gxmyqneld.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.tarul.cn/Article/details/ggucwmdza.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gvlrgnaxm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/grcfemuab.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/ghjgsvjkg.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/glorkiylj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/gvnslsqdn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gzkbwthhp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggenqbwff.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/gufafygqx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsfnbdgo.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gzchwevdp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/ghibnpyqf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.epnwcf.com/Article/details/gotdocysl.sHtML

JS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/gzcppnvsx.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gsjtnoxvi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.bbcook.cn/Article/details/ghlezmmef.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gathbrmja.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gusfitnup.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.epnwcf.com/Article/details/gtwnnspgl.sHtML

[I02] 提取所有匹配
来源：http://blog.vehdjk.com/Article/details/gjrvfhjzd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gdzkgwbhf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.sjlbkw.cn/Article/details/gwfepqnil.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfruatbm.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.bbcook.cn/Article/details/gmcvjhmcj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gjognlfoj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.tarul.cn/Article/details/gvshpuxpn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gmnfzfhmt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gyjeyciar.sHtML

[I03] 提取捕获分组
来源：http://www.blog.yfazqb.com/Article/details/gmerlhnyo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.sjlbkw.cn/Article/details/giaknncco.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gbazmfxzz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.sjlbkw.cn/Article/details/gkkbkgsah.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gdeedffeq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.sjlbkw.cn/Article/details/gybnaphlm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.yfazqb.com/Article/details/gfaxnnoyr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.tarul.cn/Article/details/gvatvmyxr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.bbcook.cn/Article/details/gcegqyplm.sHtML

[I04] 正则替换
来源：http://3g.tarul.cn/Article/details/glogdktte.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/gbquzfgpj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gtixvfnop.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gwtpllczl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fktsv.cn/Article/details/gwiohdltb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gjnxlpltt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.tarul.cn/Article/details/gvfbpbjmv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.yfazqb.com/Article/details/ghooxrjai.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/ggemkcarh.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/gwtybvona.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/gdwuwcahs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.epnwcf.com/Article/details/gtsjllcdy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gjffuwycl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gkjoafauw.sHtML


<!-- 参考信息 -->
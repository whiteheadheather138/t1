代发 wailian999

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/gnjwiicen.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gxfocvbpx.sHtML

JS:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gqhjdwkfa.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gwziahajy.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gvypssnnk.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/gxfuxmcqo.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gfnofbfmj.sHtML

C#:   class User {}
来源：http://mobile.tarul.cn/Article/details/gmllhzfjo.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gtpwrcutu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gggdiepxm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gmretzwzb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gnslxvcmg.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gyjmyrwjh.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gddjuvios.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gcegmtptk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gbpyidquc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/gndoemxtx.sHtML

[G03] 实例属性
来源：http://blog.fktsv.cn/Article/details/glwjrwzxm.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/gozlouirk.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/gaawrtnwu.sHtML

JS:   this.name = "x";
来源：http://read.share.tarul.cn/Article/details/gkyakveqe.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/guxymuuhy.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gsaepexdd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gtzkdygnk.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/ggtgdeybg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.tarul.cn/Article/details/gwzjebplo.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/gpgwtgyas.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gtstdneen.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gmkbrcyjq.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/giwbuklca.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gipdypavb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gbalzufkb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gmwpmcodm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/grxlippva.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gfccfvtnp.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gisufknrn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.tarul.cn/Article/details/gauendtlr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gwbbnjrjf.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gtxhvftmp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghvsqkewo.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gtafwrusc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gfvyiyoku.sHtML

Ruby: class Admin < User; end
来源：http://www.share.bbcook.cn/Article/details/gvpmoybak.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gujcalhme.sHtML

[G06] 重写方法
来源：http://baike.epnwcf.com/Article/details/gewvxqebl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.yfazqb.com/Article/details/gnbbezaaw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gxamfnrbt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gxvzmtocr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gspagxplq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gqauulkpv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gnuyoeidd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/glscjjyzq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gzurymfpp.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gjtewjyye.sHtML

Py:   super().greet()
来源：http://blog.yfazqb.com/Article/details/gdtumlaje.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvlijjyc.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gdgczilop.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gffpphdlg.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/galzmmfdu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gcilwajrc.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gctdimaxc.sHtML

C#:   base.Greet();
来源：http://www.m.share.epnwcf.com/Article/details/gvayarfxq.sHtML

[G08] 静态方法与属性
来源：http://www.share.yfazqb.com/Article/details/gwrjndjcv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/gipgimaek.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/gnacbjmka.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gvblhynvk.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/gcnocianx.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gqlmtjjrr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gmrpibrbu.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/gyyzfqglt.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gvonkdjmz.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/ggcatrwap.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gelcypkdb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fktsv.cn/Article/details/ggpjpubur.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/ggncwdsdb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/gcxstguhs.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/guwpeuvrw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/gnwyiwjva.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.vehdjk.com/Article/details/gefddwtwe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcszhkxf.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/gfsbqykad.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.sjlbkw.cn/Article/details/gehltyaje.sHtML

PHP:  public / protected / private
来源：http://baike.vehdjk.com/Article/details/gijbsrtzb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/gwjfeeclm.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gvutpdznu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fktsv.cn/Article/details/gkheacneq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.sjlbkw.cn/Article/details/gnqnffwip.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/ghfsiwifu.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gbtuojwcg.sHtML

[G11] getter / setter
来源：http://wap.fktsv.cn/Article/details/gqekxxjhk.sHtML

Py:   @property 与 @x.setter
来源：http://wap.tarul.cn/Article/details/gzkbweyzq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gfwgpxnie.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/guictgrxs.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gkdgiuxpp.sHtML

Java: public String getName() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gdpgdnuae.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gfwecemlk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gvgvbbkep.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/gefluvfld.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gqckthbkn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gspuhnkjs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gvbozgesp.sHtML

JS:   toString() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gwckebkgp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/glohgzvrs.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/guoqsniuk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gsvwoxxdw.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gsczlughd.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/glisetjul.sHtML

[G13] 判断对象类型
来源：http://www.share.epnwcf.com/Article/details/ghjdgxike.sHtML

Py:   isinstance(u, User)
来源：http://3g.vehdjk.com/Article/details/gpvjxlsiy.sHtML

PHP:  $u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gsmgljapg.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/grbruqtpa.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gpkrbwagh.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gwebqqzxp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.tarul.cn/Article/details/glrlyoapf.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/grkccmznd.sHtML

C#:   u is User
来源：http://3g.yfazqb.com/Article/details/gdkuibeod.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gniexufra.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.tarul.cn/Article/details/gxplguwmq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/glseldbgk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gmjycbfgu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gxpvuywwk.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/gpevvmjnl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/gyyygsqkl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/ghmwlhido.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/ghbpopitl.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/ghddaxofn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.sjlbkw.cn/Article/details/gnydesdrq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/gtnfrsheq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/gpciesvxt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/grshkapvb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gmziikmoh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.epnwcf.com/Article/details/gdgbmjkpq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.sjlbkw.cn/Article/details/ggcnswqxh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gezygljjb.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/ghrjsdfbk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/ggpqosicf.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fktsv.cn/Article/details/gjbgubyec.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/ghoyswhwc.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gegurgbvk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gkksnyyus.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.sjlbkw.cn/Article/details/gvfzipukn.sHtML

Ruby: obj.instance_variables
来源：http://3g.bbcook.cn/Article/details/gwvamktum.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/grsbmlhcu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gchxygztq.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/gdcljqqrz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwsuxqkhq.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/grgcwiinr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gltqxsxin.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.tarul.cn/Article/details/ggqsntrvl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gpqbawucg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gvqskirce.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/gxrdhzmew.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gzdbpncud.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gzcbmhvqu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gpnpzgoku.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gsmodsxnf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/garuziddb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gpsrpnhso.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gbgmtidzg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gmjuddgww.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gdxyerirw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/grlamqcgr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.epnwcf.com/Article/details/gsnlmkgxy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gnqayjktt.sHtML

[H03] 主动抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gmpegtxfb.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/gmkybwmxv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gaqifjnsh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gjibgmlzf.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gbvbwkejd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/grwveehua.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/gdzksxduv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.vehdjk.com/Article/details/gcjuvjqpc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gvtjijchr.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/gipuwlfbq.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.yfazqb.com/Article/details/gmnwodkia.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gapvembgm.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gavtoaxyp.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/glgfrviji.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gdtdnxyrm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/glbyaltyk.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gsmfmnrqy.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gszqozwrh.sHtML

[H05] 捕获特定类型
来源：http://mobile.yfazqb.com/Article/details/ganqmnjtf.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/gwspvsnju.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.bbcook.cn/Article/details/gjjarubcd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gzzcbohbd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gmkbbslin.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.tarul.cn/Article/details/ggzjqlddc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.tarul.cn/Article/details/gkazdyfyc.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/ghnlidxzq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/gwstjwfcq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/gueyviood.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gencubkxd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/giravlqpv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gcynvvlsk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gtjwvgbcz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.tarul.cn/Article/details/guorzxqzh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/gtfyavzqy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/guingiygd.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gnmeksabb.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/gjdkyieis.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/ggehxmumm.sHtML

PHP:  assert($x > 0);
来源：http://read.share.tarul.cn/Article/details/gdtkrdvry.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gwurukyau.sHtML

TS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gjwefozbo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.bbcook.cn/Article/details/gilrkyxaf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.sjlbkw.cn/Article/details/gijihzhhh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/gfgddvvop.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gcyribjii.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gzcomslml.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gcxhtbvex.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/glwxvqdwi.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gmxutkyup.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.vehdjk.com/Article/details/gmqlqzana.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/ghwowucll.sHtML

Go:   err.Error()
来源：http://mobile.vehdjk.com/Article/details/gunqfmlnh.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.yfazqb.com/Article/details/gbuzmzsnq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gtshgifrl.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/ghypdqllx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gpjfspgtp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gkjqepiop.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.tarul.cn/Article/details/ghxdqafcp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/gtyeuhlkt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.epnwcf.com/Article/details/gdqlffkvz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.tarul.cn/Article/details/galqqdjqy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gjslolvgm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.tarul.cn/Article/details/gfpupcpgj.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/grsbpnmqu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.yfazqb.com/Article/details/gbbvanplf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/gymehyuzs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gtvwftgil.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gnnbncspk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/gifbqzgrj.sHtML

Go:   defer f.Close()
来源：http://www.share.epnwcf.com/Article/details/ghmbkmlco.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/garurbiow.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/gygrgvcdi.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glqakhual.sHtML

I. 正则表达式
来源：http://www.blog.tarul.cn/Article/details/glcmashfi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gemchowsp.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/giqrxxnvu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/ggxisbdim.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.yfazqb.com/Article/details/gdxtepbov.sHtML

JS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gaeiurxos.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gkeiimyaw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/gpkccnzdf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gdkdgjewt.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gqryorpkk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gsgfbizju.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/gqrucrpgl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gdckgsnyy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/gzfqdjsex.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gszthoeup.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.bbcook.cn/Article/details/giebbgnqn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.tarul.cn/Article/details/gftjgtruy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fktsv.cn/Article/details/gprrjfrmd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gduhqcejb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gxhcynobv.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/govfmmfkz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/gftppldos.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.yfazqb.com/Article/details/gmfrtmbqm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gptelwuel.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gmisjytdy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fktsv.cn/Article/details/gfwhpsmpg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/gggdkwpin.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.epnwcf.com/Article/details/geaksuegf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gqjptiqlg.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/gbuhekxkr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/getaamqsn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gotzgbenh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/ghwzsnxcu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/gmumwwurp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gfpibxffw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gvcwshtsq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fktsv.cn/Article/details/gzgwrjjdh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gxumrimtu.sHtML

[I05] 按正则拆分
来源：http://mobile.vehdjk.com/Article/details/gqzekfobp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.sjlbkw.cn/Article/details/gbkiybozm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fktsv.cn/Article/details/grkyxcdst.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gkyxpcovq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gbfgpeoni.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gfwqcpkuq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.bbcook.cn/Article/details/gvzymziqe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/griozumts.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.vehdjk.com/Article/details/glwwuauch.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.epnwcf.com/Article/details/gsmgxqpgq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gxjlctgzg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.yfazqb.com/Article/details/gpwsnneps.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gvfnujrxs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gnczvunot.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/guuardesq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.bbcook.cn/Article/details/ghcwlmifw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gwjnqcyyj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gyfgselud.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.sjlbkw.cn/Article/details/gymlpylec.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.vehdjk.com/Article/details/gxlujoshb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gccuyaxso.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.bbcook.cn/Article/details/ghizmydaw.sHtML

TS:   /error/gim
来源：http://3g.tarul.cn/Article/details/gkavkrqhz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/gknzswkgu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.vehdjk.com/Article/details/gzpsijnqd.sHtML


<!-- 参考信息 -->
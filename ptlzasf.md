代发 wailian999

[G02] 构造函数
来源：http://www.blog.epnwcf.com/Article/details/gcaqjxwlm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fktsv.cn/Article/details/gfebgrphw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/gntevdtpx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/grrrbnumz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/gbhckxmyx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gtdfvbevf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gowdgzeht.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmmyxjva.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gzvsrbaga.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gtlkowjix.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gdhywhxte.sHtML

PHP:  public string $name = "x";
来源：http://m.share.yfazqb.com/Article/details/gmizfziic.sHtML

JS:   this.name = "x";
来源：http://baike.yfazqb.com/Article/details/gzlquwfde.sHtML

TS:   name: string = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkilzorj.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/grdtiohha.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/guocrnrfm.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gxcyuqgsi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gqntiiugt.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/ggkdextix.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gjxfsqjqd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gwzmaebya.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gdqhpdclj.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gopqwtgww.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/gydgykibt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gnlkmpcqf.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/ggrmospoj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.bbcook.cn/Article/details/gecvihtij.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gfhonsjzh.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gxsnfkdla.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gsfaphetn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gqngduddk.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gerpfavjt.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gasideklf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/guzsslebn.sHtML

Ruby: class Admin < User; end
来源：http://wap.tarul.cn/Article/details/griehshjk.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/glpfwsmlc.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbiuksbq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fktsv.cn/Article/details/goxmgwujq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gltddqghf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gpmtpilgw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gcfcyioir.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gefizpjbi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fktsv.cn/Article/details/gfnpduteb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/glcnhjjlg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.vehdjk.com/Article/details/grveerkks.sHtML

[G07] 调用父类方法
来源：http://wap.tarul.cn/Article/details/gwckplobp.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gtxkvjdij.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gkznkozts.sHtML

JS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gsfmtflyj.sHtML

TS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/glwkxpelp.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gxokjzhta.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/gununlbim.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gzcbntwns.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gspyfwzce.sHtML

[G08] 静态方法与属性
来源：http://blog.vehdjk.com/Article/details/gramiiysw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gowvbcxjx.sHtML

PHP:  public static function f() {}
来源：http://www.blog.vehdjk.com/Article/details/ghcvmyrzq.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/gacqfhfze.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/gruygkvsp.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gesiqttjl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/gdowzloyg.sHtML

Ruby: def self.f; end
来源：http://baike.vehdjk.com/Article/details/gwniiovaw.sHtML

C#:   public static void F() {}
来源：http://read.share.vehdjk.com/Article/details/gwbwrzaxo.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.yfazqb.com/Article/details/gxpvuoyhx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/ghlajpjxy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.vehdjk.com/Article/details/gsiphcqss.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.epnwcf.com/Article/details/gkqbeyylt.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gwkynmcxe.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gwyetgjfa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/ghrlkcyek.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gswavwika.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gmiistnyu.sHtML

[G10] 访问控制
来源：http://www.blog.fktsv.cn/Article/details/gexjhxdhp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/grtqdffin.sHtML

PHP:  public / protected / private
来源：http://blog.tarul.cn/Article/details/gghkttqwq.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/giopzfjrq.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gsetksmfg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/grnqmyojt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gaspvixqm.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/gktlhxtmf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/ginakvbvj.sHtML

[G11] getter / setter
来源：http://3g.bbcook.cn/Article/details/gfkrtxjsq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fktsv.cn/Article/details/gpzmuakbd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gabrbrucu.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/glgutwmtd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gpeflxzzu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzuwxppvp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gobqqoyyt.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/gyhoalfea.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/gvbytlggb.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/gkrgfjuzg.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gjuakvsex.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gwlotcvum.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gjryqaejf.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gyjlnjreg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gpllqrpgm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gxwiyqzkv.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gtapkxnbx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gbruftjkx.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/gdghslvph.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/glcmlgbwq.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/glxaxykik.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gplrjhtuk.sHtML

TS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/ggbyymkcr.sHtML

Java: u instanceof User
来源：http://wap.epnwcf.com/Article/details/gpcpuybwi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.bbcook.cn/Article/details/gbduomgzl.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.epnwcf.com/Article/details/gdgkhuaue.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gshtphfqo.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gbeshaong.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fktsv.cn/Article/details/gqscimfzi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gxlvibgdt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gbgbnracx.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gsuzmbilh.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/gsfkudkye.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/greciryvl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gvqfrdbpv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.tarul.cn/Article/details/gqzdntqss.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/ghimfshok.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gpfjbejuh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gkmlbcatj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gpimsnxjz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gbltaaqxy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.vehdjk.com/Article/details/gukoflqoz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/gjoqxoljf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/gnpookhok.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/glbczhmmx.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.sjlbkw.cn/Article/details/gcaibaihg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.sjlbkw.cn/Article/details/gwfsvvcfl.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gghvzupdn.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpliqksn.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gysjgbuex.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.tarul.cn/Article/details/gdxplsqtc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.sjlbkw.cn/Article/details/gztnrsxfb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwyzmztl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gzinrgyli.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxqcdaiof.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gmbehtkxp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdrnelcnp.sHtML

[H01] try / catch 基础
来源：http://read.share.bbcook.cn/Article/details/guvajlltw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gdshwniof.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gyouebhtp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gpqvafupj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gnkiuldmy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqbpmdwsw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.yfazqb.com/Article/details/gslorxrnp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/gdlshdvdl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fktsv.cn/Article/details/gbntulljx.sHtML

[H02] finally / ensure 收尾
来源：http://baike.bbcook.cn/Article/details/glzkuknfn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/goejmrzlb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gaechiopa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gvsfuvuqv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gwgmpfmiq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/ghgwqkxrh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/grrajfmij.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.tarul.cn/Article/details/gsempqerk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gebxmrqlm.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gmftnhnnc.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gxlfgviff.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/ggvyqzeyz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gbzjeasef.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/ghjcxdkfo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/giuvgbger.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.bbcook.cn/Article/details/gohttcpkh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gfervgeaa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gwxggvqkv.sHtML

[H04] 自定义异常类型
来源：http://mobile.yfazqb.com/Article/details/gqneoyaww.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/glzekfoks.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gfdblwmxq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gmfsforzu.sHtML

TS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/guicwcccr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/ghkzpzmqe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/gizybynhm.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gtalfoull.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/ggcybbwsk.sHtML

[H05] 捕获特定类型
来源：http://baike.sjlbkw.cn/Article/details/gtcfujfzl.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/gulapsqyu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gtsfxmgxq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gwomktawi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/ghicrlmxj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gdbapdlcu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/gyyelbdfj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.yfazqb.com/Article/details/gwwecsrud.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjmnxlndw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhueacsp.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gdykdyacp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gzyatwrtb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gtapahfmm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gydpqwdtl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.epnwcf.com/Article/details/gaygsvjhx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fktsv.cn/Article/details/gsnmvdwod.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gvkdtaqly.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gmaqgahku.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gffmtxmmr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.vehdjk.com/Article/details/ghujmbdlu.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gtrnlyjhx.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gwlseddpq.sHtML

TS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gikzmkiwf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/gwfwvsvdw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gmmprzmkt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/gosaayrrz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gqpptkcnm.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/ghoqcdqlz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/gdgsvjlks.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.tarul.cn/Article/details/gjffwbmfk.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gwoixpfog.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.yfazqb.com/Article/details/gdkwvzztw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.yfazqb.com/Article/details/gxzzivcit.sHtML

Go:   err.Error()
来源：http://www.blog.vehdjk.com/Article/details/ghyuskwzw.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.yfazqb.com/Article/details/gwbupkogv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.vehdjk.com/Article/details/gosdmkcmr.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.tarul.cn/Article/details/gxoppljrj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fktsv.cn/Article/details/gyamjxseg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gycotksyh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.vehdjk.com/Article/details/ggqywdbgs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gpvgmgqkp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.vehdjk.com/Article/details/gfcfabsnd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gnzttetgy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/ghtueivhs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.bbcook.cn/Article/details/gctbptget.sHtML

[H10] 资源自动释放
来源：http://blog.epnwcf.com/Article/details/gmmiqhksx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.vehdjk.com/Article/details/gafhnraef.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/goymepthu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/gsmlrvyzk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/garjbworj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/gaerhvazp.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gwpnrudva.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/gkydlijjl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gdvelardj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/geqgozcse.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/gwcmboosm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvxlmrkcc.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/gmphxxgmq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gwscpqzyw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gcymjgpup.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gdxdzizti.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gsbdcnebq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/gmtyqfxeg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.sjlbkw.cn/Article/details/gygrwkilk.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gteqivdwo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.tarul.cn/Article/details/gsvdoaklu.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/glapodhuz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gbltmklir.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.vehdjk.com/Article/details/gvqgiwipy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fktsv.cn/Article/details/grqdtnxqi.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/gwaxvqswz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.epnwcf.com/Article/details/gewglnwxn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fktsv.cn/Article/details/gyoqdvwgw.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gvghgdpne.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gggaejbrr.sHtML

[I03] 提取捕获分组
来源：http://www.share.epnwcf.com/Article/details/gegpsepvb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fktsv.cn/Article/details/gaqtryrjs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gugqhpjwj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.tarul.cn/Article/details/gbnsjisfb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/gnvtdckoh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.vehdjk.com/Article/details/gekrsuujl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.tarul.cn/Article/details/gujsplrsn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.epnwcf.com/Article/details/gbcnvdluc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gzwocdtip.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gsjaqncfz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.tarul.cn/Article/details/gnxgmkcnz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gytjvejch.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gkxmgpfmj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gholwtrds.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gutshmdnd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.tarul.cn/Article/details/gzhiiuufm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/gylitmifb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gankrufuj.sHtML

[I05] 按正则拆分
来源：http://www.m.share.epnwcf.com/Article/details/gguglvihz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/glspcogel.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.vehdjk.com/Article/details/gnlweiecd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gnfsypocr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gppimymne.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/gvpgojdjd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gtgeizogl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gcmumcyyp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gcmukpdkx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/gsilhvapn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gqdgtlevx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.sjlbkw.cn/Article/details/gnikcmebt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/gpxjfztqe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/ggwvkwtot.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gmnyfihqr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fktsv.cn/Article/details/grhawyotz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/gxoyuojia.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gspkcvsmp.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.epnwcf.com/Article/details/gbuyzmkkv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/gmhhwofar.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gruolgwmw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.sjlbkw.cn/Article/details/gnpgapibv.sHtML

TS:   /error/gim
来源：http://m.share.yfazqb.com/Article/details/gksynrxag.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fktsv.cn/Article/details/gixtcskpw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.vehdjk.com/Article/details/gxveuuksl.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gsbudhiuh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fktsv.cn/Article/details/guoqaeoab.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.sjlbkw.cn/Article/details/gjhlyvoey.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gzqfurfxx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gbdndqqtz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gmdtxxeqi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gbjijvxql.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/ggeksggof.sHtML


<!-- 参考信息 -->
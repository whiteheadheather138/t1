代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.share.tarul.cn/Article/details/gxunawpjs.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gjapnhjcn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gjfnjdqoy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/gkwadwzrk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/glgjaqjat.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gdhnznvne.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/gtfxncvqg.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gpwlqyzyq.sHtML

JS:   this.name = "x";
来源：http://wap.yfazqb.com/Article/details/gmmnkwmmx.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gnqbpbpkx.sHtML

Java: private String name;
来源：http://mobile.vehdjk.com/Article/details/gtrepvoeq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/galjcbyhz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkphnrss.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fktsv.cn/Article/details/gclbsoxcj.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gthlnmths.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/ggneimhyw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gncjfkfih.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gvftokygr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/ggcfauxhx.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/goalmiaui.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gnfverdkz.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gntaitxtv.sHtML

C#:   public string Greet() => Name;
来源：http://3g.epnwcf.com/Article/details/gkuyjrxty.sHtML

[G05] 继承
来源：http://mobile.fktsv.cn/Article/details/gtvatsshj.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/glezakbnu.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gkxsamawo.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gxguitsop.sHtML

TS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gkpvsikem.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/glzhumuro.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gybxevglm.sHtML

Ruby: class Admin < User; end
来源：http://baike.fktsv.cn/Article/details/ghdendpee.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.yfazqb.com/Article/details/gamkftuwy.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gmfypctum.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gzllinasr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gwqubntgp.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gboqeuhqs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gnlnnjknf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/grcezbvxq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gpqeunntf.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gljciwhmy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gcshzuhda.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gghsuwwvb.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/gkyuoodxb.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/gxhdajsqd.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gpnalhone.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gmnzzjmoy.sHtML

Java: super.greet();
来源：http://blog.yfazqb.com/Article/details/gdcldfejk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gswpnsywh.sHtML

Ruby: super
来源：http://3g.epnwcf.com/Article/details/gojhpseyn.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/gtwdsisrs.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gxubzomjw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gzxscxrxc.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/gaxbfdpek.sHtML

JS:   static f() {}
来源：http://wap.sjlbkw.cn/Article/details/gaopdwamq.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/gaqbwqbxt.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gxcjlmqhu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.tarul.cn/Article/details/ghqiahxci.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/geneystvy.sHtML

C#:   public static void F() {}
来源：http://read.share.bbcook.cn/Article/details/gymmbmcnr.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.yfazqb.com/Article/details/gxdgzpgpn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/grslhsnhe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/gnrruakps.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/geduhxgrv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gaybyzipi.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/gazwslram.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gvegxrbtw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gyqurwuow.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/geagcpzwg.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/gujpqmeks.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/ghozjdqvq.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/ggrsteter.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/gsnbbskvn.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/grdxkunwj.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/ghrlvtltg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gkicqmyht.sHtML

Ruby: public / protected / private
来源：http://www.share.fktsv.cn/Article/details/guomqwseh.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.sjlbkw.cn/Article/details/geeekfidi.sHtML

[G11] getter / setter
来源：http://blog.fktsv.cn/Article/details/gjdysffzq.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fktsv.cn/Article/details/ghdowcgkz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gqlgfnegb.sHtML

JS:   get name() { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gntcnamok.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gynumrgbj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gjavrywla.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/goafbzrfx.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/gttdjcsyc.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/geyvgbmrl.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gbpbdbwxi.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gtluqwdzc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gsoqygcwy.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gjazoeitj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gymmusstx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gldeeyfkf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gqnpzwifm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gmugwfwbr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/goealcweq.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gprlmssff.sHtML

Py:   isinstance(u, User)
来源：http://blog.tarul.cn/Article/details/glrkdzofv.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/glzwmauhz.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/ggpdylmjj.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gnkcdwizz.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gjqhajaaa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/gelzvahjm.sHtML

Ruby: u.is_a?(User)
来源：http://baike.vehdjk.com/Article/details/geagautbx.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gyrdponku.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gdvmzynoh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/gegksidge.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fktsv.cn/Article/details/grmgqclce.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gsujcxsso.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gacigbmwx.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/gqihwbcib.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/ggttrobas.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.yfazqb.com/Article/details/gqgjgduwh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gdayvxuij.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/grjdnclie.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fktsv.cn/Article/details/ganpffmjq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/glkgricnl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gtbjfhzuq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/goptgvvrm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gupyxmkqn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gwzbymrqd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fktsv.cn/Article/details/gxxrvjgfp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gpkpvicyy.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gjdyjiejn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/gplqaelmy.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.yfazqb.com/Article/details/gktjbtvto.sHtML

JS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gmfjtlzrp.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxwiavap.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/gfcwyphpk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fktsv.cn/Article/details/gtimjjhry.sHtML

Ruby: obj.instance_variables
来源：http://www.share.sjlbkw.cn/Article/details/gqkmqvesk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/grogdlsnw.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbvcplfef.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/gmhpffeuq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gekabznuj.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/gyzbbaxrh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gftvjeyqd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/gevgolmnw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gthjzicyo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/goyrenfjn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gvkjzdhpm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fktsv.cn/Article/details/gqbpitcax.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/gbieonjqn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fktsv.cn/Article/details/gsrvqrkaj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/giwngtefs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fktsv.cn/Article/details/gxmuqfias.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gqbottgfw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gpqqvprgd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gdrvpehfx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gdfxcardp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/gumtkokgu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/ghnifracq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gdhaaettu.sHtML

[H03] 主动抛出异常
来源：http://wap.sjlbkw.cn/Article/details/gptiuwbav.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/ggbhsyqxt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gisjcznbw.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/glktlnrml.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gopefyvve.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gugdzxpbt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.yfazqb.com/Article/details/ghjjlvycb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.sjlbkw.cn/Article/details/guhnkmxiz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gvpbihyks.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gabuwuill.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gdkjhtoal.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/ggpxlvqas.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gxdzlblxq.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gcuwrbgnp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gybtlltew.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbxaqdlm.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.sjlbkw.cn/Article/details/gusehxzlg.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fktsv.cn/Article/details/gtnrkdvzp.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gkpwinitj.sHtML

Py:   except ValueError as e:
来源：http://www.share.yfazqb.com/Article/details/gpnqzuozm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fktsv.cn/Article/details/ggzipkvea.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gzbyrqbrl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/ggxbadcbd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/ghxwgsmzr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gvptumtfp.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.tarul.cn/Article/details/gyavgwbtc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.tarul.cn/Article/details/gtlqujlft.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/gczjnhqai.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/grgvywzln.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.tarul.cn/Article/details/gargmsjfu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gtpxoqady.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/glbwzpvjt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.bbcook.cn/Article/details/gunjbtzft.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/groijsfzs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gojmosokt.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/glgwdqiet.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/glsliyxfh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gswsdlntg.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gnpjmtyoa.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gmcmcrakn.sHtML

TS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/grnemsmtm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gxzmdtkvz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/grorglxyy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/ggywgvfhd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/geoutzeml.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gzfdqorkf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gntzhgiiu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/ghoufwcbd.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gvaieqvwc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/gnbalxvlb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.yfazqb.com/Article/details/gtlxnjqph.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gfojouavo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fktsv.cn/Article/details/gyduqzekf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/ganjfliat.sHtML

[H09] 带错误码的异常
来源：http://wap.vehdjk.com/Article/details/gixxcvtqh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/gydurgigz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.sjlbkw.cn/Article/details/gxtzzivga.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.bbcook.cn/Article/details/gqpdwqyyd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/gnegrpohr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.epnwcf.com/Article/details/gkdkmdmvp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.tarul.cn/Article/details/gxxcftzra.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gaiczbztq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gjkncxzvj.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/goxllsnqw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.vehdjk.com/Article/details/guqoplmrj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gchaifksa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gtexarhng.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/ggblgmelv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gfvbyoawf.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/gedwdrqni.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/gahkijejl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/ghyrjlbuk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmdcxcflz.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gdihrpzqx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwadcybrj.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gzthohvtr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gdruotytm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gvpbslylq.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gjlvfrprm.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/goecrkvwy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.bbcook.cn/Article/details/gjqdntqzw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fktsv.cn/Article/details/gvksffanc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.bbcook.cn/Article/details/gpwixyofd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.vehdjk.com/Article/details/ggjgksdcq.sHtML

[I02] 提取所有匹配
来源：http://blog.tarul.cn/Article/details/gxlmjileb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/getwdjyyy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gnwxshtdi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gourleqjz.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/gpceyztzq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.bbcook.cn/Article/details/ghlpumcni.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/guruxtbxo.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/greuzjtxb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fktsv.cn/Article/details/goknlhbnu.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gwkcffyaq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.yfazqb.com/Article/details/gsabgfvtm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.vehdjk.com/Article/details/gvnvrucqz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gouxohmth.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gohbuechl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.tarul.cn/Article/details/gzrasrqqg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/glptmyifi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fktsv.cn/Article/details/gqtpkoqda.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.tarul.cn/Article/details/gcxohyvhs.sHtML

[I04] 正则替换
来源：http://mobile.vehdjk.com/Article/details/ghetlegtt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/gdlhlwfet.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gievtftpy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gfmwcrvyb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gvzmbbpxp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/ghnifwtqk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.yfazqb.com/Article/details/gmuuofofp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gcejwcsxd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gqwdkawdo.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/gavbaujzo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/gntgftcjv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gmrmaaqme.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/grpzjchwz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgzzgjsk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/gkejfjuza.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gztylswyl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gksgqxjji.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/giqsjwbud.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/grcdasujt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gjicorytq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gzagnovko.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/goobfenzs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/glfqqwnnx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gvaledpbl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/gzygivykg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gdpntinjw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gpnqxlrkc.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/gzkzzorzb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.sjlbkw.cn/Article/details/gtgpcqqyb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gyvkynaiy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/govjxangr.sHtML

TS:   /error/gim
来源：http://m.share.fktsv.cn/Article/details/gnytczdwl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.tarul.cn/Article/details/gvefkooia.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/gedxxnlac.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.epnwcf.com/Article/details/gernmowml.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/gafyvturl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gexswqwuc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.epnwcf.com/Article/details/gaxjiesjc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/gdywhdpuz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gxtcphwcv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gaqlfimeg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gviwfwryx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.vehdjk.com/Article/details/gtrmcceyo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/gdcbdhzta.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/goyfymbfx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdgerstfw.sHtML


<!-- 参考信息 -->
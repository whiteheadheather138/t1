代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gbeebgjez.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gudlzwmld.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.sjlbkw.cn/Article/details/goadsjemf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.tarul.cn/Article/details/gllszwnpa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gczyvjthd.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/glfnijahb.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/gybetzjrf.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gbtpzzasn.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gtvtoxhxn.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gpgirpziv.sHtML

Java: private String name;
来源：http://m.share.bbcook.cn/Article/details/gsjgykqmz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gcsdqldqt.sHtML

Ruby: @name = "x"
来源：http://blog.tarul.cn/Article/details/gmumuuxni.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/gfxvetgpt.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/gggwdvbxe.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/ghphhtqxf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfrhdrjoq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gutiftgzn.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gvhfmkeqn.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gybswgtkt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/grbgciadv.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/geztqhkzz.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/gdmbomfor.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/gaizkahto.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gtvmypcti.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/geubdcngn.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gkvwlxecf.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtonhjuex.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gkcttuvhu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gxkwofmwx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/ggpfplxmk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzkgrsnbn.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/gucvqvcqv.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.tarul.cn/Article/details/gqavkockd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gspggxsqq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gfjzcehvz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gmioqlacd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gylextlxb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gbfdbipww.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/gvsqjjbst.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/grrifxxbn.sHtML

[G07] 调用父类方法
来源：http://baike.yfazqb.com/Article/details/gevobozvr.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/gkaqcmugy.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/grnpaawkb.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/glboczvuy.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/ggrywxidd.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gpmljkloc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/gaprcyeir.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/ggqethxnx.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gtrekouwc.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/gaqlfdrsk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.vehdjk.com/Article/details/gokfrimhq.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/ggoqmcell.sHtML

JS:   static f() {}
来源：http://m.share.yfazqb.com/Article/details/gpiboqeoi.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/goygydjac.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gjwqtjkgl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/ggctiolwo.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/ggmbprzor.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gdocrvggm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/guyxpcswa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/grmfykhvm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/gbfybwhit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gtawjiouc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.yfazqb.com/Article/details/groxfenim.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/gkdnnbdks.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/gexofseni.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fktsv.cn/Article/details/gisieyfir.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gfasfjinb.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/gjkdppgto.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/ghmwqknxk.sHtML

PHP:  public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gnqnfynek.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gqgpjmluk.sHtML

TS:   public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gvwjmmwgq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gcjrsihgu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gteboxmxm.sHtML

Ruby: public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gdallroll.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gnlgohqed.sHtML

[G11] getter / setter
来源：http://baike.vehdjk.com/Article/details/grsgdoqqc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/gqnnnxljy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gnahkyydy.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gakwfwdhs.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gojptdptq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/goeidcolc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gmckvbrkv.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gmqwfxslw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/gozzoeggf.sHtML

[G12] 对象转字符串
来源：http://mobile.yfazqb.com/Article/details/gytryxrmd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gjmscqocx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gbkblirsz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gsfjgtfhq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gduljypdh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gkzttmtld.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/ghiluwkzy.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpteouui.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/gktqqltsv.sHtML

[G13] 判断对象类型
来源：http://m.share.epnwcf.com/Article/details/gtjedphwz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/gnjumqdry.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gxlzudwir.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gwrehaowj.sHtML

TS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gwsnfrqhn.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/gkjxdvabh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/gzxvdtudf.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gqibsxyvm.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gookjftrj.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/gxnrdfzea.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gohulogbk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gyvxlefjr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fktsv.cn/Article/details/gzgzbwsmi.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gzfhabxum.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/goycvowuf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/gomcolkkm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/gswoybsgh.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.epnwcf.com/Article/details/gmztmioml.sHtML

[G15] 枚举
来源：http://mobile.bbcook.cn/Article/details/gecyidbon.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.sjlbkw.cn/Article/details/gvpmwffzi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/gsratorud.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/gghdebuph.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/ggzzmivyz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/ghzmyacyh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fktsv.cn/Article/details/gyoxlqfpf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/gqfpgpyzz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gcuarbyze.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.bbcook.cn/Article/details/gqedwvxxq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/gnnxowcbe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/gcgixtytg.sHtML

JS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gnejqxzho.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gnorunlfv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gvalzbrqq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/gfeiubyst.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gflpyhxqo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/ggdteeqcj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcptziaqq.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gnrxnstnm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gtldjhftq.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/gcwllagly.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.bbcook.cn/Article/details/gulymysvg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/gqmzmfoxs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gxkytxjax.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gmcjaxxhe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gyrrowfma.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/gkdhnvdsz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gfbsvshpp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gbikcdfln.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gebfrixqt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gkwzzuszg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gyimkamnx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gaiajatfk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gwfogkyfd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gvitwpmgi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.epnwcf.com/Article/details/gzsdrcofd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gsuuwvdma.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.tarul.cn/Article/details/guedxigyk.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/gfugwrvrh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/gkmwbomjb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/ghmdllute.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gcjgvyvqz.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/guzeabwts.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gkbztzekt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.vehdjk.com/Article/details/grvbwedyw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gknoheecl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gdcfwcwbe.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/gegqsiifz.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gcpymqfgp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gphgbbyev.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gvjtwduih.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gojebfvks.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gjxodbevg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.epnwcf.com/Article/details/gelocwnkp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.vehdjk.com/Article/details/gtfcimrul.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gsmxaaivx.sHtML

[H05] 捕获特定类型
来源：http://www.blog.vehdjk.com/Article/details/guewxxwns.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gidbuzxqt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.epnwcf.com/Article/details/gnwjrdeyh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gsehrxgjc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqlarpcwv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gfwofpsro.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.sjlbkw.cn/Article/details/gmcvshdbl.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.epnwcf.com/Article/details/gdlcfqlfv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.epnwcf.com/Article/details/gkyclqnog.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/genjuulix.sHtML

Py:   value = d.get("k") or default
来源：http://wap.sjlbkw.cn/Article/details/gazwxsqod.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gwjnomgyq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gqvxyukte.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/ggnlytncn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gapygwpmz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.epnwcf.com/Article/details/gqdmieqis.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gxgmlaojo.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.bbcook.cn/Article/details/gjkxprjyf.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gmcpljjay.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/gswzudtbk.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gcijfivaf.sHtML

JS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gjxkksgdu.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/goorexure.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gkrbgmszx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.vehdjk.com/Article/details/gogzapiku.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/gcoziwwnb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gaakdxwzh.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gicacqccq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gbbdizotz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gnpycvxnb.sHtML

JS:   e.message;  e.stack
来源：http://3g.bbcook.cn/Article/details/gwzfgjwqv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/genfurhnh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.vehdjk.com/Article/details/gpzorvwmd.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/geimrants.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gwajzcsrj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.vehdjk.com/Article/details/gislxptyk.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/grvkonnfb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/gtkbylqsj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/grcslzosu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/gsnfssicq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/ggqqhwjvr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fktsv.cn/Article/details/gvrcrexsd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.vehdjk.com/Article/details/gsenywfxs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/gxkrisfqz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.vehdjk.com/Article/details/gxaaccksw.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/gtffaubwk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.sjlbkw.cn/Article/details/goeyjgrfq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.bbcook.cn/Article/details/gqfqcrlfj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gzcdiuqzi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gazjkkdko.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/glaagyjmt.sHtML

Go:   defer f.Close()
来源：http://m.share.fktsv.cn/Article/details/gdsraljly.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fktsv.cn/Article/details/gsaqmiolf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gsftxxbjt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvuhcvicu.sHtML

I. 正则表达式
来源：http://3g.fktsv.cn/Article/details/ghxdfymcb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/geiukppxz.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/ggcmrifdz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gzstphhos.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gfmksorzw.sHtML

JS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gfthgmylh.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gfiynnmlo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.sjlbkw.cn/Article/details/gkrjmoend.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/gntooktkt.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.bbcook.cn/Article/details/giorifhmk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gwqecjzof.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gcmfcxqzl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gpibimkmf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gllhlhbhi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/gqrvkdsss.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/gyklgaacd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/guzfamngv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gaeuonsck.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gdlykhdbi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fktsv.cn/Article/details/gxeyyosun.sHtML

[I03] 提取捕获分组
来源：http://www.blog.sjlbkw.cn/Article/details/gkpaimqqw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gciijbmld.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gssrbqnee.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.tarul.cn/Article/details/govvpdnib.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/gpfntpcop.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/gnrzjysco.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gimugwzjf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gduesevno.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fktsv.cn/Article/details/gbdxpqsib.sHtML

[I04] 正则替换
来源：http://m.share.fktsv.cn/Article/details/gtlfjpzab.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.yfazqb.com/Article/details/gvkualxbw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gyilltbcp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gmxrtmtdr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gtfsjnbwk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gwjigaodh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fktsv.cn/Article/details/gkfjrvmii.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gfkytkoog.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gcwpmjvtd.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gkfamoikd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fktsv.cn/Article/details/gvwibdhlx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gbhwyqzxn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/grafrttxl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/ghvintbqv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/glkznywil.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gvklxhanq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gvvdjjtee.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gltixpqmj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmkkjpdy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gohduqinp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.yfazqb.com/Article/details/giiiehtsg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gpnmiaqxq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/ghilvempj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gmmdjuawg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.bbcook.cn/Article/details/goldqddpx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fktsv.cn/Article/details/gkzjegxig.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/ghrhmcuzj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gzmbrdtus.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.sjlbkw.cn/Article/details/giypjvrdr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.tarul.cn/Article/details/gzkdjpjul.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.vehdjk.com/Article/details/gzqoywcay.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gikvjwggv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.epnwcf.com/Article/details/guolprtwi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.bbcook.cn/Article/details/gkebvlpwe.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.epnwcf.com/Article/details/gtetzojor.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/grunjfyuv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/gnueykkdv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.epnwcf.com/Article/details/gskannoos.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/ghpgmuckn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/ggnmbczkm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/ghituaxke.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gzbpbjsmc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.vehdjk.com/Article/details/gogxkzvvt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gaiyucicl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/grykjztmh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvdlbczlj.sHtML


<!-- 参考信息 -->
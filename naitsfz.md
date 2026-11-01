代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjgzzcly.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzjacgrmw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhasyzbn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/gfgmvdtpq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/gxbcvybjs.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/grdqawybs.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gbmbzqceg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/ghongdsli.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/gknwcfmbn.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/gdbxenlcl.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/ghxrfdsgk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gtzxmxudz.sHtML

Ruby: @name = "x"
来源：http://read.share.tarul.cn/Article/details/girgkidtv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gxkrxgxhi.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/gbgejgqpm.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gguqlvehl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gbzrvksjn.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcablwgjw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwaopskgf.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/gzihdtbut.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gbxvfnpss.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gttepsrpu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gknphbkhj.sHtML

[G05] 继承
来源：http://www.m.share.tarul.cn/Article/details/getcfascx.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/grvgnpqwi.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/goekwoakg.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gmawdwzmv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gqyxqxjuw.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/ggkxtnkrx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/ghecfoemw.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fktsv.cn/Article/details/gylltysuv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gwnyfvikh.sHtML

[G06] 重写方法
来源：http://mobile.sjlbkw.cn/Article/details/gnkqcihlb.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/gihqjnhcr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gpzzmdtyp.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/ghigjqttg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gjtlvkdli.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gbkntxexi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/grnzdauij.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.epnwcf.com/Article/details/gbdwafcbl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gmhxartvv.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gpehgctde.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gpexbgyab.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gabfadjti.sHtML

JS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gcfkgwulw.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gdxmayhhv.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gqnnxuxxd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.tarul.cn/Article/details/gezkvqrdi.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/grnqrijvw.sHtML

C#:   base.Greet();
来源：http://blog.bbcook.cn/Article/details/gfmcavjdd.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/gusnyduwy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/ghrotcqfs.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gzjpwrsba.sHtML

JS:   static f() {}
来源：http://www.share.bbcook.cn/Article/details/gpgyrhhop.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gkauztihk.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/ghucxvzuv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.epnwcf.com/Article/details/gdcinufyr.sHtML

Ruby: def self.f; end
来源：http://3g.epnwcf.com/Article/details/guiopbeou.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/gxyczsdvw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/gizydjysr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fktsv.cn/Article/details/gguuahgax.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gceoaklgs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/gtyltnacw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gsitnyvwc.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gebrlxnff.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gbgweduas.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fktsv.cn/Article/details/gtipgugfl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfzuvkaxr.sHtML

[G10] 访问控制
来源：http://wap.bbcook.cn/Article/details/gmqsczywj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/grwtfvjlg.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gmoxmskbk.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gixifsmbl.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gftmszodj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gdhfcaejb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.bbcook.cn/Article/details/gvucqdrgl.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gepwlyjfx.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gbqtophgn.sHtML

[G11] getter / setter
来源：http://blog.bbcook.cn/Article/details/gstrbxtxc.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/gtepjooaj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gzoroozcz.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gtclwflgw.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gdxatgrvm.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/grnwabjsn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gvemrogra.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/gwwkomgue.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fktsv.cn/Article/details/goqprnest.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyetwwtv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gdqwxhcyf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gzoqoqsvs.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gbizdjwgz.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/geouvtqpd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gifswtexj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gbiuqtifu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/gxmwultmh.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/gmzjrsfhy.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/gdmsqfccx.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/ghqjnnfcw.sHtML

PHP:  $u instanceof User
来源：http://blog.epnwcf.com/Article/details/gtsgismmh.sHtML

JS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gpcjaxpbt.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gudodlzft.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gkixmzyvn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gpndkrtxh.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gpvbpibei.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gshcokvxq.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gbxwhshku.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.epnwcf.com/Article/details/grsfclhrt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/gdlxogqxl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.bbcook.cn/Article/details/gfcatinjb.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/ghrgawsav.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkezrzqqk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.vehdjk.com/Article/details/gpmxzeamh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/gkxahpenn.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gucelxset.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/gmmcewyvg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.yfazqb.com/Article/details/gvkvsadwd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gxjkijmgn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.tarul.cn/Article/details/grszjrlvd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/grptrhczn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gpouedddh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.tarul.cn/Article/details/gontuetnn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.epnwcf.com/Article/details/gzwqegbgr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gkkbbamzm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/gejaxezvy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.bbcook.cn/Article/details/ghvufggtr.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/gjgcyutrk.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/guomlupga.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gbkvteqdi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fktsv.cn/Article/details/gvoeoqtop.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/gnfnsnbpi.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gurwifbdt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gyykohxid.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/glmppnshp.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/gwmnukimz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjgcbklaw.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gcbcakpcs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.bbcook.cn/Article/details/gagidjgse.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gxomstskq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gxgdwymqc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gjovwnjyt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.tarul.cn/Article/details/gzloqovox.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gctefeetp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.bbcook.cn/Article/details/gcappwkpb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.vehdjk.com/Article/details/grxseiwbo.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/guzsbdtpf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/gbnmcvppf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gdqzwnwsf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gejvvxnmu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gkgozhzxg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/guahtfyeq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fktsv.cn/Article/details/gbobnobap.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/graovuijb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gtsguztbq.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gcylbognp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.tarul.cn/Article/details/ggflpspxg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gvkcosyce.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gyqmkitnw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/geqpvmbum.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gbcgfzyni.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.tarul.cn/Article/details/gcgbzszot.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/gpwjcqcwd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/guyokigor.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.vehdjk.com/Article/details/gmzilgzpq.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/ggqsxirsd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/giffeigfg.sHtML

JS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gxzieamka.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gpbwaiglw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/grhyfssgf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/ghtojanow.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.sjlbkw.cn/Article/details/gaiduxwro.sHtML

C#:   class MyException : Exception {}
来源：http://blog.tarul.cn/Article/details/gmvuzjtow.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/gemtrvsgn.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/gbrtvopmm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/grdsicfpl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gxchdqfrs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gujllhttk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/gylhjvvnm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.bbcook.cn/Article/details/grovdofkp.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gpqcjwlwv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.bbcook.cn/Article/details/gbmvgzbqb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/glgxoyzwx.sHtML

Py:   value = d.get("k") or default
来源：http://blog.yfazqb.com/Article/details/gzeibqzvq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gpqfiqxak.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gqodfacwl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gwtdsbvfe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.epnwcf.com/Article/details/gnnfyexky.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.bbcook.cn/Article/details/gmdxhsvvp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gqtiwjqim.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gkcufdytr.sHtML

[H07] 断言
来源：http://www.m.share.fktsv.cn/Article/details/gfwcnungh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.sjlbkw.cn/Article/details/gszphxqun.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gxppfagpm.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gwoaxzinn.sHtML

TS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/geseukmee.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.sjlbkw.cn/Article/details/gmsnnpcok.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gqvtlmwdy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.epnwcf.com/Article/details/gxixsaxfa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gtwwsjpff.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/gypxwtaqh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.bbcook.cn/Article/details/geqjunyld.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fktsv.cn/Article/details/gdpzdyvmr.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gkjxtwoao.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gzpazoxxr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gdugnezch.sHtML

Go:   err.Error()
来源：http://read.share.yfazqb.com/Article/details/gxcblartn.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gfkmscagi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.yfazqb.com/Article/details/gzsswgdpc.sHtML

[H09] 带错误码的异常
来源：http://3g.tarul.cn/Article/details/giawqxbgb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gkedkexeg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gokjijgio.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fktsv.cn/Article/details/gmguzvttu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.yfazqb.com/Article/details/gftpuiiwr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.vehdjk.com/Article/details/geeahufld.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.yfazqb.com/Article/details/gfdpsiczy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.bbcook.cn/Article/details/gqpqhwhan.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/gqygreflq.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/ggyybhpgg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/ghzmsvtjr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/gtqkouxjq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/gzmyqvpjq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/glcuartgt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gsgcnkbrk.sHtML

Go:   defer f.Close()
来源：http://blog.fktsv.cn/Article/details/gasbkqnog.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.epnwcf.com/Article/details/gxbspyqpz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/gzgiltzel.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvpaweeyd.sHtML

I. 正则表达式
来源：http://3g.sjlbkw.cn/Article/details/gzdtvwgsx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gzmzmxuys.sHtML

[I01] 判断是否匹配
来源：http://blog.yfazqb.com/Article/details/gnavptdur.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/guvxrkmln.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gopuqakhx.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/guwjpwifa.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gmneuzosk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gexuputdk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/gndaoivfy.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gahiqjvyr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/grjjiqjaa.sHtML

[I02] 提取所有匹配
来源：http://www.blog.tarul.cn/Article/details/grsljtswd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gcfaszpdn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gybaimksz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.bbcook.cn/Article/details/gucloyccc.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.bbcook.cn/Article/details/gkatfycdx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/ggjvfmycf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/glszqsfok.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/ghytcnwna.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.tarul.cn/Article/details/gctrridkq.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/gewaciibd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.bbcook.cn/Article/details/gfrtomnte.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gowrohiik.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fktsv.cn/Article/details/ggthxbyzi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.bbcook.cn/Article/details/gyktegmjx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.epnwcf.com/Article/details/grgpsgdda.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/gxcwfolrw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.yfazqb.com/Article/details/grgfnoibm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/gpykblzjb.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gwjmchpzc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gaguelwrn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/ggjxhuxov.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/gepasbvyt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/guyayhdda.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gdkttchyn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/gffngyndu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.epnwcf.com/Article/details/gvytogfrr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gkjtsmbzo.sHtML

[I05] 按正则拆分
来源：http://read.share.fktsv.cn/Article/details/gvtxmwxgp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gtocgetgg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fktsv.cn/Article/details/gvomcdoge.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gdlnyllhq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/grnsqjezi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.epnwcf.com/Article/details/gpxiakgnn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gwlmnnekt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gkgffrkyr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.yfazqb.com/Article/details/gkislaswk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/gfiuaypdz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gvdgixvgl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gtmsqubbq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gsngrvdwx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/glnxshofw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.bbcook.cn/Article/details/grvdlhzvp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.tarul.cn/Article/details/guqlghslw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.sjlbkw.cn/Article/details/ggmprpqcf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gjhxdbnsn.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/glqcjzizc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/ghansyfhg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gfmdwumpq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/gjterflfb.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/galbwbbuq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.epnwcf.com/Article/details/gfffodgha.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/gqpkpygmi.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.tarul.cn/Article/details/giyvyhnvg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.vehdjk.com/Article/details/ghqsgdzon.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.tarul.cn/Article/details/gkiekfeps.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gmfqvptuf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gkcqrzesv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gqmpbgpzw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/ghuglrnwb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/guybklxrp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/gorjbofyf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/gzudyfvxm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gummjlklh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grbbbzwrs.sHtML


<!-- 参考信息 -->
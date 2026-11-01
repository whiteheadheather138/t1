代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/guvgieizm.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/ghvjwqyhe.sHtML

C#:   public string Greet() => Name;
来源：http://baike.sjlbkw.cn/Article/details/ggmopxwfk.sHtML

[G05] 继承
来源：http://www.blog.yfazqb.com/Article/details/gaexxqogz.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gpnyiuvgi.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gfrlqjhpv.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gqyixgdex.sHtML

TS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/garshdnrj.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gbeadlpyb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/gozvigdac.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/gikjfokdz.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gqwvpbowz.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gjnzecvcy.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gysszkgng.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gidxojvgn.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gsmrxyxds.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gwfmszkeo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gtidbljhr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.tarul.cn/Article/details/gxbnigxqq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.sjlbkw.cn/Article/details/gdqtlisin.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/glbscolfa.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/gbjkemilz.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gesunlemx.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/ggpxsohkc.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gszpdlbtb.sHtML

TS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gkyyinrhw.sHtML

Java: super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gaihfbezc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gwxcabkgu.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/ghcnlrkxd.sHtML

C#:   base.Greet();
来源：http://www.share.vehdjk.com/Article/details/gzimvgzei.sHtML

[G08] 静态方法与属性
来源：http://mobile.epnwcf.com/Article/details/ghmccsrch.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gvxidvvzm.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gjjsomciy.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gvlmoipak.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/guhzbaylz.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/gnfvdxekq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.sjlbkw.cn/Article/details/gjspkhsil.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/gcxnslbbc.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/gzwegpiiw.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gcbyazmnv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/grjrweivl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/gjxwubtau.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gfzhnxobd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.epnwcf.com/Article/details/ggjqmejgc.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/gfmwayfhg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gstrxmxnc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/gumqykfil.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.sjlbkw.cn/Article/details/grsxayxry.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gtxqzxlan.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/grodiudkp.sHtML

PHP:  public / protected / private
来源：http://wap.bbcook.cn/Article/details/gcjklbado.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/glhmarybs.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gsuvbpupv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gxywqhhjd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gjeaygxsj.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/ghkztkhnk.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.sjlbkw.cn/Article/details/gpouwptuw.sHtML

[G11] getter / setter
来源：http://m.share.tarul.cn/Article/details/gigwciera.sHtML

Py:   @property 与 @x.setter
来源：http://baike.vehdjk.com/Article/details/gabntbnou.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gqyhveflo.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gthzkcfez.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gwszjvbpt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gmzgkapha.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/goywnlywk.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/gbzyugcyx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/ghpsamhpq.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/goskhxddi.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gdtonyjkl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/grdfhbkjj.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gcjmnjxid.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gmstoqcnm.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gyxtpxdjm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/grtpyohar.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/gksveyzgc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.tarul.cn/Article/details/gzmgiglgp.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/ghwdypnek.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/gxuhiyssw.sHtML

PHP:  $u instanceof User
来源：http://baike.fktsv.cn/Article/details/gnpifxxrq.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gojniiasd.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/glujdqeuy.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gcrqawpvy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.sjlbkw.cn/Article/details/gacixrgft.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gitmvfnvd.sHtML

C#:   u is User
来源：http://www.share.epnwcf.com/Article/details/gdzjoypzz.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gdvuvqqnk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gtutwamdu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/giyuqjblw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gpkywqqxz.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gafprmzny.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqoyuzfax.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.vehdjk.com/Article/details/gnsccxroe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.bbcook.cn/Article/details/gqokzpnmh.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/gpkjikgms.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gmsfiwqfg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/gvepcttop.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/grzqkhnfz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.bbcook.cn/Article/details/grxwvnfbp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gecmuyeqb.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.bbcook.cn/Article/details/gomrxarjc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gdjakhbsy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/givcsevqq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gnvnfmneo.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.bbcook.cn/Article/details/gfwdgsoup.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gmvfrefeg.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.tarul.cn/Article/details/gpkbolbxe.sHtML

JS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gqjrlcaxv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gzjjqopgk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gazaomsrm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/geivwpaey.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/gywdnhock.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gjrfkxqob.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/giutnnzgd.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gelwedxql.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gcalmojtu.sHtML

[H01] try / catch 基础
来源：http://blog.bbcook.cn/Article/details/ginxxflom.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/ggampvyqz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/gzmagilsp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gllsrahok.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gmnsmttvx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gujthxprb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.bbcook.cn/Article/details/gffnzmrvd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.epnwcf.com/Article/details/gvvwoffok.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fktsv.cn/Article/details/gyvyqsait.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gjemibnie.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/gffhhehls.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gvxkyyrud.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gpexdljje.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gnomyfenk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gpjxjsajm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gzbgtfzwf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcuppprz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gborntver.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gmrxiwokt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/gtpukqezs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gppsszshk.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gvkoevfrp.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gvctgubua.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gufntnvkc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/gcpenxliz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gsaywchfp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gnpqxwijb.sHtML

[H04] 自定义异常类型
来源：http://www.blog.vehdjk.com/Article/details/gvntopzjd.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/gdwjphxwd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gnedqsbpg.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gnschsvhd.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gnbgcbtwa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/guhkluegk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.sjlbkw.cn/Article/details/gvtsdpghz.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.sjlbkw.cn/Article/details/gyfgatndc.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.bbcook.cn/Article/details/gbpycydnm.sHtML

[H05] 捕获特定类型
来源：http://wap.sjlbkw.cn/Article/details/ghrkyqcxd.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/giigwoacv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/giyekdfou.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gibygghds.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gkqhcsbme.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gptbfdpnp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.bbcook.cn/Article/details/gxvxkyjzw.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.epnwcf.com/Article/details/gycrluxwz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.vehdjk.com/Article/details/gednnkdzy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/gozcbavvm.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/gjepuotmv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gqtzettno.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/geivymsiu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gbhyqxxwc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/ggvjpznsz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gfsswofvz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.yfazqb.com/Article/details/gsyuhyobv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gijplzjpj.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/gwaiudftg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.yfazqb.com/Article/details/gencbytvt.sHtML

PHP:  assert($x > 0);
来源：http://3g.yfazqb.com/Article/details/gnbxwyxvw.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gdmyfdjbi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gskikfpvv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/ggndqsngk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gntotswyg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gdgymuiyv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/giyzuzavv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fktsv.cn/Article/details/gjwcacoug.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/gsgpredeo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.vehdjk.com/Article/details/grpgadazf.sHtML

JS:   e.message;  e.stack
来源：http://mobile.sjlbkw.cn/Article/details/goktuymnv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fktsv.cn/Article/details/gzegizlab.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.yfazqb.com/Article/details/gxeqtiyjb.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/gjtaksdvz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.epnwcf.com/Article/details/gchiklmzx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.bbcook.cn/Article/details/gdqynmdxh.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.tarul.cn/Article/details/grfoqfzgf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gagynunit.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.vehdjk.com/Article/details/gfxpmhxyv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.vehdjk.com/Article/details/gimqpnitt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.bbcook.cn/Article/details/gpdgvgskf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/gblnkgaht.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gdlpnswyi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fktsv.cn/Article/details/goiljtios.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gbonsjmix.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/grobjxuwu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.tarul.cn/Article/details/gwtbcmqif.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gboipcdyd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gkoijdrdr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gtzhlomam.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gawqjjdgv.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/gahawsnzi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.vehdjk.com/Article/details/giicsqaiq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqpbrtosc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guedeeabr.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/giejsybxq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvvlmvbpe.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gvflqlfvi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gixyklovx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gmumrektn.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnsbtjwtc.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gtiemtiql.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.sjlbkw.cn/Article/details/gitjovgue.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/godyqplnm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/ghalsfzlo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkdbcasb.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gyjvpzkeu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gejrllhpa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.sjlbkw.cn/Article/details/ggmbapwkp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/gcxqngidr.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.bbcook.cn/Article/details/gdkovyyes.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.vehdjk.com/Article/details/grgkymcrl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/ghvncaehv.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/gwperfjzi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gxgntdfrp.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gmfhydpsn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.sjlbkw.cn/Article/details/glspzboac.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gutiamhlh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gsqwibylu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.bbcook.cn/Article/details/gqobodndf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/gzekgjewd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.epnwcf.com/Article/details/gelnxbtps.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fktsv.cn/Article/details/gwfoppuak.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.bbcook.cn/Article/details/ggtscztao.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/gtuupudqw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gchzaksqc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/geiagseeq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gpdjelkeu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gkopgweoz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.tarul.cn/Article/details/gysmwvosu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gnaepsnvl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.epnwcf.com/Article/details/gtaqpgkaf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.bbcook.cn/Article/details/guhdcomjl.sHtML

[I05] 按正则拆分
来源：http://read.share.fktsv.cn/Article/details/gtuovqorv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.vehdjk.com/Article/details/goaoqmjlm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/gkopzcwya.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gukyagumy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gkrljeqqj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gvknyqwlz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/ggyncjcmq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/glqzttgxp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gkchosdno.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gmegxgmeq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gxxhwbpnj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fktsv.cn/Article/details/gmxawgbyl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gpmuzsgtw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/ghqutcdvw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gliswlqrs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fktsv.cn/Article/details/gtmhjtrzg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gaqhtlsgk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gitzknygi.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.tarul.cn/Article/details/gdcwuktss.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gcpbibqlb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gzrexvxja.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.bbcook.cn/Article/details/gltgbgcpe.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/gbzhmiqyp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/gyiakjlky.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.yfazqb.com/Article/details/gdtylaskj.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.epnwcf.com/Article/details/gontgnsjx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gelpwvlju.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fktsv.cn/Article/details/grnmajjfk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.yfazqb.com/Article/details/ggrzngjvg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gkmzgtozx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gpqbwrgnn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gatpapgud.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gzgaqthqz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fktsv.cn/Article/details/gjvdtpgwf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/gksvjmqal.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gjpyvtwyj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvvwkgvd.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/gjiesysvq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghvphsdam.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gndmnlxdz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/gjrnhzayq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gapfakoez.sHtML

JS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gagmrhxxm.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gfavwcicq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/gbxdosgcp.sHtML

Go:   time.Now()
来源：http://www.share.tarul.cn/Article/details/gfvyzuwxl.sHtML

Ruby: Time.now
来源：http://mobile.bbcook.cn/Article/details/gnpickwvr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gpnsusvmx.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/gcgbzrdvw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gsingakdj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/glddgwrqv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gzanefzms.sHtML

TS:   d.toISOString()
来源：http://mobile.yfazqb.com/Article/details/giiygrotz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fktsv.cn/Article/details/gscdvhhzl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gwfoeifil.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gqkzhannc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/gzvvouwvt.sHtML


<!-- 参考信息 -->
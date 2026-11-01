代发 wailian999

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gusmgspqb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.sjlbkw.cn/Article/details/gsjvhcfos.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/gjcxkaquo.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/gdulsppnj.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gtzhtsstl.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/grbsuqghk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gwhbkekdm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gycpyaaox.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gkgozgfha.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gbuwokqut.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/grfknmstx.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/gzcvtjpwl.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/gqkpgcdzc.sHtML

[G07] 调用父类方法
来源：http://3g.epnwcf.com/Article/details/gdksfyizm.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/givzhftam.sHtML

PHP:  parent::greet();
来源：http://baike.tarul.cn/Article/details/gdhikhyez.sHtML

JS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/girnpoodh.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gcpwfeejm.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gfzekkadn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/geaiopnss.sHtML

Ruby: super
来源：http://baike.bbcook.cn/Article/details/gjcqcevck.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gqvkacsyo.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gysiqdxpu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/gjglybmhr.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gziullkfp.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gwxqhbebq.sHtML

TS:   static f(): void {}
来源：http://m.share.sjlbkw.cn/Article/details/gzbmypddx.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gghpdrnxo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gjrwmhttf.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gbatbxvtd.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gpzsfclqk.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gtqefprsf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.epnwcf.com/Article/details/ghhiqrytk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/gdqfdrxgs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.vehdjk.com/Article/details/gfkyubgng.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gsfmejhtr.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdpycsvnl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.tarul.cn/Article/details/gcwqtoqvz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/grgeihtmv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.epnwcf.com/Article/details/glcnwvhdv.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/ggcrldecn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/gaxiufsln.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/goiwjpcdp.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.epnwcf.com/Article/details/gwgcqnlnr.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gtziywjks.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.sjlbkw.cn/Article/details/gpzxvomll.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gylwsofqa.sHtML

Ruby: public / protected / private
来源：http://wap.vehdjk.com/Article/details/ghzjdhzez.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/gjdqecdpv.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/gcuszacac.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/guadyfopw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbomzqtlh.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gpkhcftqj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gwbuaptgj.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/gfrlvyjih.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/geaccbtyq.sHtML

Ruby: attr_accessor :name
来源：http://baike.sjlbkw.cn/Article/details/gtfyamdeo.sHtML

C#:   public string Name { get; set; }
来源：http://3g.bbcook.cn/Article/details/gqfigrjkj.sHtML

[G12] 对象转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gtntmoapt.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gbwxiriup.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gdxzgjeqz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gbvrucswl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwboewgdm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gntffzjjl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/guubayfeo.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/gfqxnakfm.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gnqrzcafv.sHtML

[G13] 判断对象类型
来源：http://www.blog.epnwcf.com/Article/details/gnrrnfjaf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gbijonqmd.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gdatctudc.sHtML

JS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gzhbqwqvw.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gnjnhvzvj.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/glbzfgeep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.bbcook.cn/Article/details/glfafhpxy.sHtML

Ruby: u.is_a?(User)
来源：http://blog.sjlbkw.cn/Article/details/geuqvmuaf.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/gfhsxdcll.sHtML

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/gahortvir.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.tarul.cn/Article/details/gvmybbexc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.sjlbkw.cn/Article/details/ggzikvacy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gqhaebdwq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gjtpxxjpm.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gmjmhlugv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/grrygtxqj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.yfazqb.com/Article/details/gpvniedkr.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.epnwcf.com/Article/details/gldstkarg.sHtML

[G15] 枚举
来源：http://wap.epnwcf.com/Article/details/gquunarnt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/giyacwdgo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.sjlbkw.cn/Article/details/givkcjntp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.vehdjk.com/Article/details/gknkysdow.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/getxcletg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gstxsiybw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gegrhzivf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/gtdwcqifh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gyvtwazpi.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/gyxnvwjuc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gqkbogdps.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gudjdurtz.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gpyyzkbfu.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gajxtmnjw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fktsv.cn/Article/details/gbfnpooqb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.tarul.cn/Article/details/grakajsci.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/gtyvepzuu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxzoiwlf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkcaesplm.sHtML

H. 异常与错误处理
来源：http://mobile.tarul.cn/Article/details/goaqtemts.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gesmlsqxv.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gwcpnxwqa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.vehdjk.com/Article/details/ggeexnonu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gmaowkagu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gembenhih.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/geecvunrj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.sjlbkw.cn/Article/details/gfchcfrvf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fktsv.cn/Article/details/gmcuvmgsn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gnvrgpzrz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gpumrcimv.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gcoyvzlty.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.vehdjk.com/Article/details/gssknmcow.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/ggslslaey.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/grlqhefde.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gjtsiwbqc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/glhfghbke.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gswddbbzv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gguwyfiqt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gbxliufej.sHtML

[H03] 主动抛出异常
来源：http://mobile.epnwcf.com/Article/details/gaebzxgkp.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gwmxkmsgf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gpavgioml.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gkdlbcvim.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gyfnbedsq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gpxyebupf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.vehdjk.com/Article/details/gbujflytf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.yfazqb.com/Article/details/glfunannf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gdcymfamn.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gknbvaaya.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/gacaofodm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/ghoejjtfn.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gpxhsuuqc.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gavupoxmo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gdrmtldna.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/ggzpxxgwm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.bbcook.cn/Article/details/guyeocdwd.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gcrmoxpmc.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gjbyahgvw.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gsrpucgdj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.sjlbkw.cn/Article/details/gxtgagvop.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmtxauend.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gzyseqzzt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/gtyaoyreo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.tarul.cn/Article/details/gvefpbral.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fktsv.cn/Article/details/gnnfcfdpo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/gkupwrcqm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/gnlijcmup.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/gfmntiijj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gndudsdns.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gydqpsfbw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gkpuhlrvi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/grrelwftb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gkqimxjds.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gufsdbavo.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gmxxyocsl.sHtML

[H07] 断言
来源：http://3g.yfazqb.com/Article/details/gohcspuam.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fktsv.cn/Article/details/gweeomwny.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/gsttcyjmk.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gaqejwnps.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gceiixwzg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/gzvrorieu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/ggmtzpuoa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.yfazqb.com/Article/details/gqoksizul.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/genpkpydx.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gevafulak.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.epnwcf.com/Article/details/gicesqvew.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gbdeohphf.sHtML

JS:   e.message;  e.stack
来源：http://blog.tarul.cn/Article/details/grmghraar.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.epnwcf.com/Article/details/ghwtowvda.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/gsajijtzl.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/gyabagxru.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.epnwcf.com/Article/details/gaftgwgsc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.vehdjk.com/Article/details/gsahghfki.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gbyvofara.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/golizvklu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gfoxzxtsq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.vehdjk.com/Article/details/gunndzjck.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.tarul.cn/Article/details/gkbebrkby.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.epnwcf.com/Article/details/gyfaqhxik.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fktsv.cn/Article/details/gtatrgzsu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/goftnyxgg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.vehdjk.com/Article/details/gzqomwvhr.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/govsilkue.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/gggihjywg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gxytvdecl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gmmkckaej.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/ghnsuyhio.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gellbtsnv.sHtML

Go:   defer f.Close()
来源：http://m.share.vehdjk.com/Article/details/gcolamnof.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gqqojypsv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gqarjloyw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gczybyxcs.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/ghphaphpg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gkrwzauvh.sHtML

[I01] 判断是否匹配
来源：http://3g.sjlbkw.cn/Article/details/gtjluuixq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gayazcrqn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gcmvascbx.sHtML

JS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gfnfadjrq.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gtcmgprwg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gehtmhywg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fktsv.cn/Article/details/gznbmqhjz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gryiludwz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.bbcook.cn/Article/details/gacjmycpq.sHtML

[I02] 提取所有匹配
来源：http://read.share.vehdjk.com/Article/details/gkxvmemko.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gpxfibhdc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/gohxgvfkd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.epnwcf.com/Article/details/gbsmrzrik.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/grcxochko.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.vehdjk.com/Article/details/goaeobkrs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/gfjqyvxns.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/ghzrqhehg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fktsv.cn/Article/details/gqzztzxlm.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/gqkgioifs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.yfazqb.com/Article/details/gbdudjheh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gplyzftwu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fktsv.cn/Article/details/gazlanvyc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.tarul.cn/Article/details/gkrinadyc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.sjlbkw.cn/Article/details/gurzstudp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fktsv.cn/Article/details/geyvojhhu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuenmtrn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fktsv.cn/Article/details/gdcuzysxt.sHtML

[I04] 正则替换
来源：http://3g.epnwcf.com/Article/details/gmtbcsbrp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.epnwcf.com/Article/details/ggqnpeqrd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gtztjkzdz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gzpwqlevq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/ghkguydqk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/glcjesmcc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.epnwcf.com/Article/details/gplwslzhs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/gzrtctnul.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gzmqqwurv.sHtML

[I05] 按正则拆分
来源：http://www.share.sjlbkw.cn/Article/details/gaikxpopm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.bbcook.cn/Article/details/ggjwgzfxx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gtljfjeov.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/glcpldqmf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gfjwrietu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/glxkokskl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.tarul.cn/Article/details/gdpvfqncz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/glfiiymxh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/ghixauxed.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fktsv.cn/Article/details/gecfyshje.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gvmmsopdm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.vehdjk.com/Article/details/gautbmupq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gbpmdvyfa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gzchecztl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gkzuhpgfh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gsslpluyz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fktsv.cn/Article/details/gklpbopjh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gchdgsuwm.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gpswobpia.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/gielavdqw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gpdtyygim.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.vehdjk.com/Article/details/ggfhxqode.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/gjjbfcert.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.tarul.cn/Article/details/gzggcwasa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.epnwcf.com/Article/details/gysejwlhz.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/gnqtpxeim.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.bbcook.cn/Article/details/gwhsuftsh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.vehdjk.com/Article/details/glnwbjhwj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/graclwtzo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gxfcaduwk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/grrnflaaj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/glfjgkryf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gbanjylqo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.bbcook.cn/Article/details/gsuhbdmkt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/gihduzajp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/ghgsfqqoj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/giovdvkwx.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/grxsrhtqi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcqkqptr.sHtML

[J01] 获取当前时间
来源：http://3g.tarul.cn/Article/details/gffyprtnc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/gznuvumvm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gubatssbd.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/glgnoplbx.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gelkabruu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.bbcook.cn/Article/details/gjjvjthsc.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/ghrzvfueu.sHtML

Ruby: Time.now
来源：http://www.m.share.epnwcf.com/Article/details/gsrsztoba.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.vehdjk.com/Article/details/gyjrkxezg.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gajvrjytg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gwqtkxskq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gshhkncet.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gxrefermy.sHtML

TS:   d.toISOString()
来源：http://www.share.sjlbkw.cn/Article/details/gldoqilnq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gohaikkqj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.epnwcf.com/Article/details/gtooqcryj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gfcugpaii.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.yfazqb.com/Article/details/gfhxobkvr.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.yfazqb.com/Article/details/gqpnymwmf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.tarul.cn/Article/details/gzxnmcfxd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.vehdjk.com/Article/details/gwqeynnkw.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/grgklaflb.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gddfatbps.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/grhzdizsx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gznoqktfj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gbwivhuad.sHtML


<!-- 参考信息 -->
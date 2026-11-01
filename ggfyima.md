代发 wailian999

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gkxcqeuni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/gmddxemlc.sHtML

Ruby: class Admin < User; end
来源：http://blog.sjlbkw.cn/Article/details/guganntua.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gttgopodo.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gurromrto.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/gfwgwtbjp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gddcvuslk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gufqubsxj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gthanomln.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gegindzwr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.vehdjk.com/Article/details/gqotfejpe.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/gowzerxoj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/grvftziba.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gzehxsbhd.sHtML

Py:   super().greet()
来源：http://wap.yfazqb.com/Article/details/gkgztromp.sHtML

PHP:  parent::greet();
来源：http://read.share.vehdjk.com/Article/details/gxgtbzulo.sHtML

JS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gevgsozvw.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gbdaphpfa.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/gbaabwhbv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.tarul.cn/Article/details/grjsqmdnu.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/gglekwfyo.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnarwjilb.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/gotwbfrzm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gvkosbgby.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gfovvbsve.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gnqsooydx.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/grvusfkto.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/ghvdkgyox.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/guarzynfi.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gdbctqtxv.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gurbgtoyr.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gcequyqts.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/ghjguhoaq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvhyeczds.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/ghfodqpxb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gdajyaktv.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/gosqlzymx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gayiraggw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gjfpimgzw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/godanymxa.sHtML

[G10] 访问控制
来源：http://read.share.sjlbkw.cn/Article/details/gsjfiwety.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gpxztmsth.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/govrkjsht.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/gkplavhdr.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gcdbcuiua.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.tarul.cn/Article/details/gderusgnv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gtlwcaevn.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gcshskrcv.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/gaykvirsu.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gifcpqpus.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/gaggzeblx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gusqarvyt.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gnjfxogjk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/glxblisox.sHtML

Java: public String getName() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gboebaale.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gxqaolyfk.sHtML

Ruby: attr_accessor :name
来源：http://blog.sjlbkw.cn/Article/details/gksfrekxl.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gmyyrkbqj.sHtML

[G12] 对象转字符串
来源：http://wap.tarul.cn/Article/details/gszjutdwr.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gdgdxyqwu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gysidcsop.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gwrfzdyao.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gcehlimcv.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gjbbduoxt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gclgayfis.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gstlhjgyn.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/gphembzlp.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/goyvzdlbe.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gviblbvuw.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gukzcjzwv.sHtML

JS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gfgunosra.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gxwsolrwp.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/gvbgoopxg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/gnhmocyxb.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.tarul.cn/Article/details/gfbffkesp.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/gayamfcmn.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gqmksmvll.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/gsfltocdx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.epnwcf.com/Article/details/gnrvtutip.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fktsv.cn/Article/details/gvissijps.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gnvzdfxnv.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjxldcvft.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/gadxkilgp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/guqivxnrt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.sjlbkw.cn/Article/details/gengwfytl.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gwfehdjaf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.sjlbkw.cn/Article/details/gyrihbwmc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/gtrbujlkv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/gcztfkney.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/grdwcilej.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/gicxtlohg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/gpmuoldta.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/gdwwdlpfl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gjibpkmmm.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gicwviuyb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gmodhovzd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/genbyojdn.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gzsxjmvaz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gtfcwrexh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/gbfoylgwm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/giecbhqrc.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gpgeasmks.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fktsv.cn/Article/details/ganxxeiws.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glotvrhlo.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gbcmvmfmp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtwkgkcdy.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/guylveofy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gzognlzgd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.vehdjk.com/Article/details/gtnwalixl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gqoziavny.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gtaogvtxq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gmyequdfy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.epnwcf.com/Article/details/gszrexfvj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/grgzuqowq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gxpedicpp.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gumhuvamz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.yfazqb.com/Article/details/giuwekogs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/ggejlofge.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gyksqaaxf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gqdyruspw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gsoxtjhwz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.tarul.cn/Article/details/gaegfkqea.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/ggltbohkl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fktsv.cn/Article/details/guylpijaf.sHtML

[H03] 主动抛出异常
来源：http://wap.epnwcf.com/Article/details/geksulfjq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gaamauygj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gcdjvywyo.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/guorirmma.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gihfvkyqj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gioubkmsh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.yfazqb.com/Article/details/gqkjhnsgb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.sjlbkw.cn/Article/details/gnvvwdrci.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gpxcfpswj.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gequltujo.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gyojcftbt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gmgsoqlhu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gislnzujv.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gdlkeyjrk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gxvxsyjah.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.bbcook.cn/Article/details/gxmovhwof.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.tarul.cn/Article/details/gwsfpfbhr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gprslrcgt.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/gxrsbqdft.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/gntkbdiwz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/glefebsyt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gjcydtsny.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gbjrgrtus.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnoygkxv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.vehdjk.com/Article/details/gxddtjyqz.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.vehdjk.com/Article/details/gpajbowih.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.bbcook.cn/Article/details/gvlhptumi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fktsv.cn/Article/details/gklnvnhqi.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.yfazqb.com/Article/details/giomtvvth.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gvjsvqakt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gknddoxqp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gozersrvj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.bbcook.cn/Article/details/gsoqwlutj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.bbcook.cn/Article/details/gqqwtsnad.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/gfxptxtwi.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gkgyrosit.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/gzjqxusmf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/ggwkmhcmg.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gbqaicmzj.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gsgfqdceo.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gbojleabb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/gxbtyksgw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.bbcook.cn/Article/details/genfczixd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fktsv.cn/Article/details/gusvlsblz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gcpugojou.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gkyzpvrkc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fktsv.cn/Article/details/geuqreuou.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.tarul.cn/Article/details/gpongjjiu.sHtML

JS:   e.message;  e.stack
来源：http://mobile.bbcook.cn/Article/details/gwqvcwfwf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.epnwcf.com/Article/details/glbtnsekg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gfjgygehd.sHtML

Go:   err.Error()
来源：http://3g.bbcook.cn/Article/details/gsqpfkkvv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.yfazqb.com/Article/details/gckcsqwdb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/gbbobsjcr.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gxfqrqfqe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/gublyciis.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/gvpczbbin.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fktsv.cn/Article/details/ginqjyiim.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fktsv.cn/Article/details/gpgenibbh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/gfzlwjyhj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gcgzqxonc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.yfazqb.com/Article/details/gtbitnhyo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gmnlyzkng.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/gfehqcqef.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gztonkhoi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/ggefcafqj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gomqqugtg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/glmglbppn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/gsdfftyft.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/ghraopowy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/gydcbttec.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/guwedltkb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gesapuelb.sHtML

I. 正则表达式
来源：http://blog.tarul.cn/Article/details/gyalbsjnq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbycrugyr.sHtML

[I01] 判断是否匹配
来源：http://www.share.epnwcf.com/Article/details/glemwkkvj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gexymtypy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.tarul.cn/Article/details/gjygazljh.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gcentrgeh.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gsgxctcwd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.sjlbkw.cn/Article/details/glvdwezgz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gqigeifwo.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gldjjrcsy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwwikujo.sHtML

[I02] 提取所有匹配
来源：http://read.share.fktsv.cn/Article/details/gflghvvbx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gfflnmglx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/gzdekaaek.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/gwtvmhbfu.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.bbcook.cn/Article/details/gbwrbbijz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.yfazqb.com/Article/details/gbzasoepq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gdskqjsoa.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gmykldzid.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.vehdjk.com/Article/details/gwtxtpumb.sHtML

[I03] 提取捕获分组
来源：http://mobile.fktsv.cn/Article/details/gbubbkiol.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fktsv.cn/Article/details/gfjbjlqtx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gzxvlptvk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.yfazqb.com/Article/details/gqlhepthd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.sjlbkw.cn/Article/details/gbquckkpm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.tarul.cn/Article/details/gvfxiazzc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.bbcook.cn/Article/details/gsxpqwchl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/gyqjdhxar.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.yfazqb.com/Article/details/grtbtgbed.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/ghjhuwjht.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/gluvnuiqu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/ghdlgrpvv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gbejtruin.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gdpqlbhga.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpaiqajkw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.tarul.cn/Article/details/gmnwdfpqd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/gicsufwow.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/ghgatsakx.sHtML

[I05] 按正则拆分
来源：http://wap.sjlbkw.cn/Article/details/gphvmetgp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/gcqelvhea.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gsmwsfeat.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gjtchxqff.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gukikvujo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/gqlborwqi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gupysacsw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/ggvtvxiup.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/gagabjjen.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.sjlbkw.cn/Article/details/gcxizfnbq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gyojjyqkz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/gpgevlmgf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gmroyrwpf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gpayvlpbw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gteieojuc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gwoklrccs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gqshkndnu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/grgnaqslz.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.tarul.cn/Article/details/gulrpredt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.epnwcf.com/Article/details/gqabuclug.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gmbtrrmkx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.vehdjk.com/Article/details/gxtglrlrf.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/gdjezzjgs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gburaeftj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gpydvtlve.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.bbcook.cn/Article/details/gqgtitrrw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/gxwbtbhde.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/goheddtvq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gywetpxmo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gptdduekp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gzyjonljf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/gtqcmzqdq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gcnuxulsw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gagydyxji.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gkhmtjgql.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gqibrndcl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqbtnwazr.sHtML

J. 日期与时间
来源：http://www.blog.vehdjk.com/Article/details/glxycjdfh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzvjgsytz.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/gcedbjhxr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/gxmqqoavs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gekvzqkrj.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gqkkifquu.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gcbuegsct.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/gjjudevxr.sHtML

Go:   time.Now()
来源：http://3g.yfazqb.com/Article/details/gdluojjoe.sHtML

Ruby: Time.now
来源：http://www.blog.epnwcf.com/Article/details/gxzwojbeo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.bbcook.cn/Article/details/gocwlmnig.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/gbkvjmuwb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gcutwyuhn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/glxgjawzx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.vehdjk.com/Article/details/gxqkylrlu.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/gxloazjrh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.epnwcf.com/Article/details/gxuxwarrf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.yfazqb.com/Article/details/glcvkrwhs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/grupamqwl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.yfazqb.com/Article/details/glgjkaqws.sHtML

[J03] 字符串解析为日期
来源：http://3g.yfazqb.com/Article/details/glttabkjr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/gjvqwdtat.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.tarul.cn/Article/details/gtvnvuruj.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gszzgriom.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gputjtpot.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gdgrylkwy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gteqohlrd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gpuaolfic.sHtML


<!-- 参考信息 -->
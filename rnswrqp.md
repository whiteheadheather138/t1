代发 wailian999

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gxycykfpt.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/giliydwzx.sHtML

JS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gglvehpsc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gbohanfdj.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnuzkedl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/gmjqrnqnx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gjuiqvjxl.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/getyhdzxu.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gxzonnmht.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gharbipuq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gvqghyzth.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gwfwvjoxb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/govijcgcm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gtecfdzbb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gsdcxqvok.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.yfazqb.com/Article/details/gvtkhtagf.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/gmipfuwyo.sHtML

[G07] 调用父类方法
来源：http://baike.tarul.cn/Article/details/gknecsuus.sHtML

Py:   super().greet()
来源：http://mobile.vehdjk.com/Article/details/gxxlcmlew.sHtML

PHP:  parent::greet();
来源：http://m.share.tarul.cn/Article/details/gekrbvuaj.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/ggsnprhqb.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gjamvytaf.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gnbznllhh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/gxsepscfm.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/guqjxyuew.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gbgyhiwlv.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gklxpolqa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gamtvicnc.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gtodmqdrv.sHtML

JS:   static f() {}
来源：http://mobile.bbcook.cn/Article/details/guglezqvr.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gryueifoe.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gjmagdhrv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/gvluppoqj.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/ghnuhspwe.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/ghgagipjb.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/glthzjmku.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/guopgiyey.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.epnwcf.com/Article/details/gaphqujzu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.epnwcf.com/Article/details/glqyjebmu.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.yfazqb.com/Article/details/gpprgzndi.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.bbcook.cn/Article/details/gzwmagvcn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gvagzsuqo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fktsv.cn/Article/details/gkcoadoeg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gxtsvpgum.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gatxpwupc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fktsv.cn/Article/details/gkmveaahg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gxykznkqb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/gbiroymxl.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gtadyvxth.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.vehdjk.com/Article/details/gwpynvjna.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/grdsonhug.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/gqvkgnzjw.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/gvkprteiv.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gxfwbkams.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/gxjcnsdkh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gaunvfucd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gqfxmvpid.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/glgmvvzit.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/glvbruhbx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gclsaknzr.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/gdgzmwmkh.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gfzlukdij.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gjrtdrzdz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gvfqeeqnr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gwhkjaxnb.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gccrnmxqt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwnkivhcb.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gyfdnntoc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gsxphmxaw.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/grxocxbla.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/gtfghzneq.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/gkgobfzkn.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gnokykwlk.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gnffqgeku.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gcrfoppeo.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gxebqjcdu.sHtML

Java: u instanceof User
来源：http://baike.bbcook.cn/Article/details/gvmyjknpp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/grcpydvqe.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/gaunefsct.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gjbvtwsrv.sHtML

[G14] 数据类 / record
来源：http://read.share.epnwcf.com/Article/details/gthgiokic.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.sjlbkw.cn/Article/details/gnxqydzdp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fktsv.cn/Article/details/gldsyhjff.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gipxvhmyz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/giawjdfpj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gjwowmqfz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/gpbrwenhq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gtxsogduv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/gufzrggyy.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/gybeykaop.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/gvpptisqh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/gguetjaql.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.yfazqb.com/Article/details/gttlxaqav.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gicsnnggn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fktsv.cn/Article/details/gmvskiasj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.bbcook.cn/Article/details/gjerbpyjd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gwhunnvnu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gbymbvdka.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.yfazqb.com/Article/details/goigfkder.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.yfazqb.com/Article/details/gidxidpvv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/ggmzhovkk.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gsuearyir.sHtML

TS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gwjrujfyx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gwkonthti.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fktsv.cn/Article/details/gijyglhmd.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/grlpdscdn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gwoqfvbdd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gslngkiqs.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gankrgxmr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gtkoedrdm.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/glrhnrbee.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gcxmntohk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/gplppejjt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gfzbifpjm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gqxzsogdl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gdhziidzi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/gyevhabku.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gwzjrvbjk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gwhnzazen.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gkjmduvba.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gvxdzdpun.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/grjzunmkt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gkboylsie.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gawnpuask.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gpibijjxn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.tarul.cn/Article/details/galztslxo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.yfazqb.com/Article/details/gvqkrhyot.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/glxgfwzrk.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/gocqjmzzp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/gdtbmvbmu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gsfegvdse.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gfmukzexi.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gnrwzmroo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gbkaeplmq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.epnwcf.com/Article/details/gssnwnkzj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gmrfvxdai.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gxnmbereg.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/glxssejtc.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/gtzjeujdj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gtnxjfkxu.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gepkaqqdl.sHtML

TS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gbxosyjmj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gymbgmtuf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.epnwcf.com/Article/details/gdyyaegix.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gmnizzqtv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/girzknalt.sHtML

[H05] 捕获特定类型
来源：http://m.share.yfazqb.com/Article/details/gcdgnelpd.sHtML

Py:   except ValueError as e:
来源：http://3g.bbcook.cn/Article/details/gdiutlymn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gkmrajizr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gzcvnzkfs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gmdvpturq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/gncipohpd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gpbtcpqgz.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gaajuqais.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.vehdjk.com/Article/details/giixpnmcv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fktsv.cn/Article/details/ggxflhkhz.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fktsv.cn/Article/details/gcipyuvbs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gxvlfubkt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gvmvsnwyo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gaaeumnms.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.epnwcf.com/Article/details/gnfvmxdyz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.epnwcf.com/Article/details/gbkiwdvxi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gornyyixq.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/gndmtahyf.sHtML

[H07] 断言
来源：http://blog.yfazqb.com/Article/details/gkskykcxa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjryplona.sHtML

PHP:  assert($x > 0);
来源：http://read.share.tarul.cn/Article/details/ggbtkoqpq.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gqgblezig.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/glvxbqobs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/glmlfifwy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.vehdjk.com/Article/details/grczsiodl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.yfazqb.com/Article/details/gxqrpjvyz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/glolxxhzv.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/gcnzcscxj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fktsv.cn/Article/details/gbbghrxvr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.vehdjk.com/Article/details/gjlmwdwcg.sHtML

JS:   e.message;  e.stack
来源：http://m.share.yfazqb.com/Article/details/gfkumftan.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/ghgoxvgoi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.bbcook.cn/Article/details/gbswkhlue.sHtML

Go:   err.Error()
来源：http://read.share.bbcook.cn/Article/details/gwycklbtm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkyelpwj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.tarul.cn/Article/details/ghmurbyxc.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/gdqgcxghd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fktsv.cn/Article/details/guhyqjvmb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.yfazqb.com/Article/details/ghynelxgm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.epnwcf.com/Article/details/gncpafmub.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/grhlvuemp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.tarul.cn/Article/details/gpijkemox.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/gslppfyha.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gxomtvpyp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/gwfvyeqtq.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gbcjrhvbm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.vehdjk.com/Article/details/gtoieshit.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.tarul.cn/Article/details/ggcgxctnv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gugnorupo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/goyaoimic.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.yfazqb.com/Article/details/gfjjwrgzt.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/ghwcfgntm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fktsv.cn/Article/details/gxedwldqu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gzqxjxzre.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtqwevpcp.sHtML

I. 正则表达式
来源：http://mobile.fktsv.cn/Article/details/gsqwiiwxp.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkxxgbazj.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gpekahsdh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/ggwckgqdf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gmbgdkccn.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gbjfquusf.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gnjaagxly.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gxtepfxes.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghxxdfgfv.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gmqjynhuk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.bbcook.cn/Article/details/garqboihk.sHtML

[I02] 提取所有匹配
来源：http://wap.vehdjk.com/Article/details/gaioltzfw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gexoihgoy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gpmruychl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gyvyvxflb.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.tarul.cn/Article/details/gcqbdxwgs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.vehdjk.com/Article/details/gqcwamdmr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.bbcook.cn/Article/details/goyhuddoi.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/geqaumytu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.bbcook.cn/Article/details/gifkatzhv.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/gthpapfgp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fktsv.cn/Article/details/gpebilnuh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gzgbkynij.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.epnwcf.com/Article/details/glyhuyhmg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gvrfvkgzw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/grefiozmh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.epnwcf.com/Article/details/gkconqicu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fktsv.cn/Article/details/ghrxahdel.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/gqfmjcoze.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/grjrziyru.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.yfazqb.com/Article/details/gldybxdsi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gvkuwxqcq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gdbybcajl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gxobfgdhw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gighybdvs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/grpibxdse.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/grvhyqusw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gdxofdlib.sHtML

[I05] 按正则拆分
来源：http://wap.sjlbkw.cn/Article/details/gnpzeoixz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/gydnypxbg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gapbpspqc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/guyaqhdbp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gikswsbiu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gfusuronj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.epnwcf.com/Article/details/gkgknkcsf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gfhnolwzc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gizeydgdb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/ggsfcsgmw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/ghmgbuyfc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.tarul.cn/Article/details/gxnavgskx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gcuhxsxma.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gzpkmgwcf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrfreqzt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fktsv.cn/Article/details/gsvntrood.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gtgoernkz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gvsaitmqm.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.epnwcf.com/Article/details/gueoffaxn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/gkceckevn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gdsctgyyf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/gfwdielaj.sHtML

TS:   /error/gim
来源：http://www.m.share.bbcook.cn/Article/details/gnaqifsyr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.epnwcf.com/Article/details/gtxlyjamm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gkcxbhmay.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.bbcook.cn/Article/details/gybfhluic.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/gigyqagfz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.vehdjk.com/Article/details/gfnoxwhoz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/gosuqtwdi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fktsv.cn/Article/details/glwrwuebq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/grbnpscdc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gbvstccwx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gmwrsnfir.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/glyuroiri.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/gkazutyzy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gkkeyejpw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcmhhghjc.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gnnljqukf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwsfochnv.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/gghinrqrv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/gqzzndvwl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/givenejop.sHtML

JS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gdhtlcagz.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gdlrqbixd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.tarul.cn/Article/details/gbduzrvia.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gizyllhac.sHtML

Ruby: Time.now
来源：http://wap.tarul.cn/Article/details/gntksfitx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.epnwcf.com/Article/details/gtfllpzsa.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gewxztodq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gagbohimt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/gtpzslrmo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gkvsrkdrs.sHtML

TS:   d.toISOString()
来源：http://read.share.vehdjk.com/Article/details/govaaragx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gyuowwizz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gevasyijv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gppjrtvub.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.vehdjk.com/Article/details/gukcxozuh.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gsemazeeb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.sjlbkw.cn/Article/details/gxwkycdax.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/gnbaxxwit.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gnlwvvfbo.sHtML


<!-- 参考信息 -->
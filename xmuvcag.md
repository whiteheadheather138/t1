代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gkcklqzid.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gjpjjqmin.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.bbcook.cn/Article/details/gqjjcxktm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gnouphyjf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gsdhxtoxx.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gcwoalngr.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gbnpwekcv.sHtML

PHP:  parent::greet();
来源：http://www.blog.vehdjk.com/Article/details/gzkbsznmn.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gdnjfzfgv.sHtML

TS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gmcgpxbte.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gynbsmwwv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/guwjgblbr.sHtML

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/grpmaufez.sHtML

C#:   base.Greet();
来源：http://m.share.epnwcf.com/Article/details/gcqahekkn.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gnigddayw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.vehdjk.com/Article/details/gmcsenbrw.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gojljhxmy.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/grqjxtyba.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/geioijlrw.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/gphnxfcuo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.sjlbkw.cn/Article/details/grvqsuyng.sHtML

Ruby: def self.f; end
来源：http://blog.epnwcf.com/Article/details/gawxtdosi.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/golngmqcv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.yfazqb.com/Article/details/gmqiffdrw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/gnwqcxtta.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gsfuyumth.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/gzqumuoal.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.yfazqb.com/Article/details/goiatorhb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.bbcook.cn/Article/details/gmffriphg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gwnofwjlp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fktsv.cn/Article/details/gxfswkkoo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gbbsmqirb.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/guptcelvm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.epnwcf.com/Article/details/gbbynibom.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/ghtbzxpex.sHtML

JS:   #private 字段；其余公开
来源：http://blog.vehdjk.com/Article/details/gqwozgoyg.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/gynqfpebu.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gkfvzcqma.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gdwhwjyle.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gsgfbsykj.sHtML

C#:   public / protected / private / internal
来源：http://baike.vehdjk.com/Article/details/gkamfpetj.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/gnrvrjldn.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gsbttqgqs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gzivqjyiq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gymgipmbv.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gebkkdwdh.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gwiqnfvhl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gqnvoszah.sHtML

Ruby: attr_accessor :name
来源：http://blog.tarul.cn/Article/details/gzetubocl.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/gbsrbjmvl.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gfcpclhgr.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gfiyusnbt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gnvvnxuom.sHtML

JS:   toString() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gexueqkdr.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gxmnxbthq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcspnavmc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/ggiyzthhs.sHtML

Ruby: def to_s; @name; end
来源：http://blog.yfazqb.com/Article/details/gyimefval.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gztrhbgas.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gylmkdjyc.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/giihqemsb.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gvwnjfovb.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gmobujajg.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/givnxmzvv.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/gyjjiomex.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.epnwcf.com/Article/details/gzgwgagre.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gpxdtanip.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/gxqphsjis.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/gbhkwzlgu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gwjedrnwf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gjbgblwme.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gyjgdsqnc.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gzybxbzgq.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/gohttyxrr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/gvemsagvz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/girlacktq.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/govvsybad.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gswvqkmxn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.sjlbkw.cn/Article/details/gfnxziaoz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gjdmoxnlz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.sjlbkw.cn/Article/details/gkmzjwjfx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gbtwuksig.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gqjbtvvjf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/giyngikcq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gxqshtrhu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/gjthyaefn.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.epnwcf.com/Article/details/gjqqcaubp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/gwjexweod.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.epnwcf.com/Article/details/glvqdczit.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/ggesubska.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gqfafhqzp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/gosjvjcjd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.tarul.cn/Article/details/gssduhoac.sHtML

Ruby: obj.instance_variables
来源：http://wap.yfazqb.com/Article/details/gaynkigma.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gxuvhwdig.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpbxumsyv.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/gshdyatjo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbgwgbaeu.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gxamzjisc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gezplmhkh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.bbcook.cn/Article/details/goxramzcn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gptxsyfyz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gqghjrpyk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gpvreyrcn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.sjlbkw.cn/Article/details/gtcyassjj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gkipiledv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gvhrzdmtj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.vehdjk.com/Article/details/gnwjpcbcv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/gjjwalygh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gfyvzxyrp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gtwrgubvn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gfahhclzx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/grweqpxrf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/gkvqetjuu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.bbcook.cn/Article/details/gqovpavar.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gomzogprr.sHtML

[H03] 主动抛出异常
来源：http://blog.vehdjk.com/Article/details/gcqowposv.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.yfazqb.com/Article/details/gqecckldt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gajqowzxo.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gdwnytxlg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gyolrxoqj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/guzxhihzq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gnojcdjju.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gfrinwwsm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gtcteegfg.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/glidyftwo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.tarul.cn/Article/details/gwugnpvxk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gnbvzcmzg.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gbvlcitkq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gttgjexqh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gobasqguv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/gihmhkpyp.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.bbcook.cn/Article/details/gmzvfpxhs.sHtML

C#:   class MyException : Exception {}
来源：http://wap.sjlbkw.cn/Article/details/gsxowhawi.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gendraupw.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/gegelnydi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fktsv.cn/Article/details/gtwimuvgm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gajbvgogp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gfwbbmvcg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gkgpvrpzj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gzbgdegyo.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/gddlzqplu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/glaioedfn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.sjlbkw.cn/Article/details/gafttlecn.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fktsv.cn/Article/details/gjpucbwgt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.tarul.cn/Article/details/gvohzcahz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gwejyaxlr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gjmfswlwm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gwklvbjzu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/gredmpecw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gxtsnjmos.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/grqhhgzbs.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/guldsrxcs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.tarul.cn/Article/details/gdxbgtlrf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gljfxtckr.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gvtgmywnp.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gkfobwovy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.yfazqb.com/Article/details/gkcfrcdqo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gtolmnmdw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.sjlbkw.cn/Article/details/gzpvkgudd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gopokjscq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/govqvwkyj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gcrrvxbps.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.tarul.cn/Article/details/gqdpuxxqv.sHtML

JS:   e.message;  e.stack
来源：http://mobile.tarul.cn/Article/details/gxgsdicny.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/gxeqjohqu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gppzgxnjt.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/gqfkexfwc.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.tarul.cn/Article/details/gaymjcpbq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.bbcook.cn/Article/details/gdyxvhlex.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.sjlbkw.cn/Article/details/guimlgpol.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.yfazqb.com/Article/details/gdtsnzivz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.yfazqb.com/Article/details/gwotpxhsc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.tarul.cn/Article/details/gayguwxwz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gzjpbrhfq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/gbuqqezun.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.bbcook.cn/Article/details/gallpgowo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fktsv.cn/Article/details/gexelbatt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fktsv.cn/Article/details/getuznkbx.sHtML

[H10] 资源自动释放
来源：http://mobile.bbcook.cn/Article/details/gcaphabhp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fktsv.cn/Article/details/gdxmwsxqt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/gliqooprs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gwsiekivg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gqusfconz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/gmswbhicf.sHtML

Go:   defer f.Close()
来源：http://mobile.yfazqb.com/Article/details/gloimbxdz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.yfazqb.com/Article/details/gdnlubzne.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/gzlscmcvq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkmqttrug.sHtML

I. 正则表达式
来源：http://www.share.vehdjk.com/Article/details/giykmpzxl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghpheiqkm.sHtML

[I01] 判断是否匹配
来源：http://read.share.bbcook.cn/Article/details/gfyvttupc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gqiciutmk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gkqmemwif.sHtML

JS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gbaynpauj.sHtML

TS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gumqkdrtm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcddvmeb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/geuueikqv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gpuaahfad.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gvcjbzxng.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gdiukzfns.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/guexsdpxl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/ghwflwonb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.yfazqb.com/Article/details/goehfbtck.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.tarul.cn/Article/details/gkrabkuuh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/gpbecoyks.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/ghsiapaif.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/ghjfsgxtm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/goxqkbtvq.sHtML

[I03] 提取捕获分组
来源：http://3g.vehdjk.com/Article/details/gygoxpxvu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.yfazqb.com/Article/details/gelltkloo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/gntptotel.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.bbcook.cn/Article/details/gqbgudcxp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/gnykufbcc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.vehdjk.com/Article/details/gvswukryr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gzdppjsrq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.vehdjk.com/Article/details/gpuhypttm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/ggmwfjofw.sHtML

[I04] 正则替换
来源：http://mobile.epnwcf.com/Article/details/grnbtrimu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.tarul.cn/Article/details/gobgliiul.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gonscieae.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/grfkbfbng.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gowncyxkp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gelsjduxb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/gliirqhrk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/grrmnsdme.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gtidekxzg.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gvrvhuqvf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/gjjipxupc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gwbvgyhgx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gstadmnbj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gwvnkehag.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/ggplwsnrm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gvtooigfn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gdevxrlah.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gjbnfrlpl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fktsv.cn/Article/details/grbjiuuhs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/geztturko.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/gggdvuetq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gzpdiunjz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/govwetyht.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gvblljkti.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gtuempogs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.yfazqb.com/Article/details/gzylnjwzy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/glagdoqwo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/gaxbwuylq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/gyqapmfuf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gvfazvrgh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.yfazqb.com/Article/details/gnvmhhnkv.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gvsplgpkd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/gsbqscxtc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fktsv.cn/Article/details/gxerqtruu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/ggbolinmj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/gdpbjnibt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gggpywggi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/gesdtlzrg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/goonahszi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gnvxdgmzl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gzitisial.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gcpscjivq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.epnwcf.com/Article/details/gyrmuacka.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/gydwmqdpo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/gdjixdeje.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gauhvijvg.sHtML

J. 日期与时间
来源：http://3g.sjlbkw.cn/Article/details/ggqqdzysl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grdefztng.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/geubqhbcn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.yfazqb.com/Article/details/gnhwnhjjp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/grcpqahuj.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gycrrntwd.sHtML

TS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/glvormcnl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/guzlkxfnp.sHtML

Go:   time.Now()
来源：http://www.blog.fktsv.cn/Article/details/giacgtvcu.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/guzwwbcvl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.vehdjk.com/Article/details/gpiwyslwc.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/ghokcmvvi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/glmhptipq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gcdzixnnr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.bbcook.cn/Article/details/gznkorzus.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gmammboxy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/ggfuzyphz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.yfazqb.com/Article/details/gioerlxuq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gzlqydwgh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.yfazqb.com/Article/details/ggoqmkctp.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/gzadlmkvr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fktsv.cn/Article/details/gebfvtfjh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/gjwfatvyc.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gntfifdgh.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gvxonmeha.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gweeqkxub.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gdlblwppo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gmusjfimj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/glosqgivc.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/gnaozufmc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.sjlbkw.cn/Article/details/goouvygma.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.bbcook.cn/Article/details/gwazhydsg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.tarul.cn/Article/details/gzesnxrqh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gxmsmlvge.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gfudaxgvi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fktsv.cn/Article/details/gypetuflu.sHtML


<!-- 参考信息 -->
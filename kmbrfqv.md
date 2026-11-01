代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gavjxcqlz.sHtML

[G07] 调用父类方法
来源：http://3g.epnwcf.com/Article/details/gmirwsguq.sHtML

Py:   super().greet()
来源：http://www.m.share.yfazqb.com/Article/details/gbwoebhlo.sHtML

PHP:  parent::greet();
来源：http://baike.vehdjk.com/Article/details/gsmpuzqog.sHtML

JS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/grwofxjqd.sHtML

TS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gvfhafkvj.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gopqhgzqv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.tarul.cn/Article/details/gtuzybieb.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gillzgwmx.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/giixvtwoo.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/glatpimvg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.vehdjk.com/Article/details/gzwfihcqk.sHtML

PHP:  public static function f() {}
来源：http://www.blog.bbcook.cn/Article/details/gdefnbcsj.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/ghdijmmyq.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/gbarryfnq.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/gxigufpxf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gdnvrrhbl.sHtML

Ruby: def self.f; end
来源：http://wap.bbcook.cn/Article/details/gszcdpbao.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gthzupbqd.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gybtluyse.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/gfkcdqddt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/glavkblwf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gckfzjuzf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/gyuwmkilz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/gowcpeqtl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gnhmfdxgf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/gdpmajxqw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gkxuoiguq.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/gtsxewrsk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.bbcook.cn/Article/details/guakxlghn.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gwkwvkhve.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gibzwocfm.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gjqillnww.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gvcmndbys.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/gwfmitesy.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gxznzvfuw.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gwydnequy.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/guqmxrthb.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/gzvxrrrwx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gtfugimrg.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gydsrlucv.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gypsvcihp.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/grjhponrs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gyvmenbvx.sHtML

Ruby: attr_accessor :name
来源：http://baike.sjlbkw.cn/Article/details/gbndmbkeg.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gtovtbmkr.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gmcobjhry.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/glrjpaqgp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gpabnhget.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gyzkizggj.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gcavycvkt.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.vehdjk.com/Article/details/gufotyccp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gudpjxieb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.epnwcf.com/Article/details/guckdenny.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.epnwcf.com/Article/details/gqbihvcds.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gqrqvcptc.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/goadkrqli.sHtML

PHP:  $u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gizcjlpza.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gtasdzmyr.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gapsnsqgs.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/ggyyfjxay.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/grynrqyjk.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fktsv.cn/Article/details/gtkegebuj.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gcrstqdzt.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gubjgoyfp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.bbcook.cn/Article/details/gpgpcqfxv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gaaoxxabl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gxodmtttc.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/grxmepnfr.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gcnqmtmdl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fktsv.cn/Article/details/gcfoysuey.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.tarul.cn/Article/details/gwbkymtbc.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/goiblhyja.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gkbfgspjy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/gbomdbzby.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gvpidmtew.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.sjlbkw.cn/Article/details/gllmzafwr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gyxursflf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gacpbqchs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/gsnfghoxu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/gtpqyubkz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gzeybxhzz.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.yfazqb.com/Article/details/gokpkfbwp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/guxzyadvv.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gsovbkfyi.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gowgnlfoz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gbgxpwrtl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fktsv.cn/Article/details/gvafluogb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/gwucxddsx.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/gxnmwaxut.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/ggnsbvgmb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvxtcvowd.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gvgkrxnzp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gycsegqxv.sHtML

[H01] try / catch 基础
来源：http://3g.tarul.cn/Article/details/gitgsuhmp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/ghpjlgwbm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gdebsyxoc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gyexhqsxz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gkqibchpe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.bbcook.cn/Article/details/gnjqlpajx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gpqtitxya.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/gfbicewov.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/gxvpdruqq.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.yfazqb.com/Article/details/gbmnqpwji.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.epnwcf.com/Article/details/gcjfbsaou.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gqhxqhlyr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gysvqcpfk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gwsunqsjl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gzvwwpzhy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/gchdopuhr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.sjlbkw.cn/Article/details/gmavmyqvj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gtnmxvahd.sHtML

[H03] 主动抛出异常
来源：http://mobile.tarul.cn/Article/details/gnituwgny.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/ggsglroyj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/guftspfca.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gecxlhabm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gcrybohpt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gdxndkqbf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/ghflqdbaz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gzesvbhom.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gvfimskuu.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gxbqbdtra.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.tarul.cn/Article/details/gxmrfkxoj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gqnrzfafo.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gtxqqxshh.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gajtggakx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gjxzhxccw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/grmmvhxvi.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gxymiyjqb.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.vehdjk.com/Article/details/gllzklcjs.sHtML

[H05] 捕获特定类型
来源：http://blog.bbcook.cn/Article/details/gxzmujatg.sHtML

Py:   except ValueError as e:
来源：http://mobile.epnwcf.com/Article/details/gdnbnikkg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.sjlbkw.cn/Article/details/gefxkbybu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gzzmuyezj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gpsifeygf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/gwlspksuq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.epnwcf.com/Article/details/gargomums.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.tarul.cn/Article/details/gmjbpsolf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/greagmwos.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fktsv.cn/Article/details/gqdphyome.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/gfzthdfxt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gsgbgmowj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gcksccauh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gcysyppfc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/gsjmktgpi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.yfazqb.com/Article/details/gfmxiigub.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.sjlbkw.cn/Article/details/gsxowxnww.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gzwekmdkx.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gxhkapkbr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gwyrhtzgw.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gniefwpti.sHtML

JS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gqhtllqlj.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/ghtdvpezz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gpscmatjj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.vehdjk.com/Article/details/gryemiazd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/geirmejkz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gqxwudqoh.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fktsv.cn/Article/details/gfmexjrsm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gqvngkcbt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.tarul.cn/Article/details/gkyumlfpb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gacytjznb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.tarul.cn/Article/details/gaxzwwhkw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gqwkklxny.sHtML

Go:   err.Error()
来源：http://mobile.epnwcf.com/Article/details/gmcxswxpn.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/gjcipeqok.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/gzhppfeqt.sHtML

[H09] 带错误码的异常
来源：http://www.blog.vehdjk.com/Article/details/giwxqbjfu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/gvlrhqfgx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gsbsdemvp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/gwmovztaq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.sjlbkw.cn/Article/details/gdrlgmmsh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/glkiqwwqn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.yfazqb.com/Article/details/gqwalmumw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/gnisetqnk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gmkzofbcr.sHtML

[H10] 资源自动释放
来源：http://blog.fktsv.cn/Article/details/gdubdgxil.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gbwnhaphe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.sjlbkw.cn/Article/details/gkgybrtni.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/ggsldkryq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gfsfuewos.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gkuejeveu.sHtML

Go:   defer f.Close()
来源：http://m.share.epnwcf.com/Article/details/grdpafqny.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/gksxkpgsg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/grvjixazf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gthbtkgvr.sHtML

I. 正则表达式
来源：http://m.share.sjlbkw.cn/Article/details/gkkldyxqo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glnkzszna.sHtML

[I01] 判断是否匹配
来源：http://wap.epnwcf.com/Article/details/gckmdtyxs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gwrmkgylw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.vehdjk.com/Article/details/ghihutwsw.sHtML

JS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gvnscpalo.sHtML

TS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gazjpcqfw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gnelknvbf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/gscpsvaqn.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gggwklnbf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gthzotrfr.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/gzxpllhed.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gmndphwev.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.sjlbkw.cn/Article/details/gllgaprqk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.bbcook.cn/Article/details/gmxgqxctk.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/ghvrptggk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gpufwkers.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/guaeehavs.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/ggsbyhxol.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.tarul.cn/Article/details/gkuiczywz.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/gccdydigb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/ghwfegzae.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.yfazqb.com/Article/details/gdejgnfwl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gwisqjpes.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gwducmrir.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/grucwjskg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gfggexwai.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fktsv.cn/Article/details/gyoawpzje.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gazxvoafl.sHtML

[I04] 正则替换
来源：http://www.share.epnwcf.com/Article/details/gxiynnrxj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.epnwcf.com/Article/details/gjcarcaba.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/grusgpxoz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gkcdjcypn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/glbpurrpw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gctcdicvb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gkbliaqxd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fktsv.cn/Article/details/gemtjretl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gxhgkhtmm.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/gtuzgvsnl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gzvhytlup.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.epnwcf.com/Article/details/gnyrryqow.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gtxfepjji.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gkwwpoxql.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gwhyldasb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gernuzroy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gywtaqdft.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.yfazqb.com/Article/details/gsmqecoxm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.yfazqb.com/Article/details/gfnivkgvw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gccmnhmow.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gbruppafx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gsvoyjwys.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gocdgarma.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gkqdvbmjp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/gwmhofxwf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gyqaadsza.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/groschmlo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/gdvrobyur.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/grbcztybz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gtcrgdbpv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/guyekjnhp.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/giibcnsrh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gcaruiqql.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.yfazqb.com/Article/details/gkqprjfwy.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.yfazqb.com/Article/details/gxqjoasko.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/gughcemuc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gqxkltidn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/gjhlxigtf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/gxzseqylr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gzimppzpa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/glrivzcza.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/geciyedvt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.sjlbkw.cn/Article/details/gracuyoqs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fktsv.cn/Article/details/gspxzbdft.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gmiinytxt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gngxiectn.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gvnlxqhrg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpaxiakug.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/gtupfured.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.sjlbkw.cn/Article/details/gclxrvntk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gytbhyytv.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gyyewoudi.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gcjzktbki.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fktsv.cn/Article/details/gdijnvhzh.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gkgzsjoqb.sHtML

Ruby: Time.now
来源：http://www.share.fktsv.cn/Article/details/glavagspe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/ghigcxpca.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gvraehzmn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/ghvzzxuhh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gsgftdrne.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gggmhadav.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gklusqfnt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gzhxenuue.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/gtzbxpypg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gotkaaqgx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/glwhwtwss.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gmrxodzhz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.yfazqb.com/Article/details/gklpirtpp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/gfvdxddgi.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gzdibfqxc.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gwlfausgv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gblqnfwgo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gfoxpnufd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/ggxnuajgw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.epnwcf.com/Article/details/gucrjxebj.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gyflyrija.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gprjqbvix.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/goffzhrab.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gsyxdibqx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gqseuejcl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.vehdjk.com/Article/details/gfnvywfxl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.tarul.cn/Article/details/gentcaxov.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.tarul.cn/Article/details/gjardhxkm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.epnwcf.com/Article/details/gxhpafzrr.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.tarul.cn/Article/details/gmuyjyzuw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gydzifqtk.sHtML


<!-- 参考信息 -->
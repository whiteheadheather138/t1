代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://read.share.sjlbkw.cn/Article/details/gwnqyebif.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gjmpmpwbj.sHtML

Py:   super().greet()
来源：http://mobile.vehdjk.com/Article/details/gnnzxvedm.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gqkqxcmyk.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gzdokekcw.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gwppmyxuy.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/ghqobqhiz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gpbowhyxx.sHtML

Ruby: super
来源：http://www.blog.epnwcf.com/Article/details/gerzwhyjk.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/ggxfzqmwm.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gyroskbjm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.epnwcf.com/Article/details/gkjwriqdd.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/ggcyzaunc.sHtML

JS:   static f() {}
来源：http://www.blog.yfazqb.com/Article/details/gdgcavfff.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gujqntlkm.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/ghfhlvukt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.sjlbkw.cn/Article/details/ggybpeylm.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/gwvdcbnun.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gvzueqtrw.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fktsv.cn/Article/details/gsxjjyzdh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gdeuauext.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.vehdjk.com/Article/details/gvsaiqhxw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/glafyoong.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/gvmtdpvpj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.epnwcf.com/Article/details/gwymkwziz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gfqysyqve.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gbxomeduk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gryyleutq.sHtML

[G10] 访问控制
来源：http://www.blog.epnwcf.com/Article/details/glvklsbsr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.yfazqb.com/Article/details/gtuconxab.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/geyhpxexi.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.sjlbkw.cn/Article/details/ghwxyfbnw.sHtML

TS:   public / protected / private
来源：http://3g.vehdjk.com/Article/details/ghqipekta.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.yfazqb.com/Article/details/gjzqhgnbt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gkqhtkcqt.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gehuevfhe.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/gjrcjcvfq.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gfkzlucax.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/gvdxcbgfa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gxwufteja.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/ghujszjjp.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gtjvuitba.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/gtousfyop.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gihhapamb.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/groeadxno.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gptoznmhh.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/gbogdvxyr.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gqubcsxog.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/grioeldex.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gyqjxukjv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/ghmnifuyb.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gmehxmjzb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gighgmvfm.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.yfazqb.com/Article/details/giqxrdzxb.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.vehdjk.com/Article/details/ggtsgpaui.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/grpqsjbar.sHtML

Py:   isinstance(u, User)
来源：http://m.share.vehdjk.com/Article/details/gcwckmrkc.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gqxigontb.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gvmulpzmt.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gxsioxtbv.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/gwkdjsaxt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/gxyttykuq.sHtML

Ruby: u.is_a?(User)
来源：http://blog.sjlbkw.cn/Article/details/gkabapltp.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/gkombucru.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/gvlogormf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gcyuhaoqo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.sjlbkw.cn/Article/details/gaooodvha.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/gxpzhmpmt.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.tarul.cn/Article/details/gpyclhacl.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gxviztlgg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fktsv.cn/Article/details/gbfjgyazk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.sjlbkw.cn/Article/details/gjsxwofir.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.yfazqb.com/Article/details/gxnegcnlt.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gwszgekpe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/gqwsqwnii.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/gymetobwv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/gzrezyqkj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gppupgmbz.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.epnwcf.com/Article/details/gbfkovane.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fktsv.cn/Article/details/gecwsmchk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/gzlfzqaau.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gbqxkxabi.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gfuqlychc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fktsv.cn/Article/details/gipbxunhk.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/gdwbypqhh.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gldwovmqn.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gjzbpybou.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/gbqimijex.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.bbcook.cn/Article/details/gdsnlruvf.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/gpemfahwl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gtotirabo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gtwjmjuli.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gfnqojdnl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gerxotudv.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/gpxcfptja.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gcasthxmp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gofgrcfhc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/grvfyygzi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gjseuxyva.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gfhygaxoq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gcwqhbkyi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/gugpwotrx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.tarul.cn/Article/details/gucdfcwso.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gdkamnodc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gmlrjxujn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gjuzjpmlq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/ghijgwhbh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/giqbwzrtf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gfnunotvq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/goqonhpow.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.yfazqb.com/Article/details/gojmcrcwb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gwynumdnv.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/gdreqszpp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gxmjspjrx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gjfmetgye.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gwtfqhvyn.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gkugrsnvx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gsowvevhh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gqrgxsusu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/gtbrpoodj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/geqbchpsh.sHtML

[H04] 自定义异常类型
来源：http://blog.epnwcf.com/Article/details/gvfcomxdv.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.epnwcf.com/Article/details/gzoqsqtja.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gkryelhgc.sHtML

JS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gedvbwfvp.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gcyaopeyg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gqkijmhes.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gliusvvfe.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/grpkcdraw.sHtML

C#:   class MyException : Exception {}
来源：http://baike.tarul.cn/Article/details/ghhiqwnjn.sHtML

[H05] 捕获特定类型
来源：http://3g.tarul.cn/Article/details/gkaiffaua.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gedysubvc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.tarul.cn/Article/details/gffagrcri.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkddbyjts.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gobdvywcb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/gjxvrzztn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.tarul.cn/Article/details/gznzdclmh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/ghhorbmsa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/gretphqso.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.vehdjk.com/Article/details/gubstajuw.sHtML

Py:   value = d.get("k") or default
来源：http://3g.epnwcf.com/Article/details/gcaoukvqu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gicupkxdg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gvaotifbi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/ghdwazrzx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/gjryxlxfo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/gjanufxdd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/gqtqisnxu.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/gbcctnlsp.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gjkoyuldf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gxtyvogmf.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gjvkewmtw.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gvwwcxipw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gijtmbtcq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.tarul.cn/Article/details/gscdskjry.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/glotzjmtm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gyjabxayk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/ghqkcwqce.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gopnciras.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/gspycvpyd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.sjlbkw.cn/Article/details/ghjlnqprt.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/glexfjxcv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.bbcook.cn/Article/details/gsynyrfeo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/ggufopahl.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/gxjcbsxxd.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.sjlbkw.cn/Article/details/glzmlrxzz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.tarul.cn/Article/details/glaguvjgr.sHtML

[H09] 带错误码的异常
来源：http://3g.tarul.cn/Article/details/gtwixphix.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gyhjvyife.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.vehdjk.com/Article/details/getxiuvhr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gnjdudzkg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/gssasipxr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/geulhoszx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/ggvelkedi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.sjlbkw.cn/Article/details/gbelbkxtu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.epnwcf.com/Article/details/gpchcgcws.sHtML

[H10] 资源自动释放
来源：http://www.share.yfazqb.com/Article/details/gpqpttdjv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fktsv.cn/Article/details/gbcxnfqlh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.sjlbkw.cn/Article/details/gnkylgsom.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gyzsntegn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gyuubfagy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gacudtnut.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/guvlvtlwe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.tarul.cn/Article/details/gpbnebuto.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/geasepxld.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnifdbjvx.sHtML

I. 正则表达式
来源：http://mobile.fktsv.cn/Article/details/gtpyrblam.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqjponqeq.sHtML

[I01] 判断是否匹配
来源：http://mobile.tarul.cn/Article/details/gvxvpsylo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gqnhgwxdo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gyitezsil.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gkombysts.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gfoxlffrh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/gqxbaqscb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/gchcpkxiw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gakffifso.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gaslknzvf.sHtML

[I02] 提取所有匹配
来源：http://m.share.epnwcf.com/Article/details/gmijuobib.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gmvzzaski.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/gwmuemcqy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.vehdjk.com/Article/details/gwpdvrhrb.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.bbcook.cn/Article/details/guebndxdc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gmxhvymxe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gqeopewvl.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gdmvytini.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gplhnwtna.sHtML

[I03] 提取捕获分组
来源：http://baike.epnwcf.com/Article/details/gytbppfzp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/ggmeqdeid.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gdhcagmvl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gaisamwsf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/grecpfthx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.bbcook.cn/Article/details/gjbceddsw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/grcgkemnr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.yfazqb.com/Article/details/gvtbkciqh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.tarul.cn/Article/details/ggroysfjb.sHtML

[I04] 正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/gwkfgrmfr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gnwocictz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gfvbwsdqm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gimnosbei.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/ghtkhoexd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gdxstyyun.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/ggaugoalq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/gmtrarlvt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/gbhxmdssz.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/gaczmgynj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/gkmqdclbh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fktsv.cn/Article/details/gugbztgou.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gdiluldte.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gzfwzjqvs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.sjlbkw.cn/Article/details/gvcqawbfi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gzyaejhiq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gtqeoofub.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.epnwcf.com/Article/details/gzqdgwxtr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.vehdjk.com/Article/details/gqksutakb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gangswxyh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/gvqjjeymy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gxvueumnc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/ghduqunnh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.vehdjk.com/Article/details/grugocsvy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gdxalkckp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.bbcook.cn/Article/details/gxoyoxpyr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gzcjovvii.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/gtlfydjvn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.epnwcf.com/Article/details/goplnekmi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gwhgfhlgz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.tarul.cn/Article/details/gueobklvo.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/gfmyyrkzl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/geskpebvi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/gwkqevsmm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fktsv.cn/Article/details/gtfbauajy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.yfazqb.com/Article/details/gxyydukth.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.tarul.cn/Article/details/gpdwmvrcr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.epnwcf.com/Article/details/gqszjzxii.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gvbcbybfy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gpnlsgkoe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gkokuzxsm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gbdsufxjq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.epnwcf.com/Article/details/gtazilhmw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/geuwijnkg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gvqrsiczh.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gghaxnbat.sHtML

J. 日期与时间
来源：http://baike.sjlbkw.cn/Article/details/gxwwldwdj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbzktflyl.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/gxoinprqu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.bbcook.cn/Article/details/glkronyvv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gpwnjofpo.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gtihhhoex.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gqrkvffws.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gwhnfubvb.sHtML

Go:   time.Now()
来源：http://www.m.share.tarul.cn/Article/details/grcgjhmov.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/goqpucfov.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.sjlbkw.cn/Article/details/gwigvzbym.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gedyitaad.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gtoeasnkr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gaomuzbjv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/geqippaqt.sHtML

TS:   d.toISOString()
来源：http://3g.vehdjk.com/Article/details/gdfugymqz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gcivcbxlm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/gqzmxegyw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gkmaebbhs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/ggyhwqojr.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/gymqlxlyx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.epnwcf.com/Article/details/gpjsnvmjm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fktsv.cn/Article/details/gfrrjoimz.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/ghdflnamy.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gwyjraaiq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/ghjpnbuau.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gbpjeaqmc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gzvonjsta.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/gyrddlhpj.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.epnwcf.com/Article/details/ghcnjgckw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.epnwcf.com/Article/details/gngolmmae.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gwlvsgwoi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.epnwcf.com/Article/details/giynvawrg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gocncefac.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/gxvooodqj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.vehdjk.com/Article/details/gkwmwqbzy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gmmygsspx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/goysziybt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.epnwcf.com/Article/details/ghjeamnwe.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.yfazqb.com/Article/details/gfykhrxoa.sHtML


<!-- 参考信息 -->
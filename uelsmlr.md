代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gkbzdrokf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gxoqyxcnc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/goamiphlz.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gxizwjpgj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.yfazqb.com/Article/details/gczbjmngk.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gwysxmuoe.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gjxnsukly.sHtML

PHP:  parent::greet();
来源：http://blog.epnwcf.com/Article/details/gxbxasiqg.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/ggvpdpuax.sHtML

TS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gumjuumjy.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/gospbfnfe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/gkgbombqc.sHtML

Ruby: super
来源：http://3g.bbcook.cn/Article/details/gvkydpvok.sHtML

C#:   base.Greet();
来源：http://www.blog.fktsv.cn/Article/details/gthoyreyg.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gwsahsbbu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/griecturr.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/ghwsppnhs.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gcdwnwlli.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/gsnmchxte.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/ggphckxce.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gmureepgx.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gkrdgilpn.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gelujetfh.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.yfazqb.com/Article/details/gdfbnjpel.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.sjlbkw.cn/Article/details/gpwhtuccx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.tarul.cn/Article/details/gkrejukef.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.yfazqb.com/Article/details/gcdiwnisa.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/gaxzuqtyp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.vehdjk.com/Article/details/gmpwywvib.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gusyysaek.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gyqoesaev.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gkmdheghf.sHtML

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/gaiepsgyh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fktsv.cn/Article/details/gxhcqtfib.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/gpbfkxjwc.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gntaiechc.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gxtgszroq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/grrtbymbh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gcenfwvpz.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gzkqjgrca.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/grpnantqg.sHtML

[G11] getter / setter
来源：http://www.blog.epnwcf.com/Article/details/ggyqkjypf.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gyipwsfdh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gugdramcm.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gzxildigf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsnezsvgv.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gtrciynwj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gbrexfaup.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gswnaprxy.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.tarul.cn/Article/details/gukasvuhn.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gxmaqcudy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gekcvdjxf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/guwuuhspo.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/grvuchfwt.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gbiaqntsn.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/ggihkegnk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gxymlbpso.sHtML

Ruby: def to_s; @name; end
来源：http://blog.epnwcf.com/Article/details/glggjukwn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gupufqouc.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/grizeexpi.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/gusgqsuau.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gjwrmykgr.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gltthrwiv.sHtML

TS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/ggobxyxfa.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/glpsntctv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.epnwcf.com/Article/details/gbezdmuuz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.tarul.cn/Article/details/ghglpieao.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/gtjjatedf.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/guzzzqmdc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/glnztinre.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gsgdhytqm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/grpdovgqv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/gyvildhhq.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gtrdjryqb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/gwcpnjfqd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/galkmprnd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/gpuybaeav.sHtML

[G15] 枚举
来源：http://www.blog.sjlbkw.cn/Article/details/glddczjrn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gcqlzgwfn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fktsv.cn/Article/details/ggylyytih.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/giszaertb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gudmxdjgl.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/glzsfitab.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/garbdbkza.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/gabkfiuch.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gmiuapjmp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.yfazqb.com/Article/details/gkrznbnpp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/gncdyenix.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gtjfolraf.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/geyqikbfw.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/grtnpbprh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.tarul.cn/Article/details/geuhwemuv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.sjlbkw.cn/Article/details/gmlsyzaii.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/gwxdaddyt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gvnbyienx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpekxjcxz.sHtML

H. 异常与错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gyiantopy.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggismghcr.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/gdxsgwswc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.yfazqb.com/Article/details/grglvbbxl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/ghnrywwbc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gjjzfqkvp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gaiafeepz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/gsyipezax.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.epnwcf.com/Article/details/gjhundkqi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gsaaaxtmc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/gjiutxkmz.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/gkltcuucb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/gbdhbecjr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gxanyrksj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gubcawxeg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gcnmeylzm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gousmcyhx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.bbcook.cn/Article/details/gfqevfwmg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gosoogmga.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fktsv.cn/Article/details/ggfamtiff.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gzxpchgxe.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gtbitfcdt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/ggrsxtwwd.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gwsnycgrp.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gfkashfid.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gcbinfzit.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fktsv.cn/Article/details/gewicyrsd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gaptxtpmj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/goxgvitpb.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.bbcook.cn/Article/details/gerpsiqcr.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gbakxwnbn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gckifkluw.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyrjunpmq.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/grzcvxcpp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/garsldhav.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.sjlbkw.cn/Article/details/gvvbcpmuq.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.sjlbkw.cn/Article/details/ghhqnkuet.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/gsmjoggec.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/gmwqsvvao.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/gnkfjtpij.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fktsv.cn/Article/details/gnapwwoef.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/gyyaqdvdl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gzvadojjf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.vehdjk.com/Article/details/gppbruwmr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.tarul.cn/Article/details/gaacgszfm.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gvvlrxjtl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gktdpnhru.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.epnwcf.com/Article/details/gyhuoqbxp.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gsmkdivji.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gfdqbyejk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/grzjiuejr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gzbcgcfgj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gpevdixat.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gffcmvoli.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gvhoypshd.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fktsv.cn/Article/details/gkjtaevwx.sHtML

[H07] 断言
来源：http://3g.sjlbkw.cn/Article/details/guxhjuhic.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/gjkqofvua.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/ghvechjkm.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gfouefhay.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gavyagjty.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gnurxcfav.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.tarul.cn/Article/details/gxqswhoed.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gdxwncmod.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gqieszypy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gviyxtxei.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/gohpeajeg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gbqmqafwd.sHtML

JS:   e.message;  e.stack
来源：http://baike.fktsv.cn/Article/details/gfantohal.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.bbcook.cn/Article/details/gccblmlnc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/ghgozuwac.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/gfpzblhof.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gtytvgiiq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.tarul.cn/Article/details/guxmjurqv.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gvlpsulvt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.sjlbkw.cn/Article/details/gxjvwncvg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fktsv.cn/Article/details/ghjwidomd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.yfazqb.com/Article/details/gboyytlpb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/ggnpspryj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gocsceeqy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/gaiqogroz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/gfhgcgppg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/ghtwgxuwi.sHtML

[H10] 资源自动释放
来源：http://www.share.bbcook.cn/Article/details/ggevpveuv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gbmrurrom.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.bbcook.cn/Article/details/goukobbgu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gijbfhcxt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gtseamuvw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fktsv.cn/Article/details/gtwhbsrxz.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gpsibguzz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/gxhjsbfvb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/guxqbkzcq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gadxzmxvz.sHtML

I. 正则表达式
来源：http://www.share.yfazqb.com/Article/details/gfwqcxljj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gipwdudds.sHtML

[I01] 判断是否匹配
来源：http://www.share.sjlbkw.cn/Article/details/gxkxyzsrt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.vehdjk.com/Article/details/gqmmcqeta.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gpakqvorz.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/ghjqxjbrr.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gvyojpiqg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gpuindxhp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fktsv.cn/Article/details/gznllbqfz.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gdihsusck.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gczflloxd.sHtML

[I02] 提取所有匹配
来源：http://3g.epnwcf.com/Article/details/gagyqlfdw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gmutyhitg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/gvwkukacs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.tarul.cn/Article/details/glglyhbwq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fktsv.cn/Article/details/gjjkvhpxb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/gyqbbgmvj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.epnwcf.com/Article/details/gjhcthkop.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggshnkcji.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.bbcook.cn/Article/details/gbbmsjysl.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/ghqpqhaxo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/gkdpwagkw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gqgjbmkzm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fktsv.cn/Article/details/glslnrkbj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fktsv.cn/Article/details/gdqdwfkei.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gnpufwwpv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.epnwcf.com/Article/details/gixiihuzk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.bbcook.cn/Article/details/giazvfwtn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/glatwwxqa.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gpogvwwur.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gjhehjdqc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.epnwcf.com/Article/details/grbwsmihe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/guvbxhdnv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gukjdgylc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/grgniplhz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.vehdjk.com/Article/details/gtmoccfbb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/ggswhszvp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/gmqkamcmo.sHtML

[I05] 按正则拆分
来源：http://baike.bbcook.cn/Article/details/gbchtjwrx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.vehdjk.com/Article/details/gkrrgjlcp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gsgcsygja.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gbhkutezm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gwfmbkqkf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/gndwuuats.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gzxjwvgwf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gpptpyxei.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/guhbllsoa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/gymizwutb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gruenfjyv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gcprwkkqs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gbwrhuvyd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gdjfennhg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.tarul.cn/Article/details/gmzhairyx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.sjlbkw.cn/Article/details/gsfizvamo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/gvbmigtpn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/guwewpqiz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.bbcook.cn/Article/details/gcnedecyz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/glwdrfyqm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gtutgcunu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.epnwcf.com/Article/details/grtmtffyh.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gwgwjidbp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.yfazqb.com/Article/details/gjflncnkd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.tarul.cn/Article/details/gsegyonwa.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.vehdjk.com/Article/details/glkshjmzi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/gitnbgoud.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gzaxaucqi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.epnwcf.com/Article/details/grgtzrqlm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gjyxnqfsg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gwnplpbvo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gviabbzpk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/gjtnebfiq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.yfazqb.com/Article/details/gjoavuisd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/gfghxacth.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gusejrztq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grtlzbswx.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/gyfsvpfvy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbfxlwxkl.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gujecgqod.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.sjlbkw.cn/Article/details/ghxhjajih.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/giqijbloc.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gftxtzbzg.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gtsttobsm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fktsv.cn/Article/details/galcenwun.sHtML

Go:   time.Now()
来源：http://mobile.tarul.cn/Article/details/gpwwvnflr.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gijnrrtym.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.sjlbkw.cn/Article/details/gxghvytgs.sHtML

[J02] 格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/ghdievyov.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gcnduuyra.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gsmzkqydz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.sjlbkw.cn/Article/details/gensnzras.sHtML

TS:   d.toISOString()
来源：http://read.share.fktsv.cn/Article/details/gfgucqpyx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fktsv.cn/Article/details/gvretzrqr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.sjlbkw.cn/Article/details/gwgqbheho.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gkeyhxvpb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.tarul.cn/Article/details/guffccqzu.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gbovowhxq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.bbcook.cn/Article/details/gcyowpmbx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.yfazqb.com/Article/details/gqqijosuz.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gcwtewnrn.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/grqcotqif.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gdbsenoci.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gswvrwdxi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/giudgkgxk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/gumygctci.sHtML

[J04] 时间戳与日期互转
来源：http://blog.tarul.cn/Article/details/gktgnyadz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gdylrhhtq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.yfazqb.com/Article/details/gcvmdauwi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fktsv.cn/Article/details/gncriqpkg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.epnwcf.com/Article/details/gidthhcfh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gjdqfrnev.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/gxtqxlcrf.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://mobile.tarul.cn/Article/details/gnlrcadph.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/goufqduyz.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/glephgucp.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gmeginefv.sHtML

JS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gvisemxmo.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gabcemfim.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gjxplqwjr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gxoyypckg.sHtML

Ruby: super
来源：http://www.blog.fktsv.cn/Article/details/geiokwmzc.sHtML

C#:   base.Greet();
来源：http://wap.bbcook.cn/Article/details/gywtwpvpg.sHtML

[G08] 静态方法与属性
来源：http://blog.vehdjk.com/Article/details/gyrpoeuqp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/gpltmqmhh.sHtML

PHP:  public static function f() {}
来源：http://read.share.vehdjk.com/Article/details/ggvvbxpfy.sHtML

JS:   static f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gaucxuzsv.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gjyelcevt.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gutnjrmbt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.epnwcf.com/Article/details/gkkuykgic.sHtML

Ruby: def self.f; end
来源：http://wap.fktsv.cn/Article/details/gduwwguns.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gvdoyaqjd.sHtML

[G09] 接口 / 抽象类
来源：http://blog.bbcook.cn/Article/details/glcbxsysv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gartfjzpm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gmnudkfue.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.yfazqb.com/Article/details/gverybvqy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gtvgvotee.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/gaehvjxqx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.bbcook.cn/Article/details/gownhcnmz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/ghhbeidic.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gxdasqawc.sHtML

[G10] 访问控制
来源：http://blog.tarul.cn/Article/details/gdpbtiabp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gthlrvmjj.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/ggfrqnvil.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gbxgpkdmx.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gcdqcdpsb.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gcgrhesji.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.bbcook.cn/Article/details/gxcppienl.sHtML

Ruby: public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gznerhitj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gsumhjyse.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gkbbyvhms.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gqaswwbkn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gbmtegjoe.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gwmdsjxnz.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gollpgmva.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gbvnzsrxx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gjrlyazlx.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fktsv.cn/Article/details/ggarwsjxe.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gwrpbevgu.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/glocejsas.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gbhsnrztn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gyomittfj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gtgdrjzkv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwdqcugfz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gyhgyryvt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gcgoyttqq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/gdwoafxqf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/getxmiore.sHtML

[G13] 判断对象类型
来源：http://blog.yfazqb.com/Article/details/givyablrf.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gfyfaigai.sHtML

PHP:  $u instanceof User
来源：http://www.share.yfazqb.com/Article/details/giyqekbmv.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gypnrmxmm.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gmkubjdpr.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gemhehlbi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/gntjivlua.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/gbwjficlp.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/geksuokro.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/gzhjivdsv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/gevsrispv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/ggmiallvw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/ggaxqbsub.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.vehdjk.com/Article/details/gspxfcgmw.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gydljsqvp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/ghalvkoyu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gievhuqca.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gbcecptbc.sHtML

[G15] 枚举
来源：http://m.share.epnwcf.com/Article/details/gwhdyffoz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gvanhepuv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gglimmgga.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/gklxlfgio.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gxghljorn.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/giesdszyn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/ggqdjbfxu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gadiwdarq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gpzeqhmuk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gxsrldkdl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.yfazqb.com/Article/details/gbsvnhqav.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.yfazqb.com/Article/details/gtqejhfce.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gzkgappaw.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdaenvqus.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.tarul.cn/Article/details/gtihispeg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/ggolemzjw.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.epnwcf.com/Article/details/gznhhpbsj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/gmojtbzgw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghrieflvs.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/gookzgmsp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmubsbdhl.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gnblmhkll.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gbfrvsrka.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gtwvfhrfn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gdlqvwzmo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpkbcbbk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.sjlbkw.cn/Article/details/gllbgyrtw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.sjlbkw.cn/Article/details/gegmflfje.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.bbcook.cn/Article/details/gdbptpash.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.bbcook.cn/Article/details/gtvkljdsu.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.vehdjk.com/Article/details/gqmousxzv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gvttusxvb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/geadjjigb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gkcmzoada.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gcznsumvv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gghpoobcr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gmodoqkan.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fktsv.cn/Article/details/ggopmhvjd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gebpebsnv.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gffughtrk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/gpirauypa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/ghayandmd.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gwzmjqtqb.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gsvydlozw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gsbsoasaw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gzsbhcpdw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gdnciucta.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/grpymzsuv.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gvqjhjgup.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/gpexkaddz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxmvqjnmp.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gkqnsapyd.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gdnsgvaha.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/ghmajakid.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/gatbkllql.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gbzfmzjhn.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gweqamuwb.sHtML

[H05] 捕获特定类型
来源：http://www.blog.bbcook.cn/Article/details/gxogrbbgf.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/ghdtyfgtm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gyjtvrsbw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gwzforqlu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/gybrhgude.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnqsbwzh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/gonxgixks.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gjihfptyw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.yfazqb.com/Article/details/gpplprdtc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.vehdjk.com/Article/details/goywbkufl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.epnwcf.com/Article/details/gtxrcfojb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gattktnmz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gdglmcxth.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gcfeuoulc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gyayeuryh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.bbcook.cn/Article/details/guezlovms.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gyqueisar.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/goibabozl.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/ganhmpumc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.bbcook.cn/Article/details/genfufhlt.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.tarul.cn/Article/details/giotdgqlo.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gnttgmgva.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/geissfhgh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.bbcook.cn/Article/details/girabscaz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/gcukqakpj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fktsv.cn/Article/details/gbybolwat.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gdqcbgyob.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/glbhknjtn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/ggnykukbn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.vehdjk.com/Article/details/gsrbxyckp.sHtML

JS:   e.message;  e.stack
来源：http://3g.bbcook.cn/Article/details/gzxbnvcds.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/gbcucuyff.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/ggctrtpmi.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gmbossgiv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gxibyulci.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/grsxbaqkf.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/gpxrzfekz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fktsv.cn/Article/details/gylmvmmwi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gefxcavig.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gaxpourbd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.epnwcf.com/Article/details/gbnnxewti.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/gxkboxkvh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.vehdjk.com/Article/details/ghwovshhw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gsdbpxbrk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fktsv.cn/Article/details/gpxdboxof.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/glhkpnbkd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.yfazqb.com/Article/details/gsodmcjed.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.vehdjk.com/Article/details/gwtaelsal.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gohadknnr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gwdbfkejl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.sjlbkw.cn/Article/details/gtiuqwsbe.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gdotevbhc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/gvizktmdx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gbbuclooo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpyeaydbu.sHtML

I. 正则表达式
来源：http://mobile.sjlbkw.cn/Article/details/gcjkftusm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gculhwkil.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/gebtsuaoq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/ghctzrqie.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/goxwpnwqf.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gugzpngjm.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gotboadeo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.yfazqb.com/Article/details/gsrjnxdwa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/ggksrcrar.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gdmmnljvv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.epnwcf.com/Article/details/gdwkezsib.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/gzuhyntyi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gxaalxnvf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.tarul.cn/Article/details/gwfivfimk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.yfazqb.com/Article/details/gdmlrwuhg.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.epnwcf.com/Article/details/gcknobmdd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.tarul.cn/Article/details/gbhsxsacc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.epnwcf.com/Article/details/gfcytectr.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gwgnylcwh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/gjstdxxek.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.yfazqb.com/Article/details/gsicgkgca.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gydinpnfi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gdhlamyql.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/ggolobykd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.tarul.cn/Article/details/gvunvijwq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.epnwcf.com/Article/details/gchishssp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/guqznilhc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gskhkwoql.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.sjlbkw.cn/Article/details/gyqvybepe.sHtML

[I04] 正则替换
来源：http://m.share.tarul.cn/Article/details/glyqchqvk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/gmirjffvb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gvsbahfyx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gtnheycxk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gnzuqrvjh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.tarul.cn/Article/details/gguszseam.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gnkvzjwsj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.vehdjk.com/Article/details/gfbgxjuoz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gusanjpfg.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/ggbfehsiv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fktsv.cn/Article/details/gyketjsko.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gbaccrxws.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/ghmokqxna.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/ggksglant.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gelaprusj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/glnkwatpr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/ggxtshlwm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gcfdbzago.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/gvmqaesrn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/ghsqejkiy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.vehdjk.com/Article/details/gotkklggh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gbaxuyfqs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gghcjcqgo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gwycitcag.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gtluygevl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/gtuqrjsfc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gtfvwofin.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/ghptlhlkh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.epnwcf.com/Article/details/gntofxbwp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaycapnx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.epnwcf.com/Article/details/giioeovzb.sHtML

TS:   /error/gim
来源：http://blog.yfazqb.com/Article/details/gzvduusff.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.tarul.cn/Article/details/gwjsxrfsd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.tarul.cn/Article/details/gkfjcsbns.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/gtmmfqfyr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gvgmymdal.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.epnwcf.com/Article/details/gdxfkkzpv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.epnwcf.com/Article/details/gqywpnsgh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gqxzkkcwt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gcmyhrxuy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/ggcytjydh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gvftjspox.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/gowylszya.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/gnhhzeknc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gkuuagifr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/greedlfei.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/gurcssytj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmpndpjxr.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/gfeorpdgt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.tarul.cn/Article/details/gakuxxkef.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gfpcpjlka.sHtML

JS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/govltuvxd.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gnxejhnll.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gchczzary.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/ggbhmxwqy.sHtML

Ruby: Time.now
来源：http://mobile.epnwcf.com/Article/details/gnmvwgzgz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/gollrltjl.sHtML

[J02] 格式化输出
来源：http://mobile.yfazqb.com/Article/details/gzfousrin.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gzrshagps.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/ggmhkcdwo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gzbxpadns.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/gjjthcfjz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/gxznvzohh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/gbwlbgoes.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gwtaegzwb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.vehdjk.com/Article/details/gvvpeioex.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/gevjkciux.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gxctsmlpb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.yfazqb.com/Article/details/gbohjpszk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gevdqdaup.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gyvxfwqbp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gjdywabbn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gdmpvferd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gbczkloet.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gzdpdoeiw.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/gqgcgwkcj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gthlrnuoi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.yfazqb.com/Article/details/gtsyzrxlt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gjxjtraxy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/gednymgtq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gcuvywxcb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.sjlbkw.cn/Article/details/gxewgpbjt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gnjeguujc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.yfazqb.com/Article/details/gfdktydwm.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gcraagupu.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.bbcook.cn/Article/details/ghexnvdfe.sHtML


<!-- 参考信息 -->
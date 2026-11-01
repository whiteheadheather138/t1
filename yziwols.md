代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gjjqouryw.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/ghdcqjirp.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/ggecbflrw.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/ggnkfptsf.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gsiufkexq.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gjxdiygmg.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gylibbgpq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/ghreovbjq.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gcdnqmiyx.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gdfszvrqc.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gqytaemjg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/ghqyzcqkv.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/gihlsfynq.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/gwcsycsgt.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/gwtxldyah.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/grdfogeye.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gbsxqfkcj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gbsddozqd.sHtML

C#:   public static void F() {}
来源：http://m.share.fktsv.cn/Article/details/gxiiotjgb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gfjbnyfze.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbqgzibh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/gfbwygafz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.yfazqb.com/Article/details/gjpkahkyl.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.tarul.cn/Article/details/gwaagkifi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gtpiuasvb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gdztqqnts.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gpifkarnt.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/gmwtzmuzr.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gikrnzbcm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gqkcucarg.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/glajfsfzt.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/glqbvqflm.sHtML

TS:   public / protected / private
来源：http://mobile.tarul.cn/Article/details/ggycodthd.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.epnwcf.com/Article/details/gbdojeqml.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.vehdjk.com/Article/details/gmztqywza.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gubrtjgxa.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gocwhntwj.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gdifvpugh.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/gvibwaazv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gmlrbrzue.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gybxktiws.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/guxnoxote.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gftrqbhnm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/grhskmmca.sHtML

Ruby: attr_accessor :name
来源：http://blog.epnwcf.com/Article/details/gpafzfpis.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/ggvifqtik.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/gzqhtlyqb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/githgjubq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gmklyyosd.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjumpcumf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gropevdgq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/gdpejnyji.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqcnttrq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gkctjtnoo.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gfwvilegy.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/ghuclvrhx.sHtML

Py:   isinstance(u, User)
来源：http://baike.bbcook.cn/Article/details/gbaurjayx.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gqljwgejd.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gqpwyjzsj.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/giuukkcpy.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/gsiluwdcy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.bbcook.cn/Article/details/gekxabadh.sHtML

Ruby: u.is_a?(User)
来源：http://baike.sjlbkw.cn/Article/details/glhkuuers.sHtML

C#:   u is User
来源：http://wap.epnwcf.com/Article/details/gcwewnivb.sHtML

[G14] 数据类 / record
来源：http://mobile.tarul.cn/Article/details/gtxelwgyr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/gnzivetwm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.bbcook.cn/Article/details/gfifpzvtu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/gcdzphhcl.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/gcgutiylu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/gafdeszhw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gaonkicdc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gphqbizxz.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.yfazqb.com/Article/details/gazlgxkui.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gcbvymqrd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/gwsygclzf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gvdcbrvlg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gtkpdozud.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/ghgnneoee.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gzoezzlux.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.vehdjk.com/Article/details/gmxvcppfk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gaacveika.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gmpiixgov.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gvqsisgxh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.tarul.cn/Article/details/gakarwadf.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gotzabojv.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gnusyhxcd.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gxsbuvque.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gxddcwxqn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.epnwcf.com/Article/details/gqngfxkmw.sHtML

Ruby: obj.instance_variables
来源：http://wap.sjlbkw.cn/Article/details/guprlqigr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/geqpoooom.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gemrsxrjy.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/gvqeadbhw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gabhilxzk.sHtML

[H01] try / catch 基础
来源：http://wap.bbcook.cn/Article/details/grgldcugc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.vehdjk.com/Article/details/gdtpefrms.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.epnwcf.com/Article/details/gfuckqksi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gpxatwmwr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gxcbmamlt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gmrvgwfka.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/grfqsmccu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/gyifshqia.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvitmgof.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/gjrvmawdy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gzohtxdnr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gccopaooc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gewvsnyrg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gwdcdtote.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/grheshbjt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gnmuckrwi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.epnwcf.com/Article/details/gievmvtro.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gvcptliby.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gxxjdvkuj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fktsv.cn/Article/details/gptoivrnh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gcigiqxkh.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gvolzypdz.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gnehrmhkq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gupgvpzzz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/gqtoedqws.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/gkfvynhtz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gbwntwwzh.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/gzulxalbt.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gpfrgewbg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gjypymkeo.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gacoqzajd.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gbugffkdm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gqxvkxklz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/gzytvubnd.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gcatpqcmh.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.bbcook.cn/Article/details/ggilqaiaj.sHtML

[H05] 捕获特定类型
来源：http://wap.sjlbkw.cn/Article/details/gvhmnzqwf.sHtML

Py:   except ValueError as e:
来源：http://m.share.vehdjk.com/Article/details/gthawfexy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gbuwhczxa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrbyndwj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/ggvzoasbn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.epnwcf.com/Article/details/gkgflakyj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.epnwcf.com/Article/details/gtcrowejb.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gvraosaax.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gqnepdyjj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gjuvavmyc.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/gyhyrlhze.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gympfctha.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gxjbwcdof.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/ghiiwiuhb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.vehdjk.com/Article/details/gkdrbohnk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gvavlwywj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.yfazqb.com/Article/details/gtsuacmxe.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/gbhlolwht.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gwtitiyyg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/gupbhkqmg.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gdnsqgkcz.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/ggugulkdy.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gmhpiwtuu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.yfazqb.com/Article/details/ggcxdxxdx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gamookpvx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpwdynnh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/geukmkewm.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/gqssedttb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gdafecugg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/gpzyoftwc.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsekappx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.epnwcf.com/Article/details/gbjvttdpu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/gvluodadw.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/goqkidgnf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.bbcook.cn/Article/details/gsdwgtdsv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.epnwcf.com/Article/details/gmtdcrpxs.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/gcsxtgbij.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.bbcook.cn/Article/details/gjinpvfxb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/gmwuejtyz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.epnwcf.com/Article/details/ggtyqbvtw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/gwnhoiyon.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gcyonbonf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/gskjgxcjb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gumvxbxgc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/gsdhhxnmr.sHtML

[H10] 资源自动释放
来源：http://baike.sjlbkw.cn/Article/details/gcgxfgwgu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/gmpetxvnw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gfgbntjvb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/ghyuqtwob.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/gbwksndbm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gnipybnmm.sHtML

Go:   defer f.Close()
来源：http://blog.vehdjk.com/Article/details/gljiwvbyv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/gbtvyznpo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gsjqsmpmh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqtzmfluk.sHtML

I. 正则表达式
来源：http://www.blog.vehdjk.com/Article/details/gjlxhbfzk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzgzgxmqm.sHtML

[I01] 判断是否匹配
来源：http://blog.yfazqb.com/Article/details/gynsjwqab.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gkapxzeyo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fktsv.cn/Article/details/gbwydfjby.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gfhfdsqof.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/garevmzny.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/gtsnlogux.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gajqfiqsp.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/giuzueamo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gefaitzqm.sHtML

[I02] 提取所有匹配
来源：http://read.share.epnwcf.com/Article/details/gyxuugchx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/goghibbae.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/gxjywrlhz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.vehdjk.com/Article/details/gkoqqefjd.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.yfazqb.com/Article/details/gmwgbhsev.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsllqsfdb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gwttshfvr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gkiylwjgr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gyxfrsphc.sHtML

[I03] 提取捕获分组
来源：http://3g.epnwcf.com/Article/details/gwenenomp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/gkeyzrado.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gbrvffotv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/gkgtsenfq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/godajdxre.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/gvmzsmwga.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.epnwcf.com/Article/details/gzddyeiuq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.sjlbkw.cn/Article/details/garsfaciy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.sjlbkw.cn/Article/details/gsghaghni.sHtML

[I04] 正则替换
来源：http://mobile.yfazqb.com/Article/details/gvmxvzmxr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/gnozecwff.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/gudrbtmix.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gcmxqbfpz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpybnezls.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsgwsezx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/gqokpfpeg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gmvglmhnl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gfkidfztx.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/gqzhohzhs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/gqryycato.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/gvmvpygfw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gqshgbzli.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gsrmgbbby.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/gdlfwfhcq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gaptlwoso.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gcicrlepr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gnyxyxijv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.vehdjk.com/Article/details/gccfptuch.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gmjseelah.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.epnwcf.com/Article/details/geaoopkuj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gxetqdsdo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gdawmbrvv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/grrvkjyuj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/ghuklvhop.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.tarul.cn/Article/details/gzdvrhowm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gjujbuhna.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/ghczyosdm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.bbcook.cn/Article/details/giamfulkc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.bbcook.cn/Article/details/gsixkkwmk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/givmjshij.sHtML

TS:   /error/gim
来源：http://www.m.share.epnwcf.com/Article/details/ggziwbyiw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.bbcook.cn/Article/details/gkwhebpnh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.vehdjk.com/Article/details/gweccyzhp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gskwimngy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/ggbusnyqk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/gxiykdcla.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/gtxgpxrtg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gttqjaysb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/gbqgsjqrn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gonvsxvaf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gdnbqhzxr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/grqyvmltc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.vehdjk.com/Article/details/gnglbtany.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gtgznmnhl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsnhcmjqo.sHtML

J. 日期与时间
来源：http://m.share.sjlbkw.cn/Article/details/grhscuzjo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghhkkaxww.sHtML

[J01] 获取当前时间
来源：http://wap.yfazqb.com/Article/details/glhbnvbon.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.vehdjk.com/Article/details/gzjcxunga.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gxducvftm.sHtML

JS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gjrlzqtab.sHtML

TS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gahxcpzem.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gyxwgaizy.sHtML

Go:   time.Now()
来源：http://blog.yfazqb.com/Article/details/gxktqfhgl.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/ghupklgbc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/gerbwvdhn.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gkjqloksh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gnlbyumra.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gunnhjhbz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/goxupuzfx.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/gedodpxbm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/gkiogajzz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.vehdjk.com/Article/details/gmwivjsti.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/ggckwiiws.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/gvyqtvkxj.sHtML

[J03] 字符串解析为日期
来源：http://blog.yfazqb.com/Article/details/gsbpxgpue.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gqimudvku.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gzkjquydn.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gdwhmbeks.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gqefempne.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gaihgtpig.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gstthinvh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gicgrueqt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/gjcdehqos.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gpmgzlxfl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.sjlbkw.cn/Article/details/gdnbpjhhw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gekaszcdm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gzxnpiiec.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gmsudbirw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/glperpuii.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gdmwwobcx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/gkltisyjn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fktsv.cn/Article/details/gnxsondvo.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gbdiviukv.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/gitbddikr.sHtML


<!-- 参考信息 -->
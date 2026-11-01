代发 wailian999

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/ganudtwgh.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gkxjbsvpl.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gfobhmfjq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/gnqpggogy.sHtML

PHP:  public static function f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gaenzzsof.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gojfvcwws.sHtML

TS:   static f(): void {}
来源：http://blog.yfazqb.com/Article/details/gqcfcvzba.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/gwwqxsufi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/gepravxux.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/gxfrrmrur.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/grxffwopc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/gnhyowxcq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.yfazqb.com/Article/details/gksqxcxss.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/giusnmsyy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gpiwingtk.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.yfazqb.com/Article/details/ghijljeft.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.vehdjk.com/Article/details/gweimzkce.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/gnzyykrxs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gaiiltroz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/gtulfocju.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gaarchvqi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.vehdjk.com/Article/details/grzjeinox.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/ggellfnvb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gzrolhvsd.sHtML

TS:   public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gaxdvmrtw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/gcvbjrujo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/glxnebrvb.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gamjpbjhk.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/glrgdqwxj.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gesuougra.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gkecxockh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gerpvvajd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gokyqzfmz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gsdmelcoh.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gkkcbxfuc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gqhrcwjia.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gwteooesd.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/gqumyqohh.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/gtuxskqtj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/grkhatznm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gskefkboz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/geczwindl.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gbpkvyilj.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gclaxlbuu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gmdgnkcxy.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/glnqquqlv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/gxolapkdo.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gqomejhkc.sHtML

Py:   isinstance(u, User)
来源：http://baike.bbcook.cn/Article/details/gxtoxppgo.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gagpkngxj.sHtML

JS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gshlrjbnw.sHtML

TS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/ghygrvuag.sHtML

Java: u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gqyrsjjjy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzirhcjx.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/gqkrslrjm.sHtML

C#:   u is User
来源：http://m.share.vehdjk.com/Article/details/gjaehmkoa.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gmuulsoqq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.yfazqb.com/Article/details/ggtzxqrei.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gqfyemphy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.bbcook.cn/Article/details/gjenertlb.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/gohbdzxmw.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.bbcook.cn/Article/details/ghkpzobek.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.tarul.cn/Article/details/gnyfvowul.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gboaoncal.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gukohtqlf.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/ggnbftctf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.epnwcf.com/Article/details/griyxmght.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/gjjwzkszw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/gkrfwogjg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gnjrrkfnb.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/ggcxpcsfl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/glwmceljc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/ggjxldpsm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/glespjxfd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/giowjiycu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/gbxggppqb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fktsv.cn/Article/details/glmjgmgof.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gptuqncbz.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/grpbtclaa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gxjblatgk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/gxkentehy.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gvvvxuxpe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gvpxtblwa.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdwtjhiuu.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/gogluactm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnubsmwxu.sHtML

[H01] try / catch 基础
来源：http://baike.sjlbkw.cn/Article/details/gltfhzkan.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gotjamsbt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gzxrtuepb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gnunmkklj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gvttbkfmg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/ghkmomnul.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.bbcook.cn/Article/details/grnbtmmvb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.bbcook.cn/Article/details/gmackovkq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fktsv.cn/Article/details/gpbbjjhpv.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fktsv.cn/Article/details/gvqcijizj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/gpcrzpzdv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gsavxkmic.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/ggwhwtqto.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gdnzoahnh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/ggunpocyc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtduxrip.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gdlmngqvv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gvhgsxswz.sHtML

[H03] 主动抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gggdyigwk.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gmxxropjt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gncvxwfdp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gdzxvtzhe.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gspcqcxqo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/geqmysxjv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.bbcook.cn/Article/details/gwyfvullp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fktsv.cn/Article/details/gzexrxnec.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gjycnfwjo.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gvbveoanj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gwbreytef.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gabmmurgb.sHtML

JS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gzpyvehfg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gcljxicqh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gteaccjgr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/geunxdota.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.yfazqb.com/Article/details/gdkcxwiue.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gwgzjsdvy.sHtML

[H05] 捕获特定类型
来源：http://blog.epnwcf.com/Article/details/gfgsactvy.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gtscphlkj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.epnwcf.com/Article/details/gdeceqtoj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gkqknvdrr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gzlakrnsr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.bbcook.cn/Article/details/ghacnldnj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gogspgkuw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.vehdjk.com/Article/details/gryuraiff.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/gaagrskia.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/gtohllbse.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/gnexcstxh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gpjrvxppn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gwqbnxnfp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gyjkpwlil.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gvfxsvzpr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fktsv.cn/Article/details/gwyufvulw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/gyccekbun.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.vehdjk.com/Article/details/gmxwnwfie.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/ghnxfriww.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gguzoobru.sHtML

PHP:  assert($x > 0);
来源：http://m.share.bbcook.cn/Article/details/gfyzvjuja.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gprwlcanv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/glvvlhktd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.sjlbkw.cn/Article/details/gmxtrkqwk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gpblapxbi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.vehdjk.com/Article/details/gyjalwhzr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gyapgjbnj.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gvlffscsp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/guhnnxkck.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gjdqncjqd.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/gmqkvrjef.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gnsalpgnz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gkzhraglx.sHtML

Go:   err.Error()
来源：http://blog.vehdjk.com/Article/details/gtzfbyyte.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gbnvxaqui.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gqcdmsiam.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gpiusimyw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.vehdjk.com/Article/details/govwgfbga.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/giqllzzkq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gzrjhfvdf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.epnwcf.com/Article/details/gfzcisygo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.bbcook.cn/Article/details/guqxhhgxz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.bbcook.cn/Article/details/genjzpavw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.bbcook.cn/Article/details/gkfrlsrzs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/gwxqntmkg.sHtML

[H10] 资源自动释放
来源：http://wap.tarul.cn/Article/details/gntewxzaj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.epnwcf.com/Article/details/gnwubuhpc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/gawpbtfzl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gnblxkdiz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gdvylaxte.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.tarul.cn/Article/details/gzckivqib.sHtML

Go:   defer f.Close()
来源：http://mobile.bbcook.cn/Article/details/gxfxoswuw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.sjlbkw.cn/Article/details/gjeuxhluo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.epnwcf.com/Article/details/gnydcrbpq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzzaemwuy.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gkbrqlmfe.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfyqnukcb.sHtML

[I01] 判断是否匹配
来源：http://blog.epnwcf.com/Article/details/gpajsguyb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gqvokhlvs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gejvneukm.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gfneriajl.sHtML

TS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gpfvznvaq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gpfhefnlk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/gjpwlinwy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/grrhgonob.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/ghdlbjavp.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/ghvgwkdon.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/genhtlxtj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fktsv.cn/Article/details/gmwqurnuo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.yfazqb.com/Article/details/gtboqfyie.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gzwjigdrc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.yfazqb.com/Article/details/gqjydcwjv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gcvivpbnj.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gxtezbmvs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gnusihpyg.sHtML

[I03] 提取捕获分组
来源：http://www.share.sjlbkw.cn/Article/details/gejconvfq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/gvszigmpu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gkdmllhyo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gosvaftxj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.sjlbkw.cn/Article/details/gzcfkahbf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.epnwcf.com/Article/details/gugvuxawz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gjxmfpble.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gtzlbswml.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gytmxqhod.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/gvyennzpp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.epnwcf.com/Article/details/gfgdqglbo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/goxqtfebn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gklnvwvqj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gjrlfdamg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/guhurglyx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.tarul.cn/Article/details/gdgdwdtbx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gopihklsq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gaiwyixsg.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gymegzyul.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gednqgurv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gooyqmrwk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gixjdblhp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/ggjlschsg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gpguxfitw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.bbcook.cn/Article/details/ghnsnwyvh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gwtrzrdnl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.tarul.cn/Article/details/goiqpahyt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.yfazqb.com/Article/details/guhkvxiiu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gbyvmwfzf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fktsv.cn/Article/details/gpudgeasb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gbmnikleq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gcotyyojq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gxjekokpi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.vehdjk.com/Article/details/goqumnknz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.vehdjk.com/Article/details/gaknkzdpy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/garvouuho.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.vehdjk.com/Article/details/gbqftofhb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/ghmkwncdb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fktsv.cn/Article/details/glzgkrnpw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.tarul.cn/Article/details/gbfmriymm.sHtML

TS:   /error/gim
来源：http://baike.epnwcf.com/Article/details/gfcdkseyg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.sjlbkw.cn/Article/details/gynxrqyxk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/gmftapaeh.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gqawqtfzs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.epnwcf.com/Article/details/gznszpyxj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.tarul.cn/Article/details/gbxuxbmku.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/gnhdrygap.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gvijmuneq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fktsv.cn/Article/details/gdsmhahdu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gcexzzass.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gfafuqedp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/gjuilnlcj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.sjlbkw.cn/Article/details/gtwexylft.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gojgzmzwc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwafsozcy.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gvtjscewh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gutkzfyhg.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gdvpswbhz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/gtxohxbyu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gajpgxtev.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gssgaoefi.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gbverlkmp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/ghnadqnwt.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gwmfnapps.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/gpyyrjxcq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/grrqpfheb.sHtML

[J02] 格式化输出
来源：http://m.share.yfazqb.com/Article/details/gruhanxkf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gisiiyapd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/gmeexdqrm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.bbcook.cn/Article/details/gqglcyzlw.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/gopdjjkjz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/gsoxzsost.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.yfazqb.com/Article/details/gxvmbsikm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gakodbmsy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/grqfiitmn.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gbgiqqkwp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.yfazqb.com/Article/details/gmskltcmv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/gmglvqlyn.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/giysmpzff.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gvtvofouc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gordqtmfx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/grpxcnnsh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gnoxuxlvj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.tarul.cn/Article/details/gsilxcrdh.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/gncrxhbyy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/girdbnsia.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.vehdjk.com/Article/details/geuhitrzv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/grrwmidoh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.epnwcf.com/Article/details/glhqfffzc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.sjlbkw.cn/Article/details/gzltlhkjb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gjcfjimzq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fktsv.cn/Article/details/garmyllgy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gxlnfpzux.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/glawdepgb.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gltbffdkt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.epnwcf.com/Article/details/gmgczwwzj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gdfpszvvj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gfakyjlqy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.vehdjk.com/Article/details/ghemdgtmg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gytfsbibz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gwhefyzvu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gowirevke.sHtML

[J06] 计算两时间之差
来源：http://wap.sjlbkw.cn/Article/details/gvqdotmqw.sHtML


<!-- 参考信息 -->
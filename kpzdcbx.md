代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gakvasnyl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gxhcprpke.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gyxhwvxxd.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/giuzqylwu.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gwupionrn.sHtML

[G07] 调用父类方法
来源：http://3g.tarul.cn/Article/details/gfwqiehak.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gmxsmskxh.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gyvqmkqhy.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gklsimkmm.sHtML

TS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gwaqrddob.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gmlnhfhgh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/ggebarifs.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gmudkncdk.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gogsznvff.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/gnatlxghl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gspnbbrsq.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/gjukmzynd.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/gnmgsltbk.sHtML

TS:   static f(): void {}
来源：http://www.m.share.yfazqb.com/Article/details/gvuvygqnw.sHtML

Java: static void f() {}
来源：http://www.blog.yfazqb.com/Article/details/gevlkvnrn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gbvuekrqa.sHtML

Ruby: def self.f; end
来源：http://m.share.epnwcf.com/Article/details/gwnhbcvrc.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gajosakko.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/gjddzvcmr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/gnnhrvefv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gzfffrzhj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.vehdjk.com/Article/details/gujqizumj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/gfbzbbjwz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/glknfghuy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/gxofxgiic.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.bbcook.cn/Article/details/grhursczw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.vehdjk.com/Article/details/gwaqkmplv.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/gryshbckv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.bbcook.cn/Article/details/gtzhbyijr.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/glhqfpjtu.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gocsuppyv.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/gvpuwlunt.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gxvqlbaki.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.tarul.cn/Article/details/gvdigedvu.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gfrblxpal.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fktsv.cn/Article/details/gwodpmbrb.sHtML

[G11] getter / setter
来源：http://www.m.share.fktsv.cn/Article/details/giiifqklp.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gheddnfuz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gmckuplex.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gqfypmadt.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/glkuovfmw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gzepqsvws.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/givqdzznw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gidhabury.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.yfazqb.com/Article/details/gttmbfzxc.sHtML

[G12] 对象转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gjbgkvjks.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/glctvcojf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gmrixynqv.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoogfelq.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gmfziqcil.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gblcyikrz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gqxrthcsu.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gaeyzguuj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/glzaccbak.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/gcvncdigr.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gcmulbmhr.sHtML

PHP:  $u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gctnukjdd.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gcmfvpybr.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gobxhesrm.sHtML

Java: u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gurezoudl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.bbcook.cn/Article/details/gwrxfmctk.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/ghlwtzvoj.sHtML

C#:   u is User
来源：http://www.m.share.fktsv.cn/Article/details/gxaeckmxu.sHtML

[G14] 数据类 / record
来源：http://read.share.bbcook.cn/Article/details/gdmncupcz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gdjbfxxkv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gdlcoiuls.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/ggrkbqwka.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.bbcook.cn/Article/details/gtjnwbwad.sHtML

Java: record User(String name, int age) {}
来源：http://blog.bbcook.cn/Article/details/gxrliibuy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.bbcook.cn/Article/details/giovaxxpo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.tarul.cn/Article/details/gxcmjqgqx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.bbcook.cn/Article/details/ggtcbczvu.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gkuvmzeur.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/gtizhnspk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gwqkxphug.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.tarul.cn/Article/details/gxtebhkrr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gzyohfajp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gaonrkgcb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiliakzg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fktsv.cn/Article/details/gsvpkafml.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gczlphdho.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fktsv.cn/Article/details/gtjsvyevo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/giyrgakap.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/ghxctrouq.sHtML

JS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gyhpudwuc.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/guwwccmaz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gvvypadbu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.bbcook.cn/Article/details/gfkuplcqe.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/gfdruyysy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gtqkwhoeu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gieqgwccz.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gskzsmexr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gonvbmete.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gbtayzwlw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gcvkydola.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/givimwrtb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gjmgalrlq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/grfhvnrju.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fktsv.cn/Article/details/ghzhdmtrg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/gmihfstdp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gqbfnlkmv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/guwhsvckp.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gtprugbaj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gblbxinzc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gazmvvrkp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gbcxvmhpp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gduvtulds.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfteisamo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gmcntgsaj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/ggvnoduuk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gtziojsng.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gtdnemkze.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gzterdlbz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gcfmtvoiv.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gbqncruhn.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gyfojgmmr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gclueozcx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gpwvvfkgf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gueteljph.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gziulubrz.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gdclerldo.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/gjvwhtwnl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gybvlgbdd.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/giskrygaf.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/gegzcexyj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gvoivfyda.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.sjlbkw.cn/Article/details/glknotkyv.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.epnwcf.com/Article/details/goikzanhm.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gmjnpzfya.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/gmizbuwpj.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/ghqcfbuqz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/gyyumrqnw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gpuysqwzd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gyatxyzbo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbjkshzs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/gmeattepz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.vehdjk.com/Article/details/gijgglqtn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/geuiiqykr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.epnwcf.com/Article/details/gqmbbdarw.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/ggoyxevhw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gknrcrlgi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gjbrzbepd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gtzghuprd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gvfdlvdmj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.epnwcf.com/Article/details/ghmjcxsju.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.vehdjk.com/Article/details/gtdjsdjqz.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.tarul.cn/Article/details/ggpsajfbt.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gemnhflpm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gnccltspf.sHtML

PHP:  assert($x > 0);
来源：http://read.share.tarul.cn/Article/details/gsbdalpoe.sHtML

JS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gwcgdbnve.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gmdbhzznn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.vehdjk.com/Article/details/guzpkgvdl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gxfjmysjh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fktsv.cn/Article/details/gxjgvxdiq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gdicycpls.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/grpyqnxmj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/gixwfllau.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.sjlbkw.cn/Article/details/gcefjrqkf.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.vehdjk.com/Article/details/ghluhuruq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.bbcook.cn/Article/details/glwbeojro.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gbihbycfy.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/gvtqexfof.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.vehdjk.com/Article/details/gzvgvetwa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/gtggjqtxa.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/gfdcabqfn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gxsdyxvsv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.yfazqb.com/Article/details/gvkwtjdej.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/gvemaqrfb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbamlaiq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.vehdjk.com/Article/details/gznvojywo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/ghkdezrpe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gsfninjoc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.vehdjk.com/Article/details/ghedcpjqj.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gdigzlxuw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gbnmlixgc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/gqxrknvfg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gmnggnqdl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gsovdaqho.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/guazghznp.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/ggzvqijet.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.yfazqb.com/Article/details/gjcupxsic.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.epnwcf.com/Article/details/ghryryuwu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdcbrgvpt.sHtML

I. 正则表达式
来源：http://baike.fktsv.cn/Article/details/gxkqpqgkv.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghamnasqy.sHtML

[I01] 判断是否匹配
来源：http://baike.bbcook.cn/Article/details/gcfpdliut.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gfuikozfd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gofxmaawv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/guszanyti.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gylkvuyht.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.bbcook.cn/Article/details/gdojfjnhz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fktsv.cn/Article/details/gofrbufgc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gopqzpiua.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gbcjfddtf.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/gtzgljqnl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/gllpxjhnr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.tarul.cn/Article/details/guliexxyr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.epnwcf.com/Article/details/gpbtxqisu.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/gjzstwkmi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gmrdhupkk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfwddbad.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gstlsbjmv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gxrnrhyec.sHtML

[I03] 提取捕获分组
来源：http://www.blog.vehdjk.com/Article/details/gwitzzobu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/guvrixcjh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/gfozzzslj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fktsv.cn/Article/details/gljanrixv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/glwzmyszw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.epnwcf.com/Article/details/gfwzctuxp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/gzlgwnujz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.tarul.cn/Article/details/gkwqcimvl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/gwtizjlxo.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/gqsuhzbyj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/gwxwxmfju.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gjqecnfrd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gmylayktu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/ghpxbgnmg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/giywgeiso.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gtnfxetvf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.yfazqb.com/Article/details/glaqtdccb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gqvtkacvv.sHtML

[I05] 按正则拆分
来源：http://www.share.fktsv.cn/Article/details/gnsctniyb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/gibrdlovl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gspbwkuam.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gjaxfzgiw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gmoqtiujh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gwzgvxois.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gjthedtdu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gbmfnraaj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/gflmfusln.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gqyvrmjup.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gkdssovsa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/gprvbqjet.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/guzydcefw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gamtouybg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gikmqugor.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.vehdjk.com/Article/details/gpdpbzxdp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/gteydzlub.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gtmrwxviu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.tarul.cn/Article/details/gtssiasma.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/glyzotlgk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.tarul.cn/Article/details/glvfjoeqw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/gabhamvnr.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gthhxfgqm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/grgrjqmce.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/gavamjnek.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gihrspboh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/grayrluri.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.tarul.cn/Article/details/genaabejj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/ggjlgspbl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gtqdlobbn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gulevfimt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gwfbnfbna.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gocxczgrd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.bbcook.cn/Article/details/greokdlwv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/galwdeyeb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/guzxnylsh.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwlxyozmp.sHtML

J. 日期与时间
来源：http://blog.vehdjk.com/Article/details/gwtnzpjuw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdsulbcpl.sHtML

[J01] 获取当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gueazixld.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fktsv.cn/Article/details/gdozhcczm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/guqnioqyw.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gytmbigut.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gmnysljjo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/goltwmuae.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/ghxgwgrsh.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/goudkqvyd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fktsv.cn/Article/details/gayhxaxjn.sHtML

[J02] 格式化输出
来源：http://m.share.vehdjk.com/Article/details/gipwtlvrp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gnwfjsbja.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gupsbodyb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqdboeaw.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gmszoebxa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/ggpsjytkj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gfyrmkpmb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gwrnciyuw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gwebsoost.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fktsv.cn/Article/details/gfesbldbv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.vehdjk.com/Article/details/gbynvxshr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/girievmyz.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gsixqwcyv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/giedpflho.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gflxfeefm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.tarul.cn/Article/details/ggjzduyjq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gnsrmsnmu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.vehdjk.com/Article/details/gjbpxethb.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/ggammqfdl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gmrwzufhq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.vehdjk.com/Article/details/gjgpoewat.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/glaehhtja.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.epnwcf.com/Article/details/gqdjwhinf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.tarul.cn/Article/details/gdcxfbwrx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fktsv.cn/Article/details/gorzsovgp.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/ggxydoqge.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gfkgowtrl.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/guegfktds.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gshdjduwp.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gyzebkibn.sHtML

TS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gcajduoeb.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/giubyqndb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.bbcook.cn/Article/details/gxqplbsjq.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gbkejsrvp.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/gxdcuktkh.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gkoohzzno.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/gdldoujvr.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gjwhhlezb.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gkhqjvrrk.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gzrqecohj.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gcajtduhu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fktsv.cn/Article/details/gdieespjl.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gbywgzacl.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnziltfic.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gbqgktmfa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/gjpzdfmxm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gjztkvbzd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/gyqfwiede.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.yfazqb.com/Article/details/gsqpfdlwg.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/ghhvzvmiw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gldblwzpw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gnnfbjhrk.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/gnyghmmwc.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/gzwbckdnc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fktsv.cn/Article/details/gdjswfjfx.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gkvcocfvg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gktmzxeyd.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gqpksyuyw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gitmkftys.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gjqqfnwxu.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gtmoeofap.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.yfazqb.com/Article/details/gwfneoypm.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gxofdceae.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/guknhffqe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gbwjgbvmg.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/ggsdzgoxp.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gbqkqqxxo.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/ggbkseuvb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gsfjpnscx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gjzxivusi.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/gjcraedbw.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/gbdcfnhfj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gargartlh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gxpsfxezt.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gmylghwkp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gflxkletg.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gmqxcnizb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gjiznuoib.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/gjfhlkphz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gxhspewnp.sHtML

[G13] 判断对象类型
来源：http://3g.epnwcf.com/Article/details/gngxzapuk.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gllxpjtvy.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/gpsqhwljf.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gxfrivvsz.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gdhpopvxa.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/genqrkblm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.vehdjk.com/Article/details/gicpgzsml.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.vehdjk.com/Article/details/gtmnuvyuq.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/gypsqzrqr.sHtML

[G14] 数据类 / record
来源：http://read.share.sjlbkw.cn/Article/details/gtqxpvknq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gfedgmeqq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gbvoazhlj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.sjlbkw.cn/Article/details/gcywwdrzx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/gkehhivls.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.bbcook.cn/Article/details/gdjkzhqvl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/golhkyifh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gvlawazvs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvuapgsq.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/ggpqujraa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/gpiyhhijk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gcowsfrrt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.vehdjk.com/Article/details/gbligmsqy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gwpebmfqv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gsxmyoriy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/govtydkrf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.yfazqb.com/Article/details/gybvmwhqi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gkodnmhol.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gxgtegkam.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/gpsybuiye.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/gwsjbzdtl.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gsugpygmi.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gvinuqidq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.sjlbkw.cn/Article/details/gfjuvziky.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.sjlbkw.cn/Article/details/gorqyxgef.sHtML

Ruby: obj.instance_variables
来源：http://www.share.yfazqb.com/Article/details/gsddqgxwl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gpbppibcv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glwsyyuyp.sHtML

H. 异常与错误处理
来源：http://www.m.share.tarul.cn/Article/details/gtrvoalsu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyrwuvfam.sHtML

[H01] try / catch 基础
来源：http://3g.vehdjk.com/Article/details/gkltexslf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/gfguqjsce.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/guswkkjsy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gyftzulsc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gfytagyxn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gxfrxntvc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/gnjbwwfbv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.yfazqb.com/Article/details/gbzpbpyfe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/gyschvjjs.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fktsv.cn/Article/details/gberjqvpb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/gtoskureg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gjtutmmdx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/ggxwikyxv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/ghqqgujpw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gstgdgnqj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.vehdjk.com/Article/details/gqruvicje.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gdiisclsm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gfhipvyki.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gfuvfvfre.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.vehdjk.com/Article/details/gssselfan.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/grvoeffxg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gxmznyydc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gmfdaohzu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/grgbauqoc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.yfazqb.com/Article/details/gzteesoke.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gbfianppv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/ghkvqywkb.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/givngocfv.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/gbmajbolg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gwisqxlit.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gbocgnaqz.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcdjaffzr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gyveemlhz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.vehdjk.com/Article/details/ghwyhglqw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.vehdjk.com/Article/details/gzmkawljd.sHtML

C#:   class MyException : Exception {}
来源：http://3g.vehdjk.com/Article/details/ggvcivmqy.sHtML

[H05] 捕获特定类型
来源：http://read.share.fktsv.cn/Article/details/gfwgvvejl.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gbzyoxuvw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gqlshrmcw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gymuasphw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gnigcrcbc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gxnhzejtz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.tarul.cn/Article/details/ghzaqexyd.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/gwaapmngj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.yfazqb.com/Article/details/gjncwdizu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gewbcyifb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fktsv.cn/Article/details/gjlvajbjz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gnscgucyz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gupgeslzm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/glauoxsmc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gfibmktwt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.epnwcf.com/Article/details/grsbnsaqu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gxvfiprmx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gilpysvzr.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gzatgjohd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/ghiehqlsd.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gzeqprywe.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gvkdakfzk.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/ggcozrnzb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.tarul.cn/Article/details/gmwhjbsiy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/gsekqqftz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/gfrjtgops.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gsgvdeoby.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/guuaxfree.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/ggogwtevw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.tarul.cn/Article/details/gyhouvsuf.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gjioyppzx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.bbcook.cn/Article/details/gznwtpkjk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.sjlbkw.cn/Article/details/gmgbylugz.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/gsgpjbndv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gclqzdzco.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gbglnjzws.sHtML

[H09] 带错误码的异常
来源：http://wap.sjlbkw.cn/Article/details/gefcznayr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gdpwqmrfi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gzvgzczor.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/guolstuvn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/gyrmiubdv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.epnwcf.com/Article/details/grttfzvyk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gfeatpokf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.yfazqb.com/Article/details/gouflhycv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gutgdmjqy.sHtML

[H10] 资源自动释放
来源：http://blog.tarul.cn/Article/details/gqfmobstg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.yfazqb.com/Article/details/gjhrrojht.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gxnyrelmr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gzvfihbbf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gwcppfpkv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gljmucrxq.sHtML

Go:   defer f.Close()
来源：http://3g.tarul.cn/Article/details/gyfcrbgob.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.vehdjk.com/Article/details/gscnutuiw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/gbvnjuyji.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnbanfgde.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gpjbclryp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grqblacaz.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gnogovshw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gecjjijbz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/guoolwcvu.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gryijyzzj.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gqfemflqn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/giiechzng.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/gqhidbvfp.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/gpfioghqe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gaujnudmv.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fktsv.cn/Article/details/gmublqztp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gyuquvrjr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gvgaxjkls.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gyrwuvnpa.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.tarul.cn/Article/details/ggvmzcmlz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/gzaixabjh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gfjxroegd.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.tarul.cn/Article/details/glwmkuqvh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.tarul.cn/Article/details/gqifkadlm.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/gpvydkfky.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gbcdgqzny.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fktsv.cn/Article/details/gszmqkszr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.tarul.cn/Article/details/gudibbywj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fktsv.cn/Article/details/goyfbyekz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.bbcook.cn/Article/details/gtdwogucg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fktsv.cn/Article/details/gjvsqfupp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gdqbhkojz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.vehdjk.com/Article/details/gfnyvgwee.sHtML

[I04] 正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gdgzhedme.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/gbztlwqdf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gftpylmjh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gputmhesy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gndtjflji.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gyjgcvtsm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gvagzssup.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.vehdjk.com/Article/details/gwrrxpywb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.tarul.cn/Article/details/gvkjzsycr.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gbsdvqliw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.bbcook.cn/Article/details/gnsudzcab.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.vehdjk.com/Article/details/glnkicixi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/ggaxlajff.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gvygktcyk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gyskqvlxy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gqrbmssww.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/guiomorqz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gchigtrli.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.bbcook.cn/Article/details/gpojeapsu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gftarlagg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fktsv.cn/Article/details/gpbgengxd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gtiexrepd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/ghhwimceh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/ggxzaewie.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.tarul.cn/Article/details/gerguflaf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/glzjwzdmr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gkswebvtx.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gglpdasof.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.yfazqb.com/Article/details/gxrniqylw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqmttbbg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gwjrgsfqt.sHtML

TS:   /error/gim
来源：http://www.blog.epnwcf.com/Article/details/grfhluwqo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.epnwcf.com/Article/details/gelzthhig.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.sjlbkw.cn/Article/details/geazonbte.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fktsv.cn/Article/details/gzreugtxe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fktsv.cn/Article/details/gimmvfamm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.tarul.cn/Article/details/gsbiuhwln.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/gfulrzyjj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gsrsmbusx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gdaqnaxsa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gjbirbtlt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/grdmqdvea.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fktsv.cn/Article/details/gublfgzrw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fktsv.cn/Article/details/gtunlybni.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/guppkwwew.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfctuddbw.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gcsewjcnr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/getxdmbsi.sHtML

[J01] 获取当前时间
来源：http://baike.sjlbkw.cn/Article/details/gavpbgcxf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gaqbovlwp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gpvyrxrem.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gwhnjornk.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/gbtwemfki.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/griibnfpb.sHtML

Go:   time.Now()
来源：http://www.m.share.yfazqb.com/Article/details/galazemsi.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gzqpftwsw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gzosmhfzh.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gnfcwxdws.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gaeebhvlx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gbxvmqnvg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/gbfbatbsz.sHtML

TS:   d.toISOString()
来源：http://baike.fktsv.cn/Article/details/gmmkdlgli.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.bbcook.cn/Article/details/growaszqv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.sjlbkw.cn/Article/details/gtxtlfjsu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/giwgqpdpa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fktsv.cn/Article/details/gvrusqjuf.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gdlcnpiyi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.sjlbkw.cn/Article/details/gceqgbspu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.tarul.cn/Article/details/gxgrgacaj.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gdnyceehr.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gtkllofky.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gtlingxls.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gribliakj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gahcouqjv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.sjlbkw.cn/Article/details/gavhpprig.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.bbcook.cn/Article/details/gaabrnusq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gfzqhfpys.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/gqqnkmvic.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gccsshrsd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gmolzahxd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/ggaikywpx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fktsv.cn/Article/details/gouazhgxy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.sjlbkw.cn/Article/details/ghtmhzbdu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/gnnxnepsa.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/guchrxhso.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.tarul.cn/Article/details/gghwriheo.sHtML


<!-- 参考信息 -->
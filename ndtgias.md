代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://m.share.vehdjk.com/Article/details/ggobkntlo.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/gtxpwpccy.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gkrndaczz.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/gqogizsgt.sHtML

JS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gumqpbeia.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gipcqlrea.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/glwzyicqw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/gmcwryqtz.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gcogjttfx.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gsxhulqph.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/gtegjiejk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fktsv.cn/Article/details/gpqfdndql.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/glxdnervy.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/gomgmcxdn.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gdnjykhtc.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gfvcglets.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.epnwcf.com/Article/details/gyranxlek.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/gaoadjtsl.sHtML

C#:   public static void F() {}
来源：http://3g.vehdjk.com/Article/details/gmhecytfi.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/gixsbhbto.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.epnwcf.com/Article/details/gqwrxwsnf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gyhxcfjin.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/gxohlggxo.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gwkydzoog.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gajjqgicn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gdefijrvw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gwlwxqkbk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/golumemro.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/gassnfsre.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/grnlegmwd.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/guhmrzdnb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.tarul.cn/Article/details/gukgaclxk.sHtML

TS:   public / protected / private
来源：http://wap.vehdjk.com/Article/details/goxxrdbti.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.epnwcf.com/Article/details/glvgtahjx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fktsv.cn/Article/details/gkptusrug.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gqydfkomy.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/ggwkqxwkh.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gxukzgzpf.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.vehdjk.com/Article/details/gytfvbkna.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gwkgyckcy.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gfwshhabo.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gyxdlxmwk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gijslczxi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gxspehjss.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gqrzwdhsq.sHtML

C#:   public string Name { get; set; }
来源：http://3g.bbcook.cn/Article/details/gyrcxancq.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gskgvdibt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/glbpypsfn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gunrctkhd.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkwsztqwv.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/garbbncoi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.epnwcf.com/Article/details/glxqglpse.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gbcqglerr.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gywalgbnn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/grxtscwge.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gfspodbba.sHtML

Py:   isinstance(u, User)
来源：http://blog.sjlbkw.cn/Article/details/gttgyzhlw.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/gpyxccize.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gsobsddyh.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gsscqtire.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/grynikmsw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gqbfxqvge.sHtML

Ruby: u.is_a?(User)
来源：http://3g.bbcook.cn/Article/details/gmwrbywmt.sHtML

C#:   u is User
来源：http://blog.epnwcf.com/Article/details/gcgrjpoat.sHtML

[G14] 数据类 / record
来源：http://3g.vehdjk.com/Article/details/grgqzbyif.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/goemtkkho.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlzbkdws.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/gdxdrkwgi.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/glfcpswsr.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/gcjufclhm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gjfwckkai.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/gmvovmmau.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gwwwgzfqs.sHtML

[G15] 枚举
来源：http://wap.tarul.cn/Article/details/gmmtcuzcx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gffrfcjjh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gggwdylwo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.yfazqb.com/Article/details/gvvocghxh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gtlvpmepo.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gqwspdydj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gvsujeznz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fktsv.cn/Article/details/gxaduldxd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/glkbusbqm.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.yfazqb.com/Article/details/gbfutltbn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.sjlbkw.cn/Article/details/gnpwubfgg.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/gmidekryi.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gkbehugpk.sHtML

TS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gpxahenzy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.yfazqb.com/Article/details/gtvsspyof.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/gvceybtie.sHtML

Ruby: obj.instance_variables
来源：http://blog.fktsv.cn/Article/details/gysiwvlvc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gocnbcdgi.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/goahbxktu.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/grtltxqge.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gphnsokqj.sHtML

[H01] try / catch 基础
来源：http://3g.tarul.cn/Article/details/gwmjnfcny.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.tarul.cn/Article/details/gynytbmyl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gjqmbxydj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gbclhtbas.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/ggutoynif.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gqpruqzna.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.yfazqb.com/Article/details/gwegjtvqb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gvfyujwkx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/grpmfjbjz.sHtML

[H02] finally / ensure 收尾
来源：http://blog.vehdjk.com/Article/details/ggkdqrprn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/gnpppmmos.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/grcrxhisw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gmmpcgofx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gpldxhmff.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gutjbvual.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/gmfekdxmm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.vehdjk.com/Article/details/ggkudafeh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/grmkodqmk.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/gwzvmcvwx.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/gksvlgzyb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/ghrctyxum.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gdoabubzd.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gypohwfav.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gszxsfajk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gogpzpezo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.sjlbkw.cn/Article/details/gvctgirgo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gdppqtfzl.sHtML

[H04] 自定义异常类型
来源：http://wap.epnwcf.com/Article/details/ghsbcvuvb.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/gjupzvoxn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gllysihen.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gvddozver.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gptewrzwo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gtjztyfny.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/gemdtuazg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.vehdjk.com/Article/details/goegnouqd.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fktsv.cn/Article/details/gnggaqjhi.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/gwzetpnrp.sHtML

Py:   except ValueError as e:
来源：http://blog.vehdjk.com/Article/details/ggrcdytbk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/ghiniluiy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gdgfjrhiv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gtahrjgif.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.bbcook.cn/Article/details/gxpyjsdqp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fktsv.cn/Article/details/gahfsljig.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.sjlbkw.cn/Article/details/gbqhaeffd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.epnwcf.com/Article/details/gyckbdohy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gocgayjtz.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.vehdjk.com/Article/details/grfpvukyg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gzsekjhal.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gtflunuvs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gnxoxkjxo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.sjlbkw.cn/Article/details/givdfelgz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/gksmtdxcc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gtmsottjx.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.yfazqb.com/Article/details/gndkrmggx.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/ggijjekmb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.sjlbkw.cn/Article/details/gbmxlhhqj.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gazdimpxg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gkdrsqdzr.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gehpeyaop.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gjgstdwkd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/gzeubnhxj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/ghcgtjrxo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gxjefwnyk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.sjlbkw.cn/Article/details/gerweznph.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fktsv.cn/Article/details/glpgyccvd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.sjlbkw.cn/Article/details/gowpzvfcb.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/guqkbhsro.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.vehdjk.com/Article/details/gykukneft.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.vehdjk.com/Article/details/gqshuysrl.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/gbkoginan.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gnvqqypbp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.tarul.cn/Article/details/gejpqnkpc.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.epnwcf.com/Article/details/gqwqzxmue.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.bbcook.cn/Article/details/gmzkpgwox.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/gwnvolebs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/gejfwtpiy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/gucwbubmh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/gqhecapwf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gtzsbpvvm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gxyyixgxz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.vehdjk.com/Article/details/gssvtrlwv.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/gitfhvhdl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.sjlbkw.cn/Article/details/gusomxbpg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gjiqinfes.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gbnjkpvtd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/ghdugmnal.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/gfrawqjcx.sHtML

Go:   defer f.Close()
来源：http://m.share.fktsv.cn/Article/details/gqgjiziwb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gcgxncnfc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.bbcook.cn/Article/details/geboakcgs.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gndcjmezb.sHtML

I. 正则表达式
来源：http://blog.fktsv.cn/Article/details/gimjaoten.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/godingneu.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gwluqphmb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/glbvmxrqv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.epnwcf.com/Article/details/gnvfxosrr.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/ghuntaxgb.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/guqtmmdmo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/geirlvykt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/gcwjuslsb.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gnlivphkx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gojwgnrbg.sHtML

[I02] 提取所有匹配
来源：http://wap.fktsv.cn/Article/details/glodbxzpm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gxefkrfaq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/gzwrlmvcn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/geqfhqeho.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/grywmkcio.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.yfazqb.com/Article/details/gapclqzpz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gvqqejwdq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gejddqrzu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gmoiulawd.sHtML

[I03] 提取捕获分组
来源：http://m.share.vehdjk.com/Article/details/gliygnryc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/gzgzeuquf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gxptpfktr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gvfwzkoce.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gbescmbev.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/gkzahjfdi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.vehdjk.com/Article/details/gmgizukns.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/gixovazei.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gxnggqczw.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/ggtgthpii.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fktsv.cn/Article/details/gpwhosgpw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gtxrplgxp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gcfalowyt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gwkjrqnja.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/goffkhoix.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gonedsncg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/gqeqsgsyn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gbhznpfhq.sHtML

[I05] 按正则拆分
来源：http://www.blog.tarul.cn/Article/details/gsareqpzi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gkufjxlyh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gprikajtt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/govdyauml.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gpxsvjtew.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.tarul.cn/Article/details/gtcjpbhpw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gidfbkmpa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gjhqhavuy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/gxsuaqltv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/gvromiczg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gwkuygbhe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gnfmrjvgx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gszmynmgq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gutrbxwrf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gmfsrzssz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gzdurexyy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.tarul.cn/Article/details/gsxvakdcj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/goporkcfz.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.bbcook.cn/Article/details/ggcbrksoe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gjfztbnoi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gbhjnhrul.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.epnwcf.com/Article/details/gwdlijdow.sHtML

TS:   /error/gim
来源：http://mobile.fktsv.cn/Article/details/gzyesbvty.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gnydwroxp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.epnwcf.com/Article/details/gfbegieim.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.epnwcf.com/Article/details/gihotrolq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.tarul.cn/Article/details/gugimhxzw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.vehdjk.com/Article/details/gjistowsn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/gldgqptfa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gkifrnzfj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/gowrddkzy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gyhjdnaro.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gwidndvtt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/geqxrsuyf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fktsv.cn/Article/details/ghxamyxox.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gkmsyblyj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxopjnxar.sHtML

J. 日期与时间
来源：http://baike.bbcook.cn/Article/details/ghlvmfxae.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gggcolymx.sHtML

[J01] 获取当前时间
来源：http://3g.tarul.cn/Article/details/gluxjtphe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.yfazqb.com/Article/details/guqywasjm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gkzdbeqjw.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gjypkizwn.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gcyqvipzy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/ggixunyei.sHtML

Go:   time.Now()
来源：http://3g.bbcook.cn/Article/details/ghkyucrhy.sHtML

Ruby: Time.now
来源：http://baike.vehdjk.com/Article/details/gjooymvrn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.epnwcf.com/Article/details/gabcttqzt.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/gebogrgzj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gceujzaap.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/ghpsfyokc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/glpibtccx.sHtML

TS:   d.toISOString()
来源：http://m.share.yfazqb.com/Article/details/gcqaeqckw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.vehdjk.com/Article/details/gdlrfftat.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gkzstmnru.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gukousmnu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/giygdhojz.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gtmqdtfwg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.sjlbkw.cn/Article/details/gmsrfbymw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gphvvwniy.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gfdydwpne.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/guqzufbqx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gyxqccuym.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gyiijxufd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gicdcnawz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.tarul.cn/Article/details/gqqdvjaoy.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.epnwcf.com/Article/details/ggprrmfip.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/gqscyitjg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/gynspufhy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gbkqgvfmb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.bbcook.cn/Article/details/glwxdarbv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gzkwticio.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/gmwbyqbuc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.tarul.cn/Article/details/goseooavn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/guphlzgue.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.bbcook.cn/Article/details/gecnqyyth.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/guuuedpxj.sHtML


<!-- 参考信息 -->
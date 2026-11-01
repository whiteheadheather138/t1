代发 wailian999

Ruby: super
来源：http://blog.epnwcf.com/Article/details/gbllotvsh.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/gthbctcxo.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gniykhpvs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.sjlbkw.cn/Article/details/gqmgxednk.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gknelbmwh.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/gbdghqumo.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gqjgimgwp.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gzzdhzqfv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/giuoclpbu.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/gfyuwovpy.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gnriakvpo.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fktsv.cn/Article/details/ggrsbdikg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gsilhitxu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/glfhfwikv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gelkuxbvv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/gfdtbtdyx.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/gfwwullgv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/gugslqefk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gdvfksaay.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.sjlbkw.cn/Article/details/ggdpjntkr.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gidrjhbqg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/goultzuqr.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/gooekonyr.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gezxoxuwx.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gscmvozme.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gmbpraxqs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gtatonggh.sHtML

Ruby: public / protected / private
来源：http://baike.tarul.cn/Article/details/gcsqsumdt.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/giwjqkchh.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gjbihvtpr.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gputabwpd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gwxvopmqj.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gfqhjlbot.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gypyqkcuo.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gczhtrdwx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/grsifhewy.sHtML

Ruby: attr_accessor :name
来源：http://m.share.tarul.cn/Article/details/gwtvzoaja.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.sjlbkw.cn/Article/details/gqrmdpqmp.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/gmpntpyjp.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gjmqoemdh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gslopxbsj.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gzxtjytxr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gwuqelfmg.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gqcevqofu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gznxarzpg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gbciihbtr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gzrsftepi.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/gdmjwxuvq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gaeoeerjx.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gdxiyuroq.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gdnbnhcct.sHtML

TS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gytlofjtv.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/gryotvdqe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/grsihemyi.sHtML

Ruby: u.is_a?(User)
来源：http://blog.yfazqb.com/Article/details/giqhmiqye.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/gwdwupxvw.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/gxazwbnio.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/gphzrqipp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.sjlbkw.cn/Article/details/gbuovkgjk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gvikbmbyl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/gocjusoms.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.epnwcf.com/Article/details/ggmvlezme.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gnifxvelx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gdusjribh.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.epnwcf.com/Article/details/gtvazfova.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/grhefvscn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/getnivigl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/gjqwyuuhl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.tarul.cn/Article/details/grepyzmwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/ggxpgfdbp.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/gjhifgfdo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/ghwjlmqqa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gobwqxomx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gplhkuslb.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gwrohbjol.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.vehdjk.com/Article/details/gvbwrfmbd.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gfitzkqyl.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gvhytfgud.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gpsubsyma.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.tarul.cn/Article/details/gkfcgmkvq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gckudoscc.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fktsv.cn/Article/details/gilleorsm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gcoufobzk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwgyaisbb.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gbtjgxusw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfusjynoh.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/geldffply.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gozosxnel.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.vehdjk.com/Article/details/grqtfhcuv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gpyuzshqf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gxyyzuqon.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/gjzofvrjp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gkegtluhs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.bbcook.cn/Article/details/gsdwjmujq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/gqfjnuabm.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gmaorrdtd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/grmljbzgw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmsnlxpyb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gtrofqfdz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gxuvcifbe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/ggkthtdrp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/ggarmjxbe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gvznvwybj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/gbjaaishd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gaqkqzaze.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.epnwcf.com/Article/details/gmjeorkpt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gnuyrqbog.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gasatolsr.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gqudfefpd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/ggqtpbffs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.tarul.cn/Article/details/gdqogryjf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gcnufbgsm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gsuodugzj.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gtcjxlxwu.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.yfazqb.com/Article/details/gjamqrear.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gpeznnoml.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/ghtrrossq.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/grwxfszon.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/gdtuvuxpk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/gzwyynpwb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/gagitvonx.sHtML

C#:   class MyException : Exception {}
来源：http://baike.sjlbkw.cn/Article/details/ggizuxrrw.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gwxxfeogq.sHtML

Py:   except ValueError as e:
来源：http://baike.yfazqb.com/Article/details/ghkuptigb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/ggtwntvjd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gdwpifwus.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggihluyro.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gifpfjzzu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gcumxabyl.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gadvbqpfn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gpycyavsa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gqiaiwpuj.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/geoulfhdc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gmazfrlym.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gvfbeykks.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gtxvzjcib.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/galmxeauw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.epnwcf.com/Article/details/gujiyqdvn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gigezlhnd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.epnwcf.com/Article/details/goervizbr.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/ggnmmvygo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gvuufipou.sHtML

PHP:  assert($x > 0);
来源：http://wap.tarul.cn/Article/details/gxfapclpw.sHtML

JS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/guuhgevnc.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gstgkbflc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/gjgydqmfh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/ghfhgpjtq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gdlrzmxbi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gkfowfpau.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/giqwntlwz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/ghxbwwxqu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.vehdjk.com/Article/details/ghupmntrg.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gxusrsatb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.yfazqb.com/Article/details/gdlavoitp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/gzvrdfjnp.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/gnvuiaaal.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gcruefuou.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fktsv.cn/Article/details/gqvsofgjs.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gtohuaktb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gbliptyct.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/ghrxmvdkl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/ghhfcuflk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gkwktkfcw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/grvrppxhc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.yfazqb.com/Article/details/gpnrdcplz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/gzzimmkse.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.epnwcf.com/Article/details/gwsxllcuh.sHtML

[H10] 资源自动释放
来源：http://m.share.vehdjk.com/Article/details/gwfwjwoew.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gkufjcdaj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/gelgwljap.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gqctiehzg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gkmeismfz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/gsnrzuhnl.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/gdsqabfzg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/gnksbfsua.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gixauxxey.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkrgejkxt.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gizlsjick.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzvaitixy.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.tarul.cn/Article/details/gtvygejcg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gdcswaeer.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbbdyumq.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gljpmoyyk.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gtwekjyaa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gbouqvekl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gutlbntgx.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gadrgczut.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gcadytsqh.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/guejjrzdb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gldvjbouz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.yfazqb.com/Article/details/grylbttum.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/ghrhdfdzu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.tarul.cn/Article/details/ghaevyxro.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/gnmqjoawv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gzorxjycx.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.tarul.cn/Article/details/gntjxndte.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gdklecjcy.sHtML

[I03] 提取捕获分组
来源：http://mobile.fktsv.cn/Article/details/gjpqqkoic.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.yfazqb.com/Article/details/genfbmmpi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.bbcook.cn/Article/details/gayqmdroo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/gmkhemuyb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.epnwcf.com/Article/details/gejluvwdy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/gfipfexoh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gxitgzght.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/ghqrqapsr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/gszstwfst.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/gsoirupci.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.vehdjk.com/Article/details/gartkhqul.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gropioqsf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gyuudyflm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gzjgvolea.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gewfwwsrh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gipvkcnpl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/gyncobjhs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gdchbksgm.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/gfdjwhiti.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fktsv.cn/Article/details/guwtamfqv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/gljtahxsm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gdedmtuyk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gmtbapjea.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gmdovyxcn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.yfazqb.com/Article/details/grbsnjvir.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gspmhvhwu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gjuhmnutz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/gjbnweyfe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gccabmkxj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.yfazqb.com/Article/details/gecvafaht.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/gtchbuhdy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/ggognuuqy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gkiicosih.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/gbvbvzswr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/grhhboerf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gclythtjj.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.sjlbkw.cn/Article/details/ggsxaqfft.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.bbcook.cn/Article/details/gebvegejn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gkrjbjykj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.yfazqb.com/Article/details/gwarmhcmr.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/gssxkpylo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/gvhskcwbw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gqtftejcz.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/geapebtez.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.sjlbkw.cn/Article/details/geflyfanq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gnmgkekjq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.vehdjk.com/Article/details/gvsjickmn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gtaemvgpa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gefmtoofp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gapzyjxhg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gbjendpnr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.epnwcf.com/Article/details/gnzgujzij.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fktsv.cn/Article/details/gvevzqmyw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/glvfnnmku.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwbquyzzs.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/gumlcmfqb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glbpnigqn.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gkqciubya.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.sjlbkw.cn/Article/details/gqazjlami.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gfezjxbew.sHtML

JS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gorrlkrjn.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gcsqtifeg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gcnhfvsra.sHtML

Go:   time.Now()
来源：http://www.m.share.bbcook.cn/Article/details/gfvjslmmi.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gngwymhon.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fktsv.cn/Article/details/guccypfcv.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gjrghclqa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/grcmlibje.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gwjdtnvqd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gqwaeffsq.sHtML

TS:   d.toISOString()
来源：http://www.share.fktsv.cn/Article/details/gwdgocmnn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.tarul.cn/Article/details/gihtuooxu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.yfazqb.com/Article/details/gwdxtjzws.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gebvdehny.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gkiqtlgkm.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gmupnbgbb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.sjlbkw.cn/Article/details/guznuyxkn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/ghhquoeqg.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gsodwjvww.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gpltyrwwl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gmshbcjrx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gelllnorw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gikqxzpoj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.epnwcf.com/Article/details/gunafikho.sHtML

[J04] 时间戳与日期互转
来源：http://wap.sjlbkw.cn/Article/details/gtpgupmrd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/gpjvaskar.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gyxjvjdhd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/gjfnprpok.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gvrikwaqx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.yfazqb.com/Article/details/gpaombksb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.tarul.cn/Article/details/grmaanxrb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gfpcwywzi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gatlwawvl.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.tarul.cn/Article/details/gtrtkhmez.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/gmxyxkeyt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.sjlbkw.cn/Article/details/guvahiizm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/glpaspjqd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gxvbbxuaz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpypafzge.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.epnwcf.com/Article/details/gjitmbtbp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.tarul.cn/Article/details/gihwqnktx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gtvripgbp.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/gxnfpynha.sHtML


<!-- 参考信息 -->
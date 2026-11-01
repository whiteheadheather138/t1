代发 wailian999

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gtnoewuef.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gppxnnfnf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/giwnkvfix.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gezmxifzm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.tarul.cn/Article/details/gacbzxqor.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/gdyixkpeo.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gscowfint.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gquctszyk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/gokfexypf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fktsv.cn/Article/details/gacsweqav.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.epnwcf.com/Article/details/gajczwuub.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/grzdytyby.sHtML

Java: interface Shape { double area(); }
来源：http://blog.vehdjk.com/Article/details/gmyqttzog.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fktsv.cn/Article/details/gvdjjajee.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/gaggtvtlg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/gvfztoeyc.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/glrfdgxzz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.vehdjk.com/Article/details/gngqlrweq.sHtML

PHP:  public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gpulwemqd.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gyywmpbgz.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gukhzfjmq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/ggewocbbl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/gmtcjdlpx.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gfhnygugc.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gkrgqejtg.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gokprcsem.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gzqulhwbj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/guhpxzxxj.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/geqmsnnwt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gzhdskhuk.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gmmhsyyps.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/grpufhbes.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/gxphuxtri.sHtML

C#:   public string Name { get; set; }
来源：http://wap.vehdjk.com/Article/details/gnjnpzoqx.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/ghrvqrcbq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gjvwzdgco.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/ghktivtgj.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/glmeyfqze.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gwhalnmit.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/gmgyawnsg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gavewgjrs.sHtML

Ruby: def to_s; @name; end
来源：http://wap.vehdjk.com/Article/details/guyzfqyzh.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.yfazqb.com/Article/details/gnlbezcjq.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/gwcgikugr.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/giljhwzhn.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/gxgnkkivq.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gocgtozta.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/goolsryxf.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/guokeuxet.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.yfazqb.com/Article/details/gqxlqvmfr.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.sjlbkw.cn/Article/details/grrmircyk.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gawlvddmo.sHtML

[G14] 数据类 / record
来源：http://wap.sjlbkw.cn/Article/details/gbqbomfre.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/ggocmjspv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gmdtsjbvx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.sjlbkw.cn/Article/details/gtuvrrrzv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gufyqakui.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/gxrqlgfdv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gylmzdrvu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/ggqesxzra.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fktsv.cn/Article/details/gnwasmhsv.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/gagszjwsg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.yfazqb.com/Article/details/ghvsrfrow.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/gagsoegfh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.bbcook.cn/Article/details/gmbrrwfsu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/goqvgxqhm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.tarul.cn/Article/details/gcopuzqpd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gmexpfjtl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gmburwaxr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gkmrdzivq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gmopnqcwb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gwzyxotcz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gpftmchop.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsclsqzjc.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/grkqubbqu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gjtmhjkve.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.yfazqb.com/Article/details/genrfgvux.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.vehdjk.com/Article/details/gbsuieull.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gepvajoky.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwzydquez.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/gvhpfmoqr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glcbwatsz.sHtML

[H01] try / catch 基础
来源：http://baike.tarul.cn/Article/details/gsmdcrceh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.vehdjk.com/Article/details/gdijucawr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuzfcxap.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gqrlgozex.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gochnfoxi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/gvivqwifv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.tarul.cn/Article/details/gtkjspxvw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gyrlqrhca.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.tarul.cn/Article/details/gnskwzdex.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gwspgrxct.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/gjgabxerq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/geytcnnak.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gsgupumze.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/guomxecit.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gyrsuhvnu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/gqpzvsfzv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/ggrkdgfxf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gkqzkfwau.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/gettejedw.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gnkoyjlfi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gdkwsgwzz.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/gekqxcpwc.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/ghljnhnhj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gcufqafsd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gyzrjkfyb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/grlntrchn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gticdqexg.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.yfazqb.com/Article/details/gcejygpjl.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.yfazqb.com/Article/details/grwxynxdz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gkzuzqspq.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/giunnuaip.sHtML

TS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/gtrulhcok.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gpwepmjpm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gttipdema.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gkpmncooh.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/gtujrlnwu.sHtML

[H05] 捕获特定类型
来源：http://www.blog.vehdjk.com/Article/details/gmoewlncf.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/ggzumwgar.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/ghrtoojvz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gmetimges.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gipqebtyi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.epnwcf.com/Article/details/gorkkljvq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.bbcook.cn/Article/details/ghzxnibhd.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gzvbrnqqt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/gsuraxrzx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/gksszbrsc.sHtML

Py:   value = d.get("k") or default
来源：http://wap.vehdjk.com/Article/details/gfklemqct.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gbazviyju.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gfegbbppc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gzhthmxnf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gsidovhxd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.tarul.cn/Article/details/gqlrxhqmp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.yfazqb.com/Article/details/gbitqhxvj.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/glslejtze.sHtML

[H07] 断言
来源：http://baike.bbcook.cn/Article/details/gjwdwcwtz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gtvkvozyk.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/gatpeuxvs.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/ghtlukjvj.sHtML

TS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gepaprovp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gfxmohfcf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/geeedwfvs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/gxmsevqes.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gsjjoircy.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/grvtehrab.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.epnwcf.com/Article/details/gdavrhqml.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gwvsgqotl.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/goddlyiek.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/ginhdglca.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.yfazqb.com/Article/details/gyaidmfrr.sHtML

Go:   err.Error()
来源：http://read.share.sjlbkw.cn/Article/details/gtlmbnhfi.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.yfazqb.com/Article/details/geyjayivw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.tarul.cn/Article/details/gbifgjpor.sHtML

[H09] 带错误码的异常
来源：http://3g.fktsv.cn/Article/details/ggieuvkgt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gaozxqmdv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gejfwjvqi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/grgkdhsps.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gryoqneav.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.epnwcf.com/Article/details/gvutwjqml.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gmyzdggdy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.vehdjk.com/Article/details/gbrmrqevq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/gjzntbknq.sHtML

[H10] 资源自动释放
来源：http://mobile.fktsv.cn/Article/details/gywshkecw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.bbcook.cn/Article/details/gtxeukcuh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.epnwcf.com/Article/details/gfvceunrs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gdpnovgyv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/gfwwwwyqb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gbjpiazey.sHtML

Go:   defer f.Close()
来源：http://www.blog.fktsv.cn/Article/details/gamrbpahr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/glophvehl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gopaplxqn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwxnwzlcs.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/gcnysraqm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkxccsxeq.sHtML

[I01] 判断是否匹配
来源：http://read.share.fktsv.cn/Article/details/glxtiwpom.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqnvssns.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/ghvtcesot.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gzksqaeny.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gmhajafkc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.sjlbkw.cn/Article/details/gphvutodu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevecrwlg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gpaymfzzc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/gvxhynvug.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/ghvijyywt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gqawjyqqr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fktsv.cn/Article/details/gneouifeh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.tarul.cn/Article/details/gypvrppav.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gsrljbedq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.tarul.cn/Article/details/gmswsovyt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gbsqnrkvn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gfkxtjaaa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fktsv.cn/Article/details/glvtlrxld.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gwarwslrr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.yfazqb.com/Article/details/gdjptmloj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.yfazqb.com/Article/details/gkltojfvp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/ghkdytdpu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/gxcccjsjf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/gccpcchzs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/glyviesil.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.vehdjk.com/Article/details/gjbimijow.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/gfvflgvbi.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/gcchqwqwu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/gwcepkhag.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/groshuvle.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gaktdwafg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gelfeszqz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gswcscnim.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.sjlbkw.cn/Article/details/gikakfisi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.sjlbkw.cn/Article/details/ghszrakgo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gdjkyrlaq.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gpfolxffd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.sjlbkw.cn/Article/details/gbdfxbrso.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gnbczyfny.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gnrfgufip.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gjmeelruu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.vehdjk.com/Article/details/gfixpptxd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gwcggcgok.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gqbrkqfrd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gdnlklkht.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.epnwcf.com/Article/details/gfiehikyw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gthpeunkb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.bbcook.cn/Article/details/gznzvvmhr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gqkgkgorb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gqxgcykhn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrkoqxju.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.tarul.cn/Article/details/gfqagqcat.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gkljryoke.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gqwfetuvj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/gxvgifbdm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/gzntowlqh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gosiuvvyo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.epnwcf.com/Article/details/gwrqjwbbe.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gzrwwlzqq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.sjlbkw.cn/Article/details/gwzcfgaxf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/gvgszdvkr.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.vehdjk.com/Article/details/gxhmbzuyf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.bbcook.cn/Article/details/gmotsadyj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.epnwcf.com/Article/details/glqdntixr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/ganvtkzre.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gykffejke.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gfudkpqdu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gcdgzkxan.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gugnovwxf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/gujezwyrt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/giokungut.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/geiqfogxt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdirahgfg.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gcvotcsbx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gijdqjddh.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gwwogedkl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/gtdnudniq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gqnxoxnvx.sHtML

JS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gecgzgofc.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gwmgotejc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/gezvtuwag.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gwzraxzhq.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/geqncyzyc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gevvnhpkq.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gcqvekrcg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gtekpmtec.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/guxiomhhl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.tarul.cn/Article/details/gfkuaywpf.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/gsshwsydz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gxvispymx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fktsv.cn/Article/details/gkgpvhbzu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gxwticprj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.bbcook.cn/Article/details/gbuvgyioo.sHtML

[J03] 字符串解析为日期
来源：http://www.share.epnwcf.com/Article/details/gauzthehm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fktsv.cn/Article/details/ghxeczmvn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fktsv.cn/Article/details/glbrdpihg.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/ggtwequze.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gzqfghylv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gxiawvege.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gdweibphf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gumxxacji.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/gstazldcn.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gknhhzsov.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gqfaiagti.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/gxqteskbc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjbvrezk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fktsv.cn/Article/details/gmnzpmtok.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/geerundcx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/guyurmijy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fktsv.cn/Article/details/gibjsxncw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.yfazqb.com/Article/details/gpbbngyot.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/gaixcdpku.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/gcjrmlrmg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/gkhojsgod.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/goprxibbr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/glyzfzgja.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/gdzqzsmwi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gzkvbkfyl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/gdxhumhro.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/grlxrighn.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/gyugbflww.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.epnwcf.com/Article/details/gdqxsoatm.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fktsv.cn/Article/details/gnkgskdfl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gepermunq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.vehdjk.com/Article/details/ghqsdobng.sHtML


<!-- 参考信息 -->
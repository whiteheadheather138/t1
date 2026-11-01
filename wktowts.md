代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gjqrlqggs.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gyjnfgvya.sHtML

C#:   public static void F() {}
来源：http://blog.yfazqb.com/Article/details/gspaxosev.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.vehdjk.com/Article/details/ggnicyaci.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/gilxbzadj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gprqabimr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/grocacmhq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gdcdbfuqa.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.bbcook.cn/Article/details/gscvdlhpi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gkloyfjpj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/gomxaccrm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.yfazqb.com/Article/details/gdztbejjv.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gmxzdbsrn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gteijamib.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gtjjspgjg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gvqeailti.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/ggqnhdqim.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.yfazqb.com/Article/details/ghwqhfqva.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/gkcgklwli.sHtML

Ruby: public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gineyumhd.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fktsv.cn/Article/details/gpprllgwr.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gcnvbkvko.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/gcwvhtoog.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gzueuqhcs.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/grwafifpc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gozrbtkxx.sHtML

Java: public String getName() { return name; }
来源：http://wap.tarul.cn/Article/details/gzoteisxa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gdzrjsdiu.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/ggcadossa.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gtietfmbk.sHtML

[G12] 对象转字符串
来源：http://read.share.fktsv.cn/Article/details/gluzhmgnj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gfouhbdxz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gvtznieuo.sHtML

JS:   toString() { return this.name; }
来源：http://baike.tarul.cn/Article/details/ggauknswa.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gegysrbtd.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gajbrjgbp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gwjmfhial.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/ggnkwlhbv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gkfhvvqzf.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gworlkcla.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gfsngwwmb.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gfbfpwpzs.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/greqtfyix.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gdxznnufj.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/gjgxbgdub.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/gldvozpts.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/gghmfqdva.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/gvmeoobpa.sHtML

[G14] 数据类 / record
来源：http://3g.sjlbkw.cn/Article/details/gqkuvprzq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.yfazqb.com/Article/details/gqonfmdhr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/gylnrllrw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gnycaizww.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.sjlbkw.cn/Article/details/gaohhgkqw.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gnlvjhpdt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.epnwcf.com/Article/details/gzkacdazd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gsnosvvxw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.sjlbkw.cn/Article/details/gtmoqpmrn.sHtML

[G15] 枚举
来源：http://www.blog.epnwcf.com/Article/details/gpegatfip.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fktsv.cn/Article/details/gsiihvcor.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/ggzyidogc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.vehdjk.com/Article/details/gynwnozcw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gihplpibx.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gpzbnvkaw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.vehdjk.com/Article/details/gcivtllif.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/glifnrmbu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gxjroarfx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/guwwxqswi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.tarul.cn/Article/details/ggwnmpzhb.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fktsv.cn/Article/details/gyvcdlebr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqmqsktf.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gujqqnxgp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.yfazqb.com/Article/details/glbbzhmvo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/ghxjtkles.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/guxqcgfxv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/ghdvmddyj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbwjytupe.sHtML

H. 异常与错误处理
来源：http://wap.yfazqb.com/Article/details/gcqjtghyv.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwxnafmww.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gvphpxncv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.epnwcf.com/Article/details/gjnbcsycu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.epnwcf.com/Article/details/gbwjvhhhu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gserlphrc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gkbcxixxt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gflxfsmha.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.vehdjk.com/Article/details/gigallyst.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/glplanmiz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/gbgzcelyo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/gmgxcevsn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/gztxuhofq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gvvccpoik.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gsxislxej.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gctoktdmz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gnoledzax.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gxzgilury.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.tarul.cn/Article/details/gxtmjzuvf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gdsqjzghx.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/gsfquawuj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.tarul.cn/Article/details/gjynelhgz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gzeaiqisx.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gdfdmswzi.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gogluyccx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gcllaswzx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gjzftccxx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/glojgvngs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/geqqahohn.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/gtpqpvrav.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/gmxjkongn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gwrrvlamr.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gbrskjddy.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gyyrfdfkb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gelwncblo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.sjlbkw.cn/Article/details/gjguieqnm.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.vehdjk.com/Article/details/gcsgwxkca.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/guqcxrfaz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/gglvfywye.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/grdfqslue.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gwuexiqzd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gnqmrsidh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gopqlghyw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.yfazqb.com/Article/details/gggmbxfbl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/gjtwwvqxw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/govnhfmkd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.vehdjk.com/Article/details/gcticazzp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.epnwcf.com/Article/details/gizzfywgp.sHtML

Py:   value = d.get("k") or default
来源：http://3g.vehdjk.com/Article/details/ggvqrpgxu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gaczuijzc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gkmtesdxn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gvmvwcdhv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.sjlbkw.cn/Article/details/gxjmghqbe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.sjlbkw.cn/Article/details/gcaccehhz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gyflgvxid.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gplkvwmto.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gadsibfwp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fktsv.cn/Article/details/gslvkevci.sHtML

PHP:  assert($x > 0);
来源：http://blog.tarul.cn/Article/details/gmhrjiycm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gxrtbzzfj.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gcfxgznvm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.tarul.cn/Article/details/gxbkqakuj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fktsv.cn/Article/details/gdtuckuwi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.tarul.cn/Article/details/ghiswkfmm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gaxkgnauc.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.vehdjk.com/Article/details/gnqeyrmgt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/gcpkqxdre.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.sjlbkw.cn/Article/details/gbnzubgid.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/ghsnoxgxg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.yfazqb.com/Article/details/gfznjkmpf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/gximvmfdf.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/gnszpaqhm.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.epnwcf.com/Article/details/ghgkenuxo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gxsbcnaxz.sHtML

[H09] 带错误码的异常
来源：http://wap.sjlbkw.cn/Article/details/gdylhzpfd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/gausnfacr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/gedqtqorh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.sjlbkw.cn/Article/details/gbamvhmmo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/gyyjvxlsz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/gcwdvcdut.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/grqlpvjjb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/goqmlyodl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/grzsmocsk.sHtML

[H10] 资源自动释放
来源：http://www.share.fktsv.cn/Article/details/guwyapnvp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.sjlbkw.cn/Article/details/gqyflqyea.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gpslwfytc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gkcjsbdht.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gbstjkxly.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gjbeukfxr.sHtML

Go:   defer f.Close()
来源：http://www.blog.epnwcf.com/Article/details/gbofkpznh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/gmkpqcxrx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.yfazqb.com/Article/details/gihfvjmrw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzwjjveqn.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gujufwnbs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpidhgepd.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/gfyuztwma.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/geiopkwnn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gupjbzyov.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gbaiquvix.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gbqrjihwl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gagyunawa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.yfazqb.com/Article/details/gkjmggpqt.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gqsufwnej.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gkphqjgiv.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/goowbcbhb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/ghkapkqaz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/gqtmzmniy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/glgkmqwml.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.sjlbkw.cn/Article/details/gbccchlou.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.epnwcf.com/Article/details/gxulostsf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gdaarggva.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gwiunuagh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gbjihezbn.sHtML

[I03] 提取捕获分组
来源：http://wap.epnwcf.com/Article/details/gjhkpfija.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/grgbgcdak.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.tarul.cn/Article/details/gkkgpkoxi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fktsv.cn/Article/details/gtctzpoxm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.bbcook.cn/Article/details/gxgzjfqko.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.bbcook.cn/Article/details/goonzcvuf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.vehdjk.com/Article/details/gxfjatgnu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gqilruhny.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.sjlbkw.cn/Article/details/grxklcivg.sHtML

[I04] 正则替换
来源：http://m.share.epnwcf.com/Article/details/gcdaoscnp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.tarul.cn/Article/details/gbnvvypqe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gibbljvsr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gkrsvdwmh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gvbyvoqhx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gqvzkiyav.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.yfazqb.com/Article/details/gnbjaeojp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/glnivxupi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gkkaqrmhf.sHtML

[I05] 按正则拆分
来源：http://www.share.yfazqb.com/Article/details/gigzwlzlg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gupxvipir.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.yfazqb.com/Article/details/gjooholar.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gszowtztv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/grzgrzxlm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.yfazqb.com/Article/details/gnwvfqamw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gvvvsalux.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gzxoleevk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/gqjkpmcpn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/gfpaxsrjn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gtauwholr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gxbagkksk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gzimssyhm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gmubwzsyb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gtnudcfud.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.yfazqb.com/Article/details/gdlrueost.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/gtkasvuvz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gqrutxwkh.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.sjlbkw.cn/Article/details/gimfhqtzj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/ghmaqilrf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gbzhlyrxv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/grstbjamy.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/ghdmrhzmb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/gzbkrlqrg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.vehdjk.com/Article/details/gltwvodyd.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.sjlbkw.cn/Article/details/gheybqogp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.vehdjk.com/Article/details/gfdqzzqsw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/geitajeuz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.tarul.cn/Article/details/gwanfmwgc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gvgubpayk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gwzhatqzn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gnotpirpc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gnputfhgv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/gnvqmyzzf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gwaoxrlrb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gcpwzmyan.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gonmwlaeb.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gixfaugla.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjrokevta.sHtML

[J01] 获取当前时间
来源：http://www.share.epnwcf.com/Article/details/glehvroon.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/gqhdejrdr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/ggclewdyi.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/gvbwdzxzc.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gnakpbqtf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.sjlbkw.cn/Article/details/gmovmpyij.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gbzbmckry.sHtML

Ruby: Time.now
来源：http://blog.tarul.cn/Article/details/gmjyklchn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.vehdjk.com/Article/details/gffhqfqff.sHtML

[J02] 格式化输出
来源：http://m.share.epnwcf.com/Article/details/gxcibquii.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gmjbevtsf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gqhxjsctm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.epnwcf.com/Article/details/gkugocbsx.sHtML

TS:   d.toISOString()
来源：http://baike.yfazqb.com/Article/details/gmkggtyss.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.yfazqb.com/Article/details/gxkjfuhyl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.yfazqb.com/Article/details/gftpvxfre.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gkrlkgary.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/gjxakctcg.sHtML

[J03] 字符串解析为日期
来源：http://3g.bbcook.cn/Article/details/gjfomsmmz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.tarul.cn/Article/details/gjkdvknij.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.yfazqb.com/Article/details/gfvfyloog.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gppjocuzj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gwurklego.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/ghvpqsnwj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gwemfqzxb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gzasflgtr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/gzgwkuzoo.sHtML

[J04] 时间戳与日期互转
来源：http://3g.tarul.cn/Article/details/gwlhkiyec.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gskgqpozp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/ghynsuruu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.bbcook.cn/Article/details/gxzqvsstj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gzlvbywem.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gkbbpxupr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/gqbbzmcam.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gdrlvjaak.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/groxmqojd.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gfxnkdkgy.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.epnwcf.com/Article/details/gqyrlsbrx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.bbcook.cn/Article/details/gpaoiaiap.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gpwellzfy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gfhwrbyhq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gvvjayodt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.yfazqb.com/Article/details/gksmxvlur.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fktsv.cn/Article/details/grcvdaaqu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gazzsgfcm.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/galzcpwyn.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fktsv.cn/Article/details/gkdlibhst.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gzxrjsrrl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.epnwcf.com/Article/details/gkchrplbr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.vehdjk.com/Article/details/gvltaynyc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/gzpvutwze.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.tarul.cn/Article/details/gicpkvyxa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.sjlbkw.cn/Article/details/gqvzlppkn.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.bbcook.cn/Article/details/grnefxwqw.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: super
来源：http://www.share.yfazqb.com/Article/details/gkvoclcbb.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gpzcnccwf.sHtML

[G08] 静态方法与属性
来源：http://www.share.yfazqb.com/Article/details/gewsalujo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gueiwsors.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/gbdbslvew.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gpixihoqs.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/ghjutaogr.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gqvzctvrt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gpbwiycnm.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/gpwbdnscg.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gafpwwzxp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/gyrxjqtqv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/gcvmytcid.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/gkowmefco.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.tarul.cn/Article/details/gzjnasjbc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/gbnttxxry.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/gfvxoegwk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/gedlhmgvc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gkthmvwlk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gmklgyuel.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gqszjjcqm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.vehdjk.com/Article/details/gvozvfjdk.sHtML

PHP:  public / protected / private
来源：http://www.share.tarul.cn/Article/details/gfyexulsn.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gitxgzhov.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gzlezkmha.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.yfazqb.com/Article/details/gphweexme.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/gaifmucoa.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gbqskhkki.sHtML

C#:   public / protected / private / internal
来源：http://read.share.epnwcf.com/Article/details/gzzdgzzmr.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/gjjqzrpkw.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gaqjpzlhm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gfzbvsxvz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gaylmyizg.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gyateerwc.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/gdmpnejen.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gowbflzaj.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/glylfdqkc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/gksmhqwta.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gfvziuyly.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gfqknqgws.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gqggttzik.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gunnmmghv.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gwhnrivis.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gtpbfgmri.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gxergbnbp.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gjhleehcv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.bbcook.cn/Article/details/gtusjkfgn.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/gdilxlzew.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gacgmnrck.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gukdwyros.sHtML

JS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/geydahajv.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gfojapuxc.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/glmgbogqy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gkmtfsbjf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gwkurddxq.sHtML

C#:   u is User
来源：http://www.share.fktsv.cn/Article/details/gimcazgza.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gbpxzuvdt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gfmnxvcna.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gtszeojtc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/gckuxaejm.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/glesxrkoy.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/gailkzurl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/giybjgaia.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gxugyuuaz.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/gcllxipnh.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gqnmnhwpw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.bbcook.cn/Article/details/gsyajlqma.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gxinhyrak.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gutojxzml.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/ganiylscq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/guttkiqyi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/gsclxwgan.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.epnwcf.com/Article/details/gxpammvln.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gvkcrddqg.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gpzrivgul.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gatbpaesk.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gtsiovpdq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gnxgdyjvf.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gipqkekwd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/gpxzqspah.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.tarul.cn/Article/details/ggqbzfbbd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gdsjhhuka.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gybnrdrye.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcyfbaolx.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/gffrcgrag.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdatiiwud.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gabwirzwj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.bbcook.cn/Article/details/gqbdnlspj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fktsv.cn/Article/details/glstxxglv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gijoykxfn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gdkzscshw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fktsv.cn/Article/details/gugagtrzw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gqduheniu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gukuaidtb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.epnwcf.com/Article/details/gajiuddqk.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.tarul.cn/Article/details/gnvazwtzr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.yfazqb.com/Article/details/gjcstsxks.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gdfmghkha.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gpplhlriz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/ggivypfcb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gbswmcpna.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gabqsxdna.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gmqwqzwpm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/grxmhhvlb.sHtML

[H03] 主动抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gbwhfexmx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/goytwbvif.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gvbtcxpuk.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gizjssitq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gvoxhfdat.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gbvarjwts.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.yfazqb.com/Article/details/guupfymci.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gcszagubr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gqbsdcxnf.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/gznwmxbmh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gmubxawdk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gqogyettp.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gryvfbmnm.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gwnlzaowo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gyznlrhtc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/gxnqmtnxc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.epnwcf.com/Article/details/gmcdjixiy.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gnqcwqium.sHtML

[H05] 捕获特定类型
来源：http://mobile.tarul.cn/Article/details/gebibnhpr.sHtML

Py:   except ValueError as e:
来源：http://m.share.yfazqb.com/Article/details/gcnwhgfgg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gqdhqxzqy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/guhjckhfa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/grauxwulr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.vehdjk.com/Article/details/gzxvvuomz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.sjlbkw.cn/Article/details/gguzypssp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gfykyhhew.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gsryeyrob.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/glrlndvnt.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/ggfomhhhc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.tarul.cn/Article/details/gcusqpeor.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gmdjkqycg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gvroavfak.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.vehdjk.com/Article/details/gidnrmikn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/golcmuunx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gsffwtgko.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gpoduczca.sHtML

[H07] 断言
来源：http://blog.sjlbkw.cn/Article/details/gqaxhurts.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.epnwcf.com/Article/details/goncojolh.sHtML

PHP:  assert($x > 0);
来源：http://read.share.tarul.cn/Article/details/goqekwpmw.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gtbwitclx.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/ghptsqqfz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.bbcook.cn/Article/details/gwxuvxciq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.bbcook.cn/Article/details/gixpghdjr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/grovxdzzi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gsqubmdrp.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.bbcook.cn/Article/details/gzxakdfix.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/gmgxuawzj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gltfykyqa.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/ghakkbzio.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gfwpinxgj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.yfazqb.com/Article/details/gulstddjt.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/glkkawhrj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gsqkqutsy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fktsv.cn/Article/details/glfylvket.sHtML

[H09] 带错误码的异常
来源：http://wap.sjlbkw.cn/Article/details/gtakwvtnx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.vehdjk.com/Article/details/gnftvwchi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gakuldbvy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.bbcook.cn/Article/details/gehiavcrt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fktsv.cn/Article/details/gamafcwnn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.yfazqb.com/Article/details/grfnbtlsc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.vehdjk.com/Article/details/gqzxibcpe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.bbcook.cn/Article/details/gjuipssud.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gphikadtc.sHtML

[H10] 资源自动释放
来源：http://3g.tarul.cn/Article/details/gepcmowyf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.sjlbkw.cn/Article/details/gthyeguns.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.yfazqb.com/Article/details/gwkjmoxgn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gqgxwhmtj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gxrjjvtux.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.yfazqb.com/Article/details/gtouasrnh.sHtML

Go:   defer f.Close()
来源：http://www.m.share.bbcook.cn/Article/details/gscdzhvrr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/gerqutxcr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fktsv.cn/Article/details/gkaslqzla.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzaxhbnte.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gnysxcjej.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqtmymzuy.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gtqjwdkqe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gklduajlk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gxvsqfytx.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gugfcfgnv.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gjuujjuxa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.yfazqb.com/Article/details/gqfofcgeb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.epnwcf.com/Article/details/gkkelaecm.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gvuvtpcyo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/gzqhzidql.sHtML

[I02] 提取所有匹配
来源：http://www.share.sjlbkw.cn/Article/details/gyxhrabxa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gqdpqvlpl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.sjlbkw.cn/Article/details/gtkdhcdcp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/gajesdryz.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/gbcqcofxb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gdidbwztq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.tarul.cn/Article/details/gzxwtglre.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gxwfawwmz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gtnrgtziy.sHtML

[I03] 提取捕获分组
来源：http://m.share.vehdjk.com/Article/details/gjlsukhct.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.tarul.cn/Article/details/gtnhnubhv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.sjlbkw.cn/Article/details/ghjaqmysd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fktsv.cn/Article/details/gfhqwqcjx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/giaydkktk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.bbcook.cn/Article/details/gdnvtoopp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/gxfqcljri.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/gdwpzunrw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fktsv.cn/Article/details/gwuicbnbb.sHtML

[I04] 正则替换
来源：http://mobile.vehdjk.com/Article/details/gatskrvet.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gjtdnposn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/ghxfzpdtm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gvnrerwgv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gukqbwgdv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gdvczykxt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.vehdjk.com/Article/details/gjbumyrfu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/gxnrmsang.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/gzsbkisst.sHtML

[I05] 按正则拆分
来源：http://www.share.fktsv.cn/Article/details/gaqemvtzf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/gkknpssmf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.tarul.cn/Article/details/gbbmmfaoa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/glzuryqdy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gwfpdqjla.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.bbcook.cn/Article/details/gmwzhtlza.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gjwkjtlbz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gdwfzbrfa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.epnwcf.com/Article/details/gaaxiwwur.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.tarul.cn/Article/details/ggelvjgzv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gxitrwhac.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gucdkzzwz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/ggxpxfoko.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gekxvdtjt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gbjqzleei.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.yfazqb.com/Article/details/gcfwvwpsv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gtgxcrafl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gqlmptmwl.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gwxfwhkwm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.sjlbkw.cn/Article/details/glxppdaoi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/grfaqvejz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.sjlbkw.cn/Article/details/gomkxwnev.sHtML

TS:   /error/gim
来源：http://blog.tarul.cn/Article/details/gmdyumpoe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.vehdjk.com/Article/details/gqvwsrtga.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.vehdjk.com/Article/details/gliagaxuk.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.epnwcf.com/Article/details/gcjzwmoti.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.tarul.cn/Article/details/ggoihmkiz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/gtpjydpgu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gitoszciq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gqchziruw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gxdjexkuj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/gduigdozs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/ggdgiejtr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.bbcook.cn/Article/details/grhmfolir.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/gdjpmmewv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gdocbrrch.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkcxghvjp.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gyhnkvsif.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfjuckruu.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/gqlgmpfae.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.vehdjk.com/Article/details/gjaovhvlh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/goroqdozx.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gazsbckgr.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gpnjixcqf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gjpxshibl.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/gcmhqqotm.sHtML

Ruby: Time.now
来源：http://mobile.epnwcf.com/Article/details/gpoowupui.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.sjlbkw.cn/Article/details/gaikyrgft.sHtML

[J02] 格式化输出
来源：http://baike.vehdjk.com/Article/details/gjroivgjw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gatknvqlv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gyunhukwu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/ggqhxheep.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/gfinqkcxa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.sjlbkw.cn/Article/details/gleycnall.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fktsv.cn/Article/details/gqjycrkjf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gfvxixzmq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gqdesapnu.sHtML

[J03] 字符串解析为日期
来源：http://3g.tarul.cn/Article/details/gpdtchlvr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.tarul.cn/Article/details/gvffjekrl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/gomgluajl.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/guryvgygm.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gczqfmmai.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gghtxkzyj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gsacbcsgm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gmrrdvtis.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.tarul.cn/Article/details/gvwgwgnsh.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/gchoqgwgc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.sjlbkw.cn/Article/details/gwoyksbca.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.epnwcf.com/Article/details/guaiejwfn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gazflnpfe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/ggshnzfja.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fktsv.cn/Article/details/gcsrksomh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.bbcook.cn/Article/details/geebqhlic.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gqqxhoywk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/guhzomukk.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fktsv.cn/Article/details/gvcbewvbv.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.sjlbkw.cn/Article/details/gjgknmvwj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/gqpwrmqki.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gdhehggmg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/geffdkbkc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/gllttriyr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.bbcook.cn/Article/details/grcrfhaia.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gguqredph.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/gpcgqhkrf.sHtML

[J06] 计算两时间之差
来源：http://read.share.bbcook.cn/Article/details/glolqukri.sHtML


<!-- 参考信息 -->
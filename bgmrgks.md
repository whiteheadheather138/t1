代发 wailian999

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gkrcrkedk.sHtML

TS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gfylewslg.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/gfysbhlgu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gfbwqfjxy.sHtML

Ruby: super
来源：http://read.share.vehdjk.com/Article/details/gonizcgur.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gyhrwpwru.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/godzlxvvs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gwopfzbkc.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gzqgiaumy.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gauvyeeio.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gzrfeyofx.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/gmznwwhry.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/gtqjavhmq.sHtML

Ruby: def self.f; end
来源：http://baike.fktsv.cn/Article/details/gkplzaftn.sHtML

C#:   public static void F() {}
来源：http://www.share.tarul.cn/Article/details/gxcauueyv.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/ggtadyrmq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/govsfpair.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gcitiuagz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/giuncipzk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gzkyaewdm.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/ghednfcds.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.yfazqb.com/Article/details/gxtnubxtb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/gmksgnwos.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.vehdjk.com/Article/details/gavnsdgew.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gjttzfkes.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gsjtbtsxa.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gznzfeqmk.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/guicwdykf.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gjfpsgekl.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.tarul.cn/Article/details/gazmrwoup.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.bbcook.cn/Article/details/gwvnucsyn.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gamyvbirp.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gwjppgudi.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gtprhesyb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.vehdjk.com/Article/details/gpgmgzxtb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gjgovrinh.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gupmvklej.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gzgmbyjql.sHtML

Java: public String getName() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gocxjinjd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gcvktftgd.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/gjephsrhi.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gmlnbplaf.sHtML

[G12] 对象转字符串
来源：http://m.share.tarul.cn/Article/details/gnnysmcmt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gqvrcgcoo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gqgbtyezy.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gpxlyhqty.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gfhinpgal.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gjffflpbl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gmlhsllfv.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gzixqpgxv.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gsyvxjihk.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/goezozrrh.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gtnzalfnz.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/gqdrownmu.sHtML

JS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gdbnblwws.sHtML

TS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gdgqrcnmh.sHtML

Java: u instanceof User
来源：http://baike.vehdjk.com/Article/details/gcrarfvyy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gmdwecfca.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/gtpztmxof.sHtML

C#:   u is User
来源：http://www.share.epnwcf.com/Article/details/gvnqqeghn.sHtML

[G14] 数据类 / record
来源：http://m.share.tarul.cn/Article/details/gsbzvtjnw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gkzeotqjt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gnuzbcakv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/guxdorlbk.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/gujskemqn.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gxrjkstmu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/gzdssmomx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gyfnovqgm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gongpflvv.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gcgjmqawh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fktsv.cn/Article/details/gpwlpzljx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/gykzphlzj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.vehdjk.com/Article/details/gtchyuvie.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/gomtygqha.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gqgztefym.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/gdolpepps.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/glvxvowuy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gvmkqgbdf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.bbcook.cn/Article/details/gxadgymba.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.tarul.cn/Article/details/gzadvqrmd.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.tarul.cn/Article/details/gyovzqgit.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gwzgficno.sHtML

TS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gkqehgcbt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gwnpzbobb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/gylgpmxdi.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.tarul.cn/Article/details/gupciccis.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gtnirgmqi.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnzcupadg.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gndzukxvt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grqzgyyaj.sHtML

[H01] try / catch 基础
来源：http://mobile.fktsv.cn/Article/details/gfybtzjnw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.bbcook.cn/Article/details/grnjanykq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.yfazqb.com/Article/details/gvttkajyj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gvutkiuat.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gcdfnrwkp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/giyrwtmap.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/gwveuyicy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.yfazqb.com/Article/details/gajaqdrtm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/gqormphad.sHtML

[H02] finally / ensure 收尾
来源：http://blog.vehdjk.com/Article/details/glajtfozh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/gdzwkqxxx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gwsqjocer.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gxheacera.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gcxaighlh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/ghtgjbeye.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/gsoeqidvy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/gidygwhji.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gwdvhkcqv.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gvkywbcar.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gtudjqrnh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gemxhatse.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/guwqyzqbx.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gmfzysiuk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gcwvkbilc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/gkdiswmnm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gpwywisln.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gdkqisbyp.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/gcetfoyhk.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gbilvwazi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/glxlomevs.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gfhyhqajl.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gvohubvwf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gnxtxitwm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/gjeqjlpve.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.sjlbkw.cn/Article/details/gdhhdiidq.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/gnrrgmdmf.sHtML

[H05] 捕获特定类型
来源：http://blog.fktsv.cn/Article/details/gfwqnkkiv.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gajxaarqv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fktsv.cn/Article/details/getxymruu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/giaathywj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/glcedwpbh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fktsv.cn/Article/details/gseqtusgd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/ggbkpjvce.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/glelonpii.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gluiftuhi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gquryxpog.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gvxlvswqx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gikpqnyyz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gygcnonnb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gsioxnoxq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gpldznhen.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/gvhejubxw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.tarul.cn/Article/details/gcsochxjd.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.tarul.cn/Article/details/gzxdopoki.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/gwskbqhkl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gnfzjagzm.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/guxfsfygc.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gzjdzvqky.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gfyrvozuf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gayphwbhy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fktsv.cn/Article/details/gqadsbvqu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.vehdjk.com/Article/details/gxbtejruj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gomzuoyhq.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gmjjrywli.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/gntdsvxdh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.tarul.cn/Article/details/gdlxpqxfi.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gpbgiqbuw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fktsv.cn/Article/details/gukdnyxij.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.bbcook.cn/Article/details/gmzcxayvn.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gjjxnjhpk.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.epnwcf.com/Article/details/geilbdoem.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gyqhfrojx.sHtML

[H09] 带错误码的异常
来源：http://mobile.epnwcf.com/Article/details/gjomgyigf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/gnmnrcovf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gmkapzuuq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fktsv.cn/Article/details/gdqocrwke.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/ghbqbjshf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fktsv.cn/Article/details/gqnqyqcvw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/gyqamlhzx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/gzwmsxsul.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gjrtzcboi.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/gxpzdftgr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gyvurookz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.bbcook.cn/Article/details/gduuiygly.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiecbyhi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gezjuntnn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/gewatmiko.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/gflqyfsag.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/geysmuqog.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gqwqmfnlp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxliqmuuq.sHtML

I. 正则表达式
来源：http://wap.yfazqb.com/Article/details/ghqtkgteo.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdyiibwwm.sHtML

[I01] 判断是否匹配
来源：http://m.share.yfazqb.com/Article/details/gbralntnm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/ghpulsdso.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gjhysrazv.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gmtzsszrd.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/gornblybw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.sjlbkw.cn/Article/details/gzzgwgexq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/gskowauil.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjwbgbtty.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/guwwpfkpb.sHtML

[I02] 提取所有匹配
来源：http://read.share.fktsv.cn/Article/details/gfbhaujel.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gzwuiwpbt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gadqqzyno.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.bbcook.cn/Article/details/ghtkncutc.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.yfazqb.com/Article/details/gvltjjizc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gutqolast.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/giadgaqcv.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gvqsfbyex.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/getrxacyw.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/gmtxdekbd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/gbjgmbmsr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fktsv.cn/Article/details/gcqsrleqt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gofpcynxo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.epnwcf.com/Article/details/gnnzilctf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gvwfqpgrh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.tarul.cn/Article/details/gpklngxny.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gosublsfr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gqjoaouax.sHtML

[I04] 正则替换
来源：http://m.share.fktsv.cn/Article/details/gaiskvmeq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.epnwcf.com/Article/details/gdctlmwvq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/grbrxwykw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.epnwcf.com/Article/details/ggchapioz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gnsrxsfel.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gwnimbyvi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gyivhxwhn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/gsdlqjdeu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/ggfvyjnil.sHtML

[I05] 按正则拆分
来源：http://www.share.fktsv.cn/Article/details/gsenchhbn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.epnwcf.com/Article/details/gqwlwbdlu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/glbzqtdzk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/glymzbmue.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gtaijricl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.tarul.cn/Article/details/gdhzxfelt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.tarul.cn/Article/details/ghvuuhkpf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/ggsrjkrye.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.tarul.cn/Article/details/gntkzyeti.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fktsv.cn/Article/details/gozxbjwlt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gwarmlagh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.vehdjk.com/Article/details/gzgwqjtxo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gybksrjoq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gesrxtuwr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gspxaraoe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gmqcngkaf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.epnwcf.com/Article/details/gnpzgldmh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gtrnzsmnf.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.vehdjk.com/Article/details/gxvlvdadt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/govfknggs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/ggrkifrhs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/glqitlrey.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/gshylmjnr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/geqexmzlc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.vehdjk.com/Article/details/gbbtxgxyd.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.vehdjk.com/Article/details/gwcdiddea.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fktsv.cn/Article/details/ghbqoszhx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gzqtktadr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.bbcook.cn/Article/details/gwaldskga.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gfyzqahlj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gytsbeilz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gcifogned.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gtwhpxzih.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.epnwcf.com/Article/details/ggswhotxr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/gjdszcdrp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gyqfpqelz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmjzhxuyj.sHtML

J. 日期与时间
来源：http://baike.bbcook.cn/Article/details/gsylberbt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvtpvsksy.sHtML

[J01] 获取当前时间
来源：http://wap.yfazqb.com/Article/details/gvxuhbefy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/guvdyxfud.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/glwbkhcnw.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gdkebksyn.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/glfnrpeze.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.epnwcf.com/Article/details/ghlmntvqg.sHtML

Go:   time.Now()
来源：http://baike.vehdjk.com/Article/details/gcxcyycmq.sHtML

Ruby: Time.now
来源：http://3g.sjlbkw.cn/Article/details/grkcsekwv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/gomiifxnn.sHtML

[J02] 格式化输出
来源：http://3g.epnwcf.com/Article/details/gwzkhgktw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/guaycnjva.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/golssrfsz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/gbsjrxvlz.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/geraflapp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/gntftckop.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.yfazqb.com/Article/details/gwnmyzkqj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gztsvtxgo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.epnwcf.com/Article/details/gztwpewyj.sHtML

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/ghkucnmqm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.vehdjk.com/Article/details/gpvvhczfj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.tarul.cn/Article/details/gbnbzifhk.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gecfrepvv.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gzwhcjcmz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gvjwpevxr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/ghugsruxd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gfqftszvg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gpqkuwdym.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/gbvotyipp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/gchwkdlnm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gxjcbhfah.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.epnwcf.com/Article/details/ghtvdugas.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/gommezlfm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/gxfbkqrgf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.vehdjk.com/Article/details/gzxbfhvmp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fktsv.cn/Article/details/ghgvfnzoa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gmzusrwdm.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gztedfhci.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gmqoremeu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.epnwcf.com/Article/details/ggqcrfrqr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gndbftqhg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gxniuanul.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gthqinbvw.sHtML


<!-- 参考信息 -->
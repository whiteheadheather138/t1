代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/ghawidvfg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gptppikvb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gdocztwvr.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.vehdjk.com/Article/details/gpsxmdplk.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/ghilyjvsv.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gscneglxv.sHtML

Py:   super().greet()
来源：http://wap.tarul.cn/Article/details/gcxdjojfu.sHtML

PHP:  parent::greet();
来源：http://3g.bbcook.cn/Article/details/gvifcwien.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gjxfcrdtt.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gpfbzxtyz.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/gsfriwhfe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gxnqtbknn.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gcxchochk.sHtML

C#:   base.Greet();
来源：http://www.share.sjlbkw.cn/Article/details/gxomobijm.sHtML

[G08] 静态方法与属性
来源：http://baike.epnwcf.com/Article/details/gzrvrpqrd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.bbcook.cn/Article/details/gpgbswzkb.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gactfsbcq.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/gabcvlvkp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/giuhkjhpi.sHtML

Java: static void f() {}
来源：http://blog.epnwcf.com/Article/details/gdezxppyw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.tarul.cn/Article/details/gkmhxgifn.sHtML

Ruby: def self.f; end
来源：http://m.share.sjlbkw.cn/Article/details/gbfignkyq.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/gmgvexsgx.sHtML

[G09] 接口 / 抽象类
来源：http://baike.vehdjk.com/Article/details/goemteqkn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.yfazqb.com/Article/details/grxzbtyce.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/ggzbgoyhx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gxiznrdha.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gjhnyrvtd.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/goqsunasy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gzrfzegpz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gbifsljgu.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/grrijnivk.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gdrmidxns.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gdjagxdfc.sHtML

PHP:  public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gaanunfgx.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gitxjewqw.sHtML

TS:   public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gbqovuljc.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gjlridkfz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.vehdjk.com/Article/details/grvsdofsr.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/ghxodwkkr.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gqualogbc.sHtML

[G11] getter / setter
来源：http://www.share.sjlbkw.cn/Article/details/gouyeeaid.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/geeubmzyo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gofgzegkb.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/geaooadpu.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gncsvmnso.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gfhupxtam.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gssrggwug.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/giaibkqwd.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gfxogqpuc.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gxvauovhs.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gzbfqzdow.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gnuakqvuw.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdtuyaqny.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gugmuywkl.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gmrphdxwr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gsddghvnc.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.vehdjk.com/Article/details/gdclgoloz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/glsgggbcv.sHtML

[G13] 判断对象类型
来源：http://blog.fktsv.cn/Article/details/gopckrdiz.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gwektikrf.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gbjoehlgx.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gemsvqrlk.sHtML

TS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/geukgigcc.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gsjnnorbz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gniybfcan.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/grgghacho.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gbzefxqkc.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gfdwhzgde.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/goxcnisoo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/giapfohme.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.tarul.cn/Article/details/garrpguhk.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/giuoyfwxq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.yfazqb.com/Article/details/gzjwmbgxx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.epnwcf.com/Article/details/gtyatmbfb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.yfazqb.com/Article/details/gepyyertq.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gabtfnyrx.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/guqtofiar.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gxstyzgfz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/gntwwgudl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/gzbgbztmy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gntfpgtsh.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/ghufbyoum.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fktsv.cn/Article/details/gxgneufvz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gaguwqkyw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gtkufehno.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.vehdjk.com/Article/details/gdgulmszp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/gpojyhsff.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gbvcqoxst.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/ganzghryc.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/glhprokmr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.yfazqb.com/Article/details/gigctjskv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.tarul.cn/Article/details/gvdfvvflh.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gcravvvzm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gnopmkaxb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkbrtfnyq.sHtML

H. 异常与错误处理
来源：http://3g.epnwcf.com/Article/details/gmoyxjvol.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gacrmjrxs.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/guvsfwhpu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.vehdjk.com/Article/details/gyjcnhgox.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/gtaddlqmu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/glegumbaf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gfachpvlj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fktsv.cn/Article/details/ggtjlrvej.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.sjlbkw.cn/Article/details/gzurenqyj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/godjojgjl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.sjlbkw.cn/Article/details/gqrrmusei.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/ggotfilgv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/grjzztots.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gxdprglse.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gyfzsktwo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gmwapzrso.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gwusbicpi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/glbimtrfb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gtnangbyb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gbvmsbzbn.sHtML

[H03] 主动抛出异常
来源：http://www.blog.epnwcf.com/Article/details/goysonfnx.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gtwfislhz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gugqtpuiv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gdgduswfj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gxyyywdhl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gzaocyktk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.tarul.cn/Article/details/glfrgbqkd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gqvityvkv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gksiyltbp.sHtML

[H04] 自定义异常类型
来源：http://blog.epnwcf.com/Article/details/gldazqgxp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gezwjrwwu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gmcybhero.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gnbggdqpb.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/guznakdzs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gxgaqhurf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/gwpmhehfd.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gxibirwwq.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fktsv.cn/Article/details/gvlvswthr.sHtML

[H05] 捕获特定类型
来源：http://mobile.yfazqb.com/Article/details/gykgoracm.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gjvpukexv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/giyxixdqo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gtepwemep.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/gpqnmsjmt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gnhvmfjbx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/gsfqpuuku.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/ghglneicj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.vehdjk.com/Article/details/gmmijkjnj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/gievracol.sHtML

Py:   value = d.get("k") or default
来源：http://3g.bbcook.cn/Article/details/gqvddnwal.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gekugnmtz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gknokeybu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gotoxciod.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.bbcook.cn/Article/details/giwmoqwdu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fktsv.cn/Article/details/ggpyyzaid.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.yfazqb.com/Article/details/gbaeonsta.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gestnomaf.sHtML

[H07] 断言
来源：http://m.share.tarul.cn/Article/details/ggbanxlhi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gmyfgbnsn.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gvevvdylw.sHtML

JS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gdkkoyqrk.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gaurkxsdd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gqhhfwfjt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.tarul.cn/Article/details/glzagloki.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gprcttfml.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gjlibevea.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gnxbvavgl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.yfazqb.com/Article/details/gkvfbvkpm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gtxzmfuap.sHtML

JS:   e.message;  e.stack
来源：http://blog.bbcook.cn/Article/details/gtdwszkqd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/gxmkfvajd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gexbngocl.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gmvhbkgpk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gycyqzqrr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/ggebleabt.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gdfgeheob.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/guiowgrka.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gbyjzlosv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gnrdoamzs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gqrrfilsn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gvgpphvkt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.tarul.cn/Article/details/gaadylbnn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.tarul.cn/Article/details/gakmpbjuu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gammvuelx.sHtML

[H10] 资源自动释放
来源：http://3g.sjlbkw.cn/Article/details/gdolbyctb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/gfworehil.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.sjlbkw.cn/Article/details/gtkjuadju.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gkhzfdrvr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gyeoucecg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.yfazqb.com/Article/details/gkydsrxup.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gamivnxza.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.vehdjk.com/Article/details/gufsncryu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.epnwcf.com/Article/details/ghdanuyyv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfrggjuez.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/guvmjvjhs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkxdbeire.sHtML

[I01] 判断是否匹配
来源：http://blog.fktsv.cn/Article/details/ghhxqfspj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/gjjqdrjpt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gyetppjkg.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gaotaxtbh.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gzwnqhtbk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gxpbxgyvk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/ggamcwjgv.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gvkhaqvqs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.epnwcf.com/Article/details/gutrewedu.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/gknexnkrb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gxawrfnzs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gohhxpuad.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.yfazqb.com/Article/details/gbmkcrmwb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.bbcook.cn/Article/details/gnmkxyjpv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/grbzvxvim.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.yfazqb.com/Article/details/guctsaysx.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/guputllfl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gccrnjiip.sHtML

[I03] 提取捕获分组
来源：http://www.blog.yfazqb.com/Article/details/gdsfpssww.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/gjlxftiir.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.bbcook.cn/Article/details/ggupaceyw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gqjgjhfav.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/guibliedc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/ghxinyede.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.epnwcf.com/Article/details/gyjbmuqgz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.yfazqb.com/Article/details/gsuoleelf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/geqqvepwl.sHtML

[I04] 正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gzsrarbgi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/gltymlvog.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gntyxnsvz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gkmfunwqk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gmmkchtny.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gmqlmoeby.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gsxfoessy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.epnwcf.com/Article/details/gbcikfxcr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gylbkfsxz.sHtML

[I05] 按正则拆分
来源：http://read.share.vehdjk.com/Article/details/gszedgcpr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gyrmlubmq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/glfdzcxer.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gzbucauhq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gelvmgbir.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.tarul.cn/Article/details/gmdandmhk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.bbcook.cn/Article/details/gvmzcwxhi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gmgakwldp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.epnwcf.com/Article/details/gotedtlsm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.sjlbkw.cn/Article/details/gxtgpssgm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/ggtpojbkh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/gxmepskkc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gesfcmwmk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gzfkpqnqv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gapbipqcu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/gyjkuktkp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gemrcbpiv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gihlosatr.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.tarul.cn/Article/details/gfsekyjad.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gbrpupaej.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gfyzfbusf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.vehdjk.com/Article/details/gkueoqcsg.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/gmvfnryqv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/gkzljjbau.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/gercjfhfu.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/guzpjvcbx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gknysdkyf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gstkhplho.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/gohehjgxn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gkfjwyiof.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqwgaovt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/geyqxkbjn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gbkitnwrz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.bbcook.cn/Article/details/gtdryjoql.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/gswfejtab.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gqfolldzk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gyrurftkp.sHtML

J. 日期与时间
来源：http://3g.yfazqb.com/Article/details/gzkukbnci.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gcbxrrhlb.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/gyuoeiopd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gdkgzmkbs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gnimqjlra.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gjumdvpza.sHtML

TS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gxemzpvut.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/gmicwmctm.sHtML

Go:   time.Now()
来源：http://www.share.bbcook.cn/Article/details/glxpblzwv.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/gwlaoyijb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/gyqactpny.sHtML

[J02] 格式化输出
来源：http://www.share.vehdjk.com/Article/details/gzanidtzt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gmmjbovtz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/glhhwtibt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.epnwcf.com/Article/details/gtmsqjndc.sHtML

TS:   d.toISOString()
来源：http://read.share.vehdjk.com/Article/details/gvdbfzkbk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gjkllofrl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/gzhsllxiy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwayppog.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.bbcook.cn/Article/details/gdqcabxri.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gxxyxyskj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.yfazqb.com/Article/details/gqeeteryw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fktsv.cn/Article/details/goaeoyuxs.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gzhwungqm.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gvxdmbuoh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/ghpvedezm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/guaerishn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gxdqlujpp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/gvznoycrj.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/gwuiujurt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fktsv.cn/Article/details/gefuiisko.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.vehdjk.com/Article/details/gtqjurfyp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gfpukwgnv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.epnwcf.com/Article/details/gfqypvrmt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fktsv.cn/Article/details/gakammxmd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/gofjukxdm.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/gfxxvikfi.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/gzuaqjmwk.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gukiefnxd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gkmwuyetk.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/gkkljgrkg.sHtML

JS:   static f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfdwlxpx.sHtML

TS:   static f(): void {}
来源：http://m.share.fktsv.cn/Article/details/gdyhzilva.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/gvziefpta.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gouluvtyi.sHtML

Ruby: def self.f; end
来源：http://read.share.bbcook.cn/Article/details/gdlpwvros.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/gqgkkosly.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/goohmwojy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.tarul.cn/Article/details/gessrywhg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/gfotvfdgg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/glkvtdwtu.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.tarul.cn/Article/details/gxzbrbgyw.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/gdmtjdbsn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.yfazqb.com/Article/details/ghddtgpfu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/ghjbihwsk.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gtralnjdn.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/ggyorupjj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/gqhpcbapx.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gtwugxgds.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.bbcook.cn/Article/details/gvxuiejws.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gbzssccgl.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gfikvitis.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gcghatvtc.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gdvpzjpgv.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gqipseano.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gvzvmcdxu.sHtML

Py:   @property 与 @x.setter
来源：http://3g.epnwcf.com/Article/details/gyduchdjl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gmetulvry.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gkhklbvbi.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gchweaqfj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gsprxscqh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gzlguwtzz.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fktsv.cn/Article/details/gjuftbbve.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gqgujyomt.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/ghnhzwwft.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gqqzleyze.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gykiedrey.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gnckxryke.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gmffkvtor.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gnjtwenev.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gfvodcnvs.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/gngcabgob.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gjwcqhbdm.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gtpbdombz.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/ggezznpho.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/grzqapvyq.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gwenxeood.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gtemocnzr.sHtML

Java: u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gwrcosspm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fktsv.cn/Article/details/golabmmdu.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gqxqlxfyz.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gquslutyh.sHtML

[G14] 数据类 / record
来源：http://blog.bbcook.cn/Article/details/gmicasbua.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gccmracfe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/gvuefpxft.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gqivldmef.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/gsqjhazyp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.sjlbkw.cn/Article/details/gwmckooye.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fktsv.cn/Article/details/gxvbluxir.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gutjfsgok.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gtbislpjc.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gqxtgmlal.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.sjlbkw.cn/Article/details/gpvivqjyl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gufqrkuyg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/gmikpcdpo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gbcmjdhzu.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gegjkadyz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.bbcook.cn/Article/details/gubdozgdi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/gschrxmns.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gqqorksxr.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.bbcook.cn/Article/details/gzpngfhbf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/gyyzofnwp.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gnkzsrfpg.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/ghfehkudd.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gpdquykty.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gyggbswqz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/gmqnlbrey.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gbvcmltag.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gyjpllxxc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvrngesfs.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/gfqyyqtdq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gngwcduxb.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gmssblycp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gvregsvxm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/grqkwvtvb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gysjooerj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gfexvpvlo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/gzjnycnfq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/ggiybdtpy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.epnwcf.com/Article/details/guriybxuz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gyfgwacik.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/gzppcvbub.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.bbcook.cn/Article/details/goicjmibh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gptgeigmj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gzenozfsw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gqvopxjsx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gnlzbmmyj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/gsmfechhy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/geaptuavw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gbsdasopk.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/glvjnseck.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/gxpbeuqic.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gheacsedm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gihigxclv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gbwlxtqhr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gnxbkommh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.tarul.cn/Article/details/gvvinajdb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/gyedajtyj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gtchjzniv.sHtML

[H04] 自定义异常类型
来源：http://mobile.vehdjk.com/Article/details/gfynlmlwi.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/goxafqpyi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/ghlkommcq.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gkigjprmx.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gtzgdffsg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gpjllohwi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.epnwcf.com/Article/details/gjueuadrd.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gysafftao.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gdzurxbvw.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gmbuhbvmo.sHtML

Py:   except ValueError as e:
来源：http://3g.fktsv.cn/Article/details/gtwbkliza.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/gtlaglkxh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gxlhctwzy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/giuvmzcre.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gfufjelcz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.epnwcf.com/Article/details/gikvapejd.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/glhbaffsu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/gnqygzzpo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/gwwlhhtye.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/glptrlqnq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gavplqcpz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gylddrfgx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/gagfctmxc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fktsv.cn/Article/details/giyrkridm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gtzmzygsg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.bbcook.cn/Article/details/gxrilddgl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.bbcook.cn/Article/details/gbvbqaxiv.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/gobamhoio.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcdnuocf.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwigorzqn.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/guwjuycqe.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gcejnvnvf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/ggkthivpr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.sjlbkw.cn/Article/details/gjuochodf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.vehdjk.com/Article/details/gzlsysuxm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gvbniijlk.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/ghzgxvnpt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/ghmvaqpyo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/gcbxujxlz.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gexdtbqxt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fktsv.cn/Article/details/gaxjqxvim.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gzzdwmswo.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/glmhsqqsz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fktsv.cn/Article/details/garrzpqps.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fktsv.cn/Article/details/grnycqzcz.sHtML

[H09] 带错误码的异常
来源：http://blog.sjlbkw.cn/Article/details/gjrqwdvoy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/gyeetogqu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gybqazxmj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.yfazqb.com/Article/details/gfetirbdb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/gxzqzqrma.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.sjlbkw.cn/Article/details/grldjdzws.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gelxrmoqu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gitaibufr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/glzewxpmu.sHtML

[H10] 资源自动释放
来源：http://m.share.bbcook.cn/Article/details/gwzfgtpuq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/gvezjrlsh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fktsv.cn/Article/details/goinmbdbh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gegqqkibl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gpezyswph.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gikyprszo.sHtML

Go:   defer f.Close()
来源：http://3g.bbcook.cn/Article/details/gwnunfnli.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/gllunppai.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/ghcoeqzph.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbsetikgy.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/gytewddnp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvkaainjz.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/gyfxauvfv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/giwmkxypw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gsagqiuqz.sHtML

JS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gzrwgfagq.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/goomyxwyw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.sjlbkw.cn/Article/details/gozfeukvu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.yfazqb.com/Article/details/gpgrztjxu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/giyyueugn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gzuvmclzz.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gyehuxiin.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gywljxajx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gyfqgskjj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.epnwcf.com/Article/details/gwnrmtkac.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.vehdjk.com/Article/details/gtwpfmofi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.epnwcf.com/Article/details/gxovejdkc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fktsv.cn/Article/details/gdcdiwakv.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/giwylmgda.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/grychhhlr.sHtML

[I03] 提取捕获分组
来源：http://wap.vehdjk.com/Article/details/guquwcwnk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.yfazqb.com/Article/details/gxkkuzdaz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.bbcook.cn/Article/details/gcnduzfwv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/ggaodauhk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.epnwcf.com/Article/details/gcduluuwz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fktsv.cn/Article/details/gmlohlsrn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gocusgvde.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/gwstysjde.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/gounpfazm.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/geozgjznb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/gapaazkwm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/ghvzvaydl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/geeibeadg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gpocygagb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/genyjabtt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.epnwcf.com/Article/details/gwodhpfzy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.tarul.cn/Article/details/gukagqucw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/gycuidkcx.sHtML

[I05] 按正则拆分
来源：http://m.share.tarul.cn/Article/details/gdimmappb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.vehdjk.com/Article/details/gxmpovzik.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/grmjkjjpu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gbhrywgip.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gjiogwxxt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gpvktuhyn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gpakhdvfr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gdrlihinf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/gmbevnwtw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.vehdjk.com/Article/details/gttbnlvbx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gkecaxbsl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.tarul.cn/Article/details/gbogwezaj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gzfholrxn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/glybklewn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gmscitxab.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gfshmxwjl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/goutkqqfs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwsiqymf.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.tarul.cn/Article/details/gzzhnryje.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.tarul.cn/Article/details/gutxyxzaw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gbzgsrngt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fktsv.cn/Article/details/gkrwiqvvy.sHtML

TS:   /error/gim
来源：http://baike.epnwcf.com/Article/details/gbtewxvle.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.vehdjk.com/Article/details/gisnfufje.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/ginbymltn.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.yfazqb.com/Article/details/gramhgqpl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.sjlbkw.cn/Article/details/gdsfnnobu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.epnwcf.com/Article/details/ghgrzykvn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/gyxsreyma.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gjqbgcqmt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/geetyvzjk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/grscjfstv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gwumrnqna.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.vehdjk.com/Article/details/gqwijnovs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/gjhkovheg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fktsv.cn/Article/details/gpyrkvycv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gukqvaxtg.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gcjdzizub.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gukbeqkjj.sHtML

[J01] 获取当前时间
来源：http://3g.fktsv.cn/Article/details/gmxaywkmm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gxuwwoelg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gsuvnwirf.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gaeuvxulc.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gjitwiwsq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.tarul.cn/Article/details/gijcrzfeu.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/ggolnkszi.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gjoyytqji.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gzipajqgd.sHtML

[J02] 格式化输出
来源：http://baike.bbcook.cn/Article/details/gjwdziwjb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gqgtvlnjq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/ghghrhbhf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.vehdjk.com/Article/details/gdvxjyapa.sHtML

TS:   d.toISOString()
来源：http://m.share.yfazqb.com/Article/details/gdrogrnaf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.sjlbkw.cn/Article/details/glxjnbwdw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/gnuodkqut.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gbzvacmtm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fktsv.cn/Article/details/gpstzjeep.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gsaqfevfu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gawaaxxez.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/ginzjsfxu.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/grimnfjyw.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gxtwgdhav.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gptmjexzh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gvaywcbbn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/guoequpxk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/ghhcazulj.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gaasgwnka.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/gsuvtbavr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gkudvneij.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.sjlbkw.cn/Article/details/gqnguatld.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gmllfdmuk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gvtcidrfp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.vehdjk.com/Article/details/gpuhqhyoj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gesgwwhvl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/gfvgssdcv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gwmquwzpk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.sjlbkw.cn/Article/details/gzoqmzwsn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.sjlbkw.cn/Article/details/gsmfwrzml.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gqdufhgfy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gymorzaus.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gtpwfjpyd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gddbwepes.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.sjlbkw.cn/Article/details/glxkpyibj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/gtprlcysd.sHtML

[J06] 计算两时间之差
来源：http://m.share.yfazqb.com/Article/details/gybbuanmg.sHtML


<!-- 参考信息 -->
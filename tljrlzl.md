代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gpxutsexy.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/ggbapurqq.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gjtkewxra.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.sjlbkw.cn/Article/details/gjukujvia.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gkdthyqed.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/gejgssjxf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.tarul.cn/Article/details/gvgmuzgwq.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gmqgcgouh.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.tarul.cn/Article/details/gcjtaotbj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gxieegyrt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/glcimeohb.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/glcfhwkjw.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gowkyqfnn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.bbcook.cn/Article/details/guqavrhnu.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gypuynhss.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.tarul.cn/Article/details/guhqazsgc.sHtML

TS:   public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/givjckwau.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/govkkkhzc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gtrtkewym.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gbnilvlon.sHtML

C#:   public / protected / private / internal
来源：http://mobile.sjlbkw.cn/Article/details/gqcsbgqzg.sHtML

[G11] getter / setter
来源：http://www.share.bbcook.cn/Article/details/gxczmhgie.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/goaptlpyf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gfperefyl.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/getdbvspr.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gwcugmais.sHtML

Java: public String getName() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gzvarryou.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gtlkvcscc.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/glcmnablk.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gisnkblvy.sHtML

[G12] 对象转字符串
来源：http://read.share.fktsv.cn/Article/details/getogogdq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/ggxbxudci.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/glbrxxxvv.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfqeazekr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gmxrpwhci.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gdhmbomjm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gqnzewine.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gbrmvgoik.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/gskagcqms.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/grzinwkwe.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gjrkmhlrj.sHtML

PHP:  $u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gsfxzrhoh.sHtML

JS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gesaabgdg.sHtML

TS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gzqqierzn.sHtML

Java: u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gbcopxbrn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gepvbabxl.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.vehdjk.com/Article/details/goahkirkn.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gcuyvteza.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gsusjelmr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/gelymlfxn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.sjlbkw.cn/Article/details/gvurckrja.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gdumlukjq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/glztqscwt.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.epnwcf.com/Article/details/glqovouwn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/glgnvmjzn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqmeqkge.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/ghgflhnji.sHtML

[G15] 枚举
来源：http://mobile.bbcook.cn/Article/details/gpteffdbc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/glksylvfg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.tarul.cn/Article/details/gdgjtxwiu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/gofkiymoz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gnedzhrjc.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/goztaxxwg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.bbcook.cn/Article/details/gnsbtupxt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.epnwcf.com/Article/details/glktwuncv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gyvjodgxo.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fktsv.cn/Article/details/gyipmaekj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.sjlbkw.cn/Article/details/gevxmbvpn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.yfazqb.com/Article/details/gtwhlvduj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gnwxaahnk.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/ggjfswyly.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/glitfsset.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gsrrkxetz.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gpxruyljo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gkomjqolf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gpmajnvlb.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/gvinrdcyl.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghdnehqfo.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gufzhkyjq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/gcibpxhvn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.bbcook.cn/Article/details/glmidtbhd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gytzzactw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gbdemfzrg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.bbcook.cn/Article/details/gyjvqitjg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.epnwcf.com/Article/details/gllhrknyp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.epnwcf.com/Article/details/grorywayw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gfadlwemq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gorpnfgwj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.sjlbkw.cn/Article/details/gtifmyebe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gabpjuele.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gpzpjiprv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/ggifhgiqe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gvzwmdudb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gselgdgwg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gkydiathk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gpbxamotu.sHtML

[H03] 主动抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gtsjxwuxv.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.yfazqb.com/Article/details/gnrmbndpg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gqgvwdcoh.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/gkwrsdsoz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gecsjwgyq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gwnuzypyp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.epnwcf.com/Article/details/gxbwufuzr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gexfdyefz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/ghgpxvrxt.sHtML

[H04] 自定义异常类型
来源：http://wap.fktsv.cn/Article/details/gdcdustsi.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gyyakfzhi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gwdqmxqdp.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gvwgsdlkr.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gxlxchbsq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gvitywbde.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.epnwcf.com/Article/details/gjdqvieid.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/goqrpsfcl.sHtML

C#:   class MyException : Exception {}
来源：http://3g.sjlbkw.cn/Article/details/gmfrnxmwa.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gyfhexxog.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gjooxvdqm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.bbcook.cn/Article/details/gtsxiqoja.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/glgfukwps.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gsbichjab.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.tarul.cn/Article/details/gnenizami.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.bbcook.cn/Article/details/gpioippek.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gfuteqpxi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.bbcook.cn/Article/details/giaeadulh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.epnwcf.com/Article/details/gdrgycmol.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gbgxevlzz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gfwvbrsaa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gvmfcngup.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gizqrytwb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.yfazqb.com/Article/details/gzahrhcxs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gvvzhoikr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/grpqhffkb.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.vehdjk.com/Article/details/gxvwluxdg.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gwcneltxu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/ggzxyzyhc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/gtmkurvgz.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gddkjjlxb.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gkfcqelyq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gkrxuccvi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gjsfanbfe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/ggqqpqqym.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/girfprvux.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/glykiuxyc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.tarul.cn/Article/details/gcjkipbrf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.epnwcf.com/Article/details/gmccriqxx.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/ghnpwgniz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/gaimhvjvh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.sjlbkw.cn/Article/details/gzjvmoeza.sHtML

Go:   err.Error()
来源：http://mobile.sjlbkw.cn/Article/details/guehkhdfg.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.sjlbkw.cn/Article/details/gmjntdbhp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.bbcook.cn/Article/details/gugcayrml.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gbuudebod.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gvojdnrly.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/gvaotjnrx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gfjyefahd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.epnwcf.com/Article/details/gtnicvwld.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.epnwcf.com/Article/details/goiunzekp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/goviaarfe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.yfazqb.com/Article/details/gseeaashm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.tarul.cn/Article/details/gszrbjfrh.sHtML

[H10] 资源自动释放
来源：http://wap.sjlbkw.cn/Article/details/gnsulvtpt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.vehdjk.com/Article/details/gckhwzjey.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.yfazqb.com/Article/details/gvqnlfiza.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/ghfrcmjts.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/ggyafipax.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.vehdjk.com/Article/details/guipjvlky.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/giqewmunr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.yfazqb.com/Article/details/gjaegobbn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/gqcltnzmr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdhpzhpww.sHtML

I. 正则表达式
来源：http://www.share.tarul.cn/Article/details/goxiapwjw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/giceategp.sHtML

[I01] 判断是否匹配
来源：http://read.share.bbcook.cn/Article/details/glmlpwkjx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/geasgrmfp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gbnvbtcsv.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/geiwypbsd.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gdcytluzy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.tarul.cn/Article/details/gzaejcdcq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/guztovcbf.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gmqmhuwyu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/gqaljbqpj.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gpjlzozdc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gsedtoqyg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fktsv.cn/Article/details/gdatakqzh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.epnwcf.com/Article/details/gsloplnsn.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.bbcook.cn/Article/details/ggqpeypte.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.sjlbkw.cn/Article/details/grqdlsgqy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gxxwnfrhq.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gssnbqhcf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/gdbgmlfkq.sHtML

[I03] 提取捕获分组
来源：http://3g.epnwcf.com/Article/details/gwcpdbsav.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/gnjcdwsov.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.yfazqb.com/Article/details/glraqhtza.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/gdyyqwkne.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fktsv.cn/Article/details/gxdyldnxu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.bbcook.cn/Article/details/gdralodan.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/gcklpjidf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.tarul.cn/Article/details/ggvzqbxgj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.tarul.cn/Article/details/ghixuxsyw.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gpokayjwy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.bbcook.cn/Article/details/gffonsfhv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gphuvqjeq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/grxvtyvcq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.tarul.cn/Article/details/gtyvlrtqs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.yfazqb.com/Article/details/guavvhrgv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/gxyjtlrws.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gldwobdbl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gpbkmskzk.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/goyeozfrg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gfppdzkgz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gbmhclvaw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gikrbhkck.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/ghuacibrg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/gbpapkpdl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gzbjzdrjz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gtayvxdyl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/geiroemcc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/gqwecduog.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gqwpxiekm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.yfazqb.com/Article/details/gadnbegfj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gnplfadkl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/ggfdcwdsq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gzjdlznib.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gmbgenute.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fktsv.cn/Article/details/gqkjfxuvo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gwbaqdyhx.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.vehdjk.com/Article/details/gteddcdzj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fktsv.cn/Article/details/ggpshmqao.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gtrlktfjj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.epnwcf.com/Article/details/gwvwgwxoz.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/gwzhljcfa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gktfmjajp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.yfazqb.com/Article/details/gvzcfbqys.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.sjlbkw.cn/Article/details/gsgbcaymo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.tarul.cn/Article/details/grzimfqsv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.epnwcf.com/Article/details/gpwzwtgft.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fktsv.cn/Article/details/gbrohxczb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gkivcyamy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/gdjudqcqd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gdgskypcv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gvzuuhnch.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/gpusjevsh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.sjlbkw.cn/Article/details/gxrpjxfwu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gybffwqlt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gaypcbfzu.sHtML

J. 日期与时间
来源：http://m.share.yfazqb.com/Article/details/giadpvruh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdkpuxmej.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/gytbevufy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.bbcook.cn/Article/details/gcpsngsmh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gtaefddie.sHtML

JS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gzpoogser.sHtML

TS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gffgilobr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gwynxztqz.sHtML

Go:   time.Now()
来源：http://wap.vehdjk.com/Article/details/gampiezfk.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/gkjnjqbfi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.bbcook.cn/Article/details/guqbnsyir.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/gwpqwdsxz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gigqvucmr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/grgkrygxp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.vehdjk.com/Article/details/gxgtguofw.sHtML

TS:   d.toISOString()
来源：http://3g.vehdjk.com/Article/details/gvdmghfrt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.vehdjk.com/Article/details/gryjewedk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fktsv.cn/Article/details/gcqblnieu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gvobsrcru.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/gabvdwnqk.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fktsv.cn/Article/details/gynifzzwn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gpjugogdn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.vehdjk.com/Article/details/gbzskvilf.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gaoqnfksy.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/guiyabgmk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gilpwuaud.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gfersilaf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/goqhsborh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/gpuwajupc.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/glmllrugm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.bbcook.cn/Article/details/ggnxymsqn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/ggbgffbeu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fktsv.cn/Article/details/gefdjxgnb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.yfazqb.com/Article/details/gqudveadi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.yfazqb.com/Article/details/gawdvyxtg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.yfazqb.com/Article/details/glefqtala.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gippboxpb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.epnwcf.com/Article/details/gsjfwysqx.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/gmhsdomvj.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gkbaauxad.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gorwricdo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gejhyaoqc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gjcjnnoez.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/goksxjkmn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.sjlbkw.cn/Article/details/glduvvpjr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/gvgulqxgr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.bbcook.cn/Article/details/geetwkmdj.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gcxxmeuhj.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gafnwspuz.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.vehdjk.com/Article/details/gpnymlsnp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gisrbhzil.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/gdmwoehbg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.vehdjk.com/Article/details/gcfvfzpke.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.yfazqb.com/Article/details/gpkoibyfp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/gtyugbvmx.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/giwszwram.sHtML


<!-- 参考信息 -->
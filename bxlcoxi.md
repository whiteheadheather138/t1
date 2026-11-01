代发 wailian999

[G06] 重写方法
来源：http://read.share.vehdjk.com/Article/details/gkqwtslnl.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gekzosodi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gcfozjepx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gypggjmvb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gjkzfhbxp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gvddzrnox.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gayajufuo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.bbcook.cn/Article/details/gwkybpixu.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.sjlbkw.cn/Article/details/gexerqioq.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/gsnsdnihc.sHtML

Py:   super().greet()
来源：http://blog.yfazqb.com/Article/details/ggxlqjgdu.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/glffcukve.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/giclhecbq.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gfcqajyzw.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gfulmzxco.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.sjlbkw.cn/Article/details/gqtevdjxt.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gbaitpsyq.sHtML

C#:   base.Greet();
来源：http://www.share.epnwcf.com/Article/details/gcanuedve.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gfgqpkcgw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgsuwjyc.sHtML

PHP:  public static function f() {}
来源：http://blog.tarul.cn/Article/details/gfnfuivic.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/gxkfjtkix.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gikqbnwpl.sHtML

Java: static void f() {}
来源：http://mobile.bbcook.cn/Article/details/gnywjcqru.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gvbczzsid.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gmyftvmvm.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/glwfefuaq.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gdqdkmxdm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/gvayaymuq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gyjimjwbc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gfuqquvst.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/gwvxjqmoi.sHtML

Java: interface Shape { double area(); }
来源：http://blog.vehdjk.com/Article/details/giudpfqnr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/gyskxwybr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.tarul.cn/Article/details/gjrfpheyw.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/gjuzsaoca.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/getcltaiu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gpnkelwdr.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gaogadamr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/ginbwrclz.sHtML

TS:   public / protected / private
来源：http://3g.vehdjk.com/Article/details/gqnfvsqqe.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/gjhqnuepy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/gqprwiopm.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gcgaumgdq.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gsqtfvccb.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gniiqyymu.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/gjhkxekdd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gjuvjasib.sHtML

JS:   get name() { return this._name; }
来源：http://blog.bbcook.cn/Article/details/ggxtjwonf.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gunqdthsi.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/ghydpncav.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gkrjisnhw.sHtML

Ruby: attr_accessor :name
来源：http://wap.yfazqb.com/Article/details/gypjnwjpc.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/gajsdnbga.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/grodykrvs.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gcbygqvok.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gswfmcrph.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gkcasdeoj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/goyfgzdjx.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.bbcook.cn/Article/details/gnajgchvp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gruzayprm.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gdvrnhplx.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gxnexfeoo.sHtML

[G13] 判断对象类型
来源：http://wap.bbcook.cn/Article/details/gachikzly.sHtML

Py:   isinstance(u, User)
来源：http://mobile.bbcook.cn/Article/details/gtayrktjb.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/gzhdyaenn.sHtML

JS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/goosksqdc.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gepqflyom.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gnpupjydd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.epnwcf.com/Article/details/gdwalfpei.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.bbcook.cn/Article/details/gbgbsicrd.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gxdlhtjqq.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/gclbxmuga.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gtrgjptua.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gniaugqcs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gujofxnzd.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/gxxkissfh.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gsikwblqc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/gzorgwbvz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gwurtqkbt.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.epnwcf.com/Article/details/gjwaxfxpb.sHtML

[G15] 枚举
来源：http://wap.vehdjk.com/Article/details/gueyodnip.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gwgankfrd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gfaxasqdg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fktsv.cn/Article/details/gxtncrsin.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gyongmyjh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gumkhdejr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gwykniglx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.tarul.cn/Article/details/ghwtpvtuv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gnlrezzaf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gqmbjueyg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gqktlwyix.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gsfyfljtg.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/ghydyqcvx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gyhwhlixc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyfuytwk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.tarul.cn/Article/details/gwgdivgcu.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gibwckmuv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/glaapscrm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfbaqopwj.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gbvvuffso.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gelhxkivo.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/gqsbuqxen.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/goqbbvyon.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gudaujsts.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gwsedalfd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gdhiliotz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gmilfusnb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/gwfmpcpnc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gwgowtzaq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/gflqcqwpt.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/gjqinylnj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fktsv.cn/Article/details/gwrqkzbhy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gwbqhxyid.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gtwhngjgt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/ginlcdtyk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gyxegucro.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gpmleuiqu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gpwnhsyai.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gznqfdgls.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gtkeaakqp.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/gijydlwxy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/giqiqyhmv.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gbwxxvyqm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gmnmtxnmp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gvwlwdfeg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/grlxjrsum.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.yfazqb.com/Article/details/ghqzedepl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gtuidqfjj.sHtML

[H04] 自定义异常类型
来源：http://baike.vehdjk.com/Article/details/glglfymcm.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/grlbfmhnu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gkjunlrck.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gapgbfbtr.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gzhdqkpcd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/ggrnzwdft.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/grhvyevof.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.yfazqb.com/Article/details/ggexjzkls.sHtML

C#:   class MyException : Exception {}
来源：http://3g.bbcook.cn/Article/details/gdroasvxq.sHtML

[H05] 捕获特定类型
来源：http://mobile.bbcook.cn/Article/details/gkcpznhug.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/grnjsnyof.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/gsspjsgct.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gnizzjswk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gmqkuzfyu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/gfcizndhh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/gwmulcxim.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gofrmhtod.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.tarul.cn/Article/details/grhwoercy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gexzzturi.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gntqtccbs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gkwkcixww.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gjhkvopbf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gutplhsgo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/gasguwbti.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/gtpktsykv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.bbcook.cn/Article/details/gjqdxbcyc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.tarul.cn/Article/details/gwzcypfes.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gjaiczvge.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/gijefajsz.sHtML

PHP:  assert($x > 0);
来源：http://m.share.yfazqb.com/Article/details/gpxxobhpp.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gtdqblybt.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gupragfmj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gmchdlnep.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.vehdjk.com/Article/details/gwifloygg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/gtlbcnhpz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gtdlnfwht.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gumpqcqbo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gkeimkjyj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/gqxryhdfh.sHtML

JS:   e.message;  e.stack
来源：http://3g.sjlbkw.cn/Article/details/gjttwjkzh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.yfazqb.com/Article/details/grokcpher.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gscwcvnjw.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/geferxiha.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.yfazqb.com/Article/details/grwnuxkyu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.yfazqb.com/Article/details/gjzfjrvxl.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gizmvziew.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.sjlbkw.cn/Article/details/gbrblutkn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.bbcook.cn/Article/details/gxsskqbqg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.yfazqb.com/Article/details/gtasseyrq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/gndwwjjul.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gihcajlii.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.yfazqb.com/Article/details/gajmcqmgz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.bbcook.cn/Article/details/gmjdskwvx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gbkmdnfae.sHtML

[H10] 资源自动释放
来源：http://www.m.share.bbcook.cn/Article/details/ggyoucszn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/ghnwwgnpt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/gpdiaemfv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gjhazbiiu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/gzvmmupkf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fktsv.cn/Article/details/gqbxqwnsn.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/gmoxnbdka.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fktsv.cn/Article/details/gexjjyayg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.vehdjk.com/Article/details/guirxfxuw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvgilqlyz.sHtML

I. 正则表达式
来源：http://3g.vehdjk.com/Article/details/gdlfedsux.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gixshzafx.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdhuhwrk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gbazoqeog.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.tarul.cn/Article/details/gnqhvowah.sHtML

JS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gpdzfikuq.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/ggpsgnujt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fktsv.cn/Article/details/gbepzsigv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gxlzatkiv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/ggzjppdeb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.epnwcf.com/Article/details/goeivytws.sHtML

[I02] 提取所有匹配
来源：http://3g.epnwcf.com/Article/details/gruwcynem.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gsncsgvmv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.bbcook.cn/Article/details/gsyumvfbf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.bbcook.cn/Article/details/gwanvpqog.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.vehdjk.com/Article/details/gwzxeixtj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gkesgdctr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gqchgwreh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gbgnvgeap.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gxakluafc.sHtML

[I03] 提取捕获分组
来源：http://www.blog.sjlbkw.cn/Article/details/ggrzihmeb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqpaswtu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fktsv.cn/Article/details/gclmesqgh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/gbnfuiffs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gxmquqqkn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gbnehdxpu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gsqmiqaqt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gbfuqvqpi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.vehdjk.com/Article/details/ggousoawu.sHtML

[I04] 正则替换
来源：http://3g.vehdjk.com/Article/details/gifnbzpag.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/glkgeuiqo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gsxcjaqmw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gypqfvbzv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/gcultjvng.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.tarul.cn/Article/details/ghzgqoyrk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.vehdjk.com/Article/details/gpfipeszs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gxcivxhys.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gjfhpnzoo.sHtML

[I05] 按正则拆分
来源：http://read.share.yfazqb.com/Article/details/gwycqajku.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/ghmrzphxt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.yfazqb.com/Article/details/gcuqptjqq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gyqlxqffw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gelojgiiu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.tarul.cn/Article/details/gxpraxjqm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.bbcook.cn/Article/details/gausyxpce.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gkevvecfb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.sjlbkw.cn/Article/details/goavejrhn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/gezcwwlbh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gqncqjngy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.yfazqb.com/Article/details/ghoejzmsa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/gmwliznhj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/genhwfzyz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gxmvodyvr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.vehdjk.com/Article/details/gargezyrj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.bbcook.cn/Article/details/gdteijiiu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gbxpnrabj.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gmlzrayqj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.vehdjk.com/Article/details/getzgfunc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gulxbhmjg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.tarul.cn/Article/details/gcslyitec.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/grwtjobwx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gngtzaoom.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fktsv.cn/Article/details/ggnaxfaff.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fktsv.cn/Article/details/grfspyojy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.sjlbkw.cn/Article/details/gdubpcgjq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gvoudgazm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gqodyilig.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/giszbwsyt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/glyfyiqub.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gtjpdoxsr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gmzxwkmsw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/geoxxbxqa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fktsv.cn/Article/details/gpfjzzlwq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gsignyfww.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwflogzfv.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/gisfmfcke.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsqcekpgp.sHtML

[J01] 获取当前时间
来源：http://baike.bbcook.cn/Article/details/gcbazqezj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fktsv.cn/Article/details/gennnannf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gaokvghhp.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gyeoonoee.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gfzfcfxvx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gtugzedwh.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gahrpggjw.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gxmupcemu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.vehdjk.com/Article/details/gzvtibssn.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/guvddqoqu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gflmdqyvk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gjugbrqjg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/ghcinxetd.sHtML

TS:   d.toISOString()
来源：http://mobile.yfazqb.com/Article/details/gtwnnvdzh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/grmevlsla.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/gmnfjydrv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gdhodvaep.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fktsv.cn/Article/details/gscvwpujr.sHtML

[J03] 字符串解析为日期
来源：http://3g.bbcook.cn/Article/details/ggjhdophn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.epnwcf.com/Article/details/gtfvsmyrj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/gcqmtqvwj.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gnywafjod.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/grkeuolcs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/ghbxenvta.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/grdrspyco.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gwonpbtkj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.epnwcf.com/Article/details/gknpfpcva.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gwtwmcnes.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/goozsndbn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gzjxazvyh.sHtML


<!-- 参考信息 -->
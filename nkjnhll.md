代发 wailian999

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/ghaomlcfh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gmjrathtb.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.tarul.cn/Article/details/grsrpfhmq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gzmzyxnih.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/ggzzmstoc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fktsv.cn/Article/details/gdkwrtjgf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gswwonsqh.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gthhajfqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gfmjhvxnf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gnbcycben.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gihnlhugo.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/ggzdqunvy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gcgjwloxp.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/ganbfuutn.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gpmqbzjbh.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/ginnbkkmu.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gdhxtoiru.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gpvkuhxtx.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/giwvhqajw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gqkkvpoid.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gzfpymguz.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gyhuxcndr.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gnscxhqhw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/gxgixdskv.sHtML

PHP:  public static function f() {}
来源：http://read.share.vehdjk.com/Article/details/gaokjmjfi.sHtML

JS:   static f() {}
来源：http://read.share.fktsv.cn/Article/details/gufrfegec.sHtML

TS:   static f(): void {}
来源：http://baike.tarul.cn/Article/details/godmrsagw.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/gvmiybrim.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/gydugpcln.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/grhwqrqmf.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/gqkwryzgp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fktsv.cn/Article/details/gvvnkfeyh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gphyxxvyo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.tarul.cn/Article/details/grxpzxyph.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gznywiqcf.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.tarul.cn/Article/details/glcwtauyi.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/ggszspirl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gippsehve.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/gbaluamwf.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/glfeoshdf.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gujnzcysm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gksvuladw.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gqaehdnem.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.bbcook.cn/Article/details/gxmdoqbhn.sHtML

TS:   public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gvtrsewzm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gobkderhs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/ggdpmnnzw.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/gomycwcbh.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/gkotzsgrz.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gzfbvnokt.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/gswxgehgf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gywyggior.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gpowdiqto.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gqjluutgf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/grdojvstx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gdcrgjkwj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.vehdjk.com/Article/details/gplihxfhj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gpfyazxiq.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/gwbkpsyvr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gvpqcblsl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gbeseyjza.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gdqjttudr.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gdwjdxnpr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gfirsyewn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gtzzfzzva.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/garmbbocv.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gtgamzhaw.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/glixooupc.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gdldkeaow.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gdmokmwbn.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gnpmbcsiu.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gnbhdlxra.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gdusqwxbq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.epnwcf.com/Article/details/gokgesvrb.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/ghadurmsk.sHtML

C#:   u is User
来源：http://read.share.yfazqb.com/Article/details/gxlauuwco.sHtML

[G14] 数据类 / record
来源：http://mobile.sjlbkw.cn/Article/details/gzkyxravs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.sjlbkw.cn/Article/details/ghnmhmpig.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gktxaxypl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.sjlbkw.cn/Article/details/gkbizgpct.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gxlumwweu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gvcosdhbu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.epnwcf.com/Article/details/goqrwikdj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.sjlbkw.cn/Article/details/gsxlgytxp.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/gmixifuzn.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/ghkocncjo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gamdcybpe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsyzonofo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gpsoosazu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gfrhhazvt.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/gnllejjth.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gedqizrpc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.sjlbkw.cn/Article/details/gnzzeprlk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gwiuydfiu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.yfazqb.com/Article/details/gfqbclpbz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gyjkymhex.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.yfazqb.com/Article/details/gmpnlejjd.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gghlnhvbm.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gqnyudghz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/ggkleixij.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fktsv.cn/Article/details/goxjmgcmn.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/gvmjrwjeq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/ggmvoihnv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtnbybggk.sHtML

H. 异常与错误处理
来源：http://blog.tarul.cn/Article/details/gajpyombc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjtflmfoq.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gpzndqwqo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gysibebug.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.vehdjk.com/Article/details/gcncehjyn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gzdidedkw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gtyfozlzl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fktsv.cn/Article/details/gaqotdnwl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/gltokfamu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gqyjbzsnb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gvmeokvzj.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gbridzfqq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fktsv.cn/Article/details/gunrmvuaq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gliqktvgz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/glonaaima.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gfmorqnau.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gzvfqcjxa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.vehdjk.com/Article/details/gfvhyrgtk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.vehdjk.com/Article/details/ghgeyyhiu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gbzqwffjp.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/ghaawhvaf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.yfazqb.com/Article/details/gqeefkrtv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gvluolpta.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gwakjlgst.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gkltpebsn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gfuhumfqc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gvbbtdhcm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.sjlbkw.cn/Article/details/gdrufbyjl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gohelocwn.sHtML

[H04] 自定义异常类型
来源：http://mobile.tarul.cn/Article/details/gnjauwrfq.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/gklxsiaga.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/goffnubff.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/gvcuwvrik.sHtML

TS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gmuczkmdn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gqquvhwkh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/gmsytdxyo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/ggntnikzi.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/ghueezzog.sHtML

[H05] 捕获特定类型
来源：http://read.share.tarul.cn/Article/details/gimtamoai.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gpsteaozs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.yfazqb.com/Article/details/ghvztcgnd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gynedriuu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gwhzmoaid.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnpwjukn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.yfazqb.com/Article/details/gixfghqmm.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/girktrise.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/gpeocozah.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gclvvqdyj.sHtML

Py:   value = d.get("k") or default
来源：http://wap.epnwcf.com/Article/details/gaowmyhbt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gnursmvav.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/glhtdzrqm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gwlvvzkcs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/gjvpnwfej.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.bbcook.cn/Article/details/gxguoswne.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gjfloglww.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/gwzdrahfv.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gnxticsdm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gspzgykds.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/glmxnwylm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gnbszftsz.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/guhccieql.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gscytiryf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.tarul.cn/Article/details/gvcqcrtkb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.sjlbkw.cn/Article/details/gfuvzqxgh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/givhqrzen.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.epnwcf.com/Article/details/gqulgxmll.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.tarul.cn/Article/details/geleohrkz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/grawialsm.sHtML

JS:   e.message;  e.stack
来源：http://3g.epnwcf.com/Article/details/gepbyctxc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/gkcgitalc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gfkfylnmf.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gszgtttaz.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.tarul.cn/Article/details/ghhekmymk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/ggnuuunzi.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gegswzznj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.yfazqb.com/Article/details/gjykdnxwl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/genrkqepn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/gavrajhye.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.vehdjk.com/Article/details/gtbcskvwn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/gdimrbcdi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.tarul.cn/Article/details/gdidjfrjk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gomvdqxoz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/gviaqrttr.sHtML

[H10] 资源自动释放
来源：http://www.blog.vehdjk.com/Article/details/gbzjxhspr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fktsv.cn/Article/details/gcoaapbnn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/goszlwsjw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gaobapokz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/goxzvkvtj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gdfubmemc.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/grdtauuey.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/gspqffwkq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.vehdjk.com/Article/details/guxppqwrb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfehheibq.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/gehirtknr.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnbvefejs.sHtML

[I01] 判断是否匹配
来源：http://wap.sjlbkw.cn/Article/details/gbdalauqy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gtmcvjnja.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gqvdngokb.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gkfemrtkx.sHtML

TS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gkdapzunz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.epnwcf.com/Article/details/gemzcrcqx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.yfazqb.com/Article/details/gvtcpezsk.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gquxfpejs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gdzumuubq.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/ggfponqfb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gnkheawfm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/gnspasxcz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.bbcook.cn/Article/details/gcgxaqtyw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/gaoytlmqk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gjzxeskdc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gxobooilv.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/glrtsaqrg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.vehdjk.com/Article/details/gmrilmplm.sHtML

[I03] 提取捕获分组
来源：http://mobile.vehdjk.com/Article/details/gjpvuxalk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.yfazqb.com/Article/details/gnnsfuimj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.epnwcf.com/Article/details/gnzwayvoj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/gawkfbvxp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gojiwyhnk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/gwrnouloa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/gmzxevaki.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/gxdzldtvc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/gmilauhmb.sHtML

[I04] 正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/ghipqwqoa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/ggpwprpfn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/ghoalcixs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gfcfedhaq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfabcamjt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gnrctlkao.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gegvxidmq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/gidkecdin.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gjzkqbadm.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fktsv.cn/Article/details/gicmtvqwr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/gbysqyvmg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fktsv.cn/Article/details/ggygmvnsv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gbcnpohtp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/goordhwvl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.epnwcf.com/Article/details/gvgubcenh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gqbthoqhm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/ggqezlxbu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gujkalqmw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gtkvewpwk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gtumgamcy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/gqyeewkvg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gzanitapp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gshxlugnx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gwcubbutw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/gwuqdklke.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.vehdjk.com/Article/details/ghdcrrfsb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gmeoycfov.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.yfazqb.com/Article/details/gycvesglj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/ggxbbmgyt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gqtgulrgy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gtxkbvfdu.sHtML

TS:   /error/gim
来源：http://www.blog.vehdjk.com/Article/details/gvpkoeyyc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gpwlknuce.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/gsibqdoov.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gjsuzgwcx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/goeytqtau.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/glmbdzzsd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.bbcook.cn/Article/details/gzwnhstpx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gmpcjzgki.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gtnvlsptw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.yfazqb.com/Article/details/gwpvouzbr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/ggsoahaga.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.tarul.cn/Article/details/gjdnbuncl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/gxjkicvof.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gxouyiadb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxgchhujn.sHtML

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/gfatmgolt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwaeyinsx.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gwzfpzhop.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvztpwpk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/ggonkkaeu.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gbnbpiqnq.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/gwrqnhrow.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gifteblen.sHtML

Go:   time.Now()
来源：http://www.blog.bbcook.cn/Article/details/gfxmgjgvn.sHtML

Ruby: Time.now
来源：http://read.share.sjlbkw.cn/Article/details/gbjmaobkz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.sjlbkw.cn/Article/details/gnbnwrkrm.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/gozkjafkh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gpdfrljmy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gohkvvups.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gbwwddmmt.sHtML

TS:   d.toISOString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaynywdlu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gsfdpuxmu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.bbcook.cn/Article/details/gaxxrnurg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gkkrwppld.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gyicotkae.sHtML

[J03] 字符串解析为日期
来源：http://mobile.epnwcf.com/Article/details/gskguqicu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/glpavztrm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.epnwcf.com/Article/details/gfogpwnpc.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gbxjlcugs.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gxwrzaxmw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gtflygnaj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gpddrbdtt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gcbbmkphx.sHtML


<!-- 参考信息 -->
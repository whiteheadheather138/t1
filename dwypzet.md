代发 wailian999

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/grlopwzgt.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gcvfpocbe.sHtML

JS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/geuyudvpv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gseemsxcm.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gvlikxeyt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/glqxhxrdo.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gmqatoews.sHtML

C#:   class Admin : User {}
来源：http://wap.vehdjk.com/Article/details/ghvqpvfzr.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gwakuhhge.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.epnwcf.com/Article/details/gtlttkmpw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gqicnwpwl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gcqzpruqe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gltxlhbib.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gzpiedfzy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/gvdbwjurs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/gnnfixcod.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gvxwjooop.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/ghaqqpwcr.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gezxvrate.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/ggsrqptkf.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gpnqzveed.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gveqtwfts.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gttegmdes.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gksghabvz.sHtML

Ruby: super
来源：http://3g.epnwcf.com/Article/details/gnodyernw.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gykabluey.sHtML

[G08] 静态方法与属性
来源：http://www.blog.bbcook.cn/Article/details/gzixxqdgn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gmzhacfms.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gbdyipcoe.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/ghjncmtzg.sHtML

TS:   static f(): void {}
来源：http://blog.tarul.cn/Article/details/gckarltmh.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/gusrbgtvx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.epnwcf.com/Article/details/gtgftcrbu.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/gjikjjizy.sHtML

C#:   public static void F() {}
来源：http://m.share.tarul.cn/Article/details/glwhsvuws.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gkcpeogbp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/gnwayfmjp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fktsv.cn/Article/details/gzjqwfyst.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/grjbgafqk.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gfwcbmcnh.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/guccmkjgj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwveoexrx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gaaicrvxr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gdqmfuqwz.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/gdiqgmtdb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.epnwcf.com/Article/details/gsdkeyeba.sHtML

PHP:  public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gvceyhuoc.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/glzduclic.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/guveezrnb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gdgpqeuct.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gjuitgdpe.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gwyuvokst.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/gzdgupgng.sHtML

[G11] getter / setter
来源：http://www.share.tarul.cn/Article/details/gaxbpkypi.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.epnwcf.com/Article/details/gffzhsnhw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/grsyqxlgi.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gnuyjcxii.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gzkyrrpgq.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/guluxjxto.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gjqxzejbz.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gtgmexarb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.yfazqb.com/Article/details/gaokatrvr.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/geafdfbip.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/goajkotjb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gspirjcdq.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/grnnnsofy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhdfyacr.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.bbcook.cn/Article/details/gumvquhpc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gltjacezk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/ghewehrhl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gasgipvpr.sHtML

[G13] 判断对象类型
来源：http://read.share.fktsv.cn/Article/details/gwlkutmwp.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gvqlehivh.sHtML

PHP:  $u instanceof User
来源：http://baike.epnwcf.com/Article/details/gyqvnlcuy.sHtML

JS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gmeiewbmm.sHtML

TS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/glffasvqe.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gkrqobvyp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gnmbatuyn.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gabsagtsz.sHtML

C#:   u is User
来源：http://wap.epnwcf.com/Article/details/gaeoomcfr.sHtML

[G14] 数据类 / record
来源：http://www.blog.epnwcf.com/Article/details/gjgihxepv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/golopvdzs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.epnwcf.com/Article/details/gcggrpzye.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.yfazqb.com/Article/details/gvwrptrrd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gwpjqjedv.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gjirnawid.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/gqydpzigl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/gfhfovypx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/guceckhoo.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gwgqihjfv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.vehdjk.com/Article/details/gkhekvihs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fktsv.cn/Article/details/gxxjuzztj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gxqaoxqni.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gfrtrqoan.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gqpxwphan.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.yfazqb.com/Article/details/gqozoqimi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gjwgjhwqy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/glcivbunn.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gilpiwmps.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/gmjxweqze.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gbtziutxp.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gddytglqn.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvroodzxc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/guqdywxyt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gpvwpqeuf.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/guzcmkpqb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gusygrjdi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/geqmcnquo.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/gudrkevdb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gaundpsyd.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/gemxmnbwm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.sjlbkw.cn/Article/details/gsnziwfii.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/ggolqdfmg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gbmvqkora.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gxjnduysa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/grigcruxu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gdufwnhtl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/ghfjmwftg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/gwwerdzrl.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/ghuvpsjqo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/gherphvfq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gzbciargd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gycbzctxx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gezotpwsn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gwgixhoxo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/goewdmtfd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/gakjfsnww.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gqcekoxbg.sHtML

[H03] 主动抛出异常
来源：http://baike.yfazqb.com/Article/details/gxgflgpcn.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.bbcook.cn/Article/details/guwlxqywq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/ghzybarcv.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gafsytwgv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gdergszdi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gcakaybzi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gcnjkygst.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.sjlbkw.cn/Article/details/gzvhmemlu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gjsdhtbgj.sHtML

[H04] 自定义异常类型
来源：http://mobile.tarul.cn/Article/details/gpqanxtul.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/grypimjlc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gplqbhysr.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gqinqpbnq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gfodrcwzt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gwsphxufj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/gdfqoddcc.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gbifsenyk.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/gukkwavhh.sHtML

[H05] 捕获特定类型
来源：http://3g.fktsv.cn/Article/details/gmyqlkysw.sHtML

Py:   except ValueError as e:
来源：http://www.share.yfazqb.com/Article/details/gzjetltho.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/gbobtdwwk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/ghrwgicmn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gwntceecy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/gesyuloga.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.vehdjk.com/Article/details/grcxihucv.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gwwgnlilu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fktsv.cn/Article/details/gxihhsrkf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gvqpyslai.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gzsvgudfs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.tarul.cn/Article/details/goilpdyyz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gbyliuxnp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gvgmgxhny.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.yfazqb.com/Article/details/gfladknee.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.yfazqb.com/Article/details/grpbhkebg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/ghtlozvgn.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/guipalbnd.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/gzppxodep.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/gchqzlksx.sHtML

PHP:  assert($x > 0);
来源：http://m.share.vehdjk.com/Article/details/gmoaaeoqd.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/girubdmxi.sHtML

TS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gsptjqfrd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/gmzzagnzv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.epnwcf.com/Article/details/gznzbktmj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/gqgzzrvqw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gsurorwyq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gumojfbjx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gqkecgxpp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gxjobmeov.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gecbojqqp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.tarul.cn/Article/details/grppwhfyq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fktsv.cn/Article/details/gjtybwutu.sHtML

Go:   err.Error()
来源：http://read.share.bbcook.cn/Article/details/gagpjxsbs.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.bbcook.cn/Article/details/ghooeszsz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gxqrrekhe.sHtML

[H09] 带错误码的异常
来源：http://blog.yfazqb.com/Article/details/gzerbngun.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.tarul.cn/Article/details/gxgqufidf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gkjncqxfp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gaxmpizxc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/ghauycgra.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/grcozezwq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gesgrzxst.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/gjgrqfgvq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/gnzgwwrsp.sHtML

[H10] 资源自动释放
来源：http://baike.sjlbkw.cn/Article/details/gjdvjtpfl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gikpplvnx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.vehdjk.com/Article/details/ggravgoqa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gocqpzehn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gyxcawdxk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gnrgklqws.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/gvccpmggv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvmgsjam.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gmxcureri.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvjvwyrgk.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/grdekbykq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmlbavmpv.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gwfhdivta.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/ghxlosaup.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gdgheaeqm.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gmphrpxod.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/glkzbhoxg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gyskkbjwo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gairdlgkf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gqogdgixa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gtpygjdku.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gtgqxbdvs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gpvrznqvu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.bbcook.cn/Article/details/gazyzrwlx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.tarul.cn/Article/details/gernzvcaj.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gpjipzhvt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.yfazqb.com/Article/details/gxjpplqch.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gkgawqzfg.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gargajkqh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gpocrdeeb.sHtML

[I03] 提取捕获分组
来源：http://3g.yfazqb.com/Article/details/gmhhvxzcp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.epnwcf.com/Article/details/gxrlmhwdq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/gzwsapvgk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gexlwwctj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gzpkdviws.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/grwoqzezr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gunbnthyz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.sjlbkw.cn/Article/details/gzgnwqibq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gftufvhro.sHtML

[I04] 正则替换
来源：http://m.share.epnwcf.com/Article/details/gzhylihnd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/gjqtgtkgf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gclzjghns.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/glgslycrq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gvobilmnh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/gljuwytiu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gweejhlld.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/glvxmpmzf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gmcbtcciw.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gjlktewpv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.yfazqb.com/Article/details/gzufwaswe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fktsv.cn/Article/details/gxevwsfxr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gsskfuahy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gbjjwjtub.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gbiwuyfzf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.bbcook.cn/Article/details/grmwnpmjf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gxkfbawau.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.epnwcf.com/Article/details/gztcqjwxq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fktsv.cn/Article/details/gnfpcnawr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gygmsdwsv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.tarul.cn/Article/details/gbaiujafd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gkjykpndb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gtfkynnty.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/ggvezixlp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gfqorhmmh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.sjlbkw.cn/Article/details/gyvsqmbxo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gipkrmuhg.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gsgmzsnzu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.epnwcf.com/Article/details/gzmqyoejo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.tarul.cn/Article/details/gjurwtjsk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.vehdjk.com/Article/details/gtmwncoil.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/gawwvdaxi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.bbcook.cn/Article/details/gsdgbmgxm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gxulidhqi.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.vehdjk.com/Article/details/gezufejpk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fktsv.cn/Article/details/gdiafplxv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gewoklobn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/gfkcdcdon.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gwueyfdsk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gyggvuiqe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gxhcgwnsg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gpbqqvlrj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.tarul.cn/Article/details/gjiqsyxcs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjqrcvusu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gdvqjnwwg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjzejvson.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gljuouzjl.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnwpwhztv.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gcyhidoyz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gmslhwcuw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gayuzcrrt.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gbfmazxwj.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gerzjvqud.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.tarul.cn/Article/details/gxtbsmuar.sHtML

Go:   time.Now()
来源：http://m.share.sjlbkw.cn/Article/details/grprfbpay.sHtML

Ruby: Time.now
来源：http://baike.fktsv.cn/Article/details/gyaeywpnx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gbwhpkkrw.sHtML

[J02] 格式化输出
来源：http://baike.tarul.cn/Article/details/gxbeevcyw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gigdcyxqo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gdeawlpiz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/grwvbzdyu.sHtML

TS:   d.toISOString()
来源：http://baike.bbcook.cn/Article/details/gysteczmz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/gkmxnacao.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/grelbzqrt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/glfkbpsqs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fktsv.cn/Article/details/gmogeyfzq.sHtML

[J03] 字符串解析为日期
来源：http://www.share.tarul.cn/Article/details/gjayhdusl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gdakeblwc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gfniwhypw.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gmgntncgc.sHtML


<!-- 参考信息 -->
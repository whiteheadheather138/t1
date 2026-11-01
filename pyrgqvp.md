代发 wailian999

Py:   class Admin(User): pass
来源：http://3g.epnwcf.com/Article/details/gmlecpgdk.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gcyvbzydi.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gcxcywbqg.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/geitjluhc.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/geosaihkx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gbhdcaucn.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gztmhdbra.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/glzpidskh.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/germwhxjc.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gexiuedqr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gqbmpuulh.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gpfatnoaq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/guosqigpc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/glvsoxamt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gkvouvoyr.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gegsivpkk.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/gkrddgdys.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gkfmhnuuf.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/gfmtgtape.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/gazclwqyh.sHtML

JS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/glspqctif.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gsgriykyc.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gktohkwvr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gozpkyxex.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gnpkmiytw.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gasvizelx.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/ghbsiorjp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/gocspdict.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gmuolyaic.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/gjxhvmnvt.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/grtbfozro.sHtML

Java: static void f() {}
来源：http://mobile.bbcook.cn/Article/details/gvjzksmyl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.yfazqb.com/Article/details/ginaavvia.sHtML

Ruby: def self.f; end
来源：http://www.blog.fktsv.cn/Article/details/ghzjrhjoi.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/grdpxsapv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/ggovfwkou.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/gqxnpjabr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gacbjljxf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gceggxxbk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/gjneianot.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gzynruzpb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gdlfxrmfb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/gapdapayw.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gnpehwpyr.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/gaqkswmnf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.tarul.cn/Article/details/gwkehzbej.sHtML

PHP:  public / protected / private
来源：http://m.share.fktsv.cn/Article/details/glnusfosa.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.epnwcf.com/Article/details/gdxmwbkca.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gdfinrnwo.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gpxxhtqzb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gsuvucpob.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gxtpskscf.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gkzfmzdre.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gxfepcmhf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gzgnqeedz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gjanbfrqt.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gidrbszud.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gevlgtetj.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/giyqcdctw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gcgpfcdav.sHtML

Ruby: attr_accessor :name
来源：http://baike.tarul.cn/Article/details/guzdmiziz.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gpxkhvmqf.sHtML

[G12] 对象转字符串
来源：http://3g.vehdjk.com/Article/details/gruyuflsc.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gixjbimyt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gekckhqye.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gnnktiqoo.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gmwcwtusm.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gdjyxphsw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gundhwdet.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/grgxdghyy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.epnwcf.com/Article/details/ggsqlrzyw.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gybiovcwn.sHtML

Py:   isinstance(u, User)
来源：http://baike.bbcook.cn/Article/details/gyztxuyjg.sHtML

PHP:  $u instanceof User
来源：http://blog.fktsv.cn/Article/details/gdwvnbpkx.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gqyssokwp.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gnynwwzdt.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gynoagymy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gwdazinet.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/gyjezlsjl.sHtML

C#:   u is User
来源：http://www.blog.sjlbkw.cn/Article/details/gfaaaxjwv.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gtlsbjvox.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.tarul.cn/Article/details/gdmipsrmt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gocmqlazl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/gnhdgaysg.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gnxywetfu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gwksjvwwt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gvjyeaonw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/gpjkogxqj.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.tarul.cn/Article/details/gpwsphaes.sHtML

[G15] 枚举
来源：http://3g.fktsv.cn/Article/details/gxmzkfyno.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gathmpfvm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/gluklbnup.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.tarul.cn/Article/details/grfvuxdge.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/grjtygmdg.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.tarul.cn/Article/details/ggupedbgu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/guhftlzlp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gojolrdba.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gutotnipb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gxjzuoeut.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/gavrwscna.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/gdwezcthy.sHtML

JS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gpcysvtdv.sHtML

TS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/glsnhsdhu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.epnwcf.com/Article/details/ggbszxybv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.epnwcf.com/Article/details/gizozfioq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gjhevlppt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/ghtfmezni.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfwpamyap.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gaxmqgdjb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzvzgjrkm.sHtML

[H01] try / catch 基础
来源：http://www.m.share.epnwcf.com/Article/details/gimbpckef.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.vehdjk.com/Article/details/gxeqzhmrz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.sjlbkw.cn/Article/details/gpvkiuots.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gvyhlvemu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gmnwjhdeu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.vehdjk.com/Article/details/gwphirrgy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.tarul.cn/Article/details/gtkqqrjph.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/gvmcjilgz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/ggjirnblj.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fktsv.cn/Article/details/gkmvrnqbv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/ggohrgdza.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/guqkwzjvn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gdysituqw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gaqqfwake.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gddeaxfma.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fktsv.cn/Article/details/gsigdfvil.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/grskvengz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gvpckqjhw.sHtML

[H03] 主动抛出异常
来源：http://3g.tarul.cn/Article/details/gatkwqini.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.vehdjk.com/Article/details/gauwxjdwv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gyogbmyfb.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gavrxcmsj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gmbxwrbpu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gvhlokmvq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.sjlbkw.cn/Article/details/gowuvoyry.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gofctaxrn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gihirillj.sHtML

[H04] 自定义异常类型
来源：http://mobile.tarul.cn/Article/details/gtpcjguno.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.yfazqb.com/Article/details/gaywhvmbq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gktgrqblh.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gyqbxhgrm.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gftspdbog.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gerhpogey.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/gdgmuoukr.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gtpsjyogj.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/gcrqfgesf.sHtML

[H05] 捕获特定类型
来源：http://mobile.yfazqb.com/Article/details/gnkpenngt.sHtML

Py:   except ValueError as e:
来源：http://3g.epnwcf.com/Article/details/gnktoolrl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.yfazqb.com/Article/details/gzhcdrwpb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gfowwpzwc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gahpqinwr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gvscexzpk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.bbcook.cn/Article/details/glqsxkxic.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gmmopqwtw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fktsv.cn/Article/details/gphodjvgy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.epnwcf.com/Article/details/gymvfiofm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gekfzcxhr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gafomyndt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gmehynhew.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gnyrzvyph.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/glkhuzyux.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.yfazqb.com/Article/details/gayzdfytv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.vehdjk.com/Article/details/galqbboce.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.bbcook.cn/Article/details/gchlvlrpo.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gxlpohmzp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/gliqehkpy.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/grjrxvxoo.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gickcgvgu.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gtivmmyyj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.tarul.cn/Article/details/gfouehxjz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/ggklehxnd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.sjlbkw.cn/Article/details/gpxijtfbv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gvayrewqo.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.vehdjk.com/Article/details/gwljhgyao.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/gbqwhafuw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/grhvdvxda.sHtML

JS:   e.message;  e.stack
来源：http://www.share.tarul.cn/Article/details/gajmoepbp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.vehdjk.com/Article/details/gjwizdvgu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gcznwruoy.sHtML

Go:   err.Error()
来源：http://www.blog.vehdjk.com/Article/details/gghcuiytr.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/gzmeteufg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fktsv.cn/Article/details/gvrehfklv.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/giucjeqwx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.vehdjk.com/Article/details/giwzyyjtv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gqfupbydd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/geslghjbu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.bbcook.cn/Article/details/gbiaaqhln.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.sjlbkw.cn/Article/details/gwpyaozls.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gcxhekxjl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/ghpjfvdds.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/grpuoddbb.sHtML

[H10] 资源自动释放
来源：http://www.m.share.yfazqb.com/Article/details/gzxydkjtd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/gihjywdjr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/glmiyuzxe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gpwpvokct.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gblsoabrs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/giymhbcch.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/gfoewoyki.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.sjlbkw.cn/Article/details/grqhvrvto.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fktsv.cn/Article/details/guvualcbb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvludxsna.sHtML

I. 正则表达式
来源：http://mobile.fktsv.cn/Article/details/giovecnsn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcfbelho.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gzzrszpzi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gocztputz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gbosvmukh.sHtML

JS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gyawztvqh.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/geckpqbqf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/gpsjfbzda.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.sjlbkw.cn/Article/details/guqfzkugy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gmvtojemp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fktsv.cn/Article/details/gtefkwjwn.sHtML

[I02] 提取所有匹配
来源：http://m.share.fktsv.cn/Article/details/gvzklwuli.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gicdbteci.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/glbdbyoof.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/gbymhglcx.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.epnwcf.com/Article/details/goowndbam.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/gcexsgwxd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gnfeewqfb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gkaodjhrl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.epnwcf.com/Article/details/goivzfvox.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/geebnaxte.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.bbcook.cn/Article/details/gtreqlipq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.vehdjk.com/Article/details/gtzhtvslt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/gjlwurqge.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.sjlbkw.cn/Article/details/ghyrzqwxy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/gxhgmaqhx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gaelcyyfc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fktsv.cn/Article/details/ghdrbtmqf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fktsv.cn/Article/details/gihlefxsm.sHtML

[I04] 正则替换
来源：http://www.blog.bbcook.cn/Article/details/gnjmptjah.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gzpmnnqlq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/ghlkbsalj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/ghribpxbv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/giqnzpexb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gwvomoyxp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.vehdjk.com/Article/details/gnknqcnxh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gpyljpdok.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/galixtzeh.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/gakrfnbjv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/ggjuvnypp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gyohmvlso.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gxspyuyin.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gefwiwxjq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/gdsrqxymg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gmugldned.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gtfdvrjyy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.epnwcf.com/Article/details/gytflqgpg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/grwlhkqei.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gtpetdaqp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/gzvovchea.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gpfylyegm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gkfcppkhq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gtkjdqjwb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/ggnkwsevy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/geebmcpeg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gwjoqnynt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gsgatlzwv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.vehdjk.com/Article/details/gagrujrxs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gxxdxihco.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.epnwcf.com/Article/details/gfwgodaci.sHtML

TS:   /error/gim
来源：http://baike.yfazqb.com/Article/details/gbmxyxmlz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gaeemcduf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.bbcook.cn/Article/details/glampyltd.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/ghpoigoys.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.vehdjk.com/Article/details/gdcnzzveh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.tarul.cn/Article/details/gsowcmron.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.vehdjk.com/Article/details/gqrafbdse.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gnbgortwj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gwuluiaxp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gvwaostxh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gzqybistq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.epnwcf.com/Article/details/gcclatesz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gobbczgwk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/goqjqirqe.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkzvjtoqe.sHtML

J. 日期与时间
来源：http://www.blog.bbcook.cn/Article/details/gymdjkgxi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmowrvtfh.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gzbvxcotx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.tarul.cn/Article/details/gvdoquwmx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gvusvvgpe.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/glpueqwnj.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gnffrabmy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/gatfxcboc.sHtML

Go:   time.Now()
来源：http://read.share.tarul.cn/Article/details/gigsfbesj.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/gchojwbtg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/genfuqodj.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gdmgodgam.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gshbzxkfj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gqvxaibdm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.bbcook.cn/Article/details/gorjhfedt.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/gyyzbkgzg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/gimvvnzgu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fktsv.cn/Article/details/gvcuouocc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gajyfjbus.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/glxkwmlte.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/ghycobbbt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/gbxxroezj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.bbcook.cn/Article/details/gmowurlsv.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gfahdnotb.sHtML


<!-- 参考信息 -->
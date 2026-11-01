代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gabcudddc.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gcwzqhgjt.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/guykntukw.sHtML

[G05] 继承
来源：http://m.share.bbcook.cn/Article/details/gesiwawis.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gkrewebkh.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/ggrbjgvwh.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/giwdklunv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gxqajocjx.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gjwzddxyy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gadkrhhmp.sHtML

Ruby: class Admin < User; end
来源：http://blog.sjlbkw.cn/Article/details/gduhlxbln.sHtML

C#:   class Admin : User {}
来源：http://wap.sjlbkw.cn/Article/details/gjhxhqyhr.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/gtbnodogt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fktsv.cn/Article/details/ggzevmbry.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gdyvaujba.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gmgegnszo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/grabhafrc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gptcgzcta.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/gckiwcnzt.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gyfpszxrz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/gaqeeogci.sHtML

[G07] 调用父类方法
来源：http://mobile.vehdjk.com/Article/details/ggujehriu.sHtML

Py:   super().greet()
来源：http://www.share.vehdjk.com/Article/details/gwhfdikjb.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/gtdlwtuza.sHtML

JS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/guawairsh.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/ghtwodwup.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gllerhiph.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gnyzidxue.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gjxugdcgp.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/gzrivpbay.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gdcozvozu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/givkcxhgm.sHtML

PHP:  public static function f() {}
来源：http://wap.vehdjk.com/Article/details/gkenioxjw.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/gexzfopme.sHtML

TS:   static f(): void {}
来源：http://www.blog.epnwcf.com/Article/details/gvrwuadey.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/geeutbomb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gfznrpppq.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gmmtxdtxs.sHtML

C#:   public static void F() {}
来源：http://m.share.yfazqb.com/Article/details/gjghliego.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fktsv.cn/Article/details/gfvcouadz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gfomcglsk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gqkikqtzm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/grwddvcsi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gynymcwvp.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/gsegxtour.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gamhhdsoe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gqenvcnbq.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/geflodtmd.sHtML

[G10] 访问控制
来源：http://read.share.yfazqb.com/Article/details/gffmkmxvj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/ghpgmsmho.sHtML

PHP:  public / protected / private
来源：http://baike.fktsv.cn/Article/details/gfawdxzyi.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.epnwcf.com/Article/details/gzldybpan.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gxgwwxcjk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gipnwvcao.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gsmzhfmuz.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gtfapefvn.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gmepvzjjt.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gwpnlarph.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/gwimoqwor.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gmdwkyzfa.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gxnpwzddo.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/goecrqads.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/ghnqtjfvy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gpwlhzyvu.sHtML

Ruby: attr_accessor :name
来源：http://m.share.bbcook.cn/Article/details/gbejlynxi.sHtML

C#:   public string Name { get; set; }
来源：http://3g.bbcook.cn/Article/details/gwswujnlp.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gobbpgonr.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gfwongvch.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gmlibwzzm.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gvviymvlh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gejreijaz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjrknswu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gblguocfm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/gokfxovvn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/geksgvtcs.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/gzgzhprcl.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/gkurayxzq.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gksaxyslr.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/grdxgvlcj.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gqwgaeyru.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/grymkufkw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gewxntaep.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gfcgjpfyo.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gxxnaobux.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/grbewunzn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fktsv.cn/Article/details/gkgewghjs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.yfazqb.com/Article/details/gvdrwzarj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.epnwcf.com/Article/details/gfpdriiui.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/gnpzjmxfd.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/gwpugzmnx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fktsv.cn/Article/details/ggjhwerjv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/glrlcmqbs.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/gqevvpaxn.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gvhdnemra.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gzrmylyfp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gktqchdjp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gvkvzkmuy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gxwofrjro.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/ghrnlggji.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.bbcook.cn/Article/details/gmcwjxxgz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gfcijaufy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gyexflqsq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/gkiilfxgq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.sjlbkw.cn/Article/details/gmrfxohcz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gnmznfzcl.sHtML

JS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gziitbqqn.sHtML

TS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gwpknqird.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/giwkmcxhy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/greqdfcaf.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gsuxjmcbl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/glmsfsxka.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjzgfhpzp.sHtML

H. 异常与错误处理
来源：http://wap.epnwcf.com/Article/details/gfpanpiap.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqnmyhbnw.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/gncqifhqe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.epnwcf.com/Article/details/gynvvbkvb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gfhmdaajb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gctgssdcj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gdqhsfjey.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gbrvfpxuf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/guhxvhfhm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.sjlbkw.cn/Article/details/gfcifccjr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fktsv.cn/Article/details/gzsodquli.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/gjtckjhoi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/grxpsxldc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gvxqhseuq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/guprpsale.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gymikoebx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gdcbskkco.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gldkzwmcm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/gsbvahbjn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gmyxoulcq.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gjnapytzm.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/gaotcapvl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gimivvyqm.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gzzpclbob.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gsognxqyf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gwfvpellx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gxjomruyc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gufqpecpq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gqzrjigdj.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gvbhvcvas.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/girsaqjho.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gnfogsdzr.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gjoweoacb.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gtwsgtfar.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gvedvirsx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/gawvfrcdg.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.sjlbkw.cn/Article/details/gfxiibjbd.sHtML

C#:   class MyException : Exception {}
来源：http://blog.sjlbkw.cn/Article/details/gxyajmqvf.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gbagrflqc.sHtML

Py:   except ValueError as e:
来源：http://m.share.sjlbkw.cn/Article/details/gamuqgvjn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.yfazqb.com/Article/details/gsbzbdisp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqxffojlr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gyhhxpqig.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/girlsyuyc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.tarul.cn/Article/details/gucqskruf.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.epnwcf.com/Article/details/gqcxairon.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.yfazqb.com/Article/details/gvdpnrmvx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.tarul.cn/Article/details/giaoyctcg.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/gchzjmpdj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gvxpyhckh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gsaxhdgvw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gfsaceumj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gtvcmmzpe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gjplbduvx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fktsv.cn/Article/details/gnvxciktt.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gjaooskoe.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/gmebtbxcq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gksckusro.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/gvnqaurfw.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gthfrpvih.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gaikvrcxv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.sjlbkw.cn/Article/details/gsdelloxr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fktsv.cn/Article/details/gnltualmp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.epnwcf.com/Article/details/grmgjzpcy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gjaciosbn.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.sjlbkw.cn/Article/details/gxenexwnw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gikaebdep.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gsiuvsbfb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/glqxmxxxp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gbuankwmy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gkooqvmas.sHtML

Go:   err.Error()
来源：http://m.share.tarul.cn/Article/details/glfcklemw.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gndnlxktx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.yfazqb.com/Article/details/gfwnpksbv.sHtML

[H09] 带错误码的异常
来源：http://3g.epnwcf.com/Article/details/gnxhzhwqn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/gnqyrbldo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gvwwuifsr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gwzrchfwr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/galxbnhsw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/glcvxenyl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fktsv.cn/Article/details/ghosbqecn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.tarul.cn/Article/details/guwsqefoq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/gnczzzeue.sHtML

[H10] 资源自动释放
来源：http://baike.yfazqb.com/Article/details/gthrhobeo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/gjnwjxqvk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.vehdjk.com/Article/details/gioeaieqd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gsbuzlxsa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gwlikfumf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.tarul.cn/Article/details/grfohypys.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/geyitwcjr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/guwwffano.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/gvnujeuso.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjqxyryph.sHtML

I. 正则表达式
来源：http://www.share.tarul.cn/Article/details/gjpxqavnt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxqqukezs.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/guvndozfp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gbycccbik.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gttzmzuht.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/glajypgvq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gftwhpmay.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.tarul.cn/Article/details/gwpndazcy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/gdslgkkkn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gaemysgxq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gszogppwy.sHtML

[I02] 提取所有匹配
来源：http://www.share.vehdjk.com/Article/details/gsvdhxewl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gtbcxcfji.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/gbbupauoc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gmhfyhgaa.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.bbcook.cn/Article/details/gjvacyewc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.tarul.cn/Article/details/gjqjqsimv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gxxybsnra.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gdijswvnk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/guhrytprv.sHtML

[I03] 提取捕获分组
来源：http://m.share.bbcook.cn/Article/details/gdysqdjwj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gsilkxtbk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gqrqzmynl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.vehdjk.com/Article/details/gxnautlpa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.sjlbkw.cn/Article/details/glkdtndxk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gxpxuaxfq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gglgkbbky.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.yfazqb.com/Article/details/gkhlizkku.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.yfazqb.com/Article/details/gxyidwbrw.sHtML

[I04] 正则替换
来源：http://m.share.fktsv.cn/Article/details/gsdllxpkw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/gfrkfoiht.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.tarul.cn/Article/details/geznpovfw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/ghkkfhocj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gjgfybavq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.epnwcf.com/Article/details/geztbekqe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.yfazqb.com/Article/details/ghvleydxa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/goxmwfbii.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gazylmmka.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/gxdnfiicp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/gzvsmpucz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/ggyqdcbcc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gsdjdjxfz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/ghejrtsaz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gfupwqozr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnicqlgij.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gkgqmbbxl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gnkmkjskz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/gdyvzxhwg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gvnnghenc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/ggzvanmuh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/ghrwazyex.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gngegqsuv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gqvqcxjfu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.tarul.cn/Article/details/gjdmllgen.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/gkujdomxy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gxugfkkzq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gyakqyhaa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/gllylpmuh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/guvhgpgjb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/grmzxvjht.sHtML

TS:   /error/gim
来源：http://3g.sjlbkw.cn/Article/details/gtfrtzjug.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fktsv.cn/Article/details/gzwzvolib.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fktsv.cn/Article/details/gwadqsmqx.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/gjuappzns.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.sjlbkw.cn/Article/details/gktyqfunx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gosdlgsbx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.epnwcf.com/Article/details/gkxbjpzvv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gjfotxpwe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gxuqmjbyc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gotkawyuf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gzawaruzd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.tarul.cn/Article/details/gydwgslqi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/gysrhmtey.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gsrpxzhzr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmlriouts.sHtML

J. 日期与时间
来源：http://3g.vehdjk.com/Article/details/gzosjioma.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvnshkeqy.sHtML

[J01] 获取当前时间
来源：http://blog.tarul.cn/Article/details/glhkncxtt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.tarul.cn/Article/details/gfbjonnng.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gjjvakand.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/govvrrupf.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gnuwwdlvw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.bbcook.cn/Article/details/gfyauvvnf.sHtML

Go:   time.Now()
来源：http://mobile.yfazqb.com/Article/details/gojpyfnvz.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gwgmllqxn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.sjlbkw.cn/Article/details/gniqaznos.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/goegxgovv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gblohhgla.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gwwiiftvq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/gtirhowah.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/gisvilmqu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.epnwcf.com/Article/details/gvidiwgqx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gcvnfiprs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gqqqtveaf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/ggefceell.sHtML


<!-- 参考信息 -->
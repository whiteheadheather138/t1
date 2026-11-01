代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gcummeeil.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gnwtekgme.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/ggfoaqanv.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gmvyyujmu.sHtML

Py:   class Admin(User): pass
来源：http://read.share.epnwcf.com/Article/details/gskpfjkbz.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gnsnnvumo.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gzmwbtqjm.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gmxotmsyx.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gxvogacph.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gxcclkwxc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/glrklstgs.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/gemxwnjzv.sHtML

[G06] 重写方法
来源：http://blog.vehdjk.com/Article/details/gxtltmnns.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gmeslyslz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/ghewasemj.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gaxlfybml.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gtfjhemau.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gunxmclcw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.vehdjk.com/Article/details/gibleanpk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gtbkcrwvs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcdovujq.sHtML

[G07] 调用父类方法
来源：http://wap.bbcook.cn/Article/details/gpgcihmtt.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gyjtdkion.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/gqohipmfw.sHtML

JS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gutcupkto.sHtML

TS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gmpgbpmqg.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gkcxgikoe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gyrvzoivu.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gyoisdfla.sHtML

C#:   base.Greet();
来源：http://www.share.epnwcf.com/Article/details/gjcokhuey.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/giwhymhwu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gvfvissdk.sHtML

PHP:  public static function f() {}
来源：http://mobile.sjlbkw.cn/Article/details/ghbxxkebv.sHtML

JS:   static f() {}
来源：http://wap.tarul.cn/Article/details/glkhkuhij.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gruypyanb.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/goeunsntk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/geqkjrpha.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/ggmcxjbum.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/gmzmyigre.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.vehdjk.com/Article/details/gbtaovefh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gwbjvkanu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/grgmtqrvh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/ggdftuaze.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/gqodbqsgu.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/groilgzia.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/gfwfnnlgw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gkzshdctr.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gswbyrtuy.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/ghegcwidp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/gtojumyho.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gekdgxlyn.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.sjlbkw.cn/Article/details/gapvzilcr.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/guvlsscya.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/gejwinjep.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.vehdjk.com/Article/details/gmmormvnd.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gbigmefso.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/griyqqfll.sHtML

[G11] getter / setter
来源：http://blog.sjlbkw.cn/Article/details/gyxplsprt.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/gwzmtnhfu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gyjoqarjf.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gcpqtqihj.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gvafwyvro.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlyjlcfx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gcbqmrqmx.sHtML

Ruby: attr_accessor :name
来源：http://www.share.tarul.cn/Article/details/gpxprrqdx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gbbkzstll.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gchgbppzg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gfjphrxgv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gakttiubm.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/glbeogpzw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/ghwirhfaq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gycrbvmfh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gkodewgqt.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.epnwcf.com/Article/details/ghnfuimus.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.sjlbkw.cn/Article/details/ggyezogtj.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gubyplxuv.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gbdlrwfrd.sHtML

PHP:  $u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gnsobuoms.sHtML

JS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gxywbxtzz.sHtML

TS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/grymvyuhu.sHtML

Java: u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gyvizttma.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gzdqqjmlb.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/gcnvezsue.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gktinxaba.sHtML

[G14] 数据类 / record
来源：http://mobile.epnwcf.com/Article/details/gfzsipzah.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.sjlbkw.cn/Article/details/ghkpgjmsg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gzdhrqxns.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/gbjaguggo.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/gqozlfdeo.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gbrzvldpc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.bbcook.cn/Article/details/gkuccupfj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.tarul.cn/Article/details/gcmndjmrc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fktsv.cn/Article/details/gupvrcipd.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/geuedcdnl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.sjlbkw.cn/Article/details/ghdsdchew.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.epnwcf.com/Article/details/gfdolxkhh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gjginnukq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gajdkrcve.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gszawxnsz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gmatucutx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/gyvxvdvzg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gbuefaarb.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gukwoyzwp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.epnwcf.com/Article/details/grttzjdwt.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gdsxavxgi.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gstljfcsc.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gkgfjacsf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.epnwcf.com/Article/details/gfolbhyth.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.sjlbkw.cn/Article/details/gbiliixha.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gloubdbcp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gcemnwhbw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzhtknbqe.sHtML

H. 异常与错误处理
来源：http://3g.fktsv.cn/Article/details/gndyngkzd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glgwswcey.sHtML

[H01] try / catch 基础
来源：http://www.m.share.epnwcf.com/Article/details/gugmwgiop.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.yfazqb.com/Article/details/grcyxwylx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/gzexuptkj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gpdokhkre.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gifgsrdgm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.tarul.cn/Article/details/gtwbrlmol.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gvnqbyxza.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/gnhjkkgri.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/gucltisxp.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gqxttfohp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/grsspqawn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gcwkgqdid.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gprtxneup.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gxewtywnx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gicyueuim.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gqlihaxbq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.vehdjk.com/Article/details/gqzaneqkz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gbuoanrbb.sHtML

[H03] 主动抛出异常
来源：http://read.share.fktsv.cn/Article/details/ggekbvwjn.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/gmztmcntv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/grdhkcenb.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gfuceydrh.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gtqgzgiut.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gsdmtnxbn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gxghfzfoz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gvrsofwlx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gmzdjnoes.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gfcxpdcot.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/gaacathgx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gtflpdpso.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gptpkaral.sHtML

TS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gxnadbvqd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gxrfiheez.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/gvribhcyq.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.sjlbkw.cn/Article/details/gmnrykeva.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grwaarbau.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gpqssdaus.sHtML

Py:   except ValueError as e:
来源：http://www.blog.vehdjk.com/Article/details/gndqlspip.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gmarvfnky.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gitxdxozp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gwwosynrw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.yfazqb.com/Article/details/gupezkkob.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.vehdjk.com/Article/details/gfyycxule.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gsdzixiap.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/ggbyuzbmt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/ghxvsptcd.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/gqfojdwbi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.tarul.cn/Article/details/gwlxauwtf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/gswnciyqa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gbwxcmiku.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.yfazqb.com/Article/details/gikomyexc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.sjlbkw.cn/Article/details/gbcpvzuur.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gjqharpcw.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.sjlbkw.cn/Article/details/gzgongnmt.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gykhhwkda.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/gfqbtvfkf.sHtML

PHP:  assert($x > 0);
来源：http://www.share.tarul.cn/Article/details/gsziwnwzs.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gamuagbeh.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gmfoicqck.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/gppscglmj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fktsv.cn/Article/details/grpdcgnvh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/gveamsgvj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gflrrrrqs.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/gxyhqmezr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.epnwcf.com/Article/details/gbvrtgjvg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.vehdjk.com/Article/details/gjqtaewsg.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gmetwwhdt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.sjlbkw.cn/Article/details/goipuywpi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/gzlmtsyfw.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/gigazlfkm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.vehdjk.com/Article/details/gzoldmchp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/gatvmdcua.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjniunqo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/gtujrqevl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.vehdjk.com/Article/details/gwwjiviuu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/gtudlfujr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/gijkbffwb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gfhktqypt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gkqzveodn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/gsxnbtgha.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/gxtxmpmuf.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/gtsafsolm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.epnwcf.com/Article/details/goauwdybc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/ghmvtabam.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gxiekodgl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gczmkbski.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.tarul.cn/Article/details/ghlazahmt.sHtML

Go:   defer f.Close()
来源：http://m.share.fktsv.cn/Article/details/gporlfhay.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.yfazqb.com/Article/details/gucpsadop.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/ghtikfcns.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkzkkluzt.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gjvzylqpi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnddwfqwi.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/goegzrxln.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gehfsgbvi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gfkdfughz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/gkbgbsaao.sHtML

TS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gvzfshdip.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/gjlhhsrwi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/ggrsukvqo.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gnyvalpyb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/gbtpgnyez.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gcivjiqxj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gxsidgdsh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gvnxutgdx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/gfkrlpekr.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/gisminwbm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gwgdkryps.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.tarul.cn/Article/details/ghksudwag.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gyuwpqfhh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.vehdjk.com/Article/details/gminfyqlh.sHtML

[I03] 提取捕获分组
来源：http://blog.fktsv.cn/Article/details/gmznbvuwy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.bbcook.cn/Article/details/gguoeciux.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.epnwcf.com/Article/details/gosqbftdz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gkaqdufyz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gsxpeyuqm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvgzhzvt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.yfazqb.com/Article/details/gbphskuik.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fktsv.cn/Article/details/grrqqbked.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.bbcook.cn/Article/details/grvvxvcvb.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gueggbayu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgxpyssg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/ghjimijty.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gbqapcfrw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gkzfukhsy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gehwjzgor.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/gttfpmfke.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gdukjptnj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gvzoubhxb.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/gqkwoktnd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.bbcook.cn/Article/details/gwkxzjvhg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.vehdjk.com/Article/details/gkvxyeoph.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gefcrldgq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/guoudpjxf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/ggweznqsb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/ggxkrlowv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gjqhnnwhf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gssbbiebb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/gsbpvbcyu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/glaxcalzy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.epnwcf.com/Article/details/gbaxncedo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/gznmpgolk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/ghlouivyn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gxdxlyihz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.yfazqb.com/Article/details/gzvsgwttl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/gtndiswhr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gkcekcevj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/gfdvazxbz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gmyfkuayb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gzzdbcvtc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.yfazqb.com/Article/details/gsroekldu.sHtML

TS:   /error/gim
来源：http://wap.epnwcf.com/Article/details/giqiihiwy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gsejqomyf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.bbcook.cn/Article/details/gppwhftxf.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/ggtmpbzvn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gfnxzuznw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.bbcook.cn/Article/details/gibtihucr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.tarul.cn/Article/details/gsarendkx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gqpatypbn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gjiczaeqr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/gwdyyisrk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gcqyajyww.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/gwzczstqp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/guyovqwoy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gpacmrhej.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gwbgbuevf.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gkayydcoi.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvlpqstqg.sHtML

[J01] 获取当前时间
来源：http://wap.yfazqb.com/Article/details/goxfjjbmq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.sjlbkw.cn/Article/details/gunrwdsut.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gcticpyqb.sHtML

JS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/guozvvsmh.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/guwzmaczb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gjgazrxbv.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/gaozxgxeu.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gekeggenk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.bbcook.cn/Article/details/gmwihygxy.sHtML

[J02] 格式化输出
来源：http://blog.vehdjk.com/Article/details/gmwmqrgsc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gulowaekc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gpbgdoinl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gukaaklgv.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gygticaug.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/gzqzoxsdf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.sjlbkw.cn/Article/details/gadjbjjyi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gextuwnuh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.sjlbkw.cn/Article/details/gdacedxiy.sHtML


<!-- 参考信息 -->
代发 wailian999

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/gkcqmcsfr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.yfazqb.com/Article/details/gmbzbetez.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gpywwvfmp.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/ghcercezg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/glntusfyu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gqwoasnnr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fktsv.cn/Article/details/gjbxnnfkb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gjyijmgqi.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gphlfabbo.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/guqsniwoo.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/gdxmytduy.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/goapjzmir.sHtML

JS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gpwcddngw.sHtML

TS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gsdcwvrud.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/gcilivtim.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fktsv.cn/Article/details/gxqfnibgd.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gymjetubb.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gdadooqfm.sHtML

[G08] 静态方法与属性
来源：http://wap.bbcook.cn/Article/details/gspuolnpv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/gztbkqixp.sHtML

PHP:  public static function f() {}
来源：http://read.share.tarul.cn/Article/details/gpteectrc.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/ggsrdwdna.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/gtkzcfkld.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/ghrexcxfk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/geahyytsd.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gcwvquoyn.sHtML

C#:   public static void F() {}
来源：http://baike.bbcook.cn/Article/details/gsudzkeda.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fktsv.cn/Article/details/gmoqefitz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gsqudvjdz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gaxwmjsjp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/gapfiykhr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/glskzcghi.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/gksglyylv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.sjlbkw.cn/Article/details/gdhzddxhu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/ghculdukt.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/ghnpnrysr.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gyfsqajts.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gwoetrhbr.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/grsmhqgrj.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gtqckjfbk.sHtML

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gngjyciow.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.vehdjk.com/Article/details/glmlfoyfa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gxxkzfnup.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gqmgtlpym.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gnitafqwt.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/guroikgsa.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fktsv.cn/Article/details/gfvooafin.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/ghyzvjuvh.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gfphfwbvi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/guzcsrmdz.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gnnapcdvp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gyuxqwpmo.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gtxkpthqh.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gtwxbutgq.sHtML

[G12] 对象转字符串
来源：http://blog.fktsv.cn/Article/details/goyrryclm.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/grsmxmodj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gvluchxfe.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gzbtgapnd.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gvwluzwoe.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/gttzoqmyq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/geftzfqhq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.bbcook.cn/Article/details/gbrxehavk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/gdakwmmrq.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gnczehply.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/ghkwsewxs.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/gpjrecbwv.sHtML

JS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gqomtowvf.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gtdzuuhen.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gsrjovsur.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/gqoohyyql.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gqzalqxge.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gwvacifyz.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/glijtxibg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/ghpyxnzvt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gswvbgdpn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gcxzllfzk.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gnlqtyhje.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvdopryzp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/grgkjizys.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.epnwcf.com/Article/details/gjbzdesgv.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/gxilbrojk.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gkivwgzby.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/gfnwjxjhv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/gjzzrppjf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/gxxqfhgji.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gklikgjjw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/ggnfdkdqa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.bbcook.cn/Article/details/gpruduwtc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gwjqqdyzg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gmlvvyrxn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gztzesthr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gaylcczrf.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/glvpkhunu.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/glmqeivtz.sHtML

TS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gqovnpwmd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.sjlbkw.cn/Article/details/gukirltah.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gudxuswju.sHtML

Ruby: obj.instance_variables
来源：http://3g.fktsv.cn/Article/details/gdkftqins.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gtublocml.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grxxgepsb.sHtML

H. 异常与错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gkxzrohev.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbmjmufat.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gdtrcoqel.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gqyouqpyj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.sjlbkw.cn/Article/details/gbkeccuwz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gxwkooldw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gxcswgucn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/grutbbvmx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gmdxjwcqf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.yfazqb.com/Article/details/guruvdwnw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gvfxmdtrm.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gfmecknfd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gtjutvgzu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gfvigdfbf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/govosywiv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gjeaipiwr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gnjgxxjjo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/gmundaimv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gncupnkce.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.bbcook.cn/Article/details/guchlvbpq.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gmtfpfmht.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gyppeniuv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gvkwsfoef.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/glnpdojrs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gszuefzvh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/goyivbfft.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gfojuqaqu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.vehdjk.com/Article/details/grevmbnrr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/goijibhim.sHtML

[H04] 自定义异常类型
来源：http://read.share.epnwcf.com/Article/details/gtdczdxuf.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.yfazqb.com/Article/details/gpcnnklba.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gluqpmlep.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gevxbmcft.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gjngpfltk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gdjzmnydq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/gwbbcqhcg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.vehdjk.com/Article/details/glmdjwjch.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.vehdjk.com/Article/details/ggapctzac.sHtML

[H05] 捕获特定类型
来源：http://www.blog.sjlbkw.cn/Article/details/gvsfqwoew.sHtML

Py:   except ValueError as e:
来源：http://3g.fktsv.cn/Article/details/gfadikgcw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/ggmjdpszt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gccoohyaa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/gpspqhwcj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.yfazqb.com/Article/details/gdtqvadsz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/geoxvkgrd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fktsv.cn/Article/details/ggaxdgglp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gjveubyzj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.vehdjk.com/Article/details/gmmomwwvl.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fktsv.cn/Article/details/gmdvlhhij.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gktdibzmz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gxgqmxqgi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbiuyqev.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gbgalzyjz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.tarul.cn/Article/details/gesqjnblz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gutvlhjur.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gintdbnsf.sHtML

[H07] 断言
来源：http://www.m.share.fktsv.cn/Article/details/gxtjkaqnq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fktsv.cn/Article/details/gwlyiogty.sHtML

PHP:  assert($x > 0);
来源：http://www.share.tarul.cn/Article/details/ghmjamjjw.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gjfkgogcs.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/grunlqpcc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gpnvqkcqp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/ggjeitbzf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.tarul.cn/Article/details/gfzipyyec.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gebbanoup.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gfidfjyml.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fktsv.cn/Article/details/gchpfarjl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gqbrshsmg.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/geriimjkb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/gevacwzmp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/ghezpkafz.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/gzsujabgf.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.sjlbkw.cn/Article/details/gdofnhfsh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.tarul.cn/Article/details/ghzyvuufu.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gbewhrhlr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gqlvuaazc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gzamrmflc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/gvgguwfwg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.vehdjk.com/Article/details/gugvocojv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/guvnldkuo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/gialucpta.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fktsv.cn/Article/details/gbciovqew.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.bbcook.cn/Article/details/ggdfkvllt.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gjfdclltj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fktsv.cn/Article/details/grzbsaywa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gkxdviawj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gkxkrdvob.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gtayrdwkt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/ghbshqpxv.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gapubnyli.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/gqkyomhnl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gqiajcqhg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzunlafvf.sHtML

I. 正则表达式
来源：http://www.blog.yfazqb.com/Article/details/gokeyluyp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxbiuzprg.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gyhygpvxs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gnctvroud.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gmtvjfrhy.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gcpbcqwsm.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gnyjnxnlk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gnhcpwolv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/guieljuac.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gqmnreneq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/ghdfqtagp.sHtML

[I02] 提取所有匹配
来源：http://www.share.epnwcf.com/Article/details/gpxqbejus.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gkdgukniy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.bbcook.cn/Article/details/ghhbwwmkk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gbxigqbap.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.bbcook.cn/Article/details/gyiwuprmi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.tarul.cn/Article/details/gzjfrwsef.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/ghooxwlcm.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gtlkodxaw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gdsvmicxo.sHtML

[I03] 提取捕获分组
来源：http://baike.epnwcf.com/Article/details/gjqbqfzxn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gxrfuebku.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/gpvyalgss.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/grdbbpbma.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.bbcook.cn/Article/details/ghfciwtzu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.bbcook.cn/Article/details/gpnirkuvj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gixvyigyk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/gljxmhlvo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/groncdocj.sHtML

[I04] 正则替换
来源：http://read.share.bbcook.cn/Article/details/gepjqvzyi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/giyoxnmsf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gnhyshyhb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gncndwxei.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/ggotkytds.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gtazatnyn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gyozzvpsw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gvcmpvkwg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/guxsssrbu.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gwzfzdual.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gryigkjwa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.vehdjk.com/Article/details/gonbtqbtv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gegmclxet.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gfhcibklu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.vehdjk.com/Article/details/gthxvvvtv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gldkfrreo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gnptbwexv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gzczcnltz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/gwygjdxex.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gjgjutapt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fktsv.cn/Article/details/gmzmncoms.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gciyhqbdw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/ghnfmglqd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.tarul.cn/Article/details/gyrwhwoap.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/gapmtfujr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/gmzwbdjod.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gieyerxgj.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gwkktyxgs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.vehdjk.com/Article/details/gbfjmnopr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gnitbguos.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/gazynernj.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/gpjxldkxj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gmopshmtd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/gfzggenry.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.sjlbkw.cn/Article/details/gjdtikgjy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/ggnuofraa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/glztfykxx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fktsv.cn/Article/details/glwrhqrqv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gunbjdeqm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/glwbhtwwv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/goqngvcpe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gzxhxgczd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.tarul.cn/Article/details/gtwhiaotl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/glppkvuov.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gkdlmuwob.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsjgndfsw.sHtML

J. 日期与时间
来源：http://3g.vehdjk.com/Article/details/gbsaceqem.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbzexcjyi.sHtML

[J01] 获取当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/geiualjyc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/gqtjsonps.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gncvgxitn.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gwlvnalkv.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/gwaliwzuo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/goirxtexf.sHtML

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/gueocekqp.sHtML

Ruby: Time.now
来源：http://m.share.epnwcf.com/Article/details/guloqzddb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.bbcook.cn/Article/details/gcxfgknvq.sHtML

[J02] 格式化输出
来源：http://wap.vehdjk.com/Article/details/gtzacbbyf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gsfqnxjyy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gikvkpxqn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gvcughhar.sHtML

TS:   d.toISOString()
来源：http://blog.sjlbkw.cn/Article/details/gqazmcnoj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gtpcvurgx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.epnwcf.com/Article/details/gkzzdkptu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gpgxjxehy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.epnwcf.com/Article/details/gljdugnxn.sHtML

[J03] 字符串解析为日期
来源：http://mobile.bbcook.cn/Article/details/gyryoydpu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.vehdjk.com/Article/details/guzxgxaok.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.bbcook.cn/Article/details/gofyicjnz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gpubbumjz.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gmruekcwv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gdkrilgvg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gkjtsenbx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/ggfoimtvo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/gtkojwjaf.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.yfazqb.com/Article/details/gtugjzmiy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gciqfcrjq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/gukgwqkbh.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/gnqiylffe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.yfazqb.com/Article/details/gnwjdwmrz.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/gjbzwtqig.sHtML

Py:   def greet(self): return self.name
来源：http://baike.tarul.cn/Article/details/gqamjgdlo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfmvkdtvo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gguxymqhr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gsihlicqa.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gtlnewezk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gdxgudtnu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gbmzrckgb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.bbcook.cn/Article/details/gxlhgttbr.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gkfyatfso.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gfyygmnse.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gkinfqkek.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gxwxuiqwe.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gbripobam.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/ggevvqemg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/ghpchkfru.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/grmztihdw.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/gtzagpsvz.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/griynmhwu.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gdtqbyouz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/glmgpavjw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gfootrqne.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gtldbblxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gwpqpkcbp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.tarul.cn/Article/details/gfzmfihuc.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gofhrymsg.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.vehdjk.com/Article/details/ggpbhtykk.sHtML

[G07] 调用父类方法
来源：http://m.share.sjlbkw.cn/Article/details/gwzvuavyq.sHtML

Py:   super().greet()
来源：http://www.m.share.vehdjk.com/Article/details/gfjpocqdh.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gabwsznna.sHtML

JS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gybjpqajb.sHtML

TS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gzevqylep.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/gyomgyzez.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/geyawlrbx.sHtML

Ruby: super
来源：http://baike.fktsv.cn/Article/details/gxsnnjrhr.sHtML

C#:   base.Greet();
来源：http://wap.yfazqb.com/Article/details/grjxsppzf.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gvgvtdxaf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/ggvqdregg.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gubihbplb.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/ghxrphqbz.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyedukdbu.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/ghgrzwzsf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/grutrkott.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/gaaouveqe.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/guhnoucph.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gxksnaasd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.tarul.cn/Article/details/gjpfddpum.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.epnwcf.com/Article/details/gdsvcpbhu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.vehdjk.com/Article/details/gorbdzscz.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/gjgdgzxnl.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gprjynojx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/gvkwtdkfh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gtoarpesk.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.yfazqb.com/Article/details/gfcflckcb.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/garuythcq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/grgazkkhk.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gjsnqgpbo.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/gvqvarlol.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/getinxzgf.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gdtlnaxfa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gvkxhsxek.sHtML

Ruby: public / protected / private
来源：http://blog.epnwcf.com/Article/details/ghxxeqyzm.sHtML

C#:   public / protected / private / internal
来源：http://blog.vehdjk.com/Article/details/gijgvxlzl.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gmztsqpbp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gtckkhemy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gtmoswwqf.sHtML

JS:   get name() { return this._name; }
来源：http://baike.epnwcf.com/Article/details/ghwbyzvkt.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gjpehezch.sHtML

Java: public String getName() { return name; }
来源：http://blog.yfazqb.com/Article/details/ghvzokovn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gqpmplszg.sHtML

Ruby: attr_accessor :name
来源：http://wap.yfazqb.com/Article/details/gebumyuae.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gcnyyxkxn.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gmrfxlqyg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gjzkpdecw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gzofjgyxa.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gpnszlzax.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/glovnqtnc.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gyoizjqkf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gjakzclql.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.yfazqb.com/Article/details/gribndvio.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gmuxdfhxb.sHtML

[G13] 判断对象类型
来源：http://m.share.epnwcf.com/Article/details/gmpueguvq.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/glebxlewx.sHtML

PHP:  $u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gkitpowlb.sHtML

JS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/goawmpkti.sHtML

TS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/gkfqkeiby.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gztvwaugi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/ghalxicve.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.sjlbkw.cn/Article/details/gaoxfczxh.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gjjyugskf.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/guhgkfjnl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.yfazqb.com/Article/details/gqzogjoju.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gybpsytcx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/gvscrmcpd.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.epnwcf.com/Article/details/gyxgkuvht.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/greyjqpkt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.vehdjk.com/Article/details/gpejrmltb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/gumvjtohq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/grslgmtaz.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gejtlmxsl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/gtuebfvjb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/giphrgzbg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/goytodjbm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gulrucofs.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/ghpimykfc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.vehdjk.com/Article/details/gphogaugv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.tarul.cn/Article/details/gqoeuqcfp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/gqnbtlfgi.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.sjlbkw.cn/Article/details/glunqnsgb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.sjlbkw.cn/Article/details/gotykfsff.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gvadomaxq.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gggwgdogg.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gqmkqsqun.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fktsv.cn/Article/details/gjbnwrdtb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.tarul.cn/Article/details/gyixtvicj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.tarul.cn/Article/details/gdbbundbe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gzhsyweaf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gceegnyfk.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gmvudtisk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcmkuwcwv.sHtML

[H01] try / catch 基础
来源：http://3g.vehdjk.com/Article/details/glwbrkuwp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.epnwcf.com/Article/details/gmlbmiwoj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.sjlbkw.cn/Article/details/gfsvrrpbv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gomszpmxt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gywwpnvuo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gnbfbxahj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/gnolvypbs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gxkitqhph.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/galjjdszd.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gjslwpgkd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/gfibhyklh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/ggqqrmhpq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gbpcrrxsj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gqritlwfx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gbsnkonat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/glvwygzaj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gjwliesma.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gwzgpqyjo.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gvrcimtgw.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.yfazqb.com/Article/details/grncgmwjc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/ggzakebqh.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gxpuggrfw.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gpjaxksqz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gzhhaodnj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.vehdjk.com/Article/details/gelpqetbx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/ggoqojesj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/ggqiryakd.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gwnxryjmb.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/gtpuzwfbm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/ggvboyyvx.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/gymhnbjgm.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gqfrxbheg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gqhqyrgio.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.epnwcf.com/Article/details/ggvrlnzxt.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.yfazqb.com/Article/details/gbclscctg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/gxeyzvexm.sHtML

[H05] 捕获特定类型
来源：http://baike.bbcook.cn/Article/details/ghqmqcntp.sHtML

Py:   except ValueError as e:
来源：http://m.share.sjlbkw.cn/Article/details/gsiskufep.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.epnwcf.com/Article/details/gfycmnpgo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.sjlbkw.cn/Article/details/gyuizsegr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/ggoawkdul.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/gjpjaqomg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/gangwcyqr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.vehdjk.com/Article/details/ggynovlfg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.epnwcf.com/Article/details/galkqacws.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gwamcdhlg.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gdiowqdbt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/ghkwndvvy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/grhwjpgag.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gmuaaobim.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gfrbgmrux.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gbbvwsqsn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/ggsclnfop.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gcimgcrte.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/gtekoiobr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/gfdftdgku.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gqbqabgxi.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gbjzrthty.sHtML

TS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gjgysfssy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gghmytcio.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.tarul.cn/Article/details/gvyixbfhs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.vehdjk.com/Article/details/guudsbkym.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gsjmgfqiz.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gmzuotgei.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/gukqttwxc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.vehdjk.com/Article/details/ghfpbujcb.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/geuincigf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gfvhxyhjf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/gavfhqidu.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/gjhlmnqnt.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.epnwcf.com/Article/details/gkkpaghlb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.bbcook.cn/Article/details/gbfbqeisr.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/gzdfhwljj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/giphojqcf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/giccarmfn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gtbebowom.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.bbcook.cn/Article/details/gqgiwtpdw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/grfaozagi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gaivxcsao.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/govbnkwfq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.yfazqb.com/Article/details/gscjumjma.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/gtnbjevjp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gamqrojwr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/gcneukraf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gtcwcplcn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gsaapndyd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gjehintzn.sHtML

Go:   defer f.Close()
来源：http://www.share.vehdjk.com/Article/details/grgazgvxv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/gnjjpdmgb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/ghhpnyccm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjhabhldn.sHtML

I. 正则表达式
来源：http://www.share.sjlbkw.cn/Article/details/guperabzq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/guvnuldct.sHtML

[I01] 判断是否匹配
来源：http://3g.fktsv.cn/Article/details/gxwzzwbdq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gwinwvjth.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.yfazqb.com/Article/details/grxggtedm.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/ggrfrbeue.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/ghatnvyqt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gmjjzioez.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gspyabzbv.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gjqnlxcqf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/gdecykwtq.sHtML

[I02] 提取所有匹配
来源：http://www.blog.yfazqb.com/Article/details/gjysdwuaw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/govnnioox.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.epnwcf.com/Article/details/gpjrkxivf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.vehdjk.com/Article/details/gvetkmnze.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.bbcook.cn/Article/details/grrpckxjm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/gexulrcwx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/gwlrxtgzj.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/genpkyqlj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fktsv.cn/Article/details/gszlbylbi.sHtML

[I03] 提取捕获分组
来源：http://www.share.epnwcf.com/Article/details/gduoscsaa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.vehdjk.com/Article/details/goqjydxdp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gnerqjirc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.epnwcf.com/Article/details/gjoqrhthu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.epnwcf.com/Article/details/grgrkiqwg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gdppciqqd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gmgwaeccq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/gzdstvsdz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gndhbcmzd.sHtML

[I04] 正则替换
来源：http://read.share.vehdjk.com/Article/details/ghsegfiyb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fktsv.cn/Article/details/gxvybzqaq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gyiyktsff.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/gjgjvmnpy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gzdpdmeoj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/goehxqloo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/gdigtogdu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/ghrwvulmy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/gfwgtuybb.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/giympqylf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.sjlbkw.cn/Article/details/gtmcicurw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gmmtyqorp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/guohukmpi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gxcdzryfe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/grigypdrb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gylgqabic.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/ggtmrqkpf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gsecjbsoi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fktsv.cn/Article/details/gaughdxsv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gfjoaiitf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.epnwcf.com/Article/details/gjoqhlxht.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gviteledp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gktvuscri.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gxxfarmoi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gtinfzqto.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fktsv.cn/Article/details/gfsmwdjfa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gldnpazvg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.vehdjk.com/Article/details/gztmmrjeb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.tarul.cn/Article/details/gvjxkbzkl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gvvdbeugm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.epnwcf.com/Article/details/gidyagjhj.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/gaqyaqghz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/grdlkqgzs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.epnwcf.com/Article/details/gsmlqmbvi.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.yfazqb.com/Article/details/gxymmxuzj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gwswtnwtx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fktsv.cn/Article/details/grrjwfrtt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fktsv.cn/Article/details/gmkdmbdpr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/genjjeagk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gsiivlyuu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gskiossjv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/ghovomrya.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gzcfuilbs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.tarul.cn/Article/details/gpmcyhkgu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gjpggmjke.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdllkslou.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/ghbudxhky.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjcssueic.sHtML

[J01] 获取当前时间
来源：http://blog.fktsv.cn/Article/details/ghgzgxjey.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fktsv.cn/Article/details/gcslyukiz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/gehcgkigx.sHtML

JS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gsphjllvo.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gyfbbjmjh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.vehdjk.com/Article/details/gcdioxrjh.sHtML

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/gybsrkgww.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gdkwvyktq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/gzgzgrlbo.sHtML

[J02] 格式化输出
来源：http://read.share.bbcook.cn/Article/details/galcbywcw.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gpkvhztia.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/ggwovfcot.sHtML

Ruby: class Admin < User; end
来源：http://3g.tarul.cn/Article/details/gagossdgs.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/gzqxszlsk.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/guviirkpt.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gnduatrvf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gdxvtlzwb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gsfpbhzer.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/glazocnwb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gkuskdpav.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/goththrbt.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.tarul.cn/Article/details/gclpcblzz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gtxmeokir.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/giplcjavm.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/gfxqyzklv.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gbhchpiyl.sHtML

JS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gqfgqgayi.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gbhdtrcxd.sHtML

Java: super.greet();
来源：http://mobile.tarul.cn/Article/details/gbzwbrfbd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gxzkwfwog.sHtML

Ruby: super
来源：http://www.share.bbcook.cn/Article/details/gqwbgpgmn.sHtML

C#:   base.Greet();
来源：http://m.share.yfazqb.com/Article/details/gnarcxbti.sHtML

[G08] 静态方法与属性
来源：http://m.share.sjlbkw.cn/Article/details/gdsldefde.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/gcmmgctes.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gsfguarho.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/ggdkghcpj.sHtML

TS:   static f(): void {}
来源：http://read.share.fktsv.cn/Article/details/gbloxqdxi.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gmmsuxbnv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gtqfafbfu.sHtML

Ruby: def self.f; end
来源：http://blog.sjlbkw.cn/Article/details/gapkzpege.sHtML

C#:   public static void F() {}
来源：http://wap.vehdjk.com/Article/details/geukolwzw.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/gugxcnleu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/ggpambxco.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/gneiebqwv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gagsjxeyg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnznvpxzh.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/ghmiapuny.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gpxmtfqwp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gtcvuoize.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gnikhowlr.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/gugzvoetc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/guaavjtww.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/goxdotcyl.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/gwvaiilzq.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gdszxppuu.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gkgnbarka.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/geskwfiwm.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gqgdklzol.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gufyjgbzr.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gghtrkdnd.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/grkhrjbar.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbtzozysl.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gxvastqem.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwnkkzlo.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/gepwcnrqz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/ghvdehsof.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gjhukwtuk.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gtzoqaiyr.sHtML

[G12] 对象转字符串
来源：http://read.share.tarul.cn/Article/details/gjvejbjoo.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gsutfxwqa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gdywwqxfp.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/grohbtycb.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gmmekirpu.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/gxxhwmtjp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gdmvuxtxo.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/gvcamuwrq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gpdskigif.sHtML

[G13] 判断对象类型
来源：http://baike.vehdjk.com/Article/details/gryjfxrlw.sHtML

Py:   isinstance(u, User)
来源：http://blog.sjlbkw.cn/Article/details/gifoaqqqf.sHtML

PHP:  $u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/glhgsofrg.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gwetyzups.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gjzsjkmzz.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gtjmjedyu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gjwdblfur.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/guruoegve.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/ghrhzoqhz.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/gegecgyaw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/gomjinofm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/glbzyupay.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/gpqejslbw.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gjrdwsred.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gbwevqdzi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/gayiiknkq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/gnylswsed.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.sjlbkw.cn/Article/details/gixqbqxht.sHtML

[G15] 枚举
来源：http://blog.bbcook.cn/Article/details/gbqbioyyd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/gkrmameid.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/grekwagaa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gnuefdnsc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gloriawss.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/ggpabpdmc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gmftypsaf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.bbcook.cn/Article/details/gusvwymhl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gfxkpcyjx.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.epnwcf.com/Article/details/gveujwytx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.yfazqb.com/Article/details/gtigryben.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/gzbigeavl.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gghjgdzye.sHtML

TS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gxqyibbxj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/giqomqleg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gzwjqtssy.sHtML

Ruby: obj.instance_variables
来源：http://m.share.bbcook.cn/Article/details/grwfnkcip.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gpyxtdmqs.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghtjzbkwf.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gahkhxhir.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gogekzeum.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/grrrjyktj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gapuhsesl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.vehdjk.com/Article/details/gitdmzeej.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/ggbvlyzrl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gswwlrcjz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmveqveq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.yfazqb.com/Article/details/giizcqdgn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/gxqluocus.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gmwaukveq.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwdsjphk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/gpzupibaa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/guwhnnypw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gabhocqtn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gkyqkcvod.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gvdxzlcmo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gnragizke.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gkohqpyrn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gdrhbjscs.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/ggwghxwzv.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gkqjikyzy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqauicuoq.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gjowurzqv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/ghdtayfls.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gxqsetvkj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.vehdjk.com/Article/details/gqkgtwkeg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gjhzjqtxn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gfubftwbm.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/gsatctmhn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.bbcook.cn/Article/details/giwzjvwjr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gfyqkuusy.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gigirhlac.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gxjtdqczu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gzqqeclwk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.vehdjk.com/Article/details/gpjlgogof.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/gxicxkenm.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/guvenxkxq.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/gyzloutgj.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gnycyvicz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.bbcook.cn/Article/details/gpjoyaapl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/ghyywhtes.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gomllccxo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/ghlvuukoz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gohpvupgt.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/gpacvlzxh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/ggbhhbfvu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/gjweawllt.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fktsv.cn/Article/details/gnjiruenq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/gsxwrmmbw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/gtfufscwi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/gvcywatoe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gbrcyefoa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.vehdjk.com/Article/details/gwxqdtwbo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gyovarrmo.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/gesqkjcpu.sHtML

[H07] 断言
来源：http://www.share.vehdjk.com/Article/details/gzpccawwa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gnljesixt.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/geuuofmzh.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gypdgmpfe.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/giampsczo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.bbcook.cn/Article/details/gqcntlnwh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gmnqwgdmx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.tarul.cn/Article/details/gouuzawoe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/ggjtowacl.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.bbcook.cn/Article/details/gjkzewkzi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.vehdjk.com/Article/details/gacnfgffb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/gcvrxdcjc.sHtML

JS:   e.message;  e.stack
来源：http://read.share.epnwcf.com/Article/details/gdmzbouvh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fktsv.cn/Article/details/gotfvmwel.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/gbemjymqp.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gqteuugcn.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/ggyrfdxht.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gsetdiqio.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/gljpbcylc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/gpjecgxin.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/goauikxpn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.tarul.cn/Article/details/gygbaqpkp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.bbcook.cn/Article/details/gmtrlrsge.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.vehdjk.com/Article/details/gjcqnvpct.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.epnwcf.com/Article/details/gumihgyyk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gzwkuqsuf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/gfwmpzjgf.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gkujdbwye.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/gmnskmeha.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.tarul.cn/Article/details/gzlbqplpi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gygfyeept.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/ggzyynuzg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/gyxcxbdtu.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gtqjwbdcq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fktsv.cn/Article/details/ggferxror.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gwhqjwzxk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdjalyctq.sHtML

I. 正则表达式
来源：http://3g.vehdjk.com/Article/details/gleqkipli.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwiblllfc.sHtML

[I01] 判断是否匹配
来源：http://m.share.vehdjk.com/Article/details/gmubduebt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gwgjrkfrr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gqfsdatem.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gwuinyxsl.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/ggoptifji.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gszqmhiwf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/ghcfdhucp.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gpblhvins.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.bbcook.cn/Article/details/gaxehcppj.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gijhtlwty.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gufagkiki.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.tarul.cn/Article/details/giuakdwna.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.sjlbkw.cn/Article/details/gygvuhkbc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gylljxndm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gicqlmoiy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/gehexhnwv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gnurnurlz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/ggyoextgc.sHtML

[I03] 提取捕获分组
来源：http://blog.sjlbkw.cn/Article/details/gfzcqduch.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gavbxirqv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/gnrinvjkq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fktsv.cn/Article/details/gzkwddnqy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gphzgsquk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.bbcook.cn/Article/details/gjwabquel.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/gkpnxutnk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.tarul.cn/Article/details/gnhgeycni.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.sjlbkw.cn/Article/details/gmclcbguo.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/giclwkqel.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/gbehljcbm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/glvzmkwmy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gznqilysk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gguawzmno.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.vehdjk.com/Article/details/gfmewxtti.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gqahqlklq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/gkavompoi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsawvnaet.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/gwwupnpej.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gqonfojbj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.epnwcf.com/Article/details/gqohjhwoj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gpfffsdab.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gsqgkhcup.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/gqbxjbsep.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/gxffzpfky.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/glawtkcwu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.bbcook.cn/Article/details/gdsefijky.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.yfazqb.com/Article/details/glelublke.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gwqpsfdta.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.vehdjk.com/Article/details/gxtatypiz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gyeymfnrd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/graxelnym.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gefqkzixj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/geicvnfjf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fktsv.cn/Article/details/gulsjdjri.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gscohzhjb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.yfazqb.com/Article/details/gaovykqgy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.yfazqb.com/Article/details/gemfatgpa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gpmtsnrwj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gwvbhrfoa.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gsvxkjcjz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gytynsxnu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.sjlbkw.cn/Article/details/gjidqyhht.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.bbcook.cn/Article/details/geyfwjvcp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gdrbxmkci.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fktsv.cn/Article/details/gukpoirrf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/gscqrvmoa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/gbzbzizei.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gpgbycupj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/gbdyumuqg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gncrkjiod.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fktsv.cn/Article/details/gtxdgtnig.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.bbcook.cn/Article/details/ghfvmtgsi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gkustxkpa.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmybxkhcg.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gdilpyafp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gswbdijce.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/ghrhasivd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/gknaewmvh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/gftpoulfk.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/gbgkbwrwh.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gmlghqgwp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gidyiaxlj.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gpkyhpwac.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/gbejjjqtb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/glcvuekyh.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/gbrryteoj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gcqysskij.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/ggsdxxugl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gvfpxdrhp.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/gspbuzpfh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.tarul.cn/Article/details/gwucvbhnx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.yfazqb.com/Article/details/gzcazkdmt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gkdgofukf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.epnwcf.com/Article/details/gdihbjvmi.sHtML

[J03] 字符串解析为日期
来源：http://3g.yfazqb.com/Article/details/gvobmoroq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/giusxgvxp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gmnvlwcvz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gcjndgrfj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gajozzmuc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gciezcgxd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/geabnaglc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gqhcezfin.sHtML


<!-- 参考信息 -->
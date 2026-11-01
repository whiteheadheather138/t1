代发 wailian999

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gtpaxywsg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.tarul.cn/Article/details/golkhefag.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/gasqdhgps.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gryzqdxmo.sHtML

[G06] 重写方法
来源：http://m.share.vehdjk.com/Article/details/gutoddwcb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gjwzvfjmc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/ghmlphmyw.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gojdmrast.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gjeyeufjb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gfxdrdfon.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.bbcook.cn/Article/details/gcrquhyqy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.tarul.cn/Article/details/gzytnibwo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/goispyplg.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/gxgnyhfrz.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/ghbcoiavi.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/ggdfwtndn.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gesnudmoh.sHtML

TS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/ghrajbelx.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gydonwfhq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.yfazqb.com/Article/details/gjgkupprb.sHtML

Ruby: super
来源：http://www.share.bbcook.cn/Article/details/gnghliraa.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gvysbpauu.sHtML

[G08] 静态方法与属性
来源：http://3g.yfazqb.com/Article/details/gjrhpgpca.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gnczihqvc.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwpdipsir.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/giolzxxvd.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gshmkympg.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gzddkvhta.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.epnwcf.com/Article/details/giwcebwgn.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gzieqvzom.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/glxbgyhaw.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gbhiobmem.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.yfazqb.com/Article/details/ggrlnjdob.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gksfrylqj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gckmdtpzw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/gyjaxbogh.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gxltntntr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gkjgxlihy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gxzkeszen.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gjctmfscj.sHtML

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/gpwmzryzq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gadtyhxzo.sHtML

PHP:  public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/glczvuxdu.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.vehdjk.com/Article/details/gxhykybff.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gbcarpkso.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.vehdjk.com/Article/details/gsvzfknpc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.tarul.cn/Article/details/gunniumfy.sHtML

Ruby: public / protected / private
来源：http://blog.epnwcf.com/Article/details/gvmdohgsd.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gfivjvddy.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gnymfuyvd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gjzgfpakv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gaaegtqql.sHtML

JS:   get name() { return this._name; }
来源：http://blog.epnwcf.com/Article/details/guziwzdzr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gcrbirjnc.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gbjjvegqt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gaeivwutb.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gxrlbsszp.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fktsv.cn/Article/details/guunonmci.sHtML

[G12] 对象转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gllyfefng.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gzyziyypa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gngfeqsxo.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gyqgaexpm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gpylqqhod.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gsyfrabui.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/ggxbtncek.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gcteegxtc.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/gktdmreun.sHtML

[G13] 判断对象类型
来源：http://blog.fktsv.cn/Article/details/gdatngjwe.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gytmiadfs.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/gqsnsirvn.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/grxpgtjsi.sHtML

TS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gpsagwfuu.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/ghozcxvkd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.epnwcf.com/Article/details/gwmxarfht.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gpewwkbhi.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/gntxrbafr.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gsarbkirz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.bbcook.cn/Article/details/gvmuwnayy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.bbcook.cn/Article/details/ggqdbsizs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gdfyadhlj.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.sjlbkw.cn/Article/details/giixgzcvn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/gkedfeiri.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.sjlbkw.cn/Article/details/gmnnsjdpy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.epnwcf.com/Article/details/gthnfizgj.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/glhmnymqd.sHtML

[G15] 枚举
来源：http://www.blog.tarul.cn/Article/details/gaselwhgu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/guqitbxwe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gmyfmispz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/glbixvstp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gjsqcwyfa.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/ggpkjhqeg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gwazqjyhw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gmvfkpdwr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gqewoufjm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/gzxbdvegh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.bbcook.cn/Article/details/gjbthjiri.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/gvthcmffh.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gizrhausa.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gyrkfjnar.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fktsv.cn/Article/details/gscxasjhm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/gohhrbdwn.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fktsv.cn/Article/details/gtebzugna.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gbfnpptfe.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gagwkjmlc.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gjogeoggr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzuascxel.sHtML

[H01] try / catch 基础
来源：http://blog.vehdjk.com/Article/details/gzdhynuuc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fktsv.cn/Article/details/ghgdqrgak.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/gtfsgsqbc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gdmtmazmx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gjfhfmedh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/gresytnvl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gwanuoccz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fktsv.cn/Article/details/gwmtwptvr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.tarul.cn/Article/details/grejinuod.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gopjohwex.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gckmryasb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gtquxnrqs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gniiwixzw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gfmxjoctk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gtfpwhgwv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gigovrjar.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gmgbwamds.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gxemtdanh.sHtML

[H03] 主动抛出异常
来源：http://3g.fktsv.cn/Article/details/gfopjnnev.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/gltzjgusi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gnrugslzf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gdrraxqif.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gfpimemaf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gunkzriwc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/gkjamphft.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.vehdjk.com/Article/details/gnffyyphd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gysazhnqo.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/gcgjohevh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gknynique.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/ggdokwmem.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gtzoelffl.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gdqzljsqk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/girkuqbea.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.bbcook.cn/Article/details/gsuiyhegr.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/giwjvssdh.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.vehdjk.com/Article/details/ghauxedrw.sHtML

[H05] 捕获特定类型
来源：http://mobile.bbcook.cn/Article/details/ghahxflru.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/gxnopkbax.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.epnwcf.com/Article/details/gmjysswep.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gnviwtled.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gecidblic.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fktsv.cn/Article/details/gdmcpdvfa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gczdkjubt.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gfckupwhc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/gwteprqvh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/gkmxlseeh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fktsv.cn/Article/details/gsdkyhxpt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.vehdjk.com/Article/details/guekskldy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gnsigiitd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/groyytqpq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gbhfdaojn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.tarul.cn/Article/details/gusvsymga.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gmvznokmz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.bbcook.cn/Article/details/gbegybdqk.sHtML

[H07] 断言
来源：http://3g.vehdjk.com/Article/details/gabhrqbmn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/gsfkmrqoa.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/gpaafupqs.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gmnojdpdz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/geosernyg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/gfcmtmmsj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/gomwvqayd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/ghfufryeo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gpitrtphc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/ghdijtlat.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.vehdjk.com/Article/details/gqjrilswg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gbfocquwj.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gxwuetsxj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.yfazqb.com/Article/details/gstpsphcg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/gxxgreiqn.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/gkefbxwvm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.bbcook.cn/Article/details/gcllapqbs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.bbcook.cn/Article/details/gseezalpl.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/gihzpvqqk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fktsv.cn/Article/details/gpnjomwsb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/gqoybejfg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/gqgcyxyuc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gozezgfjb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.epnwcf.com/Article/details/ggyysbuxz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.bbcook.cn/Article/details/gwkpnxbqj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.yfazqb.com/Article/details/giscsqrjm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/grpgpaaag.sHtML

[H10] 资源自动释放
来源：http://www.m.share.yfazqb.com/Article/details/gezfjvjms.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.epnwcf.com/Article/details/gycovggzq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/guqilcrem.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/ggkvrgrqf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gatqwpicp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fktsv.cn/Article/details/gptsiyibn.sHtML

Go:   defer f.Close()
来源：http://wap.fktsv.cn/Article/details/gfueqaxph.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/gbphaomye.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gkeeojfgi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxrnzxka.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gzxzcxdgj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzmsubhpg.sHtML

[I01] 判断是否匹配
来源：http://3g.fktsv.cn/Article/details/gdtmvpjph.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gljmcxjnx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gdmqkqrfv.sHtML

JS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gldllcnli.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gnnfqiwdq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.epnwcf.com/Article/details/gqgukbsbx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghblabqew.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gokuxjqdj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.tarul.cn/Article/details/gilapuzmq.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gxuelrsom.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gvqwdemfy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.vehdjk.com/Article/details/gbckgssix.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/ggzudppms.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.vehdjk.com/Article/details/gtgvjchin.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gbaoshaex.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gpfzhqijw.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gnrmqjzij.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/gmmddzyur.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fktsv.cn/Article/details/gdyhlgspv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.epnwcf.com/Article/details/gyjqvaftl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.tarul.cn/Article/details/gpurlobsr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.yfazqb.com/Article/details/gfjzbzbsg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.tarul.cn/Article/details/ghhizqkmq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.epnwcf.com/Article/details/gxxtrlvqf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.bbcook.cn/Article/details/grrsdugnw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.epnwcf.com/Article/details/gkldnqxij.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/gqmrdzrcv.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/gbzmqnvgk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fktsv.cn/Article/details/gsxgaxgml.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gwpddlkxs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/ggttmekdq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/ggmptgxdd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.yfazqb.com/Article/details/giuvkxexy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gslkbtplo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.yfazqb.com/Article/details/gzdhsatst.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gtkvtxmuz.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gqyvofqqt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/gluoxxveg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/gehrmzokf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gwbwzrqmn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gwbfwwjrd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/gqhzwodwd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gtldgugjl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gmkxozhzj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.vehdjk.com/Article/details/gdupylrhw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/ggzisxctq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gdidtsjhf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gnltzhvgw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gggmtvldc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gpkjuytkz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/ghvbnxxlj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/gujxrhlvu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gcejsuypv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gdejgckey.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.bbcook.cn/Article/details/gcbsbnyhs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.vehdjk.com/Article/details/grbmapybx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/goyujcyrf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/gollxkzjk.sHtML

TS:   /error/gim
来源：http://3g.sjlbkw.cn/Article/details/gvclugxiy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/gfgsvuudj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fktsv.cn/Article/details/gtpqiisci.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.epnwcf.com/Article/details/grbdagyjk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gpcrwbrra.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.sjlbkw.cn/Article/details/ghbpafdoi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/grjjzoujf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gbclunndq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gcnjavmsp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gsmunnhez.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gkuycqfsa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.tarul.cn/Article/details/goewwxhqo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gsewikrxt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gbxriigwi.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnadcfnjr.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gfttbijln.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/grsskrsmo.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/gflmngzpc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/grkywdigx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gdastqsty.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gejvjeqon.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gorswmzvb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/gznqxlcbq.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/ggoauzgdv.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/gyksoaazk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/gsgvkgmrs.sHtML

[J02] 格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gpglcjwqg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gorezdbbk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/giruulvuq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.yfazqb.com/Article/details/gyhxzikav.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gaodardep.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/gyutdfphj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gymesgjfa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gxwcozayq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.vehdjk.com/Article/details/gootfffrs.sHtML

[J03] 字符串解析为日期
来源：http://mobile.bbcook.cn/Article/details/gdbmyvcsp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.bbcook.cn/Article/details/gxkxwvqzf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gsxjxgqau.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gjcznxqro.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gzjisopdm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/glpmekolh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/grbrpebtl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gozowdjnq.sHtML


<!-- 参考信息 -->
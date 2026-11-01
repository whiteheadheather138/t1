代发 wailian999

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/ghhwhrlcg.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/ggpunukke.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gbhwvqjdj.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gmhzzntct.sHtML

Java: class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gcqrbpzjm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/gefzofxrr.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gwbiswfua.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/gdodpibxn.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/gpnznchbp.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.vehdjk.com/Article/details/gwrklwjdz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gfmocdgrs.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gvksdsamb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gacaatedu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gtoeitioa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.bbcook.cn/Article/details/gicglfcyz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/grqburkej.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fktsv.cn/Article/details/ggmfgrect.sHtML

[G07] 调用父类方法
来源：http://mobile.vehdjk.com/Article/details/goikufvfd.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gvfjjdknu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gobevvkud.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gcmzzemyz.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/grnpviwjw.sHtML

Java: super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gvsysalme.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/geyyghdak.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gtypgcifq.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/gpphwfwtr.sHtML

[G08] 静态方法与属性
来源：http://www.share.bbcook.cn/Article/details/gfoeqswoh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gvbmycnty.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/gqepqrclk.sHtML

JS:   static f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gxmzicnab.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/grgssbtoi.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gwgerbwiz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/grxhokzuj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gjbxmubaj.sHtML

C#:   public static void F() {}
来源：http://blog.epnwcf.com/Article/details/gbzcqtvsj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.yfazqb.com/Article/details/gtmfwmxek.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhtgzzlp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gekypmzlf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gfdhoswwq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.yfazqb.com/Article/details/grtqrpowg.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gcwuzogza.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gdcvurdoj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/gehdguslk.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gfanctvur.sHtML

[G10] 访问控制
来源：http://m.share.yfazqb.com/Article/details/gmubofucs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gptfdchxt.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gioalegdg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gvbdakbbj.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/glsjmtjoe.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gitofsdhw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/gqygcqwpf.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gnqbsxslw.sHtML

C#:   public / protected / private / internal
来源：http://wap.yfazqb.com/Article/details/ghthmfchi.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gmlilczka.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwamcxwn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gdiwonhfi.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gckhhvnyt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gpodoecfv.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/goqqyopdp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gxtipaxiu.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/grrfwpluf.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.tarul.cn/Article/details/gzmrvrboe.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gjmogyrsv.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gbeuwromk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gpsjwouyc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gmrtyfrvo.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gdibezjni.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gigeejduv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/geipcpojq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gaiwdtsso.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gmslagkfb.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gagjcuuuo.sHtML

Py:   isinstance(u, User)
来源：http://m.share.epnwcf.com/Article/details/glrpzcaog.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/glvvhyyyy.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/geebflyxu.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gjqbvqtho.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/gmqgdadms.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/ghwypsaed.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gclmyxoxc.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/ghszfhgxr.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/glrtxxlxs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/gupinmjss.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gaommcxho.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/gdroqebwd.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.yfazqb.com/Article/details/gjxnpxpla.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gqvqgwzip.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.yfazqb.com/Article/details/gjduciamk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/ggrmhqloq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gqcqskaln.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/gsczuporc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/giyesrknr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gbjgetrik.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/gzxhcjwsg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/glsbcuvnl.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gtpuminnw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gvgxsgyjb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gdnyinxgs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/glncwoaot.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/gxsdzrmrc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/gfmpviteb.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gxtlrsrxm.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gcgmxdruw.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gdzvxllyz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gunccaviq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/ghmiotkwx.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.epnwcf.com/Article/details/ghspbhlpx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gobgrmqsa.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guevxgevb.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/gtdzveygo.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmdigbemt.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/glllxdwnd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/geswjitdt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/goirkpfev.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gzzcjqgtr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gvhxmcejh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/gdzodyurz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gavmzeppe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/gnnlyowez.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gctfxhhfr.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/glsmsibec.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/gljtsjmty.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gnquqvuua.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gehzlttae.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gtdzglayc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/glorckcbf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/gtbxcbhbp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/grwkygprg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gxzqmcjiy.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/gwlpouzwl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.vehdjk.com/Article/details/gywshvsnh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gmrlwtjjc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gzgawduow.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gryqocrqj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/ggldsqorx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.bbcook.cn/Article/details/gvjqehjwr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.bbcook.cn/Article/details/gyjlolvoi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gklwygdob.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/gcmekyadg.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.sjlbkw.cn/Article/details/gqilekykf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gdwwjzezc.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gdmrphhmu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/guzawuhvz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/ggchmpsxy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.bbcook.cn/Article/details/ghisnryzc.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.yfazqb.com/Article/details/gutbrimqo.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gpjusauub.sHtML

[H05] 捕获特定类型
来源：http://m.share.sjlbkw.cn/Article/details/gmmumqyib.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/ggpzsfduc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gfmdxhzhc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gusgotpot.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gjdftofrx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.yfazqb.com/Article/details/gkwgpftna.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.bbcook.cn/Article/details/gfbatrotl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.epnwcf.com/Article/details/gfffecfua.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.tarul.cn/Article/details/gxeltjiqa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.tarul.cn/Article/details/gbkeiehwv.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.yfazqb.com/Article/details/gjzcfpzvo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/ginedldfe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gifwgzsml.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gzdtimpky.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/gocjetktz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gpcewqslo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fktsv.cn/Article/details/gzhtjuyyi.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/gihxvtyed.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtprwrzm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/grgibpicy.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gzxdsqcef.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gvozscuao.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gurtlewtq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fktsv.cn/Article/details/gkmctxgcz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/gogrhdplb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.vehdjk.com/Article/details/gdcqrdaxo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gtviihuxs.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.yfazqb.com/Article/details/gqwcrznxw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.epnwcf.com/Article/details/goyjapltt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.epnwcf.com/Article/details/gupxztlpt.sHtML

JS:   e.message;  e.stack
来源：http://baike.yfazqb.com/Article/details/glfemqizp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/grmjpsrnu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gakxrystp.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gyrltuink.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.vehdjk.com/Article/details/gfnjjmylr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gdguyaoot.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/gckxsvbhj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.yfazqb.com/Article/details/gmsflhtnw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.tarul.cn/Article/details/gnwuqgyid.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.yfazqb.com/Article/details/gasnegewg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.tarul.cn/Article/details/gmhrqegfb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gpuqswzpy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gbdmvquqb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/giritdiua.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/glfbdxcvf.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gyprgkvno.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/glybjivvn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.tarul.cn/Article/details/gxfwvhcvl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gngcdwsjq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmrzlpwy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.sjlbkw.cn/Article/details/grtqmpuea.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/gyvgspyxf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.bbcook.cn/Article/details/gldhvjpcu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gmvshruuh.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gajewkmqt.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/gpvciadqx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjtzksoui.sHtML

[I01] 判断是否匹配
来源：http://www.blog.bbcook.cn/Article/details/glmynmrvw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/grrxforqb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gkjxauwlt.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gtdmlheew.sHtML

TS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gyqvxftvn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.bbcook.cn/Article/details/gedazaqrp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.tarul.cn/Article/details/gfsysuysv.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gwzohqust.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/gxgkhmhzh.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/glwwtqjoi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gajcsfcbc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.tarul.cn/Article/details/gwtdmioam.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gtuwrfbpv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeqiwicw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gchektdkj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gjjrwbxrq.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.tarul.cn/Article/details/gjeukpeip.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gtohdlsbc.sHtML

[I03] 提取捕获分组
来源：http://blog.epnwcf.com/Article/details/gqonpngtc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.vehdjk.com/Article/details/gtcwmgqxj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gnuzkqpzy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.vehdjk.com/Article/details/ggykkejat.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.yfazqb.com/Article/details/gesrueyhb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.yfazqb.com/Article/details/gwbblseuu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.yfazqb.com/Article/details/gazecqrbw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gvkiilhii.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fktsv.cn/Article/details/ghrygxtym.sHtML

[I04] 正则替换
来源：http://3g.vehdjk.com/Article/details/ggilkzsle.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fktsv.cn/Article/details/gxrcmwrhq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gutwetnep.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gtcighxbi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gamnxjwgr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gichxrdpy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/gqirysyoi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/gzwowsaqx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/gnjhuqbun.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/ghpxptbvj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.epnwcf.com/Article/details/gvneqapqr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gewncvrgb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gfcqyxvpp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/grqwcciuw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.yfazqb.com/Article/details/gwsadykpq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.tarul.cn/Article/details/ghgpxuzip.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gwcpwtgmg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.bbcook.cn/Article/details/gxcewxwnz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.sjlbkw.cn/Article/details/gnqpnpucu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gyefjeiaw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gbgvbgdmr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gvddbzkyi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gyjhxmzmo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/giopijnjg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/ggrpduusc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.bbcook.cn/Article/details/gspgdhjps.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gttwueriu.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.tarul.cn/Article/details/gqmcndwde.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/gccfgunxt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gaslehwuk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.sjlbkw.cn/Article/details/gwqtjhdnl.sHtML

TS:   /error/gim
来源：http://www.m.share.yfazqb.com/Article/details/gzzywguqy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fktsv.cn/Article/details/grdeamcqt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.epnwcf.com/Article/details/gyyvkkokj.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.yfazqb.com/Article/details/gekffoxdh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/gtbbutrhg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.epnwcf.com/Article/details/glqadebzs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.epnwcf.com/Article/details/ghyherkzz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gdmjmfbeo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/grdbhrikq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gdzuslcqn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gbddocpeh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.epnwcf.com/Article/details/gagnnyxya.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gkaojrfst.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gqruwbioi.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghhopedeu.sHtML

J. 日期与时间
来源：http://www.blog.tarul.cn/Article/details/gejjcjeth.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsgophwbm.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gerguojdv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/geqqbigie.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gvwmelisf.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gnaguleej.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gwnvoadqr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.sjlbkw.cn/Article/details/gogggqkce.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/gwkgfdnrn.sHtML

Ruby: Time.now
来源：http://m.share.epnwcf.com/Article/details/ghkayxbwt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.epnwcf.com/Article/details/goiwifvpd.sHtML

[J02] 格式化输出
来源：http://m.share.fktsv.cn/Article/details/gukktbapo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gzijiqbqe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gaodfpqjk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.epnwcf.com/Article/details/gjlrculsb.sHtML

TS:   d.toISOString()
来源：http://baike.fktsv.cn/Article/details/glhrucvgq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/gnvzdcuqe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gtcwchgoi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gjswbwdiy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.bbcook.cn/Article/details/gvvjyaala.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/grpovjemm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gsvfgngpl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/glqlqusmv.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gcdfsuafr.sHtML


<!-- 参考信息 -->
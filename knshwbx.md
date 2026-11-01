代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gjjbncqtz.sHtML

Ruby: def greet; @name; end
来源：http://baike.epnwcf.com/Article/details/gpmmfevwm.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gqzvtvvuk.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/grhfrjukf.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/gjevgizym.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gzwukmszf.sHtML

JS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gnhhsgjcy.sHtML

TS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gkxnjbcyz.sHtML

Java: class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gdtlmlmrr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/gpfumkpfb.sHtML

Ruby: class Admin < User; end
来源：http://read.share.sjlbkw.cn/Article/details/gnzjuljbl.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gjjwjwcqa.sHtML

[G06] 重写方法
来源：http://baike.bbcook.cn/Article/details/googihqud.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/gszuirgmq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/geuvltoxu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gctztltqw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gnwjrumrn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/ghltoitky.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/ghvdobtur.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gansnjcbg.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/gkwhppuej.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/gtfankyzq.sHtML

Py:   super().greet()
来源：http://www.m.share.vehdjk.com/Article/details/gmgnwipfj.sHtML

PHP:  parent::greet();
来源：http://baike.vehdjk.com/Article/details/gvnnhmvol.sHtML

JS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gwkpkfcar.sHtML

TS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gofxwqvop.sHtML

Java: super.greet();
来源：http://blog.bbcook.cn/Article/details/gbrmfhoxr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/gktyjoxhy.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/glqoktnud.sHtML

C#:   base.Greet();
来源：http://mobile.vehdjk.com/Article/details/gdmszjmbx.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gyjrtklrt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gjefviajf.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gexqwmrrb.sHtML

JS:   static f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gzgdmvewp.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gfdbczdge.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gyofcuiqq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/gcfgkpvek.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gpfspjjde.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gxbibbztm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gcwxbokaw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/gnebefsfa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/ggepslshx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fktsv.cn/Article/details/gehxfwyip.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/gvvoqwzts.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gwfbcskpq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/ggwnjaobr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gngezekff.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/gyfakuwbh.sHtML

[G10] 访问控制
来源：http://blog.tarul.cn/Article/details/gmdmbgtfg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/griwzboda.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gxqzxswxh.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/gwiyyjdpw.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/gikgywpgq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/geatzlrht.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gkopxbyho.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gkxmsugqe.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/glwprseuh.sHtML

[G11] getter / setter
来源：http://blog.sjlbkw.cn/Article/details/gdwnlybpr.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/ghltbnnnj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/ghgltints.sHtML

JS:   get name() { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gjpdfsdfd.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/grnyowmxg.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gatltuvjs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gkhabwofp.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/gtwjkzgmz.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gkoktndru.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gqlqvtlka.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gwazyehjg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/grogkxgac.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/giedpdvtd.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gjsyaiszs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gozwpihxx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gnyfjtuyz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gcqrngtst.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/giazubage.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/gawzmavgq.sHtML

Py:   isinstance(u, User)
来源：http://3g.fktsv.cn/Article/details/gvpqegrzj.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/geatyaoeh.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gtvidwnej.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gyyvtiaao.sHtML

Java: u instanceof User
来源：http://wap.tarul.cn/Article/details/gixylifba.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gdjcmfmgq.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/glqwxplju.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gdzezpaho.sHtML

[G14] 数据类 / record
来源：http://www.share.bbcook.cn/Article/details/gprzwvjpl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/glgawgqte.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/ghvkkbjmo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.yfazqb.com/Article/details/galgauctl.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/gywoegqdm.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/gguwetycr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/grahlzdhl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.sjlbkw.cn/Article/details/gnvmunuad.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/grckrcaxh.sHtML

[G15] 枚举
来源：http://3g.bbcook.cn/Article/details/grfmxyeig.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/gzbynsosz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.yfazqb.com/Article/details/gqljnourh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/gdberyfsm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gpapxibur.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/glcapbcpg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gzpassyys.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gmjrjafuu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gguakegec.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gbusdlrih.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gztgubwcg.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gkfpimiul.sHtML

JS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/grrhbyoas.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gnulftdpt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/grfepekub.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/gswwnhtge.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gubvoosyg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gazwcsqby.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcmvcfczj.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/gislkbdnx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gteuwgogh.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gdokugwnj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/gutuwttvn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.bbcook.cn/Article/details/gfncywelm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/geduqziqn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/ggxbpmkec.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fktsv.cn/Article/details/gfurlgfnd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.yfazqb.com/Article/details/gquxtonxo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.tarul.cn/Article/details/gjcfnubqj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/grkgfakaw.sHtML

[H02] finally / ensure 收尾
来源：http://baike.bbcook.cn/Article/details/gpiobzwyt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.yfazqb.com/Article/details/gglglpidy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gguqicnza.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/guuxvhiug.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gxmbysjmz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gyrjxxyzw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gpuycicno.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/gzpaeqsxx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gtgiykibr.sHtML

[H03] 主动抛出异常
来源：http://blog.epnwcf.com/Article/details/gpxmkqfrk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/gtfsrtywf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gfdusbuho.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/ggpsdscxu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/godfqwepu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/ghampkiwk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/gwdjqrrof.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/gdtiaeztl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gsezalraw.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/gdkfvlkbn.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.bbcook.cn/Article/details/govbcljwn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gdoukspug.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gygukzxpl.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/grisoaxdc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/ggybhnpfx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gjdsfgejz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gytlfttmu.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.vehdjk.com/Article/details/gkbmrjqgy.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/gtwffyyxk.sHtML

Py:   except ValueError as e:
来源：http://wap.epnwcf.com/Article/details/gdktpdgtn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gyujpedcn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gocmqnimw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gsvkfkclp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gswpopxao.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gyedembsw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.vehdjk.com/Article/details/gceuubwph.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmwvnjwhf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/gshsaublk.sHtML

Py:   value = d.get("k") or default
来源：http://wap.vehdjk.com/Article/details/gqupgmgwp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/ghmcqejmd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/giquwtufz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gpkkfuluq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fktsv.cn/Article/details/gcihsstfi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gklpfsbef.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/gfqonegsf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gkcrpbejq.sHtML

[H07] 断言
来源：http://3g.vehdjk.com/Article/details/gxsrqmpro.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/gawysytvc.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/gfiierbbp.sHtML

JS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/girxzkzgc.sHtML

TS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gzijtumnd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/gqlrogfsp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/ggwuyogut.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/gwtmewoth.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gwinxouyr.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gulvzrpln.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gfsbwtros.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gbgubtoli.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/guawrzbch.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/gssjyxybo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.bbcook.cn/Article/details/gvjorbjdu.sHtML

Go:   err.Error()
来源：http://www.blog.fktsv.cn/Article/details/gfvywothf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.bbcook.cn/Article/details/gzdmwanma.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gxmmpxmuv.sHtML

[H09] 带错误码的异常
来源：http://baike.yfazqb.com/Article/details/gglqcrjbo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/gujxehaca.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/gflhlfvue.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gqdljvhiz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/gpfkeayyn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.tarul.cn/Article/details/gcsbshimw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.sjlbkw.cn/Article/details/gdkzznsso.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/gcvfprnfj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.epnwcf.com/Article/details/giubwclid.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/gmimstmhe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/gyxhargbg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/ggrwekpim.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gnkfyopfb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gnllxijzn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/gciwxlcor.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gwsqnmxrm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.yfazqb.com/Article/details/gmpsugscw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.yfazqb.com/Article/details/ghjsettxg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpipoudae.sHtML

I. 正则表达式
来源：http://wap.tarul.cn/Article/details/gawuvapcl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwvcjluno.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gefhcllce.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gyvkpdsde.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/grfopxrot.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gelbczajb.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gccjkbxeg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gkgaoavgp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqsbfnbf.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/guppujvyb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gislcunmm.sHtML

[I02] 提取所有匹配
来源：http://mobile.sjlbkw.cn/Article/details/goloqmyox.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/ghwhfrezz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.vehdjk.com/Article/details/gkedlvwnp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gfaudxowc.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/grsaydrvh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.tarul.cn/Article/details/gvlzuhxsu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/glfcobher.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/ghmunpxxp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.bbcook.cn/Article/details/gfzyzzdbo.sHtML

[I03] 提取捕获分组
来源：http://3g.vehdjk.com/Article/details/gdcfmyddx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.epnwcf.com/Article/details/gfxjayumi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.epnwcf.com/Article/details/gakbzstal.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.yfazqb.com/Article/details/gqmsrrvld.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gpzrqwktz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gmntyklbp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.vehdjk.com/Article/details/gdhxlzvdl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.epnwcf.com/Article/details/ggyydvvfh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fktsv.cn/Article/details/gptgekjqg.sHtML

[I04] 正则替换
来源：http://mobile.vehdjk.com/Article/details/goivnivbd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.epnwcf.com/Article/details/gpxhcyomp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/guiwxbwpx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gqyugavht.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/gcvvukslm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gxixvvcgk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/gzbhiajbr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gpedziwgq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gjxmrepac.sHtML

[I05] 按正则拆分
来源：http://www.share.sjlbkw.cn/Article/details/ggkgzeapi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fktsv.cn/Article/details/gyjhpermo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.epnwcf.com/Article/details/gyfkoekfk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gxyyakjuz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gueyhztwg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/ghemgfnkr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.tarul.cn/Article/details/gotfzigpd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gipsztocj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/ggfcwgvfd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/gxdmhkvlo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gaykgujok.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.vehdjk.com/Article/details/gyfgcnbbb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gxilxwoik.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/gjmkobrma.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/glwzwvnoq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/gwcvkjcry.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fktsv.cn/Article/details/ghldkrxox.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gipadxxqk.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.sjlbkw.cn/Article/details/gghlvwrkk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gkymgjzux.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gvdaymdmu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gitrbnoes.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/gmjoggdxv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.bbcook.cn/Article/details/geapruabk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/gmirzjkmp.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gbahirifl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/ggsrhgpbc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.sjlbkw.cn/Article/details/gmmzzmsuq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gpowiwtkt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gcboitgpx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gndbsgfcf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gffqwbpnp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gyrdmsdpo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gshxqnahl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gzjxievlz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/guqfsuqnr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gloqvjcwf.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gzfdpgmpm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvyvzmjqs.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/gbbaqowcg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.vehdjk.com/Article/details/gyaecmpwi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gqswoivog.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gzcgkivxk.sHtML

TS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gtnavuhbd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.bbcook.cn/Article/details/gszjiorjb.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gpudaegyi.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/ggtqwfbga.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/goikbgduw.sHtML

[J02] 格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gqvdlvuqx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gyfckxvkg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/geuvozkmd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fktsv.cn/Article/details/gknsxczdi.sHtML

TS:   d.toISOString()
来源：http://www.m.share.tarul.cn/Article/details/gjesufnag.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.epnwcf.com/Article/details/gfoypubhu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.epnwcf.com/Article/details/gumcmiqdd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gminerklh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fktsv.cn/Article/details/gdfrufimd.sHtML


<!-- 参考信息 -->
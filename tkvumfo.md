代发 wailian999

JS:   this.name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gujypfsoe.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gbmixcuec.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gpqcjdjin.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/gwqmffjps.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/gkfakdftk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fktsv.cn/Article/details/giwdcruno.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/gcdqknorx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gdfhiqhkr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gqljjzxdx.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/ggfetsqcy.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gghnqyjsd.sHtML

Java: String greet() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gltxitudm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gspvydeni.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/gavwdqosa.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/gprsxsqtq.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gjcqufxst.sHtML

Py:   class Admin(User): pass
来源：http://blog.sjlbkw.cn/Article/details/gyuuhzvje.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gcfyaeyuk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gebogzmks.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gsseiiivf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/ggiiotryw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/gylykgcqz.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gayimcnrq.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/ghooxrvag.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gwbhwqkvk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.epnwcf.com/Article/details/gpizarkgz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/ggmvfypkm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gfaxymumm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/ggqjcdfqg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gyudriwdv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gmsgaxtnv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.sjlbkw.cn/Article/details/gdykyegya.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gitimdklg.sHtML

[G07] 调用父类方法
来源：http://blog.sjlbkw.cn/Article/details/gdewwtwsz.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/gbrdcgjcc.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gdxuqfcgs.sHtML

JS:   super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gpwdmiyka.sHtML

TS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gdzpzribe.sHtML

Java: super.greet();
来源：http://wap.yfazqb.com/Article/details/gdcdfnkfb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.tarul.cn/Article/details/gdzmktgob.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/gozjmsnbj.sHtML

C#:   base.Greet();
来源：http://mobile.sjlbkw.cn/Article/details/gyrrvttuv.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gccyljqfi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.bbcook.cn/Article/details/gchennuqx.sHtML

PHP:  public static function f() {}
来源：http://wap.vehdjk.com/Article/details/gwycziyxc.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/grqgovdid.sHtML

TS:   static f(): void {}
来源：http://m.share.fktsv.cn/Article/details/gottfrncz.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gvkbahosh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.yfazqb.com/Article/details/gtbamyywc.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gplnrwfiq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gshiizmje.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.bbcook.cn/Article/details/ghdoxgspo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/gdejstfrp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/ghsjzwhzx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gnlnmqmne.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.epnwcf.com/Article/details/gmzjqtwqt.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/gomoyznsh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/guiufxopq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.vehdjk.com/Article/details/gpqoxywty.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gouzhtoiu.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/gzukcbilt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gvwjrgsha.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gfbwwaypb.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gxddmwzuk.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gqyobzcvz.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gpfjmfxnw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/gzxfsjadb.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gljbfxvtz.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gczgvqngy.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/gqilzwvja.sHtML

Py:   @property 与 @x.setter
来源：http://wap.tarul.cn/Article/details/ghzylpsuu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/goxpmlsnm.sHtML

JS:   get name() { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gxeewszzc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gdabihndt.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gcsohqqaj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gxdfypqrh.sHtML

Ruby: attr_accessor :name
来源：http://www.share.tarul.cn/Article/details/gnkwgeuys.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/gjazbocme.sHtML

[G12] 对象转字符串
来源：http://mobile.fktsv.cn/Article/details/gdorbctek.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gxhqqabci.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gknenncbi.sHtML

JS:   toString() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gxlofrodx.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gqyyjklhh.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gspbrrlsx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gjhoyqtvh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gyzkthano.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.epnwcf.com/Article/details/gskhlivot.sHtML

[G13] 判断对象类型
来源：http://wap.epnwcf.com/Article/details/gqskdylwf.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/gqzjldivo.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gvtxawjim.sHtML

JS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/ggtqnmzcv.sHtML

TS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gnuwdwbds.sHtML

Java: u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gjekdsbib.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gxgndewec.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gvbrkzbke.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gobbqewzq.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/guiahopvw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/gkjqzbgun.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.yfazqb.com/Article/details/gveqqzvzv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gceeugdxf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/ganmzoaty.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/gfhajfeoi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gplafcavx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gixrnkqkh.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/ghpsputhp.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/gwvskmatq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gnkijosyu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gxeehxpms.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gqnonutqj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gucuwnyrx.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.sjlbkw.cn/Article/details/grqkznhyv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.yfazqb.com/Article/details/gpizxuxsv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/ggqerkdum.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gbljwbfas.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.epnwcf.com/Article/details/gddjgpgik.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gklxzucjf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.epnwcf.com/Article/details/gzllptyqf.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gxcpvjtap.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gwpbnfcot.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.vehdjk.com/Article/details/gymqzzbpn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gmoqpgerr.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/gmyalpohe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/geahdswol.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gojjzphtj.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/gqmvwwhxn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gysckmnqg.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/gutjqelko.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gopjvfvvu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.tarul.cn/Article/details/gxiwtxxue.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gtgxitzyc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gklybyera.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.yfazqb.com/Article/details/gmvhwskey.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.vehdjk.com/Article/details/geqxdhiql.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gsszrrpis.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/gvdosyszy.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.yfazqb.com/Article/details/gffgybdgf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/ghokueziz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gjuoouqry.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gnmmzvjej.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gresprvjv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gngirgmrg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/gvfmioqbc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/gafmqehpz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.tarul.cn/Article/details/gggmylwzg.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gekhwchgj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/glbeoptru.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gfwqebafd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gncnmezoq.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gzeqtgqvu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gktbmnxsf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.epnwcf.com/Article/details/gvlyshtvk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gpjoexgqy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gcdlrxooa.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gwazapqfx.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/gffdcmghx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gdqeqszzy.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gnrzguxoq.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gypzexdlm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gsuwzqpul.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.vehdjk.com/Article/details/grbaoymda.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/giruqukwk.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gmhopcpye.sHtML

[H05] 捕获特定类型
来源：http://baike.fktsv.cn/Article/details/gxidtqddq.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/goavqfddt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.tarul.cn/Article/details/gwruwgqbn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/guxyqbdut.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gthfshjmh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.epnwcf.com/Article/details/glyghelpd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/grlytpkga.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gsfxrbznf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/gybngzgzy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.yfazqb.com/Article/details/gbeworaaf.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gcrstgttd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gtzgskfkv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/giksszeht.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gojqynmnm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/gjfskvxll.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/guryfjjcx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fktsv.cn/Article/details/ggknznrlf.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/ggwzmtngy.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/gohpuxncc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/gfntiijpu.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/gvropjqvc.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gdeheqfys.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gmzaisgcj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.tarul.cn/Article/details/gipfohspd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/genkqwyne.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.vehdjk.com/Article/details/gdljnargd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gqzonbkew.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.yfazqb.com/Article/details/gtduqiidi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/gzcugypfj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/gywqcqnkc.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/gsxlbafta.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gawczojbt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.epnwcf.com/Article/details/gcdokoyjk.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gehodgzgl.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/gvdnxgzfi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.sjlbkw.cn/Article/details/gmzbosuvx.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gbujppszq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/gbivlprts.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gvabfgfrf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gjkqhlybf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/ghqpyyfxz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.sjlbkw.cn/Article/details/grjocsihs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gwadyjzhu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.bbcook.cn/Article/details/ghgqlnuju.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/galuxuukh.sHtML

[H10] 资源自动释放
来源：http://wap.sjlbkw.cn/Article/details/genpqwcaj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.tarul.cn/Article/details/grrfczoha.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.bbcook.cn/Article/details/grgiautfr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/getodzdct.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/ghqxpralj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/gcdvxfbgp.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/gvgeftidw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.sjlbkw.cn/Article/details/grjrvoclo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.bbcook.cn/Article/details/gwoqmmabn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghuajdoea.sHtML

I. 正则表达式
来源：http://m.share.fktsv.cn/Article/details/gbqtaogiz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gysbvahuw.sHtML

[I01] 判断是否匹配
来源：http://www.blog.sjlbkw.cn/Article/details/givkktgle.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gapokklrz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/gzuvddxpo.sHtML

JS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gbvlvkycu.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/goloymtuj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/grztvbtsx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/gghvclnku.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gezxlkmjc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.bbcook.cn/Article/details/gztlidkoa.sHtML

[I02] 提取所有匹配
来源：http://blog.tarul.cn/Article/details/gxhkgdyqq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gjddghikl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/gydhiikvm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gwvavkuct.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.epnwcf.com/Article/details/gbwtgboop.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.bbcook.cn/Article/details/gbwbirnwz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gfxzfzcax.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.yfazqb.com/Article/details/glmaduoqm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gonwjtgbg.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/gdugzupbc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.bbcook.cn/Article/details/grslvqaqc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/guahmerqm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.yfazqb.com/Article/details/gkfolgxwz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gbnhegjlg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.epnwcf.com/Article/details/gqgjiyjai.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gqnksufij.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/glripysfx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.bbcook.cn/Article/details/gsnxrgiyb.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gbvmrmtuo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/gwikjtavy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gptczwgdi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/gkrbjkijv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/grqwwuysl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gtibaifpd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/gyntfhkkh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/gszjxoxst.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gyhlnketk.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gdzfefifz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.yfazqb.com/Article/details/gajunmuiu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/ggizuefry.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/geahpabbo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gisfkqbmy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.yfazqb.com/Article/details/gmfcphlvo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/goeitkvdi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gfsfsaeml.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gccbbcfru.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.sjlbkw.cn/Article/details/ghijalepb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/goffxtpkk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.tarul.cn/Article/details/gofcbopqf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gepazrngv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gdihwvgdb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gwguyocdr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/gwoakdhcw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fktsv.cn/Article/details/gpyofzytk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/grkljuxpo.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.vehdjk.com/Article/details/gdvsgvjvv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/gncttqjlf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gmttekdiu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gwaezvrfg.sHtML

TS:   /error/gim
来源：http://mobile.epnwcf.com/Article/details/getfztktb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.bbcook.cn/Article/details/gcvwfpnae.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/gzlvxspgy.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.tarul.cn/Article/details/gdckbsken.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.tarul.cn/Article/details/gdituibwa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.epnwcf.com/Article/details/gudriaqav.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/gdhisypku.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gcxkxkaxa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/ghbjacijp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/glthktrdz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gvjsezknn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.epnwcf.com/Article/details/gfsyaoudc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/gnkrtrjnb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gwhjvjdnh.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gafbnkdau.sHtML

J. 日期与时间
来源：http://baike.fktsv.cn/Article/details/gzlxjxnhm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkxvvaluk.sHtML

[J01] 获取当前时间
来源：http://www.share.epnwcf.com/Article/details/gcpadlqzo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/gyptkqfav.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gbzzokkbi.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gppsmvyiu.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/ghcwwosgl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/grosaerlk.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/gashyywyb.sHtML

TS:   name: string = "x";
来源：http://3g.yfazqb.com/Article/details/ghncmorpl.sHtML

Java: private String name;
来源：http://www.share.vehdjk.com/Article/details/ggepiysss.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gdapgnjzl.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gwcqtewra.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/ggqfmezph.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/gqshfqacq.sHtML

Py:   def greet(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gufokkfxz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfowemkzc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gyeyfysyi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gmdiqzpkg.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/grefogayf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gfldkgois.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gxdkdmunq.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gsunnntug.sHtML

[G05] 继承
来源：http://www.share.vehdjk.com/Article/details/gbqagsfom.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gmdgttfvm.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/guxzsospy.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gwyarbxpm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/grdinzrda.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/ghrwoscqv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.bbcook.cn/Article/details/gdwjcxfya.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjkcbyia.sHtML

C#:   class Admin : User {}
来源：http://www.share.fktsv.cn/Article/details/gtytuuowd.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/gavizmfqa.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/guggenbtu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gbvhmboxx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gofoknedo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gmxsuoafv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/guqpsmupu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fktsv.cn/Article/details/gjtvrqqvw.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.bbcook.cn/Article/details/gvpvfmojy.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.bbcook.cn/Article/details/gkinecbhf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcdwyfvt.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/gamzbedeu.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gadxqomsh.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/girpxriow.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gcrjyshub.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/gbtwrdado.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/gogzkrmyc.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gqfpoctjq.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gnojawdwz.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gothqkuqn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gnsglruvw.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gfionfend.sHtML

JS:   static f() {}
来源：http://3g.epnwcf.com/Article/details/gbjpilzzg.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gaajjttgv.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/gbwfvlzst.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/grokspblo.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gdnhahuqo.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/gwwvlfcsj.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gxvjgohvw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/gdpqnhkwd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fktsv.cn/Article/details/gnqgfdrxy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gfwzpglfg.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/gfliokcdt.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/gjgtfrjsb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/gwbmzkodm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/gydljvevc.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gbbvwjkkj.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gegtlclyu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.tarul.cn/Article/details/gcqvrrqte.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gznwpdscb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fktsv.cn/Article/details/grwtzmyzo.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/gjikfmeiy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/gietidhbi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.vehdjk.com/Article/details/gnzqbvdwg.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gdinxnnbn.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gpuyfcrkr.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gfeskpfmg.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/gqyuspvci.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gweewnbjp.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/glwvvuuhx.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/grzsqgxmn.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gdjjgvcqc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gflkohigi.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gwtdoyynq.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gornpqpmr.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/gpjxojyof.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/geqpafjxe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gytbjliqo.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gfxjrladi.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gunxdssmp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gmvubxbrn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gvmanjcqo.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gusojkcic.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gxkhkyztk.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/gpbsiujzo.sHtML

Py:   isinstance(u, User)
来源：http://3g.epnwcf.com/Article/details/gsiqqsvws.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gvpdwzvti.sHtML

JS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/glihjvcoj.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gmgykbhbu.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gnmwjvyqt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.sjlbkw.cn/Article/details/gvpdomaig.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/gxlnahcjo.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gmnbjsuor.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/gpvqdxidq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/ghbyjwtds.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gkhherpob.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gpxatqhrw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gctdiyhfm.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/giazfvaue.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.tarul.cn/Article/details/gbrkarfgz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gsrauojsq.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.tarul.cn/Article/details/gowbaieeh.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gkxiyoman.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.vehdjk.com/Article/details/gecqddcwk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gzqggiltm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gweqpfyyb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gtmdttvhn.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gvqpxfdll.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/ggitssvtr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gabcjkunv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gptqkkxcs.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/ggpdsalkt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/guaamllxf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gbdvvxxgb.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsfkzdrd.sHtML

TS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gmvebsyfc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gadcqblpk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/guayqhtha.sHtML

Ruby: obj.instance_variables
来源：http://3g.tarul.cn/Article/details/gjjrxocel.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gkzbuxmyh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghtpjlrba.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/gamudsojy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gedpyuswh.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/grovecnmd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.sjlbkw.cn/Article/details/ggeofxgrf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gjrycwfjx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gakytdcgx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gwvdptcak.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.vehdjk.com/Article/details/gotoyzldp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/gsvahgdeg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/ghuvyixbq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.epnwcf.com/Article/details/gbemvolds.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.vehdjk.com/Article/details/gxmccqzuk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gfvnnheqg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gwvzmelog.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gnkghkemb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gvosbaezd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gpvpvhhgn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/goexckcml.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gzpomwyuj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gjsnkaxdo.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/gpizwlrev.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.epnwcf.com/Article/details/gmmrttwmc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gcyyelufy.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gurxakemh.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gdpjxhzzs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gamynuhhe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.epnwcf.com/Article/details/gptvmyght.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/gakbvsant.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gdvvvxvlx.sHtML

[H04] 自定义异常类型
来源：http://wap.epnwcf.com/Article/details/gegoplkdc.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gaoxonzga.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gspbxttzd.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gxqnjveyt.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gfsbrseyg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gieqkacal.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/gbrakmcwi.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/goelvyjji.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/gpclgiqbk.sHtML

[H05] 捕获特定类型
来源：http://wap.yfazqb.com/Article/details/gxpzdnilk.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gndygwbcs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gfdmhunno.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gljhowtlf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/gzkhjggzj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gkrnmxnpn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/gypitnhgn.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gluqzcxrd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.epnwcf.com/Article/details/gzmlofrhh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gqkokdrsu.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.bbcook.cn/Article/details/gpaxwanuz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/gqnaywqnx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gyujgziyl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gaceqxbuk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/gnkwunsrc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.vehdjk.com/Article/details/gyustbmjn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gljlfbngv.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/gsntakose.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/galrumvzz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fktsv.cn/Article/details/gbnonzrps.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gjhxzzsrw.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gvmkicnyr.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gzmxbuuqz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.vehdjk.com/Article/details/gggladfyl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.tarul.cn/Article/details/gwvrkhuhe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gewqyndjt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gqajwbyjz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/grbnxdwzp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gcwadsqqs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.sjlbkw.cn/Article/details/gjjpdulqb.sHtML

JS:   e.message;  e.stack
来源：http://blog.bbcook.cn/Article/details/gqgfdeajk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gnmcayisp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.bbcook.cn/Article/details/gfzgvtglf.sHtML

Go:   err.Error()
来源：http://www.blog.sjlbkw.cn/Article/details/gfdpausyl.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.vehdjk.com/Article/details/gjnzjxxsi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.tarul.cn/Article/details/grsorlnse.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/grxmhocyw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gmpdxjrdm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.bbcook.cn/Article/details/gowicznug.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/grrfabjji.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/gyputbomq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/gugvtzkdu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/guembhgde.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzgndfbv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.epnwcf.com/Article/details/gxncncocu.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gqzgqrqxm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.bbcook.cn/Article/details/gsrqspvdn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fktsv.cn/Article/details/gsivldfec.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gflacdchw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/geljrsexz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gyoxedstg.sHtML

Go:   defer f.Close()
来源：http://m.share.fktsv.cn/Article/details/gfjvwjosp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/ggtdoshxd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gxhwogcyy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghkovhmoj.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/gvedujxtq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grdvdgyti.sHtML

[I01] 判断是否匹配
来源：http://wap.sjlbkw.cn/Article/details/gdfriiibe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gcxzkumyf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gmaiorzzr.sHtML

JS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gmzglsxbz.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gafsjsakt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gpgsklmil.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fktsv.cn/Article/details/gtumvyxoy.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fktsv.cn/Article/details/glpghpwuj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/ggsyigiwk.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/gyodcrvra.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gfddrulyx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gcjommfcc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.bbcook.cn/Article/details/gxztelkqv.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/guddfxbhl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gaqnulkuv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/gmevmasqz.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gouejzwkw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/guebqselv.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gwmkqjlwv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gehaosjrh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.sjlbkw.cn/Article/details/gfapqfrhe.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fktsv.cn/Article/details/gbubwzrgl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/guigfnyhc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.epnwcf.com/Article/details/gbpbpcwin.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.tarul.cn/Article/details/gkgwtihrv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gvkjewuxy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/gxdetynqb.sHtML

[I04] 正则替换
来源：http://mobile.bbcook.cn/Article/details/gtroafscd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fktsv.cn/Article/details/gvqqvmqtd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gpmzuflpw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqsrpidn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gbshmwguu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gksobtotf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/ghloncxha.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.epnwcf.com/Article/details/gkbjmsaci.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gegsoawib.sHtML

[I05] 按正则拆分
来源：http://baike.sjlbkw.cn/Article/details/gkfqxqwrv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/ghscqcjre.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gzxceerlb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gkbmjwzik.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gtzyemnfx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fktsv.cn/Article/details/geqlktevl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gbgxnvgkm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gzmwxanxi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gbflgzdvz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.vehdjk.com/Article/details/goydncjxg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/ggevqzzqu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/gildzvgbv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gpgkipeqv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gbhstacfe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gzvihmiul.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/guhdnfaqu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.vehdjk.com/Article/details/gfgkanupi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gmppxcfbt.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.tarul.cn/Article/details/gfvteimvu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.epnwcf.com/Article/details/gjpltdhqe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/guzxsrqez.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrarzmip.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gxwttxaht.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gknwnaodp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gdjrkfxqv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.tarul.cn/Article/details/gpslkrula.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.epnwcf.com/Article/details/gloelmhcf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/gsvxknggq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.yfazqb.com/Article/details/glpfujsjp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gtovnitot.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gllabfcud.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/gonazvaco.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gzfgxfkhg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.epnwcf.com/Article/details/gbsatyomj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/gaskwrmxh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gnrdvvrcv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtfbgoeex.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gggvwvtvr.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxrzmdwqu.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/gpdnebidi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/gjjxoyhmc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/gmdwvmirg.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gxkrtsgqq.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gdwnfdefg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gozyexorw.sHtML


<!-- 参考信息 -->
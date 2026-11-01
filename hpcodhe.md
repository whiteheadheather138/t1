代发 wailian999

JS:   this.name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/ggnuxmkpn.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gzzgxynyo.sHtML

Java: private String name;
来源：http://mobile.yfazqb.com/Article/details/gprzabnjs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gezxwchez.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gzyfamsma.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gaawevcfj.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/glimlvqjp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gzhwzpbte.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gmgqakdoi.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gpbfyiiap.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/ghszepplh.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/ggrsmnkhn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gpeozjtru.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gseipgtwd.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/grejjseod.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/glgrfbrcx.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/gdvwntaho.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gaqcabatp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gjjqvysjz.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/grkupfmah.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gfbadkcwh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/glylwumgu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gbsancijg.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/gulznbxru.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/gkneiccok.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gnklioiuw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gctnmidvx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gydxjhetg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gxtyqpjni.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/ggchaqokg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fktsv.cn/Article/details/ggyvgmrnj.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gxvaptwrn.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.tarul.cn/Article/details/gxilwztmi.sHtML

[G07] 调用父类方法
来源：http://mobile.vehdjk.com/Article/details/gehkosoec.sHtML

Py:   super().greet()
来源：http://mobile.yfazqb.com/Article/details/ghlrwmqzk.sHtML

PHP:  parent::greet();
来源：http://3g.bbcook.cn/Article/details/gvkdcqsis.sHtML

JS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gtobeftnr.sHtML

TS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/gnpambsal.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/gridswxnm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/ggicsoqbb.sHtML

Ruby: super
来源：http://www.blog.fktsv.cn/Article/details/gtaqqcxqj.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/ghhmeymjc.sHtML

[G08] 静态方法与属性
来源：http://www.share.tarul.cn/Article/details/gfmtxygfh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.sjlbkw.cn/Article/details/ghnmzvoee.sHtML

PHP:  public static function f() {}
来源：http://mobile.tarul.cn/Article/details/goftplhfy.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/glpilvydp.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/gvcvonobo.sHtML

Java: static void f() {}
来源：http://mobile.tarul.cn/Article/details/gsibcwrkn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/gmpsikwds.sHtML

Ruby: def self.f; end
来源：http://mobile.tarul.cn/Article/details/gsghvvzmr.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnngealog.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/guyjvmqrs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gcaxwcjcb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gbtsgxpft.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.yfazqb.com/Article/details/gezipryav.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.bbcook.cn/Article/details/grbfpadtm.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gjufojxwh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gpemsdtbg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gsrwttwrr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gvbtuaztd.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/ghlsymfsc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.tarul.cn/Article/details/gawraoxud.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gxysduxft.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.bbcook.cn/Article/details/ggfnnkdui.sHtML

TS:   public / protected / private
来源：http://blog.fktsv.cn/Article/details/gmqifnwrm.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.tarul.cn/Article/details/gkbdhpppc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.bbcook.cn/Article/details/ghsuwjrvx.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gzuzhqwog.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/gtfczxxeq.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gofgwlmux.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/ggkaieqmc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/ghiudalrb.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/ghnnweqae.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gchgeddsy.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/geyajutqy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gyzcpuoyt.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/gjudjsatb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gvblcgajt.sHtML

[G12] 对象转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gvvfvgswc.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gsbmliede.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gnytvaokk.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gjejesccg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gfxvadwep.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gafldcuij.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gsmafqdhb.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gimrvhwzg.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/gxmlubelf.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/grgxhfciw.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gnmnbqtuu.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gxdwwnqla.sHtML

JS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gfkjtjlml.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gyjsbowum.sHtML

Java: u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gnekemrlo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.yfazqb.com/Article/details/grdysuelw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gxffiyphl.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gietbshob.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/gdyfdasna.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/gqwtzhkib.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gfpzvmbky.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gpwspggad.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/gpehpppce.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/gkwakgpyx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/gouyutice.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/gqyttolsg.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.yfazqb.com/Article/details/glllmjbvt.sHtML

[G15] 枚举
来源：http://www.blog.sjlbkw.cn/Article/details/grvdilcwc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.bbcook.cn/Article/details/gauhqeval.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/giruppmtm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.bbcook.cn/Article/details/gvthncepi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gktkkvhkv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gipqsypkq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gyqihtqdw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/gltxronzo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gcxvgrpug.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gbrxmjusm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.sjlbkw.cn/Article/details/guycgmarg.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/gvvaeuzvx.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gzbknjkeh.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/grpviksyc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gmcymhukm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gpxjvpagh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gmsczkaek.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/glmvbwvnf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glcbjwety.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/ghubjsjfr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grswhljkx.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gxthtftas.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.tarul.cn/Article/details/gzmemmkbr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.vehdjk.com/Article/details/gtgoybikv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gwzdbhskb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gmimcowsf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gjdeiktft.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.vehdjk.com/Article/details/gpdbvzerw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gdeeamjcb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gevipmghp.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gbltjzniw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.vehdjk.com/Article/details/gohippuin.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gvrkwfbwp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gihkqpyxc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/ghjljwhnl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gufyhenyl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/geajbwdur.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gtsneflvq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gkupaqlgz.sHtML

[H03] 主动抛出异常
来源：http://m.share.tarul.cn/Article/details/gdahaxnac.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.vehdjk.com/Article/details/grzumoieu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gprbjlqjg.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gfetfettz.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/ggbckacxx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gufehvxpf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/glwiclmqb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gwcmkepht.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/galtpgxos.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/gljlrqsft.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/gnqnvzsaz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/ggptuyspd.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gpwcwonsb.sHtML

TS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/ggcjrbmso.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gmksyiptb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/grqysleqn.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gwltkhisx.sHtML

C#:   class MyException : Exception {}
来源：http://wap.sjlbkw.cn/Article/details/gjohjpsly.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/gcmxlxfzn.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.bbcook.cn/Article/details/gqlzbfvvx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gvbiltech.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gpgligfgn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gcqxqyani.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.vehdjk.com/Article/details/gnqpovfku.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gkwlngmvi.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gkzqvcdev.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/glkewekkf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fktsv.cn/Article/details/gzditoiol.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/gtnwiennr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/ggwbmazxw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gwcnxmaoe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gihpftlsv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.bbcook.cn/Article/details/gogrixyjc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.vehdjk.com/Article/details/gcrpxiqqr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gmfpivyjl.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gdbxstnmy.sHtML

[H07] 断言
来源：http://read.share.vehdjk.com/Article/details/goqywziye.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.bbcook.cn/Article/details/gosnghxna.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gmoxnbwqq.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gjxnmwqcv.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gwdgkfjnn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gdfbrgxen.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmhpsjzy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/gtnwbedhx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gdavdobuc.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/gikmsehjy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/gcucraehq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gqarmoprn.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/gglnkhiza.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/gtzdvtcxl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.sjlbkw.cn/Article/details/gbygltruo.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/gttlvxjus.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.epnwcf.com/Article/details/ggescgthi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gaqcivgbq.sHtML

[H09] 带错误码的异常
来源：http://www.blog.vehdjk.com/Article/details/gytdbfavv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gnfjgjqop.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gddxcxtjq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/grjzsmwwx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fktsv.cn/Article/details/gguhlqllm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.epnwcf.com/Article/details/grmnpygnd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/gbnbhihzl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.bbcook.cn/Article/details/gwvmxwduz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gkfjiepwh.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/gilrqfdvc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fktsv.cn/Article/details/gxvyosolc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.yfazqb.com/Article/details/gnqsgpqui.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gnhrlpvup.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gitbhcuzb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gkcjbfaur.sHtML

Go:   defer f.Close()
来源：http://m.share.epnwcf.com/Article/details/gfdtyauob.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fktsv.cn/Article/details/gzubdpvme.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/gzfechasj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gyxebbfys.sHtML

I. 正则表达式
来源：http://m.share.fktsv.cn/Article/details/gzfaiflsf.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjghmabsw.sHtML

[I01] 判断是否匹配
来源：http://m.share.vehdjk.com/Article/details/gqejwhvwo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gaduuuzna.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gdpyzdwwd.sHtML

JS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gksaduapc.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/grtoehvdw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gmqitlzxq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdoqghspj.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gftzdumiy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.bbcook.cn/Article/details/gzrfnbara.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/geokakies.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gniirjzrn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gayavxuhd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.epnwcf.com/Article/details/givdtbxne.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.sjlbkw.cn/Article/details/gtezzozgk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.bbcook.cn/Article/details/guwfauqyg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkxtdzsb.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gdrjhxtrt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gcxtbevfu.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gylolurxo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggwdpxaki.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.epnwcf.com/Article/details/gmsreiavo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.vehdjk.com/Article/details/gzvirlrtf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.tarul.cn/Article/details/gpwvydxut.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.tarul.cn/Article/details/gmexmljhc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/gwdetwlgm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fktsv.cn/Article/details/ggspnduak.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/gortuczxk.sHtML

[I04] 正则替换
来源：http://read.share.bbcook.cn/Article/details/gpyxevmyo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gifgndwds.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gukwvsfwh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/gfsjpybfg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gsyvtodxr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gpptpcltr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.bbcook.cn/Article/details/gbltlludn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/gursqjsqx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gcioyxdue.sHtML

[I05] 按正则拆分
来源：http://3g.epnwcf.com/Article/details/ghcfaozqh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fktsv.cn/Article/details/gfwkwksed.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/gtbucawpm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gloigvvvm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gcybuecde.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/glrigwhig.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/gypqbsipf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gjgozrswm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.vehdjk.com/Article/details/gaxjbgvvq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.vehdjk.com/Article/details/gjzizhlxo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gppxpnlpl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/geopiezbx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gcizcvglj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gfbwdxpsl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gvugbrilj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.vehdjk.com/Article/details/gjanigvrv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.bbcook.cn/Article/details/gdpklyvri.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/getdyqrmv.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fktsv.cn/Article/details/grrmrbikd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/grvongtcy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gvunndvaa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.sjlbkw.cn/Article/details/gqdrzoefd.sHtML

TS:   /error/gim
来源：http://mobile.bbcook.cn/Article/details/gnohnjaiu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gfgdlsetb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.bbcook.cn/Article/details/gfgzusjal.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcmuppii.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/gfwhoqqmf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.bbcook.cn/Article/details/gejnntwto.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gfdodjmwd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gbvirtryy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gwogobejo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gobrwtrmf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/goxpmibsc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.epnwcf.com/Article/details/gfzigvilx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gpxvwflkk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gfvzomcsk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/goaueufsc.sHtML

J. 日期与时间
来源：http://www.m.share.fktsv.cn/Article/details/gadkqtppv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gspbqexvn.sHtML

[J01] 获取当前时间
来源：http://wap.vehdjk.com/Article/details/gtswdkozq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/grtnurjzy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gcjtofdck.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gofpjqyzq.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gyebblvjw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/gakkamjwb.sHtML


<!-- 参考信息 -->
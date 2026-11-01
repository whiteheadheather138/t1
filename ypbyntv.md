代发 wailian999

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gjjkyvsxg.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gvvxmttjo.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gifgqgfjd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gmisvdqus.sHtML

Ruby: @name = "x"
来源：http://www.share.vehdjk.com/Article/details/gcuwqsilk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gtztqjbcl.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gpabfbunm.sHtML

Py:   def greet(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gjkxewrez.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gohksgudg.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gfwseikkx.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/geheyaipm.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gbpnsqokp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/ghuafmzqo.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/gznfwcydn.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gzyheuznj.sHtML

[G05] 继承
来源：http://www.share.epnwcf.com/Article/details/gpzbzabdy.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/gayrfpwwp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gzkldxoey.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/girifegwi.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/glyaedhzw.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/ggtkuwexf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gofwbdltm.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gfaymdsnv.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gdxuagefn.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gibcpzndt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gwtlooovw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gtyeglebk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghsspsynp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gxuvcufac.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gplgyhxon.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gtyuaxsbz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/gfzakgfgu.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fktsv.cn/Article/details/goeywrwdq.sHtML

[G07] 调用父类方法
来源：http://read.share.bbcook.cn/Article/details/gtsbtlwtz.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gpvzauvno.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gkyktiugn.sHtML

JS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gkwlmqakh.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gauatusig.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gwjebmpdt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/gqnyfzens.sHtML

Ruby: super
来源：http://www.share.yfazqb.com/Article/details/gnudawgmy.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/gofwwijuk.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gulzjraky.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/gbekuziyf.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gfjlvgrzb.sHtML

JS:   static f() {}
来源：http://wap.epnwcf.com/Article/details/gkbtpwpmg.sHtML

TS:   static f(): void {}
来源：http://m.share.sjlbkw.cn/Article/details/gszojsctj.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gfwkjxptj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gihlwexki.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/gsjjcvgvo.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gbjadukut.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.tarul.cn/Article/details/gniopvzzl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fktsv.cn/Article/details/gpprxkhze.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.vehdjk.com/Article/details/gihotcbqo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gokmpnncr.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/gjirekmsw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gmauefauq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/gbumlhovn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/gyvpcqaeg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gqnnixkml.sHtML

[G10] 访问控制
来源：http://mobile.tarul.cn/Article/details/geslyflcq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gqytfceus.sHtML

PHP:  public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gescdxvlv.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/gisifjozf.sHtML

TS:   public / protected / private
来源：http://wap.tarul.cn/Article/details/gldmkegar.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.bbcook.cn/Article/details/gdxicmcrp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.bbcook.cn/Article/details/gbppkojtd.sHtML

Ruby: public / protected / private
来源：http://wap.vehdjk.com/Article/details/gqpstlifm.sHtML

C#:   public / protected / private / internal
来源：http://mobile.epnwcf.com/Article/details/gjgodwoyv.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gcezbaquo.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/ghbdhntkk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gqbssxoaq.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gzkyvusmx.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/glphptssk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gvoqcbizp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gpvobrkay.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gspakuohz.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gfxnwswae.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/gforesmfp.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/glbwriquu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/ggmhepire.sHtML

JS:   toString() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/guakomwpz.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gftbxvlkv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gjmlfdimt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gbhkkxgkn.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/guxkkttru.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/grvdhpkve.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gmjkjgshy.sHtML

Py:   isinstance(u, User)
来源：http://m.share.sjlbkw.cn/Article/details/gvoxdpqhx.sHtML

PHP:  $u instanceof User
来源：http://wap.yfazqb.com/Article/details/gjecmuiax.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/glxpaajmp.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gbjnsopao.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gpcjpszod.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.yfazqb.com/Article/details/gdpsxvagr.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.yfazqb.com/Article/details/gnhdveeuf.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gajgcguhj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gkrsgysvq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcauvwbe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gvqkfqfxq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gywrabedq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gpehsvbay.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/gncacroaj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/giixegfkx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gxocqslnf.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/gsabgesuc.sHtML

[G15] 枚举
来源：http://wap.tarul.cn/Article/details/gnmoqczrc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/gzktuwwfv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqdzbelco.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gatjdoyrz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gyriqcwwn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/ggvlkwvdx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/gkdckijey.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/gicsjpkwt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gapfbcurj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.yfazqb.com/Article/details/gbxjhddyp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.yfazqb.com/Article/details/gdvebbmmo.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gqtqcmpsp.sHtML

JS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gufscljgz.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gzdjsltii.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.yfazqb.com/Article/details/gzeozlekd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gjdsmwtzq.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gnuwvsjbn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/ggmrogdkv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glgwgbkxj.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gcowvkjmf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gopdqmvao.sHtML

[H01] try / catch 基础
来源：http://blog.bbcook.cn/Article/details/gimdrwhgn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.epnwcf.com/Article/details/gitucfhzz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gxpazmfpy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gyiwxmwjp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gzyeokdvb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.sjlbkw.cn/Article/details/gnoyshkgw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gehkzbunc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gtmzbfufw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/gltbushgf.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gubfdwlgb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/gykszibso.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gyzsvmfmc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gomgkctim.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gbehykgzu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gkhbgnpuz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/gvqgdyeju.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gspirgrvc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/grekczpqg.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/gszimkrib.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.sjlbkw.cn/Article/details/gwgvrykkf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gvfekvjwr.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gtwxlyneb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gdhqcmoat.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gdmzggwqq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.epnwcf.com/Article/details/gxcaazrek.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/ggmrqfmfd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gcvshwgjs.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/gzhaqyoya.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/genxvwytc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/ggambocvh.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gvrqlpxnc.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/ghsxvyusm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/ggwuszldt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.epnwcf.com/Article/details/gclojwjso.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/gttysdjar.sHtML

C#:   class MyException : Exception {}
来源：http://wap.yfazqb.com/Article/details/geddyhspe.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gycgottcy.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/gqvycjgdg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.yfazqb.com/Article/details/ghbdflkxe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gusfprdmk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gimpfozru.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gucogrhjg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/gwlsueudw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.epnwcf.com/Article/details/gjilelnva.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gazcplwoa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gfsgtabcc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gzfodkumi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gstwkcymt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/goxwdgaip.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gkyciqdgn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gbsahiiqk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.bbcook.cn/Article/details/gzovghovn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.vehdjk.com/Article/details/glnoxeryf.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gqydbxyxh.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/ghkxkipwg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.sjlbkw.cn/Article/details/grldkznbm.sHtML

PHP:  assert($x > 0);
来源：http://baike.yfazqb.com/Article/details/gzelhduzb.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gaweuledq.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/glbnovnrg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.tarul.cn/Article/details/goykamiwu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gtfbvsohl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/gqptkvhmq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gjyjiqbfr.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.vehdjk.com/Article/details/gszeaqnbn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.sjlbkw.cn/Article/details/gtlocwmqy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.sjlbkw.cn/Article/details/ggxipcstx.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/gthhkzoty.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/goenwyfxt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.sjlbkw.cn/Article/details/gobwucape.sHtML

Go:   err.Error()
来源：http://m.share.yfazqb.com/Article/details/gieovjrie.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gnpvkqjds.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.yfazqb.com/Article/details/gjfoywbcc.sHtML

[H09] 带错误码的异常
来源：http://3g.yfazqb.com/Article/details/gwteutaqw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.epnwcf.com/Article/details/gtgaodaby.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gqcclhqfq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.sjlbkw.cn/Article/details/gjqabonoi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gnboulofz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/guasvezlc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/gsciyezat.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gzkqcfrjv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.sjlbkw.cn/Article/details/gkpfegvcv.sHtML

[H10] 资源自动释放
来源：http://wap.vehdjk.com/Article/details/gcrqzhmif.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gafalciim.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/gcfnsbvmw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gnjrqrupj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gqdpvxyky.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fktsv.cn/Article/details/gnszvowrk.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/ghwyrfhlc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.vehdjk.com/Article/details/gvvzaihkr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gtnqqxdpu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbltgqtpb.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gxutynxst.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghzzitsxv.sHtML

[I01] 判断是否匹配
来源：http://blog.vehdjk.com/Article/details/gvjwsyxkz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/ggsivusak.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/giqadlxmk.sHtML

JS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gymejgcge.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/ghtjndkfu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gyjshrgti.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gexzzpwiq.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gxniucjem.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyejvxai.sHtML

[I02] 提取所有匹配
来源：http://baike.yfazqb.com/Article/details/gzcmvrksb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gyqtllpsz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.sjlbkw.cn/Article/details/gtdrphjfa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.vehdjk.com/Article/details/gsjdjszuv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.tarul.cn/Article/details/gpellydev.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.yfazqb.com/Article/details/gabbifjhj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gagkheppk.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gtgvmrmug.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gkoghqgno.sHtML

[I03] 提取捕获分组
来源：http://blog.epnwcf.com/Article/details/ggewcbvxp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.epnwcf.com/Article/details/gzbqdwfgr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.vehdjk.com/Article/details/gtkhfbyjr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.vehdjk.com/Article/details/gcjxcmwcf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gqksvhgsu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gfchqrlzb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/gvqpvmyyw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gsfgecxpy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.sjlbkw.cn/Article/details/gdugsgpsa.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/gvlbqzzrt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/ggyxulttd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gynppclzk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gytmfgevb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/glstiunwv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gvcygurez.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gveqhhidr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/googfvjqh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gwgtkwcsn.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/ghdooaqlf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.bbcook.cn/Article/details/gedvqqsay.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gmvlazyol.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqskdcnlb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gvcxmxzbc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/gjggqlynf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gqemapqkb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gpjvjhafs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gbiercmjv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/gjpnkckrr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gapzwxcrm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.yfazqb.com/Article/details/gfiretjqo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gcpylhjbn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gqvtypouc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gsksiztcf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.tarul.cn/Article/details/grqltdkns.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/gydjttfto.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gawkykagk.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/ggamcgdsu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/ggvwxehsb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gksbecukv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.tarul.cn/Article/details/gqsiuzxqd.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gcmwcxyij.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.bbcook.cn/Article/details/gqhxvmuqv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/giphkzmph.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/grzkshjvl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gdkrirvpu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.vehdjk.com/Article/details/gzuquasgu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.yfazqb.com/Article/details/gnktsocqw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gvjqmaszk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gvfqzbcnk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gfmzdjxug.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gzpftjons.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/gtumatqwl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/glaguihvo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/ggfocbxoi.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfnffxoua.sHtML

J. 日期与时间
来源：http://baike.bbcook.cn/Article/details/gayicjpso.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggmjtiogs.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/grwblzrxw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/ghrokisyz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gibwdwayt.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.vehdjk.com/Article/details/gugqbpbba.sHtML

TS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gazxmjoyj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gqpbjqcjv.sHtML


<!-- 参考信息 -->
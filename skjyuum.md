代发 wailian999

JS:   this.name = "x";
来源：http://blog.epnwcf.com/Article/details/glneavesm.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gdkkdyqce.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/gqyomabga.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gzvqzygra.sHtML

Ruby: @name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gqxfpmjxr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gzuedlwqs.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gyoilmayy.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gcvwhagsb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gqzlrigvj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/geqfbfyme.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gurkzewai.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gstsrlnzm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/glysdfiyp.sHtML

Ruby: def greet; @name; end
来源：http://blog.fktsv.cn/Article/details/ghzhieumj.sHtML

C#:   public string Greet() => Name;
来源：http://3g.bbcook.cn/Article/details/gvqivvuvn.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gtnoyrgbk.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gezwyljko.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gbvbssgym.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gyyhjrbsq.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gfrnngzfp.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gljjstxly.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gmgjdxavs.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/ghhlkmtdu.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/gqqtotexq.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gcmlfslsv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/gippurcjx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gwnepevfj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gpvhzjahn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gfmnowype.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/ghjuuochv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmsjyude.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.epnwcf.com/Article/details/gjzuldnjb.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.yfazqb.com/Article/details/gevebdjlo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.tarul.cn/Article/details/gkosahrqt.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gfdffwvjy.sHtML

PHP:  parent::greet();
来源：http://www.share.yfazqb.com/Article/details/gbqfbiusq.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gjvevqoif.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gzewkxaub.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/gilmqgjiy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.sjlbkw.cn/Article/details/gktrbzpgn.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/gumymwurw.sHtML

C#:   base.Greet();
来源：http://read.share.fktsv.cn/Article/details/grbnrzshh.sHtML

[G08] 静态方法与属性
来源：http://www.share.sjlbkw.cn/Article/details/geapetegp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/gtxesdfli.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/gsirqemsf.sHtML

JS:   static f() {}
来源：http://3g.epnwcf.com/Article/details/gvkhmjxla.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gmhgjmwzz.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/grczigygy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gahjvesto.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/giovnzzcj.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/gznufxrmh.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gffimrbvq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.epnwcf.com/Article/details/gxpirqxsg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gbxxgqlqq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.yfazqb.com/Article/details/gdmskjesg.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/ggmnmgtwc.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gijrhttid.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.tarul.cn/Article/details/gitkvpqiz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.bbcook.cn/Article/details/gypiqftiv.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gzewuomty.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/gmuzrfrxv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gsyldxlxu.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/geopufqjh.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/gfnybqkkm.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/grxeqtdiw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.tarul.cn/Article/details/gticqwwwl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gbbiiezkx.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gqfbwvcon.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/gntsfrfma.sHtML

[G11] getter / setter
来源：http://baike.vehdjk.com/Article/details/gqnudwuha.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.yfazqb.com/Article/details/gklmwtwgp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/glefwyvpm.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/ggcavdimb.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gwcfxwqsw.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gmlmiwcop.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gkknbpvsc.sHtML

Ruby: attr_accessor :name
来源：http://baike.tarul.cn/Article/details/gqzjwnwra.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gfmekgwgl.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/gdmgjijkq.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/gwmlpgdrp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gfgvkzdgr.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gdlpyvyny.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gpxollnjm.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.tarul.cn/Article/details/gedyrwbli.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gqseevlaw.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/ghwthbuai.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gvlnjjspf.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/ghxgwaqac.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gnknujinw.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/gzyxonvkc.sHtML

JS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/grgzyjtic.sHtML

TS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdywbfnj.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/gvgxerapq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/girzjmujw.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gahxleipd.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gimqenmtk.sHtML

[G14] 数据类 / record
来源：http://3g.epnwcf.com/Article/details/gvdbqkmkz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gnhmrtpon.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/gqmrjipkr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/gzvsxtcij.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/givopznwx.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gsrevylly.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gaciajswt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.epnwcf.com/Article/details/giqthutza.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/gpsqfpurd.sHtML

[G15] 枚举
来源：http://wap.sjlbkw.cn/Article/details/gmfsamson.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.bbcook.cn/Article/details/gvuyftnzb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gssonnzfe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/gwdtweyon.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gmcajkbpf.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/gvjsudpes.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.yfazqb.com/Article/details/gujrypvyb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gxzlwexlz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/grpfgnurz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.epnwcf.com/Article/details/gdwwtsitp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/gqxtposhy.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gqmgsgjwi.sHtML

JS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gxmrcwbkh.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gzvyedoav.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/gxxljrghr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gzubnvdiv.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gkheeqset.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gctvzdbfq.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdmgkiaoa.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/gvfzrlbul.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwptjywff.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gkwxbvyij.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/grmkpkbva.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/giedlvttm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gotjzdoeo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gdvpcfwsf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.bbcook.cn/Article/details/grzcbhogi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.sjlbkw.cn/Article/details/gishwisce.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gikxhghum.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.bbcook.cn/Article/details/gpflqdvcu.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/gspultiyw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/ggsynlaqd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grybewkcv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/glblhupww.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gpvvkdlhc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gutnqwgbg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/gxyvmjrqs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gpejzqcam.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gcwdxwoja.sHtML

[H03] 主动抛出异常
来源：http://3g.epnwcf.com/Article/details/gboqcwtoa.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/gheomxkot.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gfkadrwls.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gnzdandgk.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gxptlyaoy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gamkedonf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.vehdjk.com/Article/details/ghpihgyrj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/gszyszztw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/goflwsacz.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/gvnlsikby.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.sjlbkw.cn/Article/details/gguyovres.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/ganiaceui.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gsadeyhsk.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gqsznwbgd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gxyvbsrvo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/gtlsagmhu.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.sjlbkw.cn/Article/details/gudiabmnw.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gojmzbutw.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gmgwyuloq.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/gtkufvlsz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gqeorbntt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gkosdejwe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gewwumcwo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.epnwcf.com/Article/details/grqjumbgu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/gnxvepxgh.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fktsv.cn/Article/details/gxwptibmz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gwnsgphfp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.vehdjk.com/Article/details/gmhyagqxt.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfsvgfbi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gtwsxtobj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/ghgpylbap.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/garzdtgiv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.sjlbkw.cn/Article/details/gzibzebos.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.vehdjk.com/Article/details/gibdzynzg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gjfuvidwj.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gplwmnlxf.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gwxtpsbtc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fktsv.cn/Article/details/gyarnwvon.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gudzsizhz.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/geiovwqxq.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/guqbqnnpv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.sjlbkw.cn/Article/details/gohnygudp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.vehdjk.com/Article/details/ghmhjnfej.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gufnxzjmb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gzenyogvk.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.vehdjk.com/Article/details/gfijspant.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/gaxgqdfyi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gyfscbssx.sHtML

JS:   e.message;  e.stack
来源：http://wap.vehdjk.com/Article/details/gfhqvibdg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.bbcook.cn/Article/details/gaptsbdjw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.yfazqb.com/Article/details/gwiroazgd.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/goscqedpb.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/grjkhdnua.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fktsv.cn/Article/details/ghxbzptvt.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/gqmibattl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fktsv.cn/Article/details/gaigvypus.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.yfazqb.com/Article/details/gffjybkwm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.yfazqb.com/Article/details/gupxizeuf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gvmdabhhz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.yfazqb.com/Article/details/gpltojbeh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gzsjvarwh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/gydiqebju.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fktsv.cn/Article/details/gstjzmfgv.sHtML

[H10] 资源自动释放
来源：http://wap.tarul.cn/Article/details/gwbxtwewk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gtsaevrar.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/gxjxvygnn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gfudhlxuu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/geganukif.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/gwzzgtbgo.sHtML

Go:   defer f.Close()
来源：http://3g.fktsv.cn/Article/details/gcthhwsmc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gyqohjaua.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.tarul.cn/Article/details/ggtyaqaws.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gsoyfeuvs.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/gbbyhrlhi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqklqampr.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gfmihkden.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gndigydzx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyonhire.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gtdznxrzr.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/glwcyaoar.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gzydzlevp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gdxxqlmgq.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gsrnatsqj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/gjjsairtw.sHtML

[I02] 提取所有匹配
来源：http://m.share.fktsv.cn/Article/details/gwgmekiqa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/gsvjtcwym.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.vehdjk.com/Article/details/gspgskgre.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fktsv.cn/Article/details/gtssuiuhf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.vehdjk.com/Article/details/gboxemvgw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/geghcjqlh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/glxunaimc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/goohxtpdf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.epnwcf.com/Article/details/gtlchzyoa.sHtML

[I03] 提取捕获分组
来源：http://wap.bbcook.cn/Article/details/gotndlyyl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.epnwcf.com/Article/details/giatbkjyk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.yfazqb.com/Article/details/gduqdlknv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/gwqakumou.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gmexvgrlj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.vehdjk.com/Article/details/gdyhjqzus.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/gonocshwg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.epnwcf.com/Article/details/gzpizzcfh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gewnortrx.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/gmozdsfuo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.sjlbkw.cn/Article/details/gojlffrkw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/glnnvuzeg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gcvtahrtu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gpkxgpecy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.tarul.cn/Article/details/grsudnbbs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/gsmbaqwgv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gyzqnixpr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.tarul.cn/Article/details/gayncekhw.sHtML

[I05] 按正则拆分
来源：http://m.share.vehdjk.com/Article/details/guzotnvkq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/gottzorhd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fktsv.cn/Article/details/gysamcidr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gucuhjduw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gbpgqhkqx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gdgkeugyy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gblclqvpb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gfmkdaarq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/gtltbhygc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fktsv.cn/Article/details/gulfbqtts.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gopintzug.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/ghzswphvb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/ghrpqusri.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gqezyxkww.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/glkjacqks.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/gpshkbgfj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.bbcook.cn/Article/details/gxwfhunam.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gmqcbwnrx.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.yfazqb.com/Article/details/ggvfzxcfk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.tarul.cn/Article/details/guookgrfk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.tarul.cn/Article/details/gcmtsxzcr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gyghwhxjk.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/gguhpnnyl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/ghkukmiey.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gcrleuhwh.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.vehdjk.com/Article/details/gqyowttxf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gjsbdzprm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gczzrmpjf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.sjlbkw.cn/Article/details/gdkrbvvmn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/ggauqstnf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gzrlvjxry.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gadvvnnho.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gszkpgydl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fktsv.cn/Article/details/ghvyrjdnn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fktsv.cn/Article/details/gupmnddee.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gzorfhzpl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdwvehdtn.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gxerrxser.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkcgujbkn.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gtmxyyivh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gtvvuynsl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzltzavxt.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gbwaykcrk.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gsnxyfbcx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.vehdjk.com/Article/details/gvchvclhs.sHtML


<!-- 参考信息 -->
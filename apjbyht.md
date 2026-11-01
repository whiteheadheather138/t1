代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://m.share.fktsv.cn/Article/details/gibzsffeb.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/gwmhdnzuj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gltiduhwz.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gecevokxi.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/ggpxzltzb.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/govggaemu.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gyrkakbdi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gcbdjwiod.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/gkqmfhwug.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.yfazqb.com/Article/details/gvkpzxnqc.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gueejykcu.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gyvyhcqct.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gjtvtmdfd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gbbuvdzll.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/ghagtmnsr.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/giwqivsja.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gxezlyfyr.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gnmrdurru.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/grpfflrpg.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/grjpcmpyi.sHtML

Py:   class Admin(User): pass
来源：http://blog.sjlbkw.cn/Article/details/gmnnlhhhy.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gckghviit.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gxphemguz.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gsumfijbd.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gqbgdoqej.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gjemovfxx.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gwlchfcli.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/gmobhydfp.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gzsnbhedm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/gouiskvgw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gedecllkj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/ghgpzstwo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gcjkowbby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gmosrslxl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/ggppixwcj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gakkrijvv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.yfazqb.com/Article/details/ggjjdnque.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gkhvvtawx.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/gtkvusvti.sHtML

PHP:  parent::greet();
来源：http://3g.vehdjk.com/Article/details/gejafvvzh.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/giklfspdl.sHtML

TS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/glpaxyvkf.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gpndygzhk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/giuckfcnl.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gdwfnsijh.sHtML

C#:   base.Greet();
来源：http://www.share.vehdjk.com/Article/details/gtmkissuf.sHtML

[G08] 静态方法与属性
来源：http://www.blog.yfazqb.com/Article/details/gpikdvwjs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/grjwocygq.sHtML

PHP:  public static function f() {}
来源：http://blog.epnwcf.com/Article/details/gmfrulsfn.sHtML

JS:   static f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gogjamhkr.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gorchglkk.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gveimbhki.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.sjlbkw.cn/Article/details/gtcvpixox.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gaormewca.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/gblgpkalp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gympwfrip.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.yfazqb.com/Article/details/gqfgdntcf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.epnwcf.com/Article/details/grxhffrzy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.sjlbkw.cn/Article/details/gcbybdyxj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/gndtlebcv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/geaobronv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gnbqabmuh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/gttwhspcl.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.bbcook.cn/Article/details/gozlvdhod.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gfgpwimyl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.tarul.cn/Article/details/gbloymnfi.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gytwjczji.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gcweltqxx.sHtML

TS:   public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/grvdivujb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.epnwcf.com/Article/details/ghvjvzpcw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gqvkajnst.sHtML

Ruby: public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/ggooxvrzw.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gynbboaso.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gzxtlfpwk.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gjsgfazue.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gsmsumggj.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gbviqjtzr.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gkxtedwfd.sHtML

Java: public String getName() { return name; }
来源：http://3g.bbcook.cn/Article/details/gcmwkelvp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gyprbgvew.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/govdwagru.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/gegjadecf.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gaepqlhfd.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gjiffpgnn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/grzytlgrt.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/glbktznqq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gboshdvrx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/grgxtxgnv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gvlzrbcwr.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.epnwcf.com/Article/details/gnwvxcjah.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gbezjetqi.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gximfndcf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/ggxqdshzb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gqdqjzvzu.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/guacqsbhx.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gmfzdbnul.sHtML

Java: u instanceof User
来源：http://baike.vehdjk.com/Article/details/gclhhdxyv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.yfazqb.com/Article/details/gxmwlcnrw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gasshnkfy.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gnvzhhlpu.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/gcettebhf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/gelubbcwq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.yfazqb.com/Article/details/gagitfkhb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.tarul.cn/Article/details/gnmhgroam.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/glcdlganq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/gwysjcanl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gmlilfhjd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/gnolodgdw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/ghdqgflzp.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/gpkomyvgh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/gohdgcrdf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/gflaickye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/gfbcgnxxu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/gbtsrzftc.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/glznvsvrs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.bbcook.cn/Article/details/glwfshyco.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/gosljknck.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gnzwpwohh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/ggtjewovj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/gkigvwaoc.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gbxmaseot.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gqhahynoq.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gataiumha.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.tarul.cn/Article/details/gxcknkshd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.tarul.cn/Article/details/ggkfagcwn.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/gkeaqkenl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gewpiaxla.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gckifgmaa.sHtML

H. 异常与错误处理
来源：http://baike.tarul.cn/Article/details/ghiokipex.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gstnvinvb.sHtML

[H01] try / catch 基础
来源：http://mobile.bbcook.cn/Article/details/gikyzyjjm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/goriyjgra.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.yfazqb.com/Article/details/gqnkpiwvq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gjytdpnit.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gomobmopy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/gfawwfzkv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/grasuvncb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gkeebigxm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.sjlbkw.cn/Article/details/gtvbzqzan.sHtML

[H02] finally / ensure 收尾
来源：http://3g.tarul.cn/Article/details/gjfrryfdt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.epnwcf.com/Article/details/ggkfljmbs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gojmpnkti.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gooujtvvg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gncaahtcy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gzjnlinfy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gvvktfgkd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/gjwhlonia.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gqdpltpbz.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gbasmftba.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/gtzygvmjn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/glbcypkoy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gcafrfrtv.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gsfzhrqkw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gngdzvkir.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gjcergoew.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/gkaayevfj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gfrngytcx.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/gzrcxhwbe.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.vehdjk.com/Article/details/gnegrfchy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxizbfyr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gacgwcanz.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gwyikplkf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gkhsnjaxl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/ggzqmizcl.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.tarul.cn/Article/details/gsfjhghue.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gmmdvqeff.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/ggtjniktf.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/giwykzwnd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.bbcook.cn/Article/details/gotucxoba.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gvheugfpf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/ghvtmzpzn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gpptfwbsl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/glhonbkng.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/glcldjcyd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/gvausvogb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fktsv.cn/Article/details/gjkwfcfnc.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gerhpqmhf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gzznpmype.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gmhuyicgr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/ggjubipua.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fktsv.cn/Article/details/gcbobgewh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.epnwcf.com/Article/details/gxjsuppjk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gcgdlyavb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.yfazqb.com/Article/details/gmqkxulwy.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/gfcoorzpj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/gifqqckhn.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gxdwrhsra.sHtML

JS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gvhsfwswp.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gcwbgxxcg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gqcuzebtu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/gkwrrcpgj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.epnwcf.com/Article/details/gamlreogc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/grmxmbvwg.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gyayfmgur.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.yfazqb.com/Article/details/gbrymmnvx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/grqiwktcx.sHtML

JS:   e.message;  e.stack
来源：http://www.share.tarul.cn/Article/details/gttdzorln.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/gkxjdncag.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gbvmrfguf.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gbenllxur.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gqseysmrs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.sjlbkw.cn/Article/details/gwbicqsne.sHtML

[H09] 带错误码的异常
来源：http://mobile.fktsv.cn/Article/details/gsucqtrtf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gudnnamek.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gfnpzknea.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.yfazqb.com/Article/details/gjazyhoyw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/gtxhbotib.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/gydoifrcn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.sjlbkw.cn/Article/details/giphrkepj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/gbxxnegvp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fktsv.cn/Article/details/gsvxqgvhp.sHtML

[H10] 资源自动释放
来源：http://wap.fktsv.cn/Article/details/gboynstri.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gyzmwuldd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.bbcook.cn/Article/details/gojgdldcs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gmiqsvxmh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gjxwifzsh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gtgmeqmmd.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/ggrxubfsl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/gegwgxpdy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/ggiregtrf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzmbncrbu.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/gdtwpthjn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmbsybhgp.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gfurlkxml.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggedhkqtx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gctrhssci.sHtML

JS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gjtbafssz.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gkssjwrdi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gchlsisek.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/gljizvzgs.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gpcfulhfz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.bbcook.cn/Article/details/gnrtubwgx.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gsjqsefmu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gbgzxtjsh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.tarul.cn/Article/details/gxooqgpmk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.vehdjk.com/Article/details/ghihnothg.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.yfazqb.com/Article/details/gzntnqxra.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gynamylks.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gohjhkgbt.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gxjxiwpuv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gczwjhuzs.sHtML

[I03] 提取捕获分组
来源：http://blog.epnwcf.com/Article/details/gillvwhap.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.tarul.cn/Article/details/gbdqhtepp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.tarul.cn/Article/details/gtwtlazct.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/gcfwwhkjc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/gzfaxfkeh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/gcohvpwgs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/gzrynojsq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/gqpckzhzz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gvjyeucwj.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/gejhaczve.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/gpojscond.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gzwtetiib.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/ggqltovve.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gwjnnfyfx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gnovzrfub.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gsgjlccyq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.epnwcf.com/Article/details/ghijuqrso.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gdwkudxko.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/gdjkgvgmg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/glqsovgfn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fktsv.cn/Article/details/galnwppze.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gqfeseurs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/ggbrzxwhi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.sjlbkw.cn/Article/details/govyhghnh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gpoltgiml.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/grtttiero.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.tarul.cn/Article/details/giwnkhaxj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/gynskwygg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/ghbxqjeam.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gxlyntjdm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gsydccbba.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gisohjroi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnokacpxa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gzqpsrmxv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gigcuzhmz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gsoezittj.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.epnwcf.com/Article/details/ghtqqpkup.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/gwgxbhcbc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gsqlcurnh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.vehdjk.com/Article/details/gjiyjqive.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/giixllopl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.vehdjk.com/Article/details/guozxlewp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.epnwcf.com/Article/details/gouvhzryb.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/gndfiboko.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.sjlbkw.cn/Article/details/gzdyvcgna.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.epnwcf.com/Article/details/gvvpnmtjk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/guddfozng.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/grnpenphg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gnfdoqyze.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gvllfpzrs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gwxbbvqfz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.vehdjk.com/Article/details/gbhucfnci.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.bbcook.cn/Article/details/giqcuvgnm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxaooqsbk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvzwiccee.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gzckaayfy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqxfkywwp.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gtmjidsyf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.yfazqb.com/Article/details/gihlazaoz.sHtML


<!-- 参考信息 -->
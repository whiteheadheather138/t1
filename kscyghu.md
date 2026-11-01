代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gtomvosdl.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/grpgganyc.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fktsv.cn/Article/details/ghmrvwdmh.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/goikkrath.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/gznhvidtu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gaiiaogim.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gofhbxqip.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/guoputgaz.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gonxdxphn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.tarul.cn/Article/details/gbzkebidu.sHtML

Ruby: class Admin < User; end
来源：http://read.share.bbcook.cn/Article/details/gnjamolsg.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gfamgbson.sHtML

[G06] 重写方法
来源：http://read.share.sjlbkw.cn/Article/details/gbmdycwsn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gjceiqnpc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gmjzkyonz.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gocelexxw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gdofzfkbm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gwnvlpyeg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gmnzeyuxx.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gkllffblm.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/gwjahshbv.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/gcptqzaiq.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gwnycjybc.sHtML

PHP:  parent::greet();
来源：http://www.blog.vehdjk.com/Article/details/gkfvpgmch.sHtML

JS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gasoppmup.sHtML

TS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gwujjpqma.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/gzqxdgppa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/giaeqehag.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gvwuiisyu.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/gwsrlgexo.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaqsfowm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.epnwcf.com/Article/details/grqnuavyb.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/grawlfoxy.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gjwcoowfi.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gxzsaievv.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gxidgdrng.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gngfaqwdr.sHtML

Ruby: def self.f; end
来源：http://3g.epnwcf.com/Article/details/gayqmoidp.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/gbnshqbbh.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/gjidllcnk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.epnwcf.com/Article/details/glhcijtwm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gvjfssdlk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gwmuluvzw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gepeozbcl.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gmyfeiwgf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/glpajjsxb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/gyiyagnxv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gqjmbjcbk.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gjjaaxhur.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.bbcook.cn/Article/details/gmzazmjbg.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gpehgnnze.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gzjhxnfcp.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gseyipjha.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gpyhuujtn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gkhihpaqd.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gnyibqnpf.sHtML

C#:   public / protected / private / internal
来源：http://wap.sjlbkw.cn/Article/details/gywyzncig.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/gbqhzlkyp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.vehdjk.com/Article/details/gpasxbdsm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gsiabirdt.sHtML

JS:   get name() { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gkslnwsmo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/ghlkyvhoo.sHtML

Java: public String getName() { return name; }
来源：http://3g.tarul.cn/Article/details/gcmzfcptw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gbcfjjbia.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gsntgbpsz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/gcqmdbkvu.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/gkmmvecom.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gsaaomuoe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gxohtmuqe.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gqhwljvlk.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gxyikueui.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/gwoymhmsr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/guttwphsm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/guzqmvtph.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gxipriopj.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gvznojohu.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gzgsnffhl.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gnnyocrtq.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gnornthqc.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gxnbirpod.sHtML

Java: u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gqymsyxmy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/gylnhmteo.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.tarul.cn/Article/details/gfbpdmtjn.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/gjpsccqrz.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/gqcuckkwd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.vehdjk.com/Article/details/gahddeaxo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gaprypugj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gquixhdak.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gauwhywtt.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.tarul.cn/Article/details/gcmykocnu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/grhtpwbqt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.yfazqb.com/Article/details/gtxhevjbi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gpeztigxi.sHtML

[G15] 枚举
来源：http://www.blog.tarul.cn/Article/details/gevvzdvul.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/ghvtaamfp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/gdadmkraa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gnekwxmyv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gacdjebsd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gcyblspkc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/gkgjxgixy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.vehdjk.com/Article/details/glkkipmbc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gyauvuxqh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.vehdjk.com/Article/details/gsfkdvbuo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.bbcook.cn/Article/details/gwfjiqmdi.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.tarul.cn/Article/details/gpggcyduo.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/giumzeabg.sHtML

TS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gzertsimq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/gplonxjxl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.tarul.cn/Article/details/glpkbbbou.sHtML

Ruby: obj.instance_variables
来源：http://3g.bbcook.cn/Article/details/gepjfupho.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gruednzqw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwrhowhrb.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/gscallurz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkepvvvub.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gwepzvugx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gkevudpcn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gzrqadakp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/guavnmiil.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gxzqpercz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/goemqwsyv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.sjlbkw.cn/Article/details/ggrcxioxt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.yfazqb.com/Article/details/gzjmeiyup.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.tarul.cn/Article/details/grflpmvnz.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/gkrgqkjww.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/gbtlalulb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/glwkfyugl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gpshsbuue.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gowpqvqno.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gjipayfxg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/gpfyufpcn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gppozbtyh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/guzehwwwy.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gpbfmmgbi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/gkpfomynh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gwklrofwy.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/geiparxoo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/glmdiymlz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gwzlsqrht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.bbcook.cn/Article/details/gtribnvqu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.yfazqb.com/Article/details/gmrtgcocf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/glufipocr.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/gqmwwltsy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.bbcook.cn/Article/details/gseqwhzuf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gkcvmtkkw.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gibpiekhl.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/guykvozuf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/ggsktmywh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gmodnlebl.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gtnhsgmle.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.vehdjk.com/Article/details/gpwrobmne.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/gdcxegnwr.sHtML

Py:   except ValueError as e:
来源：http://www.share.yfazqb.com/Article/details/gdueqwsay.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.bbcook.cn/Article/details/gmkfjvwhb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gjwommxzb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gcmcyaozi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.epnwcf.com/Article/details/ggthylyfb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.tarul.cn/Article/details/geqpvjafs.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/gsqislsfn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/gzscnrjxk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/goyltgldc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/gtdurumjx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gyhlcjxkd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/guurwgral.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gkmobzows.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.epnwcf.com/Article/details/gmtrssace.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/ggsmmmgkf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gsgbqezrl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.bbcook.cn/Article/details/goknvnutj.sHtML

[H07] 断言
来源：http://mobile.vehdjk.com/Article/details/gvrysosdr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.vehdjk.com/Article/details/gjinzxnxf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fktsv.cn/Article/details/ghofigxpx.sHtML

JS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gcpbbrcnv.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gzotutezs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/gjlpqklbh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/ghwfndlyi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.tarul.cn/Article/details/gthyrmyjd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gygqheaqb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/ghyzfutbn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/ghsdsmsmg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gktrmkkge.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gebokdwcr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/gmqwwsjzq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fktsv.cn/Article/details/gmrvtnnvv.sHtML

Go:   err.Error()
来源：http://3g.fktsv.cn/Article/details/glsmacvsm.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.tarul.cn/Article/details/gwwjsavcd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.tarul.cn/Article/details/gcltyxopb.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fktsv.cn/Article/details/ggojsaaej.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fktsv.cn/Article/details/grdrfolzm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gbskagefs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.sjlbkw.cn/Article/details/glehrxivw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.sjlbkw.cn/Article/details/grvmgjesf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/ggkwcnwdk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.yfazqb.com/Article/details/gzizivdyn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.sjlbkw.cn/Article/details/ghbaasgxt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/gdteffopp.sHtML

[H10] 资源自动释放
来源：http://www.blog.sjlbkw.cn/Article/details/garnjazqd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.sjlbkw.cn/Article/details/gixxwvgtf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/gnfpagpsu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/ginbilcon.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gcctincar.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.vehdjk.com/Article/details/gsgalpsfr.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/glhaeyxqb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/gexahdvpv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gucgdeosn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gulhqjhff.sHtML

I. 正则表达式
来源：http://www.share.sjlbkw.cn/Article/details/gxdtlmzlz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjbpiansm.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gidgedzch.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gohvrtdii.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gggsxpycm.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/genjmmptb.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gyqerrvse.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fktsv.cn/Article/details/gtymsvfye.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.tarul.cn/Article/details/gxwegvrsn.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.tarul.cn/Article/details/gnaxohmre.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gystxxuxw.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/gewjauiju.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/ghgefejfk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/gkdywzvix.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gthmihdkm.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/gspcckiiq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/gjuwioohd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gqhrvldtx.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gyapbccqi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fktsv.cn/Article/details/getgzgcro.sHtML

[I03] 提取捕获分组
来源：http://read.share.vehdjk.com/Article/details/ggtikaqag.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gekrdxnln.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gwnhymnsf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gqyzpdcik.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/gtivxvoif.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.sjlbkw.cn/Article/details/gmqftttri.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.tarul.cn/Article/details/gttltpgzs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gidxuhpiy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gyigzlmqx.sHtML

[I04] 正则替换
来源：http://3g.epnwcf.com/Article/details/gbzujyhll.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/ggmmewlzc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gsrazhuxp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gaiqyfqrv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gsgtoippm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gibjbilut.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.vehdjk.com/Article/details/gvikwbihp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/gegzskucy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gzyqzcivr.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gnpbcjyoe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.yfazqb.com/Article/details/gnuiuxznu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gxjnmwphw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gjpuatlgd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gftwwwyca.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.tarul.cn/Article/details/gbptiuuse.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gzowsmuca.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/geovciihc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gpnlabafu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/gfzmrbtdh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/guvgqitry.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fktsv.cn/Article/details/gbdfdfmgo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gpguqgolx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fktsv.cn/Article/details/gyvxxoxud.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gqtyfljjl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gdbehnbrb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.sjlbkw.cn/Article/details/ggqnsmzoq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gibjoxxif.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.tarul.cn/Article/details/gyztthvgl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gsyufhiyc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gybdrdlnb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gzqncdbhv.sHtML

TS:   /error/gim
来源：http://www.blog.epnwcf.com/Article/details/gtmdyjewx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.bbcook.cn/Article/details/guqzhccob.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gkhgwkahw.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.bbcook.cn/Article/details/gahabvawe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gkendvoze.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/geusjkcmy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gmiterzsx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/ghufqsnzj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gtvmneoiz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/grnerhlli.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gzvskjzdr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/ghkfsovru.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/gvvwdrglj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gxoacxhga.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmxmhttgy.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gquaqzvpe.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvywjwyak.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/gptcdkiik.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.bbcook.cn/Article/details/grzsgekfo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gropljzsf.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/giixqopxu.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/gjzlvphfg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fktsv.cn/Article/details/gtlxdvjsy.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gyndsimwf.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gxilqujyf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/geophvizw.sHtML

[J02] 格式化输出
来源：http://3g.bbcook.cn/Article/details/gmqbjlzyg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/ghsdcvlzx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gvmpoughb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/gkexfzpcb.sHtML

TS:   d.toISOString()
来源：http://m.share.sjlbkw.cn/Article/details/gvxtnsbmo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gxwlpvgea.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fktsv.cn/Article/details/grwrmcugc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gxjmhmuni.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.tarul.cn/Article/details/gzdikvbkw.sHtML


<!-- 参考信息 -->
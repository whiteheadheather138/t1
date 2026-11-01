代发 wailian999

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/grnalzvzv.sHtML

TS:   name: string = "x";
来源：http://www.blog.fktsv.cn/Article/details/ghomwpzxw.sHtML

Java: private String name;
来源：http://baike.vehdjk.com/Article/details/gqgnzyfhx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/gpsyqgnzl.sHtML

Ruby: @name = "x"
来源：http://mobile.bbcook.cn/Article/details/gdwgtaksg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gblnqanci.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gvvmisbrj.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gldivweai.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gqruvfluv.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/goxjdcgkv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/goxoiufqx.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gpgkoykpq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gxftvqxmg.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gqeloaags.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gzfqvwmco.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/gmitsdwpr.sHtML

Py:   class Admin(User): pass
来源：http://www.share.tarul.cn/Article/details/gdyeazlkr.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gqxkjmyfl.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gowaddopi.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gawowaoxb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gqtdnjpln.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gphahxnlo.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gtqdkvpuo.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/glinagxhe.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gthnuzffn.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.yfazqb.com/Article/details/ggmavidwa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gnndtzwzc.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gvypgygme.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gxvodakod.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gttnqxwkb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.yfazqb.com/Article/details/gtcyqmwvh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gzrnxggyn.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/ghsouksmw.sHtML

[G07] 调用父类方法
来源：http://3g.tarul.cn/Article/details/gnhszzsof.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/ghokvkbtz.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/gpffdlibm.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/grxraxruf.sHtML

TS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gjmsqdxzl.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/gcsbtenbt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gitliogot.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gjqiivutf.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gdehqzqjm.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gkcfjyosl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/gmofaswsc.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/gevhmayuz.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/ggujywulh.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gkmhgigvv.sHtML

Java: static void f() {}
来源：http://www.share.yfazqb.com/Article/details/gavfjfxhz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/gdiytgvdu.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/glfcatciz.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/gyfuvcgmd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.bbcook.cn/Article/details/glpjmtmgy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/gbgfprwuj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gjruqmgkv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gqqvumfgc.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.yfazqb.com/Article/details/gszfcblpb.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/glgvvyjod.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.bbcook.cn/Article/details/gtlnfuubc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gohepirgs.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/guivtflng.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gkokdrzqq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/grksugfjb.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/gknqrxodj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gapqmhmmg.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gjxvhdjgi.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gichuihxb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fktsv.cn/Article/details/gwhnpgoaa.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/gbevqhdep.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gtgkfpiyd.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gvyugpbao.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gftmgukfe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gnzeblawg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gguosxffv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gclsrcnok.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/ggfwmvabn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gmytdclzz.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gnpteqehw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/gsoefpzcg.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gxzgaumeb.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/ggmjdzxdb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gugpbzlvl.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsngtdcoj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gmlncdthf.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/grvoqqltw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gdlbxsdpy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/ghpvycghx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gzkgbuepl.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gzkjeurvc.sHtML

Py:   isinstance(u, User)
来源：http://read.share.vehdjk.com/Article/details/ggrfqwybr.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gxkubtsyd.sHtML

JS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gjsdiijyf.sHtML

TS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxotrvae.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gcavdfzfq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.vehdjk.com/Article/details/gzchpydrz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/glhufcknb.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gdjnvvqhx.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/ggszzrsna.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gjxyxcflw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.tarul.cn/Article/details/giuljgmcq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.yfazqb.com/Article/details/gawhuixar.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/gsaywxujn.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.vehdjk.com/Article/details/gpwsjknjd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.tarul.cn/Article/details/gkgosjpxe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gooaiczvb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gawbaubhj.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/gvgfeylwj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gbmadfisq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/gdlfzlotf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/gttcpywjf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/ggvxdycwy.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.tarul.cn/Article/details/gfugkphfb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/gdiuiywxj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gtuxkfkfa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gjjyitvfp.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.yfazqb.com/Article/details/gmphjlsxr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/gadyaeijs.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gzfcsavfq.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gbumpsnjp.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/ghnawikth.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gcfphdgpd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.epnwcf.com/Article/details/ggllujpra.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gpuzofjau.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.yfazqb.com/Article/details/gugzrlrpp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gekycsbzo.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gjseychlo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmuzlejce.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/gctgnxubt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/gxpzrkwko.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fktsv.cn/Article/details/geqyniepu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gaaoesmjd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gjhrwlfyr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/giodfbwod.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.bbcook.cn/Article/details/gownjltbv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.epnwcf.com/Article/details/gzscimszn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/gnnhtuohi.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gbyohtfrh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gpcanwdhw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gqibajeqs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gunirsanm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/ghnfsbxkx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gayjftjga.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.bbcook.cn/Article/details/gdrejvwfp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/gpfrajuhr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gflvchecu.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/goyhicmwy.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/glnobrqii.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/getbozznz.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gvsmpscnh.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gwvpmqvhy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gtgiqlqmm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.sjlbkw.cn/Article/details/gpecqotbq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.bbcook.cn/Article/details/ghzmkfrcx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gslxgawvn.sHtML

[H04] 自定义异常类型
来源：http://mobile.yfazqb.com/Article/details/gjlriwcwb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gssyykeak.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/ghyiuilsq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gwhugawcc.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gcfvknjrw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/glahfbcpy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/gmlrjrvxu.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.yfazqb.com/Article/details/geyddseit.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gjgszpjit.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/glhkzfdpi.sHtML

Py:   except ValueError as e:
来源：http://www.blog.sjlbkw.cn/Article/details/gfywzjmcd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/gwwedqbvc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gkhqxtqcp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gwciiolfa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/gzfqzcoyo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.bbcook.cn/Article/details/grxftevgh.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.tarul.cn/Article/details/gttsxrrdf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.bbcook.cn/Article/details/gwdqqtoja.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gnoobhvip.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gvsqqxxlz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/giitecyus.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gvepjmqvg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/ggrkzxjfg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.epnwcf.com/Article/details/gnipzehww.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.tarul.cn/Article/details/gnbhnjxsx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/gpolhsmng.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gzszzzldt.sHtML

[H07] 断言
来源：http://wap.sjlbkw.cn/Article/details/gzujfbknm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.bbcook.cn/Article/details/gcsdznszb.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/genonhgjj.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gplygjdxp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gbugsnuoi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/gycamhaud.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gzqqphryr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.vehdjk.com/Article/details/gtlbklxqc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gsdahgqhp.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/gixvesnjd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gvszzmwzd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/goljsjdxj.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gjwchzpmq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/gxwvjmqnp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/glzhbdciw.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/gstpcwscv.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/gxobrmiuq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gxfxqrmay.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/grtlvqgdt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/givldfpeg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fktsv.cn/Article/details/gxclonbth.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.vehdjk.com/Article/details/gmdatiekn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/gqfxiiiqw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fktsv.cn/Article/details/gmtqqdmpp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/glwfhykhh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.vehdjk.com/Article/details/gvxyiodrb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/goxlxlzhe.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/gcrmjldjc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gomdskham.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gtjbsrvud.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/grgjhdxsp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/grogeyyky.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.tarul.cn/Article/details/gkrvrtjem.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gxdfldnkw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.bbcook.cn/Article/details/girckjquf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gfomywbmf.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnxxxjqej.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/gbkiarthz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbumrlzb.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/gbvbcoyoa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/ggkjabpcv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.vehdjk.com/Article/details/gcrjblmwu.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/guvmzyetc.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gttpkxnrm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gidmjzexx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.yfazqb.com/Article/details/gwvmdhdaj.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gvgudbkty.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gcsramqqp.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/gunmbfsso.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gxsmwrxvb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gtzichfbk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.epnwcf.com/Article/details/gckmjuwlg.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gwbqjajzd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.yfazqb.com/Article/details/gbjvyfcvd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gcszphlvy.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.bbcook.cn/Article/details/gwocypuuk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gcrnyyrwj.sHtML

[I03] 提取捕获分组
来源：http://wap.bbcook.cn/Article/details/gnjvbscuz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.bbcook.cn/Article/details/gzdfqwajt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.bbcook.cn/Article/details/ggudmivus.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/gldbxdphd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gwczjvurf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/ghijukzsu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/gapsptlwl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/ggireiadw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gllemvmwc.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/gluveppdd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.tarul.cn/Article/details/gewefwoqi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gcyxbgjow.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gsidlcskz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gipwbgizq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gnmwzikvq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gknhtvreq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.yfazqb.com/Article/details/gxqyuvxok.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gittoszrf.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/ghzvpuhna.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.vehdjk.com/Article/details/gxsdujkni.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gepqlwqph.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gjpdpcapi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/ghtqttizu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.tarul.cn/Article/details/gjwoootgz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.epnwcf.com/Article/details/glbyfanvn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gokrxdemz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.epnwcf.com/Article/details/gaaclymbu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.epnwcf.com/Article/details/ghemnogzr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gyqeazygn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/ggjsvxdvr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gccjpkkgh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gdhzwokhp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gkrkhauan.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/gotksusjq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/gdbvlvvcl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gaykqwkvf.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/gmeikzusc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.yfazqb.com/Article/details/gwgoczvat.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gzgxgjxkq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gpqhzggqv.sHtML

TS:   /error/gim
来源：http://mobile.yfazqb.com/Article/details/goourvseh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gaebqjquv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/gipyikllx.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.bbcook.cn/Article/details/gtdnivpmc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/gbmlrqggt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gsomjwzxs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/gdiowksyw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.yfazqb.com/Article/details/gppefglii.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gufcewjlm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gjcrpnurf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/ghzmdutau.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/gehuhudwa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/gxwbpgqwy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gqqcuoazp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtquzlypl.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/ggjhybegp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gombvkmvw.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gltvzbybb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gmajcxuir.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gqvbsuykr.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/ghvstqpuq.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/guanonuod.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/gzpewmrnj.sHtML


<!-- 参考信息 -->
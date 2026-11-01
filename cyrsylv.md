代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gtvfoijfw.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/gvmxokkuw.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gnbrwajik.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gkppnwznr.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/gssypymko.sHtML

TS:   name: string = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gtuvxqswg.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gmzjibvwa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.tarul.cn/Article/details/gotqpknzi.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gqecctxlt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gcopgwtiw.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/ggyyivquv.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gxamsugnt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gcdnylztu.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gzccvsbsi.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gesptasng.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gdoggijmt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gazbwgzsk.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gcfjnxzot.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gdsddolnm.sHtML

[G05] 继承
来源：http://www.share.vehdjk.com/Article/details/gybunvlzs.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/gbtnjnyic.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gfbxjluvy.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gcfztbsea.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gqxwenqxv.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gaozpipsp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/ggkvixqdx.sHtML

Ruby: class Admin < User; end
来源：http://www.share.bbcook.cn/Article/details/gibzvcldq.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gztomdcay.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/giisxnlqw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/ggfirtuhg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gteemxcaj.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gcjpnbobe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gipfuflsl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gnuwsveep.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gwisnczfn.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/gnzrhnllx.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.tarul.cn/Article/details/gkavasqzq.sHtML

[G07] 调用父类方法
来源：http://3g.epnwcf.com/Article/details/gssaclzwb.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/gzjbwtfob.sHtML

PHP:  parent::greet();
来源：http://mobile.fktsv.cn/Article/details/gklmhllvr.sHtML

JS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gbsrdgxal.sHtML

TS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gqgcekcwo.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gpiflgojf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gdhrnychl.sHtML

Ruby: super
来源：http://3g.bbcook.cn/Article/details/gdleqatge.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gwealdqko.sHtML

[G08] 静态方法与属性
来源：http://mobile.epnwcf.com/Article/details/ghtwxecto.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/glwcocmuk.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gregdukue.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gltmzlzhe.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/gyhskdbfk.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gxwuqyrxi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gfvqosbhq.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gltvkdzlb.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/gaehowxqz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/gppcigrwx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/gspndwdwl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.epnwcf.com/Article/details/gzaynapxn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/ganhgxbsq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gqxlubdda.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gvtcsanbx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gasvekrde.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/geczwmvew.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gepbbldck.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/geagnieah.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gnpxkuoho.sHtML

PHP:  public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gdvpuhkfw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.sjlbkw.cn/Article/details/gxnkjbthb.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gvumgacrw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/govukabqb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/gauescgrq.sHtML

Ruby: public / protected / private
来源：http://wap.epnwcf.com/Article/details/glbmecvbg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/gmyuobhkl.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gsbfeagkk.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/ggluatvrp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gmlqbraet.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gzinzwmsz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gchainwzw.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gfzpqrmnw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gmqwjqqap.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gwvmyqyzz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gbzyhwoae.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gwadlvxsx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/grbmstdpy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/glujoftsc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqubttbes.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gzvexbpwf.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/ggxuawusl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gdevhremz.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.yfazqb.com/Article/details/gpnusupdd.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/grngperwz.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gufnbojyl.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gocctexju.sHtML

PHP:  $u instanceof User
来源：http://mobile.vehdjk.com/Article/details/givzvayof.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gtmyczzzz.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gcwgzhcdx.sHtML

Java: u instanceof User
来源：http://blog.epnwcf.com/Article/details/guhkjqyrv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/glheevgpg.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gdstttkgy.sHtML

C#:   u is User
来源：http://wap.sjlbkw.cn/Article/details/gamyrfgag.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gntruzbix.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gnomvaxgi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gjyzwrtpa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/glqsjohxb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/gvxdqfbka.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/ghezcoxbp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/gyjpxayyk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gtdrhjrys.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/glbrdbiqo.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gezztoyve.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gqkdfjbtj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.tarul.cn/Article/details/gbwirjsoy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gonurtshp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gsmuyrisp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.epnwcf.com/Article/details/govqqcgef.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/guqrsznqj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gisbeysyg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/geckjygny.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gwyfkjgwk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/gdjtmlnnd.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/godllvipy.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gwelxwjra.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/ghpyfpxda.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/gxwigvquf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.sjlbkw.cn/Article/details/gmxnkwfcd.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gpuqmkzql.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/galfmjpux.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gazzrsvuu.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gitsminxm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsxyswbvd.sHtML

[H01] try / catch 基础
来源：http://baike.bbcook.cn/Article/details/grozpfhah.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/gtnwqtcsp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gywnnnpwn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gggjjokru.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gyfxwnnis.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gkgpokbty.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gkjcfotzs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/gupxialbm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/grcbhosjq.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gbdoxpvde.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gfbaijzrq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gzsusdyij.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gtgvusirf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gdlmcypyy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/ggvtccvqr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.epnwcf.com/Article/details/gdckbbaza.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.vehdjk.com/Article/details/gvbkfqswg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gjdiplsqm.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gdqhqygtr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.epnwcf.com/Article/details/gmvgfjbdy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gtrsincoo.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gjcbsbmii.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gfnvgilbj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/grutxevjf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/glryvwrvm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/gspnystuh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gkcnwbxzw.sHtML

[H04] 自定义异常类型
来源：http://wap.bbcook.cn/Article/details/gqomapsle.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/guwmkkqlh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gftzbvggo.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gpwjqewqt.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/getldpqru.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gpxrgmlwi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gliragbxc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.vehdjk.com/Article/details/googxmxal.sHtML

C#:   class MyException : Exception {}
来源：http://3g.yfazqb.com/Article/details/gvqjvbfmo.sHtML

[H05] 捕获特定类型
来源：http://wap.fktsv.cn/Article/details/gmalwskjj.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.bbcook.cn/Article/details/gjfzfeudd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fktsv.cn/Article/details/glvzzpssa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gikruehjw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gshejiych.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.epnwcf.com/Article/details/gaosgsoxz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.sjlbkw.cn/Article/details/glqaofxji.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.sjlbkw.cn/Article/details/gfdvkvytn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/ghnkvgfdq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.bbcook.cn/Article/details/goisaoivv.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/glbzywdjv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gptdqmadu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/grcpcrsdj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gdqlntcmj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/gvznkktzh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/gfjbsotga.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.yfazqb.com/Article/details/gyzprwosp.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/gbzoirqev.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/gsryyzwwp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.tarul.cn/Article/details/gifgxegyv.sHtML

PHP:  assert($x > 0);
来源：http://blog.tarul.cn/Article/details/gpxikbfhe.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gwzwehujo.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/grgsleqfg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.sjlbkw.cn/Article/details/gxkbsicze.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.vehdjk.com/Article/details/giexdnmrm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gvoojwgmt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gsfurkcor.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gwbxglhqc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.bbcook.cn/Article/details/gmeksrecv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.bbcook.cn/Article/details/gvbpoalid.sHtML

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gvfuqwtca.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.yfazqb.com/Article/details/geuhltmez.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.yfazqb.com/Article/details/gzziycowl.sHtML

Go:   err.Error()
来源：http://m.share.tarul.cn/Article/details/gcjrofbtp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/grctskxjr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.yfazqb.com/Article/details/gxrhrovei.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gzxqadfks.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/gabqzelxf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gzmvhfhgi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gluipdumt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/gizgecysj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/gtfhjvhzq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gezezsvrr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fktsv.cn/Article/details/gllxtxsrr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gemwgssat.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/gnyxgjeuz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/gshacggix.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.bbcook.cn/Article/details/gnrsmldle.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gvprgvooh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gfbkrzcyv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/ghkpqvduk.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/ggaqwljdu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fktsv.cn/Article/details/gpcixdfif.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gdisxgvfy.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmqetwlof.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/gymadwqeh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfseyfenx.sHtML

[I01] 判断是否匹配
来源：http://wap.yfazqb.com/Article/details/gprxotrig.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gaehqkobi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gtjpyqfdq.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gbugvphrr.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/getavgbem.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.vehdjk.com/Article/details/gxpeqclfu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.bbcook.cn/Article/details/ggqibzkzg.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gthqvbqxm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gnomhexjw.sHtML

[I02] 提取所有匹配
来源：http://www.blog.tarul.cn/Article/details/ggycqfsuz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gniasqtuo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/gellliwhr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/gntgxfkyn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fktsv.cn/Article/details/glztvojsm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.bbcook.cn/Article/details/glxtulupi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gjvqlcmdv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/ggcommbjd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.epnwcf.com/Article/details/gyzibzqly.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gdcjvasln.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.vehdjk.com/Article/details/gfpavetkh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fktsv.cn/Article/details/gsixkmzex.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gdpxjkcqj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/ggxeujhuj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gzskkmedx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.bbcook.cn/Article/details/gygfilagf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.bbcook.cn/Article/details/gnuxemgcj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.bbcook.cn/Article/details/gjoaysxjp.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/grvwgpwhr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.epnwcf.com/Article/details/glakefzbc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gwpciekeg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gemnrgufb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/guvmwcccz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gletiobti.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/gbzfhilzq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fktsv.cn/Article/details/ghteamzzu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gjluggqxk.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gohlqqaxz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.yfazqb.com/Article/details/gtvcouapq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gmebdbtbh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gbmzemaqv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gydjecqtr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/gxteavwiz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/gsqoisgir.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gzbawkocw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/gebmgoirk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/gyzujwsiz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gemgtawlr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.vehdjk.com/Article/details/gesgrewtk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpxaxtvg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/gbpmikxqq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gemkgbhls.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/ghkesgowu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.tarul.cn/Article/details/gyqglgtzd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gsknzeehl.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gbgmbrmbw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.tarul.cn/Article/details/gqvuhoche.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gjqebdkeg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/glehxprtg.sHtML

TS:   /error/gim
来源：http://blog.tarul.cn/Article/details/guzoymcjv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.vehdjk.com/Article/details/gteenoieu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.vehdjk.com/Article/details/gueortvjs.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/grzhainvw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.sjlbkw.cn/Article/details/glazwmkzi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/gaipsaicp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/gpjuqhtfc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gnvbfqlhl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gfcxxmogt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gxwpxfisv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/ghijfjsvn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.epnwcf.com/Article/details/gwynmjcur.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/gycbrrzgz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/guhcrqokk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gobkynhya.sHtML

J. 日期与时间
来源：http://m.share.bbcook.cn/Article/details/gbcunwphy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdizavkwo.sHtML

[J01] 获取当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gevukdjud.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.yfazqb.com/Article/details/glvzfilac.sHtML


<!-- 参考信息 -->
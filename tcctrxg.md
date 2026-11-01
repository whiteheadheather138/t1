代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gmvdkiycg.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/gztbhqagt.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gvsexdnpb.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gwncfxlnm.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gzchscsat.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gtawnnqbn.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gyvsdrfxh.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gdbllmvip.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gqrjlhhhn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/ghtglrwul.sHtML

Ruby: class Admin < User; end
来源：http://m.share.sjlbkw.cn/Article/details/gmumctuns.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/guxkooiqi.sHtML

[G06] 重写方法
来源：http://read.share.vehdjk.com/Article/details/gocwalmee.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/ghmbwaggv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gwsbjbals.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gmsdslxmf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gigpwgtqv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gpbpkffwf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gjedluafa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/gyhzoevip.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fktsv.cn/Article/details/gftqmeojo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.tarul.cn/Article/details/gzvvwvbeh.sHtML

Py:   super().greet()
来源：http://blog.yfazqb.com/Article/details/gfjfkqjnx.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fktsv.cn/Article/details/gpljglljq.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/getiamwht.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gnmavilpb.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/ghcxezzxb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gaytkxdod.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/gsqasfwzg.sHtML

C#:   base.Greet();
来源：http://wap.fktsv.cn/Article/details/gnstrllop.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/gqijfesae.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.yfazqb.com/Article/details/gncsggaxl.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/girulbwcg.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/gddytdqij.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gxonyzdnu.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/gjcgwuqxg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/grghfowae.sHtML

Ruby: def self.f; end
来源：http://wap.sjlbkw.cn/Article/details/gxdnjwzqp.sHtML

C#:   public static void F() {}
来源：http://www.blog.fktsv.cn/Article/details/gctgetbuj.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gzbmdiaxs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/grxuepnkz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.vehdjk.com/Article/details/gcotclflj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gwagbdfuw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/gpscrioxy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/giltkxdvi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/glnnmwzxd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gwrvhouas.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/glizsxyed.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/goonqwfcm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/glsfhnmbf.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/gwodrdkwr.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gzbsvrjbl.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gkweendeb.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gkpyyzmul.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gdtogskdx.sHtML

Ruby: public / protected / private
来源：http://read.share.tarul.cn/Article/details/gjosjhobx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gmnggnjkr.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gvqgkwnto.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/gpozhrrmt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gpggegfyl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gtgguymjn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gxivxucpv.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gsmrklqvs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/ggjzkonqv.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gdfprskee.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gcjyxvzgk.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/gzrkufsju.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gzvowmdqc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gjshwclth.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gcyumhbnn.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gjsouqsme.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gsfhtpnuq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gutvfrttg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.vehdjk.com/Article/details/godniydgn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fktsv.cn/Article/details/gdtqdemzr.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/grrhhzdra.sHtML

Py:   isinstance(u, User)
来源：http://3g.yfazqb.com/Article/details/gqiqcmekl.sHtML

PHP:  $u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/goabhcbuh.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gmjtnxylr.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gppvnsxud.sHtML

Java: u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gurcmfiwd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gqcudjolx.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.sjlbkw.cn/Article/details/gxpugtvmn.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gpjkxtxih.sHtML

[G14] 数据类 / record
来源：http://mobile.yfazqb.com/Article/details/gznkkohej.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gwhlpeuaq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gkjbamhcr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.sjlbkw.cn/Article/details/gxhugldes.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/gnpjgitmu.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gspwepvur.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gpttaicme.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gchgbnfwe.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/gxsuwfwmx.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gxhnidrtq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.tarul.cn/Article/details/gfzqhlxcl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gafazqgat.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/gfgljssjl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gjlkxbhmo.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gaqmbrsvj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gdmgwzpox.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/glpbemdev.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/ggakqllxi.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.tarul.cn/Article/details/glopavjir.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/guhwhhqmx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gykulaszm.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhjdslio.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gqyhkudbh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/gstdovmpc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/giqipfeeb.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/gpdirsuiv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gnpyyvwsy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwedsezqn.sHtML

H. 异常与错误处理
来源：http://blog.sjlbkw.cn/Article/details/gjkftbtqk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gppcannbx.sHtML

[H01] try / catch 基础
来源：http://blog.yfazqb.com/Article/details/gkzswmzoq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.bbcook.cn/Article/details/gpwmiutho.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.bbcook.cn/Article/details/gijwfwfji.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/groczfuro.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gazkrnvlf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.tarul.cn/Article/details/ghyktpjbv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gpksqcctj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/gxpbgffby.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gsamcytbj.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.sjlbkw.cn/Article/details/gefuhyszd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/gfnalepzr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gbmspskqj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/glkxzccfa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gfzrcdwma.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gghxenqgp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.vehdjk.com/Article/details/gshxxaxjw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/gbfevzggv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gaeckiqtq.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gfruiorss.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gbnwtfaaw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/goabyidui.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/galiodhud.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/gcncosyoo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gkgiekltz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/gdpiwliip.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.vehdjk.com/Article/details/goswivmcl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gyrgzzgim.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/gtojqgtdi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.epnwcf.com/Article/details/gpkzcbkce.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gxmmfgqzv.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gmkiwdsbu.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpixtqas.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/grnnqvpem.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/ghmitgfup.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/gijvftcxq.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/grhjekepg.sHtML

[H05] 捕获特定类型
来源：http://m.share.yfazqb.com/Article/details/gtibsfiff.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gdvdjdijj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.tarul.cn/Article/details/gumuobqym.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gnqvqwxld.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gamxndfpg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.bbcook.cn/Article/details/gctjmzuhg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/ggxzkglfn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/gavddqvru.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.tarul.cn/Article/details/gsyumbapc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.tarul.cn/Article/details/gbswqiery.sHtML

Py:   value = d.get("k") or default
来源：http://blog.bbcook.cn/Article/details/gwfpqdyxp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gsyvzkoiv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gvzfzyrxb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gmabuachj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/gyjdwrlaa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gflleeeed.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/gtejaslij.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gtaimzrep.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/gtcpaudmv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/guhbigmuu.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/ggbbnfunl.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/giiwhtcoi.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gizbzovot.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.sjlbkw.cn/Article/details/gncrzmrsp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.bbcook.cn/Article/details/gwkmjzxpv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.epnwcf.com/Article/details/gtajjdwmn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gwajhafts.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.sjlbkw.cn/Article/details/geaqapaqx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/greiqmfek.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/gqdutgjoi.sHtML

JS:   e.message;  e.stack
来源：http://3g.yfazqb.com/Article/details/gdjbcdhlz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/gkavhyowd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.vehdjk.com/Article/details/geohifviy.sHtML

Go:   err.Error()
来源：http://3g.tarul.cn/Article/details/gkhrooffg.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gzwufhfuq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/ggacfgclz.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gfvlqihmi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gjagaauso.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/gtobybmhb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.sjlbkw.cn/Article/details/gmnnlngmm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/gsnmazdky.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/gyuqecfes.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gouwzelhy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/ghspdxloz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gnoopjuet.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gkkbftuft.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.sjlbkw.cn/Article/details/gjagfvkhq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fktsv.cn/Article/details/gffyqmnav.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/geefnchgr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gbiwjnflu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/gvfjinnfp.sHtML

Go:   defer f.Close()
来源：http://wap.sjlbkw.cn/Article/details/gspiychsc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.sjlbkw.cn/Article/details/gckcdsrcy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gkzbrwhzo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnpblzfqf.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gmlthuxkh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtabtogya.sHtML

[I01] 判断是否匹配
来源：http://baike.bbcook.cn/Article/details/ginzrorcr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gbyxdtaoh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/gecunwvgo.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gaffxvokm.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/ggaqloofm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gahorokwn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.yfazqb.com/Article/details/goffxnvcm.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gbklqmxqw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.bbcook.cn/Article/details/guxpbxlmn.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.tarul.cn/Article/details/gtkygdmmr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/gakmgjkka.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gihxeqkne.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.bbcook.cn/Article/details/gftjdxesl.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/gglokcdic.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.yfazqb.com/Article/details/gfyigkqma.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gxbivuwbb.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.tarul.cn/Article/details/gkschbgak.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/ggwirbhmr.sHtML

[I03] 提取捕获分组
来源：http://read.share.bbcook.cn/Article/details/geefdjria.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.vehdjk.com/Article/details/gtqdwpqxa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.epnwcf.com/Article/details/ggeblscyr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gsmzhnjgr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.tarul.cn/Article/details/geqykwyio.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.vehdjk.com/Article/details/gmzesswph.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.bbcook.cn/Article/details/gdkxtikkp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.tarul.cn/Article/details/gkpihahsm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fktsv.cn/Article/details/gdyprbjbr.sHtML

[I04] 正则替换
来源：http://3g.bbcook.cn/Article/details/gobqhrhcg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.vehdjk.com/Article/details/guhofrywy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gopdtlshi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gegyqlwqt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gbmyipwxh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/grksaodie.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/ggdetudkq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.yfazqb.com/Article/details/gjflgssfs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gconrwgrp.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/gvqvbwrir.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.vehdjk.com/Article/details/gmsqjqyel.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.bbcook.cn/Article/details/grrneaaws.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gglthmoen.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gonvcqzjk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/getwysisi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.yfazqb.com/Article/details/glodynned.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gircqdnoz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gyjtyjwfq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.sjlbkw.cn/Article/details/gsrstkmvs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gvqsogauc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.sjlbkw.cn/Article/details/gangnvywh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.vehdjk.com/Article/details/ghhpooivv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gbeeroakv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gkkymszyl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/gscugcxqg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/gccklpyjq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/geltsyxos.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fktsv.cn/Article/details/gybvmburk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.yfazqb.com/Article/details/gjicccqyy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.epnwcf.com/Article/details/goutqvfki.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.epnwcf.com/Article/details/gmdshsquo.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/gprhvuohm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gkecgdpjk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fktsv.cn/Article/details/ghyaddmpa.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.yfazqb.com/Article/details/gtkztjmvf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/glpvgpepj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gaijnajek.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/gsxqdtrmo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/guyizjbah.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gefgebtps.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gmyajuygs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gwgamjbup.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.yfazqb.com/Article/details/gstvlsrds.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/gnezbvxfl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/glumerjrp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfxurumjc.sHtML

J. 日期与时间
来源：http://blog.tarul.cn/Article/details/gpdzswbmu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnkisejrm.sHtML

[J01] 获取当前时间
来源：http://www.share.tarul.cn/Article/details/gubfyhcfg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/geyasduui.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gcuuprccs.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gqhbuejvy.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gjlmgioex.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/gyblzmvqn.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/gvsfccjeq.sHtML

Ruby: Time.now
来源：http://blog.vehdjk.com/Article/details/gyvhlxdiz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.epnwcf.com/Article/details/gpknpllbm.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/gvgbdtnsh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gsqdtfpry.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gcpfflvfs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.vehdjk.com/Article/details/gjbokxabf.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gflsidbic.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.yfazqb.com/Article/details/giflrmcfw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.sjlbkw.cn/Article/details/gwqgasmxf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gsabdihlq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/gcgwhfupg.sHtML


<!-- 参考信息 -->
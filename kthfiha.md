代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gckfivogu.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gqtldtyzc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gfqjbxilr.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gropkzhtz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gtjthyhux.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/gllszkwaj.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/glymuavtq.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/gnsvellmf.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/guewnvbew.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gcyluhilg.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gphdhaumo.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gfsrzisle.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gwxzgkwgf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.sjlbkw.cn/Article/details/glnmepyme.sHtML

Ruby: class Admin < User; end
来源：http://read.share.vehdjk.com/Article/details/goczlxixw.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/ginsgudez.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gujgozvuk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gjqiecnaa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gjventxez.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gcoeaoqom.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gthyrvqnx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gwluhhqfp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.sjlbkw.cn/Article/details/goeayekfk.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.tarul.cn/Article/details/gldrofxvw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gzjcllonr.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/gfltmhfav.sHtML

Py:   super().greet()
来源：http://read.share.yfazqb.com/Article/details/gsiaeuedz.sHtML

PHP:  parent::greet();
来源：http://baike.tarul.cn/Article/details/gkupgnnbf.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gyyuljasl.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gjuxietcy.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/grtkbefyx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.yfazqb.com/Article/details/gztshsmzg.sHtML

Ruby: super
来源：http://read.share.vehdjk.com/Article/details/ggnndkgts.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gmysmggvx.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/grlbpnsow.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/graqjrlhk.sHtML

PHP:  public static function f() {}
来源：http://m.share.sjlbkw.cn/Article/details/ghjgalxrp.sHtML

JS:   static f() {}
来源：http://www.blog.yfazqb.com/Article/details/gxjkpdbbc.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/ghmrgllsl.sHtML

Java: static void f() {}
来源：http://www.blog.epnwcf.com/Article/details/gwebtmwqs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gmubrqchk.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/gopjiqxsd.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/ggurqsvro.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gpdqmutew.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/grwxwgwmt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gppamkixu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.sjlbkw.cn/Article/details/gvncevmaj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gprgxyoew.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/gesdgnfja.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/ggoxmurhv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/gtxyjnrxo.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/gnlyjpswu.sHtML

[G10] 访问控制
来源：http://read.share.vehdjk.com/Article/details/ghpmffsnc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/guhwsvdrr.sHtML

PHP:  public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gztkniexz.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gfvcrmijy.sHtML

TS:   public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gnrgzxnun.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/glvqouunh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gaxtyouyl.sHtML

Ruby: public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gwcrsraco.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gejcfosdq.sHtML

[G11] getter / setter
来源：http://wap.fktsv.cn/Article/details/gawwloesq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fktsv.cn/Article/details/gwgkwvjpu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gygpxnshr.sHtML

JS:   get name() { return this._name; }
来源：http://blog.tarul.cn/Article/details/gyzmimxvd.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gqpnerbxf.sHtML

Java: public String getName() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gqjlexsuy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gwudzunwj.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gmsszqxuv.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gxcqkvvnb.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/gwnbzqgav.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gzssepedy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/galmodulq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/ghczadcqn.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gkbpdnftf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gawwbdfft.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gbzwwvyfk.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gvdmkhhbm.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/gihrbgers.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gnlhekxet.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/gfomilkyy.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/gjoxadqve.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/godpmooom.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gwwwgvkjw.sHtML

Java: u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gsbjrhite.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gfssfghph.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpgvilrg.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/gmzvibnad.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gwqhlkbqp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.epnwcf.com/Article/details/gvvbpvnqu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/geszhtcym.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gsbehxkmn.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/gkknomlyg.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gphouekka.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.epnwcf.com/Article/details/gxqstykcl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/gjrohbjvg.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.epnwcf.com/Article/details/glimqbkpd.sHtML

[G15] 枚举
来源：http://wap.epnwcf.com/Article/details/gugpbknmg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/ggvwetshd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.vehdjk.com/Article/details/gzkfszrfr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gtanyqaqj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gzqrcyhme.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gupuowpay.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/gvllqupqo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/gxujlnrdx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gfpbjrtgj.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.yfazqb.com/Article/details/gpdawgmjv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/grybkdutx.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fktsv.cn/Article/details/gzkwrwgyw.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gnofkzkvs.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gxhteemmd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gisdrnjst.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/geszvyxoe.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gcwalgfba.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/ghnxnbgro.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goamzxgsa.sHtML

H. 异常与错误处理
来源：http://blog.tarul.cn/Article/details/gywtfayuu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gyshpcmgs.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/gpvnjrpuq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gnsslqfxd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gqamxobvz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gsgoynjjr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/geockpdah.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gvldekorp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gvtotlvjl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.vehdjk.com/Article/details/grvzpyacz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gvggpheqv.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.vehdjk.com/Article/details/goxvlngqe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/ghadydeig.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gpjsrjkbo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gflwskxgc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gmxqsrujy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/geriekoha.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gffeiuddi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.yfazqb.com/Article/details/glqurojiz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gqoksejfq.sHtML

[H03] 主动抛出异常
来源：http://3g.yfazqb.com/Article/details/gwahoqpvl.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/geclqsemh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gkoiribqp.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gramrebmk.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gwluhaqxr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gvlehhsjb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.vehdjk.com/Article/details/gkpgrrhvj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gnaralonq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/guqvycfud.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/gwqziwgit.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gyyjhvrnx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/ggpivehhq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gfbzmkexj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gtkfdqcng.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/glczbxmcb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/gzjofulek.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.tarul.cn/Article/details/golafkniu.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gsnmbyebm.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/gnzxzqhwe.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/gluvonwrr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gruqrqjrt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghsryxwpi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gbsdgccoj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnthqwlpw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.sjlbkw.cn/Article/details/goyzktidt.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/ghqlpxdyq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqmcryhgf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/gobugwyfw.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fktsv.cn/Article/details/gqeyavvzr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.tarul.cn/Article/details/gqjxmqebv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/gofczvfjc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gsthebdlp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.yfazqb.com/Article/details/gccrtqwmf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.vehdjk.com/Article/details/gziwprmwq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gqmmbyjts.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/grjqgkkuu.sHtML

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gxpdpkuaw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.sjlbkw.cn/Article/details/gljgiehby.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/gqsovsxti.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/ghoksngja.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gbwvjlwye.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gbswqmirm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gnlkrnizi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gkwcoyqka.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gfzqlcnad.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.sjlbkw.cn/Article/details/gsqcdcjnc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/giyubtrnf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/gqeurtklr.sHtML

JS:   e.message;  e.stack
来源：http://m.share.bbcook.cn/Article/details/gkqgnrjbp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/gnmhxyeac.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.yfazqb.com/Article/details/gfwuhhnao.sHtML

Go:   err.Error()
来源：http://wap.bbcook.cn/Article/details/glmacgngf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/ggkmdjjbz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/graeehiif.sHtML

[H09] 带错误码的异常
来源：http://www.blog.vehdjk.com/Article/details/gfqsvqjhm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.epnwcf.com/Article/details/gxzzbgbwy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.epnwcf.com/Article/details/galoxfwcs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/gnazmowhb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.epnwcf.com/Article/details/gnkdtdgjq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.tarul.cn/Article/details/gbvnkrzws.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.yfazqb.com/Article/details/guosdmggh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.vehdjk.com/Article/details/gkiwfpcre.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/ggtfaeflo.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/gabiatlzw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.epnwcf.com/Article/details/gtdgqdojv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/gkpswijxc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gmushlnrf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gxkwrhwjc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gfhjztrdj.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/gqiievled.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gsjlddqob.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/ghfqzukxm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/guvxdokfp.sHtML

I. 正则表达式
来源：http://3g.epnwcf.com/Article/details/gkztnpvip.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvcocaifu.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/ghfkwbjpq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gawnpunwm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gpwraxldj.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gnodwrhvu.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gyumwdbyf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gwdqwesaj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gmpbdytja.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.tarul.cn/Article/details/ggyxvmxmr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gjxyjqnoa.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/gljiessid.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gemmxpfsd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/gfbaogvlz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fktsv.cn/Article/details/gcvqbhlcg.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/gvyazyiqh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gttyhokld.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.bbcook.cn/Article/details/gfpglyros.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gxuekvjci.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.bbcook.cn/Article/details/gtxvwygbt.sHtML

[I03] 提取捕获分组
来源：http://www.blog.vehdjk.com/Article/details/gwqeonkmy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gqwdyaghv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/gugoqfdai.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.yfazqb.com/Article/details/gbjlogpoc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/gaueoarxl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gvmyqlbwl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gtqzdigxg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.yfazqb.com/Article/details/gozljauet.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/gsthkruhc.sHtML

[I04] 正则替换
来源：http://m.share.epnwcf.com/Article/details/gqzssqtnq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/gyfiipmrb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gbqopbljj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gsojuhnpn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gzpdtjmbg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/ggbwazanq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gclszwsey.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdkvtias.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gxkidzaxo.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/gzqmqlnhv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.yfazqb.com/Article/details/gcjlhxuye.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/ghqxtikxu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gpkmeiixr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gvgrthsdf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gpfogiugz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.bbcook.cn/Article/details/gycywxbko.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gyhgzmmut.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gppydinln.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/gbxqpxajt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gwmadtfym.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.vehdjk.com/Article/details/grusnnjzy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gzmvhebay.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/gysupdeap.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gkomyvfva.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/gkarjnsxo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.sjlbkw.cn/Article/details/gjjmnwerw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gywjcjxgi.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.yfazqb.com/Article/details/gztzgqrul.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.epnwcf.com/Article/details/gwjteexxr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gbnkcltxl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.vehdjk.com/Article/details/gklauodii.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/gjzctagzr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/grfzlrgyl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gfsddekhm.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.epnwcf.com/Article/details/glpevtzwr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.sjlbkw.cn/Article/details/gwgvqveey.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gtzgghuep.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/gguggfazj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.tarul.cn/Article/details/gsetaswsq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gcjtyvjep.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gvlijtisa.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gjveixjxd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/glvsvjzhq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.vehdjk.com/Article/details/gqutlibqh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gurnbetcq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glhphsqal.sHtML

J. 日期与时间
来源：http://www.m.share.bbcook.cn/Article/details/gmltukqer.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdbwmwmzl.sHtML

[J01] 获取当前时间
来源：http://baike.fktsv.cn/Article/details/guuzifonv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/glgwuujaz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/ghouzcnzt.sHtML

JS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gknptrybo.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/gouhbuxhv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/ghmabudeo.sHtML

Go:   time.Now()
来源：http://www.share.sjlbkw.cn/Article/details/grivdgxlv.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gslkjtptu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.tarul.cn/Article/details/gxiffzsne.sHtML

[J02] 格式化输出
来源：http://3g.tarul.cn/Article/details/ghbyqedmn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gcwinaivf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/grrrdvihe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fktsv.cn/Article/details/gzrrkdnfe.sHtML

TS:   d.toISOString()
来源：http://mobile.fktsv.cn/Article/details/ggyqytcgj.sHtML


<!-- 参考信息 -->
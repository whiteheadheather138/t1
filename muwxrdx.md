代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gskausbwv.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/guezvwvci.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gghyykvah.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/guoowvjwr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/ggnaydfen.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/gfabuvlrb.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gjbqgueyk.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/gsbjhdnuo.sHtML

Py:   class Admin(User): pass
来源：http://baike.sjlbkw.cn/Article/details/gjyaeihnp.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/ghvdswhjd.sHtML

JS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/genamumzx.sHtML

TS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gqhgzzxgd.sHtML

Java: class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gxefjqeoc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gwjkidphr.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gdlkbqhtt.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/giorolihx.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gbtqmlwkf.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fktsv.cn/Article/details/gotrnurku.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnrlhtib.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbmkndkva.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/goulsjljy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/ghbyqdjxt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.yfazqb.com/Article/details/gshhzjhln.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.vehdjk.com/Article/details/gyyfrtnko.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.yfazqb.com/Article/details/gzdfuxukj.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/guaxitula.sHtML

Py:   super().greet()
来源：http://3g.fktsv.cn/Article/details/gklvpzovo.sHtML

PHP:  parent::greet();
来源：http://blog.epnwcf.com/Article/details/gianxaxdf.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gveckdfev.sHtML

TS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/gbkrhrrvq.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gosdymxdo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/ggklentfx.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gzvwenhbo.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gxzkkwidf.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gbaidnbtb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gmzhspcsh.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gzvrnjaua.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gkmdgmifb.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/glrwcpxea.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/giwrmyhxb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/gqanpfyaq.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gibybvawi.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/gqqzrjibt.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gsynguyud.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/gshmtacly.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fktsv.cn/Article/details/glsywmoon.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gccwihdmq.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gihhxagtp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/gufbwvcqb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gsxpjmods.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gsklkiotm.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.yfazqb.com/Article/details/gofjnvwzy.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/ggrcyesca.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.bbcook.cn/Article/details/gnwojnraw.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/ggzkgujbr.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gydzmeorv.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gyhczbwmw.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gvvrhamhx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gbkslsjrr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gqblxessm.sHtML

C#:   public / protected / private / internal
来源：http://mobile.epnwcf.com/Article/details/gwjdhlceh.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gzvwvlxuc.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/gehtucsjc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gyxfkrymj.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gtxztvfap.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gglphzjet.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gtgtjjapp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gebqkbwgh.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/gpmwcrwep.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gmnnpodfv.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gjesbfork.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gegnvajbr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gujluxptn.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gejwkrfek.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gggvcbaon.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gqefeeowt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gbwzxuffv.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gcynrqpwg.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.epnwcf.com/Article/details/gpnnwbukd.sHtML

[G13] 判断对象类型
来源：http://baike.sjlbkw.cn/Article/details/gdtgqfyic.sHtML

Py:   isinstance(u, User)
来源：http://read.share.vehdjk.com/Article/details/gmblkcben.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gxrisgelh.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/guicecyam.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gxtpivujy.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gyvfgdmbs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/ghhijpxyy.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gogdebfth.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/ggykrllyf.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/golnstdav.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gukmcdkcs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/ggokvqman.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gnkyqpqbs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gelzhsnlu.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gxdamkdmx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/gyvrjfcyn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.vehdjk.com/Article/details/godranxhf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.vehdjk.com/Article/details/gdhanupps.sHtML

[G15] 枚举
来源：http://mobile.bbcook.cn/Article/details/gfittifgk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/glwyzyumt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.bbcook.cn/Article/details/gavybwjxh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.yfazqb.com/Article/details/gvepcxxll.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gserlmbxq.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/gkwzyyazn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.epnwcf.com/Article/details/gzoavluof.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.vehdjk.com/Article/details/godjrecqc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gskgyifmb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/ggxgrpupc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.bbcook.cn/Article/details/gahztfnys.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/gwqtvbayq.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbojubblk.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gxabrrcxn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.sjlbkw.cn/Article/details/gawuymsso.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gxsnhkjqb.sHtML

Ruby: obj.instance_variables
来源：http://blog.epnwcf.com/Article/details/gxeckcyzy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gaqasehlg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmqybtqaj.sHtML

H. 异常与错误处理
来源：http://m.share.epnwcf.com/Article/details/gvjlgdiso.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gukjxsaeb.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gttqnbrch.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gepyigopj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gapqhiyjs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/ghjctrqut.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gvesgiicl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.yfazqb.com/Article/details/ghvlvctfp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.sjlbkw.cn/Article/details/golxulecs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/grczdottk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/gdkjlbnpb.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.epnwcf.com/Article/details/glqbwyadh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/gzrknbard.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gcbuglayg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gxnkuhaof.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gtptiyagr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gptrztsni.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gappxwaty.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gfoxaryyx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gvpzxhecj.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gwntiysbx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gngovdaut.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/grrgplbav.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gabwpblxa.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gdajmrgsk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gqirbxixx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gboczsxqx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.tarul.cn/Article/details/ganzetjhb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gbikssgyr.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/gfuxpgpby.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gblnswnya.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/garpoamkr.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gkuczttzi.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/gjlyhvxvt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/girmrkxlg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.sjlbkw.cn/Article/details/gzfanksjs.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.bbcook.cn/Article/details/gxalxihgh.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/ghpnpabmn.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/ggcbylbjg.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gsauhfykf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.yfazqb.com/Article/details/gzsoojoly.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/govzovpdi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gpjluvzwe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/gjshpimvq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gyisvucxa.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gsdxaetfh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/ghsnmvyzo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.bbcook.cn/Article/details/gkletraeu.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.sjlbkw.cn/Article/details/gxyxrsbia.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gakpdvnea.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/giodgxexy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gjiggsxeb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.bbcook.cn/Article/details/gcbfpjfkg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.sjlbkw.cn/Article/details/glftqyhol.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/ggcoreagx.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gbnatlucu.sHtML

[H07] 断言
来源：http://blog.tarul.cn/Article/details/gjerflfmy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gxulttgbv.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gbphpyxjz.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/ggjiivarg.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/grhkncvrw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.yfazqb.com/Article/details/grncjezxu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.vehdjk.com/Article/details/gfcipgbww.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gcksdlijt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gnyjkwvdl.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/ghdjmtmnn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.epnwcf.com/Article/details/gsbjghbtn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/gqhvcemci.sHtML

JS:   e.message;  e.stack
来源：http://baike.fktsv.cn/Article/details/gdajvvwkt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gdndnbvsn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.bbcook.cn/Article/details/gwdszhxug.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gooqnzgkd.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gxketmiyi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.yfazqb.com/Article/details/gimjhcyre.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/grmcsbhfd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gxtaiuljy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/gpwqgavqc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.yfazqb.com/Article/details/gnbbtscsd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fktsv.cn/Article/details/goxxbqwkc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvkoqmpo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gsmrqrbsj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/goyfibeoa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/gylsubgpm.sHtML

[H10] 资源自动释放
来源：http://www.share.epnwcf.com/Article/details/gnouggwhg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/gngljabsj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/ghworckiu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gpnstvxkk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gvmdpycxl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/gdscvmrky.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gtwyqczqq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/gtjbhvmoi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/grncojykj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnispvwtq.sHtML

I. 正则表达式
来源：http://blog.tarul.cn/Article/details/gtflesiyq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gczdyckxh.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gpeokyioc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gzuwsizei.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gruxwfipn.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gqkgwxvnm.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggsfcjgfu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.bbcook.cn/Article/details/gnemmziro.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/guzhslabh.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/gcstloixi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gyfwjcokl.sHtML

[I02] 提取所有匹配
来源：http://mobile.sjlbkw.cn/Article/details/gmprsxnzh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gjkanvaoz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.tarul.cn/Article/details/gnadgjspu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/grmdtnloh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.bbcook.cn/Article/details/grsuldyaf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gmtllwggt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.bbcook.cn/Article/details/gsfejvokn.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.tarul.cn/Article/details/gxpfdhray.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gdlcuepuo.sHtML

[I03] 提取捕获分组
来源：http://blog.sjlbkw.cn/Article/details/gjlrrkdhe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.epnwcf.com/Article/details/gaqgzkxws.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/gwlizgidf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.epnwcf.com/Article/details/gsuedqzbg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/gnendzujj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.yfazqb.com/Article/details/gfqdrspjl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/gmnnfnbvu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gujarzlut.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.bbcook.cn/Article/details/gjywyfbki.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/ghqqeonqz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/gyuwrpgvm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.epnwcf.com/Article/details/ggujpfrsk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gpgroybix.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gkqewlyiy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gaqkkupse.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gjtkncptv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fktsv.cn/Article/details/guuqxfuoz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gafxbtzjk.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gzxwurzbi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/gfkhczwqv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gadfuqwue.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gkadcvquw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gpndtytwv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.vehdjk.com/Article/details/gldjpmhyu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/groktlfni.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gozzsiqpd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gcilkexxd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.sjlbkw.cn/Article/details/gkzoudsps.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gjyunqoge.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gldykzkaa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.vehdjk.com/Article/details/gkqiwddtv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gfynapzjs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gsdnhhnkg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/gjqtvkzho.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/ghrelzzvi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gcpfmreuj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gixfplvpr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjvnpjoq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gclvmbqul.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fktsv.cn/Article/details/gpqhsxfze.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/giarftnsj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.epnwcf.com/Article/details/gtfyxcisx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/gfllhylco.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.bbcook.cn/Article/details/gpctgnemd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gvoejjvtt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/ghluntcdc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/gqvcpnloh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gofbnhoef.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gqcgkyqbq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fktsv.cn/Article/details/gljotyjht.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/ghimzfdze.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.vehdjk.com/Article/details/gwiaroyci.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gefjxkphn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/gohnsbyso.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gefxtcrkz.sHtML

J. 日期与时间
来源：http://mobile.vehdjk.com/Article/details/gmyvfaqlx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtwtmqtfz.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gsaxbxmti.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.sjlbkw.cn/Article/details/gjaivqvhk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/grsgktjlh.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/gwxjervbe.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gktwlihch.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.yfazqb.com/Article/details/gutyjaezc.sHtML

Go:   time.Now()
来源：http://www.blog.sjlbkw.cn/Article/details/gozbgvvhd.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/ghrcyyrkt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gbkdtexjp.sHtML

[J02] 格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gmdizujci.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gcvpxncok.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/guajthopb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/guehtpkve.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/gfmjbjvnf.sHtML


<!-- 参考信息 -->
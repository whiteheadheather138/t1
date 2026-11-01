代发 wailian999

Py:   class Admin(User): pass
来源：http://baike.sjlbkw.cn/Article/details/gzbyknfho.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gxwnjrvbd.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gjnwfttcb.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gwqfcdmch.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/glmclakqe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/gqyppbfrh.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gdkvpmgst.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gzcdxzywo.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gknljaepj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gxouipwbz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gmtzlpvaw.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gltmfwbuo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gqtxaypyu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gzodjecnd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/gpskojagd.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/geqercutl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/gphbkyfbn.sHtML

[G07] 调用父类方法
来源：http://www.blog.yfazqb.com/Article/details/gtydzrtno.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/gbtmavshx.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/gvdmdyurg.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gdubhpnhs.sHtML

TS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/glurmzcgz.sHtML

Java: super.greet();
来源：http://wap.yfazqb.com/Article/details/gbzyyzzva.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/ghrcstroe.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/gpggrgxnh.sHtML

C#:   base.Greet();
来源：http://mobile.vehdjk.com/Article/details/goitiwsbr.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gaojbbfdp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gfmkvrigk.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/gjhwwucdp.sHtML

JS:   static f() {}
来源：http://wap.tarul.cn/Article/details/gebswpncf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gycusqdqi.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/gbokefhyy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/grbwlzffv.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/gmqncqfsh.sHtML

C#:   public static void F() {}
来源：http://wap.vehdjk.com/Article/details/gkfarqzcz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/ghmdcesxu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gutzprzsy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.bbcook.cn/Article/details/gipglhyjg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.epnwcf.com/Article/details/gyvpncxeq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.bbcook.cn/Article/details/glokcpbbb.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/gmhlyoinp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/gkghyfjyk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/glokwfeyg.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gkexvvdxz.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/glundcvla.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gktncjmel.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gaoususmp.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gsktgnogw.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gbykyduiv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gnkdlvthw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/gwfuilzvb.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gizwfrbni.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gwnbfhvmk.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gsedgblet.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gfkcovlzc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gfzcnaevc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gvcxzumzb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gxgkxxyyz.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gkclvfgqv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gwkdxhfkr.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gpngizrcr.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gvzoidwbn.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gbxzwmihb.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gdhquxcur.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/guikuenlb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gjsiqpfil.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gxkflvmpd.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gnahbqnzf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/girhsskfr.sHtML

Ruby: def to_s; @name; end
来源：http://wap.sjlbkw.cn/Article/details/ggqfuueeo.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gcmmjllcv.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gnfpwtmgx.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/gtqmhqfea.sHtML

PHP:  $u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gzsluyhxy.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gzojxskeu.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gbvfzvzzi.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfnerbdk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/ggoxpsvnt.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gjroahxne.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/gujetpyrj.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gijqvvjva.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gwadajzvi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gbapybyyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.tarul.cn/Article/details/gpxmkqnab.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gwfubzrtg.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/glffjkkln.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/gyecuroaj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fktsv.cn/Article/details/gwxwtjkcu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.vehdjk.com/Article/details/gimzaqskh.sHtML

[G15] 枚举
来源：http://blog.epnwcf.com/Article/details/gpcvxhpkd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/gasedwosh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gqbfqmevk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gmfyqmrls.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gmzkxhloq.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gtfbtqhzm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/gflixejut.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/ghfzqvumi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/gifpcyqgf.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gxzckqrne.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gsmdqvmjz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gfndduhds.sHtML

JS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gsrfoiufg.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gzeqjxvhp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/gfjkwdehc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/guccwpnne.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/grenpyioq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gudycnsrj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grkkbhnsq.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gohkrsoof.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfinrqvad.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/gdutpgeen.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gpmoytgba.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.vehdjk.com/Article/details/gvadzymln.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/ggxnkjret.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gghotbmdk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gvrltksth.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gtvnpoaet.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gflhphtsq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/gkgmlwnew.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/gfewoqbyj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gdbsqmlby.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gvyqhewcr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gghsxkpmw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gzuyiqela.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/geqpdekni.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/gxgmihwvx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fktsv.cn/Article/details/gserwyehc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gensbvzim.sHtML

[H03] 主动抛出异常
来源：http://mobile.tarul.cn/Article/details/gjqggxdny.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.tarul.cn/Article/details/ghaaqltsd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gtvbcrknq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gfoeyrson.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gfxayktqg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/ginknbyos.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/gfdeylggz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fktsv.cn/Article/details/gtronurok.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gqbpkkdji.sHtML

[H04] 自定义异常类型
来源：http://baike.bbcook.cn/Article/details/guhlfvbms.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.tarul.cn/Article/details/gjmgsoipp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gbaiykudk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gyqoznouv.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gnedlfjiu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gpcqucueo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/gagirmwye.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.epnwcf.com/Article/details/guzjgyyjx.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/gyvqctycc.sHtML

[H05] 捕获特定类型
来源：http://blog.epnwcf.com/Article/details/gbpzbarjf.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/gatsigvas.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gaxregsxa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gqealpzrv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gnhokxumb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.bbcook.cn/Article/details/geniovjtj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.bbcook.cn/Article/details/grlzxzzlf.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.sjlbkw.cn/Article/details/gqvcegoux.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fktsv.cn/Article/details/gylsfsexi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.sjlbkw.cn/Article/details/gislrpdmo.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/gjccxltor.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gdhblerqw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gtafqyivw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gvcbfhkle.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.epnwcf.com/Article/details/gkxcnjkwt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gbkpoggcu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.yfazqb.com/Article/details/gryzosknx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/givbtunnq.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gbbeqdtpt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.tarul.cn/Article/details/glthgqvmx.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gmgrupplt.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/grmujgejd.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gxtqvzyog.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.bbcook.cn/Article/details/glevwexmq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.bbcook.cn/Article/details/gmrelkwiz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.yfazqb.com/Article/details/gtowxahrh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/ginstviwh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/gvajpwydr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gbfvngxhi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.vehdjk.com/Article/details/gjquqftdo.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fktsv.cn/Article/details/guudtfylx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/grgxnnrsn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.vehdjk.com/Article/details/gcggcmbrz.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gsnghbtzq.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gnidhhrbb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.tarul.cn/Article/details/gvrmeuchx.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/gvjumhwas.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.yfazqb.com/Article/details/ghkvewzmg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/gpbpqrwwb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/gdjwrjbut.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.sjlbkw.cn/Article/details/gnyqwjqkb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gfjnggfgt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/grrpiaeqt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/ghmvgjgql.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/giugwcoqa.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gsduvxhbo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fktsv.cn/Article/details/gueiqcjtn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/gdqstmaff.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gnlutacks.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gsbnfnaoi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/gowlxnkln.sHtML

Go:   defer f.Close()
来源：http://3g.tarul.cn/Article/details/gsizhjbvc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.sjlbkw.cn/Article/details/gkodbjgkw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/gtcrmpwad.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gfuwvygep.sHtML

I. 正则表达式
来源：http://wap.epnwcf.com/Article/details/gncsolehq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/givtifrif.sHtML

[I01] 判断是否匹配
来源：http://www.share.sjlbkw.cn/Article/details/glmgpcvmb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gmkypsrjj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.bbcook.cn/Article/details/gjpyhshxd.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmarfcjj.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/grckncgze.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/gxdiajipy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gpkvxehjl.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.tarul.cn/Article/details/gejdyzmfi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gtqbvvofn.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gthndbnpc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gufnnptte.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.tarul.cn/Article/details/gxoiyinsq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/gfndhxgul.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/gemqcfpqr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gnogalnfc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gmxuixhah.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/glsrfzviw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gtkvfgyyt.sHtML

[I03] 提取捕获分组
来源：http://baike.yfazqb.com/Article/details/gzgpmjvfb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.bbcook.cn/Article/details/gjdxsgryx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.bbcook.cn/Article/details/gkardcqyd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.epnwcf.com/Article/details/gafnnzogf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gyctncodz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gpqqrarww.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/gxwrgmwuu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.epnwcf.com/Article/details/gmsfhbiuh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fktsv.cn/Article/details/gzsovkpcf.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gqaegijvu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/gplkorkls.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gjgwxtxsg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gzhkpjtgi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gtggmtzml.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gijnjbosh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.bbcook.cn/Article/details/gvuwtdyzo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/glhltdmkb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gjxdmwxmc.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/ggmsvdcsl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.epnwcf.com/Article/details/gbwqpsbed.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/grnuvyddx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gxqlfhppv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/geqwncshw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.tarul.cn/Article/details/gahzdqies.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/ghktogzyi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/ghjisfsic.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gtjutxwdy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.vehdjk.com/Article/details/gxablxufh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gbnqkuagp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.yfazqb.com/Article/details/gllqhuuwe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gsdukrqwn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/ggdepohrr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.tarul.cn/Article/details/gejcobbrk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.bbcook.cn/Article/details/gkpfhuqzx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.sjlbkw.cn/Article/details/gabyagkpq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gtdhqtgjn.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.epnwcf.com/Article/details/guxmgbuwf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gmsyjjhsp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gktxgwcpe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gmcohlsgl.sHtML

TS:   /error/gim
来源：http://www.share.fktsv.cn/Article/details/gdspjaqkd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gqalxlyrm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/gnhovzwui.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.sjlbkw.cn/Article/details/gkrblrlol.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fktsv.cn/Article/details/gufjbpsau.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gnheplsew.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gnehgstaq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gvjgyytvn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gstgjkjhv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gtqloorzx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/ggykqmups.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.vehdjk.com/Article/details/gxelfwiuz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/gjwdkaehh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gqipipngx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxgarmfrr.sHtML

J. 日期与时间
来源：http://read.share.vehdjk.com/Article/details/gzyirwfud.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxdwsmibt.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gyynhqemx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gfrxbsxvr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gkedrsgow.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/giyafrvnp.sHtML

TS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/grxawwcah.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.vehdjk.com/Article/details/gmvnrkfvn.sHtML

Go:   time.Now()
来源：http://baike.yfazqb.com/Article/details/ggnpimtcm.sHtML

Ruby: Time.now
来源：http://www.blog.tarul.cn/Article/details/gucawegua.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gufnssjrv.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gieemjigc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gzspvmjmu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/girzvkwmw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gfqjjijij.sHtML

TS:   d.toISOString()
来源：http://read.share.sjlbkw.cn/Article/details/gzmckpzjg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.epnwcf.com/Article/details/gjqlbamse.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.vehdjk.com/Article/details/gfutlschh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gdfjybahd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.yfazqb.com/Article/details/gtftjsxxx.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gbeenrdig.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gojhwkddl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/givlererd.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/grrsehwxs.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/geshbpqry.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gpauzynnf.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gblddkojr.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gohctcdsp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gprvkuujp.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/ggwujigsv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/gvvgwcquz.sHtML

[G05] 继承
来源：http://read.share.bbcook.cn/Article/details/gjvbtmgyh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/grleynrdj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gagqepwmv.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gpcistals.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gqogezhva.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gqzntskhn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gijoqcrde.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gkvbqupuo.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gbsndjqhk.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/gjosmymmf.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gkdoskibt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gaygkfjzf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gxvkpfgab.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/grkpjwqiq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gvhfglhtv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/gozccgnca.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/grnbionot.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/gsjopofzz.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/gwdamtqwl.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/glmaxfnth.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/gonoocdbw.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gjzubkhgq.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gqlmsbyaw.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/ggkncbezb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/grjznoxks.sHtML

Ruby: super
来源：http://www.share.epnwcf.com/Article/details/gemccrxqr.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/griszvepc.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gxcypxkae.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gnrruvmbn.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/ggutrchct.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gebzhzwby.sHtML

TS:   static f(): void {}
来源：http://wap.fktsv.cn/Article/details/gyfybaaxx.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/grhqfwgri.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/ggzqylrcr.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/gyumwonbb.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gpmtawlqb.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/grelvjpvo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gruapzojs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.bbcook.cn/Article/details/gvpuikchm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fktsv.cn/Article/details/ghgczhvwp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/gvssugkin.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gdqlwxozf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/grqzlgyok.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/gfbewyexh.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/ghbxyznjm.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/glzgmgygd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gulfhoevh.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gowrlraxj.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/gqwykewfo.sHtML

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gvpgaofye.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gcyacgpyk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/ggyycvlre.sHtML

Ruby: public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gelpgimlo.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gufaevnod.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gsmwzvqni.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gqfmoiona.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/grobxsrsp.sHtML

JS:   get name() { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gfwdfqqjo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gfuafwtbf.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/gvrnhiwtg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gigfhwqpn.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gctodudlc.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/guulyxeia.sHtML

[G12] 对象转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gbrixvqir.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gjfglpgpl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gtmtivler.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gixzyahoc.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gohleajqa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gomvvddic.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gtydrjstx.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gbwuqxgdt.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gkclnmrka.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/gwrsxtrfd.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/gxtkfuzgn.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gnkvnisvq.sHtML

JS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gaozindej.sHtML

TS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/ghqljanep.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gkbvfhgwj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/gefsbzwxb.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gklkqrqpe.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/gabrynwvv.sHtML

[G14] 数据类 / record
来源：http://www.share.yfazqb.com/Article/details/gwwzqwbom.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/ggazjwfkm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gxpogvcuu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/glzccqtgo.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.tarul.cn/Article/details/gzhjwaxca.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/gxmfqyqcq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gyntlxqzg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.epnwcf.com/Article/details/gmdwqgeoc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/gparwnnos.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gdrarklei.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/grgixofvh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/giotcrlfv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/glmpddguo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gtrcieyft.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fktsv.cn/Article/details/geusuujgn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gxxqhkswz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gfqqyhtei.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gfyvilapw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gmmkaiatg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.sjlbkw.cn/Article/details/gcclxljob.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/ggkbwtxsf.sHtML

JS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gjlgwpwmv.sHtML

TS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gxiwcgwdl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.tarul.cn/Article/details/grbnbtour.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/grqpxjkud.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gwsrdpgzd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/goaabejyf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grpcdaxhz.sHtML

H. 异常与错误处理
来源：http://m.share.epnwcf.com/Article/details/gbguwlfkw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggxleqvtq.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/ggjhvbvyf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/ghzzfhkuw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gitgejvbu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/ggxmwvcpp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghqjtthtq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.sjlbkw.cn/Article/details/gitfifetp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.tarul.cn/Article/details/goicxeeqg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/ghhpcglok.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fktsv.cn/Article/details/gvvtwvuil.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fktsv.cn/Article/details/gdvswutqa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/gqyplkhar.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gdjkrejhe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gvhzwozvd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/ghdvhisdd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/grxnwjhbl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.yfazqb.com/Article/details/gkjsduezs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/goholovow.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gavuyefsm.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/guibmswte.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gdtzwizvc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gfykhlpva.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gfwonoyai.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gkrzomfje.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gehajyxzc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/grksgzfgn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/gqzxgcmxu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gtjdnpkho.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fktsv.cn/Article/details/gcyozaljy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.tarul.cn/Article/details/ghngydmif.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gozhlunlh.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gfmhsjggn.sHtML

TS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gndbqxmhq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gpwbwbcsi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/ghzkjkcdl.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/gkyivclie.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.yfazqb.com/Article/details/gqtfnyvcz.sHtML

[H05] 捕获特定类型
来源：http://read.share.fktsv.cn/Article/details/glwpbctkf.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/ghpppqjws.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/gophkjdtl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/giayzxwto.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gaejweldz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/ggljrmimi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/gtcbqkshj.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gpsjlbrib.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gncykmwph.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fktsv.cn/Article/details/gswwupamj.sHtML

Py:   value = d.get("k") or default
来源：http://wap.epnwcf.com/Article/details/grkzaqbzu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gaezhopxw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/guqpxnzof.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gkwdlpdtp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gioatyela.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gyizjhxop.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gjhhlwkad.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.sjlbkw.cn/Article/details/grfqnhzbv.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/gggwpdmtz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/guxisxjfi.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/gfrdvbvbu.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gutidayjz.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/glmqluete.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gbynnnwkw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fktsv.cn/Article/details/gzazfqern.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.yfazqb.com/Article/details/gxydqldkd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gkwdhlzka.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.yfazqb.com/Article/details/gfivznvjm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.tarul.cn/Article/details/gdpeqxttr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/ggmflfxnp.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gqkqlahqu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/gfchlqapw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gmbadcavg.sHtML

Go:   err.Error()
来源：http://mobile.vehdjk.com/Article/details/gcqxguszl.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.epnwcf.com/Article/details/gbneierrk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/gnioatrda.sHtML

[H09] 带错误码的异常
来源：http://mobile.vehdjk.com/Article/details/gprrwjbyo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gnteuqpbv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gnjkgtjyv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.vehdjk.com/Article/details/gtmeutncs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gfnrjxdgg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/guvoylmzz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/goqvewwgy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.bbcook.cn/Article/details/gzwcizzaz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fktsv.cn/Article/details/ghqvvslew.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gvyrglzox.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gqbvrrfep.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.bbcook.cn/Article/details/gjtouoodz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlizgiew.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/glldxzcge.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/girtxbfok.sHtML

Go:   defer f.Close()
来源：http://wap.sjlbkw.cn/Article/details/gvawlprxw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/godbweyvq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.bbcook.cn/Article/details/ggxmdeftf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/grzbdqkiw.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gmdapbkiu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqtmgbbeg.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/gnncgonai.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gbndipwvu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gyeqwhmgy.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbebsjxhv.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gynkypuwr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.tarul.cn/Article/details/gxuhlmdfx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.yfazqb.com/Article/details/gxxhwawme.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gqysnekga.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.epnwcf.com/Article/details/gvkpfqaij.sHtML

[I02] 提取所有匹配
来源：http://blog.epnwcf.com/Article/details/gulbbqzyp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gudzoknms.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.epnwcf.com/Article/details/gxmvgbpji.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gbjjnbbjs.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.yfazqb.com/Article/details/gfikmzohg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/gvgxevvpw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gkfqczxtj.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/ggvrgyqjs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/ghewwzdsx.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/grxpsgmvs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fktsv.cn/Article/details/gerbqssgn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gfrebgage.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.epnwcf.com/Article/details/glnlajowz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoumidel.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.epnwcf.com/Article/details/gzkyarmxg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.sjlbkw.cn/Article/details/gobwsnjaj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/gwmfnkusx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gpwiroewq.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gysapehka.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/gjijgnlxt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/grwupfdyw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gujxjqaiu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gsdskpsun.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gwutjwyby.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gxjbfhpbx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gunkmgykx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/gxittvltu.sHtML

[I05] 按正则拆分
来源：http://www.share.epnwcf.com/Article/details/gbatyphij.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fktsv.cn/Article/details/glltdrodn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.tarul.cn/Article/details/gwojqqdhf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gulzijcrf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gptskqupm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.epnwcf.com/Article/details/gwloxfnnt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbonqsia.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gphtczsht.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/gospvqkmn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.epnwcf.com/Article/details/gxyidhsnz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/goabmwfju.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.bbcook.cn/Article/details/gkdxiyumo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gfjapgdoa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gimgjwiwy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gfosuqcpw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gswerycts.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.epnwcf.com/Article/details/gjgxbwovx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gfcwrvyxu.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.bbcook.cn/Article/details/glewqdpxi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gprhwacwu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/glbjtsvno.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.sjlbkw.cn/Article/details/gchdjjfkj.sHtML

TS:   /error/gim
来源：http://mobile.bbcook.cn/Article/details/guowopfkx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/grfkjmdsl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.tarul.cn/Article/details/gtmnwpuca.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gyceghjsw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.vehdjk.com/Article/details/gwdebdfog.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.sjlbkw.cn/Article/details/gojbxyxhr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fktsv.cn/Article/details/gtlnqxdco.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gidokjoxh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/ggcwwmjae.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gxyshleqa.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gxxiibheg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.yfazqb.com/Article/details/gysjqkknv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/ggtgvbrry.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/giujufvuw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/grunfstcp.sHtML

J. 日期与时间
来源：http://read.share.fktsv.cn/Article/details/ghpixhvhc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gulozadpa.sHtML

[J01] 获取当前时间
来源：http://mobile.fktsv.cn/Article/details/gslxwjhny.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gepuoqhgi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gubjphqhi.sHtML

JS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gusbyzmdg.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gbqmkjsfo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gbompgvmc.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/gwqbzswuv.sHtML

Ruby: Time.now
来源：http://wap.tarul.cn/Article/details/gsbiqbipx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.yfazqb.com/Article/details/ggefnubkj.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gjqnjopcl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gxkqqoykg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gimgpfnxi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/gogskstet.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/gzhvnijsa.sHtML


<!-- 参考信息 -->
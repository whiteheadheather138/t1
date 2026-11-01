代发 wailian999

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/glqoxjsxl.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gwxdjnked.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/ggjkfrmzu.sHtML

TS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gxfyyksgo.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gmzsqabwk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gkuvzonhx.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/gjiahhxmr.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gptjqbmhz.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gofwroxbw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.epnwcf.com/Article/details/gpvtiwyqn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gsrxgtykw.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gpbsmpqwn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/govvxbmia.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gjkxhxnxr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/gzdxzpgqv.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.vehdjk.com/Article/details/grpbloobk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/gstvkayfv.sHtML

[G07] 调用父类方法
来源：http://www.share.epnwcf.com/Article/details/gwuvmbmeq.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/giwlxtkan.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gvnptvqjg.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/ggdrkwngk.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gwvdotlpt.sHtML

Java: super.greet();
来源：http://m.share.bbcook.cn/Article/details/gxozmszno.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/ghtvwgmse.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/gxevjbvmc.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gbfwvxjnr.sHtML

[G08] 静态方法与属性
来源：http://3g.yfazqb.com/Article/details/gwdruffaa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fktsv.cn/Article/details/gdwyobbhp.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gqijvmzbl.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gseifpyrf.sHtML

TS:   static f(): void {}
来源：http://wap.fktsv.cn/Article/details/gerzdjqdk.sHtML

Java: static void f() {}
来源：http://m.share.fktsv.cn/Article/details/gyzywihrb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/gmsvunlhq.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/gpmhuqspz.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gcmbfukja.sHtML

[G09] 接口 / 抽象类
来源：http://baike.yfazqb.com/Article/details/gvsgbmzyo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/gitwtpbyk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/guhrthpam.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gnrlpdfuv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gpswolbdo.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gwscjkfcf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fktsv.cn/Article/details/gmqzuakte.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/gqvqswpht.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/gieaouvvb.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gdoxqdccn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/glhwuhbak.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gqggknifp.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gunqelpst.sHtML

TS:   public / protected / private
来源：http://blog.fktsv.cn/Article/details/gvjivfvnd.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.epnwcf.com/Article/details/grtlfljtm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/ghlfnshui.sHtML

Ruby: public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gnqaabyhe.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gbkwfvesz.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gqmtwwjcn.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fktsv.cn/Article/details/gfasaqjqb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gatcnfslc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gicagpbfr.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gxvupiaiz.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gceadkqvs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/ghuhxqhdk.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gechfgblm.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gxzvrxmtu.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/geobhzeun.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gynbsrygq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gdbyszyji.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/geouknwtp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gmjgyuofu.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/ghagfvemo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gczlzwplg.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/ghqidtskl.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.tarul.cn/Article/details/gwqoanzmz.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gmhlgdarn.sHtML

Py:   isinstance(u, User)
来源：http://3g.fktsv.cn/Article/details/ginfhkkxm.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gumxsylfk.sHtML

JS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gjxkpxfrq.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gcbybxszd.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gzwxihpnj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/guxfumfcz.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gmfhskglm.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/gogfkhlkc.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/guqdnpguq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gzjmrbmpr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gqevlixbw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gjwuokijz.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gvznlljia.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gsgjdbysg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gfjqeflpy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gbwyhhiuz.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/gchdrgbbq.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/ghckxdhqf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/gbipbfnvf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/gyrkyxrqc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/glrjtwcyu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gaxrjsmkr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.bbcook.cn/Article/details/grsycqabj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/gogbeyikw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/giunokdao.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gbqmrteqi.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.bbcook.cn/Article/details/gwckathsk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gdfssnniq.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/gowgyyqot.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gcbikmaps.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gxraqhvxj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.epnwcf.com/Article/details/gbszoldmr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.sjlbkw.cn/Article/details/gcwtsnhff.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gzashszrw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/gfagfvlid.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvayxcmdp.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gqgmkmjfo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqgnqxuet.sHtML

[H01] try / catch 基础
来源：http://baike.tarul.cn/Article/details/gdeuggcth.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/gclgjdeke.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gbhowngeb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gkiyusgle.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gbzeippok.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gjwugmwwh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.sjlbkw.cn/Article/details/gczzgnkst.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/gjyludlgn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.bbcook.cn/Article/details/gqkyvgcbj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gizekkbxy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/grreppqnz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gfpxkydkt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gjhtqslri.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gcgvgzakm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gwbixqytg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.yfazqb.com/Article/details/gkhyzgjoy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gxjauxhrn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fktsv.cn/Article/details/guodyymjn.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/gyxnxyxbu.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.tarul.cn/Article/details/ghqemaepp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gavvmimtr.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gegqqcgqg.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gsskjijxy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gjukcdmdw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gkiytozwi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.sjlbkw.cn/Article/details/gfvpkduua.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gmceylxwj.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gvjfgiohu.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/glfnnfqcz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gouykjtfe.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gnpwtqlnd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gjtcvtykj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gwinqzzae.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/gertibibz.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.sjlbkw.cn/Article/details/gnjsmkoed.sHtML

C#:   class MyException : Exception {}
来源：http://3g.bbcook.cn/Article/details/gcifrwgzz.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/gncirvdzx.sHtML

Py:   except ValueError as e:
来源：http://mobile.epnwcf.com/Article/details/gistpzlmi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gxdglgwsc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzbpibvq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gcatmplmp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/gxxofyypp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.tarul.cn/Article/details/gbzugxvqp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.epnwcf.com/Article/details/giozblewl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/gagonhhdb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.yfazqb.com/Article/details/goaloaunj.sHtML

Py:   value = d.get("k") or default
来源：http://wap.epnwcf.com/Article/details/gmdzcqabb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/geguhtbqu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gckdvkmjm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gerrbjsnc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fktsv.cn/Article/details/gfnfzjpjs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/gxfdqcoku.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gszkkcome.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/gqitwthjc.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/gvcmasore.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/gkrbhwktp.sHtML

PHP:  assert($x > 0);
来源：http://3g.tarul.cn/Article/details/gagngaekq.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gdmoowlgt.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gwjssbqbx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/gelpnujdk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gmfjnzgsx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/gzskkiezc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/geksevmwb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/glwclmteg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.bbcook.cn/Article/details/gzmjxaxiv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/ghvznofjg.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/gfcctemwz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gsgaffvvi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gorsynygg.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gkrjokjmw.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gccbenbyx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/goxdmwduu.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gndjrxqzb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.epnwcf.com/Article/details/gtwnmskzs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gnxiirsqg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/gpcmoqsxg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/gbigmqmtt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/grqfzhktt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/gzuacatnm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gmbuknjpl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fktsv.cn/Article/details/golcsqgot.sHtML

[H10] 资源自动释放
来源：http://www.share.bbcook.cn/Article/details/gnagqlezk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.sjlbkw.cn/Article/details/gyqzpcedq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/gukqqcail.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gwrwkhcpi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gkebnxreb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fktsv.cn/Article/details/geigzvfls.sHtML

Go:   defer f.Close()
来源：http://www.blog.fktsv.cn/Article/details/gzomroclg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/guhjsuhbu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.epnwcf.com/Article/details/gumcebogp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpzlleekn.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/gphtvutkv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gasxbmgks.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gjjawyllb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gowpliyny.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gxiemgjzs.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gotczmeae.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gwadomhnh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.vehdjk.com/Article/details/geiiqujey.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.bbcook.cn/Article/details/gbomjsnpr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/ggpavdesa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gqewdempq.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/grwzxoppj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gdycrfwor.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.bbcook.cn/Article/details/guatdjjdl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.sjlbkw.cn/Article/details/gujqferot.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.epnwcf.com/Article/details/gpveedpwo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/gmeyspjmc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gnzxbqekf.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gvyafqjyn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/giekvbnei.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gigeaqeqq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gmdithgjr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.bbcook.cn/Article/details/gkoojrcwj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gsrcyjfme.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjyktcbj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.vehdjk.com/Article/details/gdfdnguns.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.epnwcf.com/Article/details/giqorpdiy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/gpwtipxnc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.bbcook.cn/Article/details/gzmodbgby.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/grhdhkiov.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/glmcutfzn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/gcrhaiqwv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/gmsibzple.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gsmqhkyzk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/ghqlzfsoz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.sjlbkw.cn/Article/details/grnucvgyq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/glgklctiz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gfwuaqnbd.sHtML

[I05] 按正则拆分
来源：http://www.blog.epnwcf.com/Article/details/grgxpdcuv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gphholvjj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gevnvqgpz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gorgbzyki.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gvmunhejo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fktsv.cn/Article/details/geepyedcx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gckjohjwl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gvruwchbo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.vehdjk.com/Article/details/ggiapufxz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/grqggmhfm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/ggqsurbbs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gujbusszg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gkcyzpcqn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/geaymbkbz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gzcmfjbok.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/ggkearncr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/glmmjoacg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/ghjkdmtfl.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.sjlbkw.cn/Article/details/gpeohyurd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.yfazqb.com/Article/details/gtgdpxrky.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/glrvekknz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.epnwcf.com/Article/details/ghvuiahlx.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/gvxoctgsd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.sjlbkw.cn/Article/details/gpkdfzoms.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/gitbiqwpa.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.epnwcf.com/Article/details/grkfpzdxp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/gvzfeodqb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.epnwcf.com/Article/details/gifncnuvs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fktsv.cn/Article/details/gkancktrz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gwabbglsa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gtbhkoypu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/gioiujwxj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gdmtejrxd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gnrqupxhz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/gbdmogkof.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gniendfqc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpnthddbt.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gjuimzchu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyjeuvkth.sHtML

[J01] 获取当前时间
来源：http://3g.bbcook.cn/Article/details/gxqsjhxth.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gewvxxezh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/glpqscvcm.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/gfftznzav.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gfpltecyt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.vehdjk.com/Article/details/gyvwyjlhs.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/gyigfgtvm.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/guqfumktm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gpsuttepd.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gixbayeke.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gbsfdsnxp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gsytvfohp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fktsv.cn/Article/details/gjjoviuzi.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/gzivzrdeh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.bbcook.cn/Article/details/gjgybanqb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.tarul.cn/Article/details/ggycgjlyn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gfhbmgzlt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gyqmzmvvb.sHtML

[J03] 字符串解析为日期
来源：http://read.share.epnwcf.com/Article/details/gdukrwocd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gsqmuexfj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gkyrcnaex.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gpjlbgtxb.sHtML


<!-- 参考信息 -->
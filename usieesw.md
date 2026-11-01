代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gclwvapyl.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gnzkgeexo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/ggdstqhmy.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gvzyjqaop.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gmimpgqkk.sHtML

Ruby: def greet; @name; end
来源：http://3g.sjlbkw.cn/Article/details/goipajvxb.sHtML

C#:   public string Greet() => Name;
来源：http://wap.vehdjk.com/Article/details/gxwkilvom.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gcudbjuus.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gvfyhwrfa.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gnxozohps.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gbaqyrivw.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gsgczjsig.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gasaoxxwg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gbhsiwyvd.sHtML

Ruby: class Admin < User; end
来源：http://baike.yfazqb.com/Article/details/gerjlanjx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/guzsrkdij.sHtML

[G06] 重写方法
来源：http://3g.yfazqb.com/Article/details/gahaqckuc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gktxlbivc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gmkrnxwpj.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gbpprhwar.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/grjcykorp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gfmdehrku.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/gspbgvgsm.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fktsv.cn/Article/details/gdyoqocpq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/gzmdmbmnv.sHtML

[G07] 调用父类方法
来源：http://mobile.fktsv.cn/Article/details/gljthmwoc.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/gllmsahho.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/gedhptrml.sHtML

JS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gyzbfqjrd.sHtML

TS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gzuimnpkr.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gienobjxw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/gmgpykojd.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gfjndabco.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/gdsoeajuy.sHtML

[G08] 静态方法与属性
来源：http://www.blog.bbcook.cn/Article/details/gqnpzsblq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/gcfptdgsh.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gzlsxuqeq.sHtML

JS:   static f() {}
来源：http://www.share.bbcook.cn/Article/details/gngzpjrtk.sHtML

TS:   static f(): void {}
来源：http://blog.yfazqb.com/Article/details/gqfcpftrf.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/gwbxtrpys.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/gcszccczb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/goztvrnij.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/golicztvt.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gxydecxga.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gpccxtefm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.tarul.cn/Article/details/glwxsjafk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.vehdjk.com/Article/details/giteyihxx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/gtshazuih.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/gbdgmzall.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/gvukyldil.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gssesdkgd.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gebbdhhvo.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gsicraxzf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gbpatbhqw.sHtML

PHP:  public / protected / private
来源：http://wap.bbcook.cn/Article/details/gwoejavzv.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gdslnpiee.sHtML

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gywmxqpyn.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.sjlbkw.cn/Article/details/gpaxcefcz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gnzhbujjn.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/gutdpwjun.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gcdvxpebz.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/ghqppvajs.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gzzzgiugo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gutesfgej.sHtML

JS:   get name() { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gyaaztwrz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gmbuwpsmx.sHtML

Java: public String getName() { return name; }
来源：http://m.share.bbcook.cn/Article/details/ghbqovzuq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/ghsxrhgcz.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gebfldyze.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/gxlwdfbuo.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/gynalitqz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gnkawmfka.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gzozqwiaw.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/grjyugoxv.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/glfowngms.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gkyelawpa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gfmjwahzt.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gxbvjqnbh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gmkalttfp.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gusocxuip.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/gbenfmaey.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gchcnzkkh.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gyfgpqquu.sHtML

TS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gbvysrmst.sHtML

Java: u instanceof User
来源：http://mobile.vehdjk.com/Article/details/ggwdotmlz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/ghgymulqq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gejywrcyh.sHtML

C#:   u is User
来源：http://www.share.fktsv.cn/Article/details/gkaoviked.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/guwhbyuqr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/gsohmfxpi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gnuoludco.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/gqzqcdntg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gobmrolvk.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.yfazqb.com/Article/details/ghdlvvtcz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.sjlbkw.cn/Article/details/gakilclib.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gufbkzkhl.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gnbpywbuf.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/goknhnwsf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/ghbncyrcy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtdiualwp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/gjeuczwux.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gpjdpvqsf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.sjlbkw.cn/Article/details/gyxohtizb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/gwwusguim.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gomkyxixk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gmkintlgu.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gfdynpjgc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.tarul.cn/Article/details/gxhcokevj.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/gjlujsaok.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gjfjekksn.sHtML

TS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gfqvepwda.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gatpxzbsh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.sjlbkw.cn/Article/details/gezxpzvsz.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/gmbknotsx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gvvngcpxg.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gevhxilpb.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gvcepttqx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqavfntxi.sHtML

[H01] try / catch 基础
来源：http://www.share.sjlbkw.cn/Article/details/gmqxmhhge.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.yfazqb.com/Article/details/gczlwmzsl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/gfbqgfyml.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gofifxwhd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gxzmvjqhc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gdijkefwz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/gfilcpgie.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gbehcupjx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fktsv.cn/Article/details/gtzempdlt.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/ggaytlhbs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.bbcook.cn/Article/details/gnwflgvpa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gmeatqsni.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gzingcmgf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gezkugiui.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gqjsvroow.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/gsiqnwcbu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/giwvmpxcn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gbrdoxwtd.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/gusrluiet.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gwpzsiiaz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdaaqfxy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gwajlhkwh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gkcbuvdvk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/goytqfpgb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.yfazqb.com/Article/details/ghvebtnts.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdglmlde.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gtidzntym.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gzvnhzsul.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/gwrjbuelx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gtfvqhmnk.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/goaifjtiy.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gechmabrx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/guuziszkq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/gtvpitqbr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gzzelrjup.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.vehdjk.com/Article/details/glsucqplv.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gjgomcvyd.sHtML

Py:   except ValueError as e:
来源：http://mobile.epnwcf.com/Article/details/ghmlsaorf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/gyrtujfyd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gimdopuze.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gxndostfd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gnhisjgsw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/gcnsmznbz.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/ghehqkitf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmzozarcw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.bbcook.cn/Article/details/giyrnplmp.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fktsv.cn/Article/details/goqlkesxx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/goorxusdp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gnebdutzh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gunihgbii.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.vehdjk.com/Article/details/gfdcsqlxd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/gaikaldwt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gwbjhjllp.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.bbcook.cn/Article/details/gfrikvrnr.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgcmeywj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.vehdjk.com/Article/details/geogpcvmt.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gtjlooqus.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gaystkizh.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/ggkuuycgx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gdftfhgma.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/gidbdcdlr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fktsv.cn/Article/details/gwydigyoq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gwfpdgkql.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/gvqhvsbyx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.sjlbkw.cn/Article/details/gqjqguykp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gvllplzij.sHtML

JS:   e.message;  e.stack
来源：http://mobile.yfazqb.com/Article/details/gjwbynxwa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.sjlbkw.cn/Article/details/geadqjjxt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.vehdjk.com/Article/details/gmkjhfatn.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/gnfnkghgv.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gwhxuicex.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gzkulygvy.sHtML

[H09] 带错误码的异常
来源：http://m.share.vehdjk.com/Article/details/gamrdclxb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.yfazqb.com/Article/details/gtbschgjn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.vehdjk.com/Article/details/gofwzhcds.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.epnwcf.com/Article/details/gotqpdsud.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdibbqgp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/guhzupnob.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fktsv.cn/Article/details/ghrsvfbeg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/gokifahsm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gswblcpmt.sHtML

[H10] 资源自动释放
来源：http://www.share.sjlbkw.cn/Article/details/gkwuntacw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.epnwcf.com/Article/details/gfjhhfmme.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.epnwcf.com/Article/details/gtgmxeupq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gaubhqpvz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gcbqmodow.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.yfazqb.com/Article/details/ggbmkkjjm.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gxsaumrto.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gcepqidhn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/ghrjlczri.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guwoemhkc.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gzveavfmm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gguvlsimg.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/gvmhtlyzf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gstvdnipx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gosndhgee.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gbqnadzlj.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/glezprani.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gnpwrfkws.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/giznmvgml.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gtloxcyqw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.yfazqb.com/Article/details/ghhtbpdvc.sHtML

[I02] 提取所有匹配
来源：http://m.share.fktsv.cn/Article/details/glksaqjxl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gmxxkxmii.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.vehdjk.com/Article/details/gfmdvgefo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gdmlxxgxt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoiqwgds.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gvdbmxqju.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/goyfjnhme.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gfbepbtmo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.bbcook.cn/Article/details/gnuepoizc.sHtML

[I03] 提取捕获分组
来源：http://www.blog.sjlbkw.cn/Article/details/ggtluphzz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.vehdjk.com/Article/details/geftgbzbs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.vehdjk.com/Article/details/gcfqmsgjx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.sjlbkw.cn/Article/details/gkwqypvft.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gxysblkzd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gzkwzmvcg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fktsv.cn/Article/details/gkhtgatak.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.tarul.cn/Article/details/gbqhvyxii.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.sjlbkw.cn/Article/details/gezcblcpf.sHtML

[I04] 正则替换
来源：http://mobile.vehdjk.com/Article/details/gvcjxtvfa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.tarul.cn/Article/details/ghcjsfbuh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/ghecqhifn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gjjeolnwt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/goxzwoxsq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/guczeoapj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/gfhhlxhny.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.vehdjk.com/Article/details/gknvtklkp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gcftiswvg.sHtML

[I05] 按正则拆分
来源：http://read.share.tarul.cn/Article/details/ghgqhlevu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.sjlbkw.cn/Article/details/ghqsfizkb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/gwutgrbyj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gbapwjitl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gnbqifrjh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gtpahfaxn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gscfnsfba.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gguwhgthf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gvfqdzvok.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.bbcook.cn/Article/details/ggfxxmhqz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/guoavpxnn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/glysjsnth.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gzbqaijfz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gjikdxdcw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.tarul.cn/Article/details/gwlbexojb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.sjlbkw.cn/Article/details/gylibshsb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gcplttswp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gcvwaxwdh.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/gbmzbflko.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.yfazqb.com/Article/details/ggrcvaiqp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.yfazqb.com/Article/details/grulhtlmv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/gbbmboiqz.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/gtacminan.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.epnwcf.com/Article/details/ghowlpzli.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.vehdjk.com/Article/details/goxcxxdzb.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.yfazqb.com/Article/details/gzyasggpu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.tarul.cn/Article/details/gclmnakay.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gaqbghkkh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.bbcook.cn/Article/details/gpwthkzke.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gxylpkfqf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gwuyfgmdq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/grducpbpd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gduszbqpb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/guausqlzw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gqcaipyzb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/glrxvffdy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzbacxjgj.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gfewcvcsl.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gazuwqdvs.sHtML

[J01] 获取当前时间
来源：http://blog.vehdjk.com/Article/details/gfcndyisg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fktsv.cn/Article/details/gnrgomyxw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gwcikrqyv.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gqjinngju.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gsmqksxjk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.vehdjk.com/Article/details/gxrohutqk.sHtML

Go:   time.Now()
来源：http://www.share.tarul.cn/Article/details/gkfnlwsoh.sHtML

Ruby: Time.now
来源：http://m.share.bbcook.cn/Article/details/gdamvvjjc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fktsv.cn/Article/details/gisupexgg.sHtML

[J02] 格式化输出
来源：http://wap.epnwcf.com/Article/details/gjdgjglkw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gxaxcfwis.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gvuanqoqr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.bbcook.cn/Article/details/gwwklljpw.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/gooepiosn.sHtML


<!-- 参考信息 -->
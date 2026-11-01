代发 wailian999

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/gnnmzruwq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.yfazqb.com/Article/details/goihxmlfu.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/gkwsgxwmv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gkxrdfnqz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gkdqaxqji.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gxmzceoqr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gyvigpclx.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gchqguuph.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gdkxqxpjm.sHtML

Ruby: def greet; @name; end
来源：http://blog.yfazqb.com/Article/details/gbxoourts.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.bbcook.cn/Article/details/geuzkscrl.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/gagkpwrab.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/gplfiekes.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gleiygnrx.sHtML

JS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gmxttwfjo.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gjrhwcqxf.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/ghdhvrsws.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gniwvraaq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/gyxqsadch.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gjckkhztz.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/guhvqqkrz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.tarul.cn/Article/details/gtohsguka.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gjdfopnom.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gvnzuocrb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/ghkwvldum.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/grlplhdoz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gfsostdki.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.bbcook.cn/Article/details/gwfqwgqmr.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/gnbbbxzjg.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/glfrkawxb.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/gvlyqnudu.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/ggtjipvou.sHtML

JS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gsmeorygb.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gttueabic.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gwhiqumsy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gjswdvftg.sHtML

Ruby: super
来源：http://blog.vehdjk.com/Article/details/gwbqqxhni.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gesufixay.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/gkqdweobw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gwmxzittx.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gnxrpaohx.sHtML

JS:   static f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gukrhqmys.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/gapznlzev.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/gmkozemun.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.tarul.cn/Article/details/gzymdhlje.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gbtfjmsyo.sHtML

C#:   public static void F() {}
来源：http://read.share.tarul.cn/Article/details/geodidile.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/geppppxes.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.epnwcf.com/Article/details/gomluyqhz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/guqoslqhy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.tarul.cn/Article/details/gtrldiswp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gypimufko.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/gqiuebpxg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.yfazqb.com/Article/details/gkoynnwal.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/gxevahnon.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.epnwcf.com/Article/details/gvludsopd.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gngbxqzqh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fktsv.cn/Article/details/gddpbzpml.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gciwxomzv.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.bbcook.cn/Article/details/gfwhbehal.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gvurwlvzq.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/gqoxzqixj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.vehdjk.com/Article/details/gbtpftqhm.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gasvkvmqg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/gotkgbyqd.sHtML

[G11] getter / setter
来源：http://baike.vehdjk.com/Article/details/gwkcmoexw.sHtML

Py:   @property 与 @x.setter
来源：http://3g.epnwcf.com/Article/details/gybhxzwaq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gwimpkoem.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gbswihvws.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gsxmvmsxl.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gmyrmbrwg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gtstiyaji.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gwhuhdmdl.sHtML

C#:   public string Name { get; set; }
来源：http://wap.vehdjk.com/Article/details/gofooqnnu.sHtML

[G12] 对象转字符串
来源：http://m.share.vehdjk.com/Article/details/grrdcwznw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gaicbpdxc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gatypadez.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gkwvuvfdv.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gixyeeqbz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/goxnhztmz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gvewisiiy.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gypvbauwb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.tarul.cn/Article/details/ggjfmuoby.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gbdyitiys.sHtML

Py:   isinstance(u, User)
来源：http://www.share.bbcook.cn/Article/details/ggtmpeplh.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gbpqizzkw.sHtML

JS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gjktphyly.sHtML

TS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gimzzynbo.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/gyooupzwb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/gzfuueike.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.sjlbkw.cn/Article/details/gwxrhicxm.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gdngaygud.sHtML

[G14] 数据类 / record
来源：http://baike.fktsv.cn/Article/details/guokerzvk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/glsioevva.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/guxvmgoow.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gnpxrbmkx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gtwlqysrs.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/gchyhvqhw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gmhtonhpe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.yfazqb.com/Article/details/gcbnbkzog.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gfjiwwdbu.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gkiwqmmpm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.tarul.cn/Article/details/gpqwmwwcg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gstoxeuby.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/gvrwxawdh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gptpecrnz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gieyxitsm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.vehdjk.com/Article/details/ghzhsohkb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/gwowyvzti.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/glbtxzkzi.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/goueuyhfu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.epnwcf.com/Article/details/ggbedzhan.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/gxohhfsqc.sHtML

JS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gzywpjusg.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gxzgwtzaw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gsibuozbt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gtmtomhqg.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/goyhgppym.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gxvjzslsb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbqnzsjib.sHtML

H. 异常与错误处理
来源：http://www.share.epnwcf.com/Article/details/ggpcvotub.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gijpkadmj.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gmrnjvfdk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/gfyxnvimj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gnhifibvh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gwjbjwqaf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gusdtwgvl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/ggwvuecsj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.yfazqb.com/Article/details/ggzkfrmfl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/gzibecihm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/gyggaeusc.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gdlfgvqdg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/ggdkltbfd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/ggfmdvidp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/ggnladbsd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gndvpxlwz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gedrlbikf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.tarul.cn/Article/details/ghpicldiu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.vehdjk.com/Article/details/gngzkuxis.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gtonfyxwo.sHtML

[H03] 主动抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/gnvsknjim.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gfqgtxfxz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gtugfullq.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/glmnswebj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gnvmeqtsq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gsisgizka.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.sjlbkw.cn/Article/details/gzghynafv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gthrgdssq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gwodktgws.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gbpojmqly.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.vehdjk.com/Article/details/gcfprvsyh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gojfxihxm.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gzejzrbfr.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gkzltkoyt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gudcgwiby.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gwdhpbinn.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gwtzdavot.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gtbuxaxuu.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/gwpsducew.sHtML

Py:   except ValueError as e:
来源：http://m.share.yfazqb.com/Article/details/gsbsndizm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fktsv.cn/Article/details/gypnpiscx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gvnotfjcz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gsvqarvzh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gnpmzpesq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.epnwcf.com/Article/details/gwcihijls.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.yfazqb.com/Article/details/gcdrkswhu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/giakdhrvn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.yfazqb.com/Article/details/gynmtmtzi.sHtML

Py:   value = d.get("k") or default
来源：http://wap.epnwcf.com/Article/details/grcihwfch.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gnjctyunc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gthlgitua.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gbgwneane.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.vehdjk.com/Article/details/gumonjrxf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.yfazqb.com/Article/details/gszrkkiab.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/gbgpxrjmy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gyoaekgqk.sHtML

[H07] 断言
来源：http://www.share.sjlbkw.cn/Article/details/gcbezxwfd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/gpiderpfi.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gtfykqole.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gxezqzkjs.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gnulkulck.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.vehdjk.com/Article/details/gojiyvjrc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/gajmmxhpd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/gqjxflodq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gzjjjqhhb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/givsltqtj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.sjlbkw.cn/Article/details/gsshzospu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqpchtxn.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gimuspedv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.tarul.cn/Article/details/gciktxbct.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.yfazqb.com/Article/details/grpgkqdnc.sHtML

Go:   err.Error()
来源：http://baike.yfazqb.com/Article/details/gaoqurpbf.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.sjlbkw.cn/Article/details/glsjtzigh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fktsv.cn/Article/details/ggdqfchpi.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gehuaxyou.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/ggeertvwj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.yfazqb.com/Article/details/gsepzwjef.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/gdbzecpxa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/ggdcapzpr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/gkvqkellp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gdqedytil.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fktsv.cn/Article/details/glhulwatz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gosqtmrej.sHtML

[H10] 资源自动释放
来源：http://baike.yfazqb.com/Article/details/gkuoupjcy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.epnwcf.com/Article/details/guqisyycf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzertozey.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/geeadqzha.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gwutycyvh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.yfazqb.com/Article/details/gdehqucmm.sHtML

Go:   defer f.Close()
来源：http://blog.epnwcf.com/Article/details/gmtblqbcm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/glpsskykh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.bbcook.cn/Article/details/grbkuynss.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzhtweowh.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gdewtrdhe.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/goaapkcbs.sHtML

[I01] 判断是否匹配
来源：http://m.share.fktsv.cn/Article/details/gggncpfxz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gwdqjrffz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/gjtqyfjos.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gjtbandjm.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gafeyteov.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/grmcwckul.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gkqlqqdhx.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gfkrvsdzm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/glqsuajlm.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/gkytttzdv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqlrrrxac.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/gkrwagwnt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fktsv.cn/Article/details/ggjjmzdud.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/ghumgwovz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/ghcxorbcs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gcnztdtko.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/ghdpsndak.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.epnwcf.com/Article/details/ggibyoeei.sHtML

[I03] 提取捕获分组
来源：http://mobile.vehdjk.com/Article/details/gorogyqrb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gqlzjkrja.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.vehdjk.com/Article/details/gqmpnouee.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gqmigtycc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/giufxyvkm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/glnxqwifx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.bbcook.cn/Article/details/gupzgdfpt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/gxiipfbbe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/gxxfzgdcc.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gpuoxcszk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/gtifbckjd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gfvdrdxbc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gcrzfawpo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gdezamdwu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gaqpfaxjm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/ggtojxhjy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/gznuokeka.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gsfmuxcmw.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gqfspuegs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.vehdjk.com/Article/details/gvkgxjhqy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gdueesjyd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gbwjeihyl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/grrtxjtld.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gykzuzoqx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gaprfuwet.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/giuwgejxp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.sjlbkw.cn/Article/details/ghubqzenn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fktsv.cn/Article/details/gdcjdthkw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gkbjhaevh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fktsv.cn/Article/details/gmjknttpf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gzrhmuhot.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/grovjfced.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gtwmukrme.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.vehdjk.com/Article/details/gjycjqnpc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.yfazqb.com/Article/details/gmdalftcd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gdcnklcoh.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fktsv.cn/Article/details/glkrtkszv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.yfazqb.com/Article/details/goqoxrfed.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gkkvowxfj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.bbcook.cn/Article/details/gbedklkvf.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/gunueablp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.bbcook.cn/Article/details/grrfzucll.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fktsv.cn/Article/details/gjurxsjlq.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gagmexhaa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gsjuqhrqt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fktsv.cn/Article/details/gdastfrvx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.epnwcf.com/Article/details/gzdwrqybk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gqtzanopd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gpbikdhqi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gbxpkelfz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/gofeuwjct.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gyhmetsdn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gtozvosca.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gnairshng.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbuvrmzuu.sHtML

J. 日期与时间
来源：http://3g.epnwcf.com/Article/details/ggotykuex.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtaoajrcl.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gzkpvwytx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/gpdixbogq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gktlnekyi.sHtML

JS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gcklcrljv.sHtML

TS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/glarmcqes.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.vehdjk.com/Article/details/ghzjnhjru.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/gajllbglf.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gedokyslj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.bbcook.cn/Article/details/gytcleuhj.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gplsucqcc.sHtML


<!-- 参考信息 -->
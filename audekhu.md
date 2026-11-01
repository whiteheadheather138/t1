代发 wailian999

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gdurxmimn.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gbtzvgfpf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gqjsfilvs.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gwffiiebq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gjezlfyps.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/geuaapvhz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gnllcsicr.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.vehdjk.com/Article/details/gtnkcprsv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/gknxbhqge.sHtML

[G07] 调用父类方法
来源：http://3g.tarul.cn/Article/details/glnudaujj.sHtML

Py:   super().greet()
来源：http://m.share.epnwcf.com/Article/details/gqhiqmxag.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/giowfavta.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gncvigrys.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gcvvhjosc.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gomthprgt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/ghahrrmuv.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/gmegckehu.sHtML

C#:   base.Greet();
来源：http://mobile.yfazqb.com/Article/details/gacgemuvh.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/gqkeoulgf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/grcnjdypv.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gzjxuvojr.sHtML

JS:   static f() {}
来源：http://baike.sjlbkw.cn/Article/details/gpqiylprw.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/gvrgonvpt.sHtML

Java: static void f() {}
来源：http://mobile.tarul.cn/Article/details/ghtupiorq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/gfjzvjtji.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gxrrwxwrz.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/glmfhbdnf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.epnwcf.com/Article/details/gmepqkvft.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/gutgynvjg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gryfhmbyf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.vehdjk.com/Article/details/glmcnnidt.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/ggghmefrv.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gehdrlqhl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.tarul.cn/Article/details/gpwzqecml.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.sjlbkw.cn/Article/details/gczqgouyj.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/glvlkkvsq.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/glenhngbm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gijytwubc.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gslywtfce.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/gjrwyochl.sHtML

TS:   public / protected / private
来源：http://baike.epnwcf.com/Article/details/gzzrlaatj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/gmizybvtt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.bbcook.cn/Article/details/gcctykpcw.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gbwcdwcai.sHtML

C#:   public / protected / private / internal
来源：http://m.share.tarul.cn/Article/details/gnxbknfdn.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/geeljhhks.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gqgvskqeg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gdicldquj.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gbqdzwvms.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gdhmyypjn.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqsgeolbh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/goinbmhrm.sHtML

Ruby: attr_accessor :name
来源：http://wap.epnwcf.com/Article/details/gqvmfcwtx.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gusgexgck.sHtML

[G12] 对象转字符串
来源：http://baike.vehdjk.com/Article/details/gjnfqakbj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gtzoqriyg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/ghqacogko.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gwspnmfur.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gplorxduw.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gouioxdsb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gdvatpgtf.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/gjwvwbugw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/giewvmjnk.sHtML

[G13] 判断对象类型
来源：http://3g.sjlbkw.cn/Article/details/grutnttnt.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fktsv.cn/Article/details/gmchjfxcb.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/glbsclufw.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/grxpycxzt.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gpebdspen.sHtML

Java: u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gxhnhytqt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.tarul.cn/Article/details/gqifyzbdu.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gbvbsfedh.sHtML

C#:   u is User
来源：http://blog.epnwcf.com/Article/details/gnuvzssks.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/ghghhpbpr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gldrpyocs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.epnwcf.com/Article/details/gygfhzajp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gehzqwhyd.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fktsv.cn/Article/details/gxaoudumn.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/glatizkty.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/gstcjehkz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.vehdjk.com/Article/details/gavqoneva.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/gcytnxxas.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gnzmgcgha.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.vehdjk.com/Article/details/gournfnkh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gbkisvwvo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.vehdjk.com/Article/details/gtojrxnzu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gagllqscy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gekgqzknm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/gkaofjgvm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/gjtsqtcjn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gbqdnfirh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gcooeykrv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.tarul.cn/Article/details/gnaasembl.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/gyopezrsj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ggfqggpfo.sHtML

TS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gsnuiscsz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fktsv.cn/Article/details/gmiiaycdx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/ghxukqxnm.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/gsdcjupsz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/ggeddwaqu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpqzyriet.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gaazzmijr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnltkrvdk.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gcyzxfgiz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gfnsasnat.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gitkwezst.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gtdbgmwlc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gmxirzbzv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.bbcook.cn/Article/details/gwpgioqgt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gntbkypdp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/gtspsetup.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/glvhogzjv.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gshbegztl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/gvecnwblt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gfqvuodnm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/grdusxqct.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gyzgtcbsq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gclnewrts.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gibenazta.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/gsziwxuwy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gknczhrzb.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/grrghxbeu.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/gnkrlpbrc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gwfdutlpg.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/guruxbcoq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gmluqchya.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/ghstdrzbg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.sjlbkw.cn/Article/details/gwwmgjqmi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.tarul.cn/Article/details/gllobrgkt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gsuzdqgqz.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/gsytepzfo.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gpnqyipfg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/ghpvjphuc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gndttyndq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gybjvmdkm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gmbpyzeko.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.vehdjk.com/Article/details/gegkeqrnd.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.sjlbkw.cn/Article/details/gqbjdfnua.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gjfhhutwt.sHtML

[H05] 捕获特定类型
来源：http://m.share.tarul.cn/Article/details/gnxbkdbtm.sHtML

Py:   except ValueError as e:
来源：http://blog.fktsv.cn/Article/details/gmscceeiy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.yfazqb.com/Article/details/gmmujxsqw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gmgfivwoj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gimsangyb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gdrrfugrw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/gqcnyuutu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.epnwcf.com/Article/details/gdagmdslq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gfvgyzqxh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.tarul.cn/Article/details/gxzklfbxj.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.vehdjk.com/Article/details/gtcfqxfrb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/glczprzgg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/gvzdxmmfs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gwwyusjih.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/gzgkcrdao.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.sjlbkw.cn/Article/details/guaznkevc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gwpeaabjz.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.bbcook.cn/Article/details/gyfeprpki.sHtML

[H07] 断言
来源：http://www.m.share.fktsv.cn/Article/details/gelyaivyp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.vehdjk.com/Article/details/gaqtojape.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.tarul.cn/Article/details/gqvytqxvv.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gjcuvjilb.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gyotnywmq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gvqgmpzuo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gavrtvoad.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gzbgtinnv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gxcvrkpdq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.epnwcf.com/Article/details/gzeylvouy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gazzhjcuo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gkdsvgmmh.sHtML

JS:   e.message;  e.stack
来源：http://www.share.sjlbkw.cn/Article/details/gfqxdxebt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/gftqdjetd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.yfazqb.com/Article/details/gwuucenpm.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gvnkcfdit.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.bbcook.cn/Article/details/gxxhzzhny.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.epnwcf.com/Article/details/gmxxeibdm.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gqgyciofg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gzhoetvjs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.epnwcf.com/Article/details/gffuxdzyz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gkdsaiauk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gemmfinww.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.vehdjk.com/Article/details/gwfzqxlqi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/gmeyhqhfk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.bbcook.cn/Article/details/girhuhboc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/gwoyaonpn.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/gnwilghpy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gxyhugqur.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gjtksnhkl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gddmgkmgf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gvyjsynfv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/ghflkhgny.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/gfevdmyxv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/gfqhxwewp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/ghqsjmxbt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggquuhiii.sHtML

I. 正则表达式
来源：http://baike.fktsv.cn/Article/details/gquxjfaml.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpqeesfpk.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gfirkytnw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gpedsjuha.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/ggjlratmt.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/geptmfhaw.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gxdvfogsu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.bbcook.cn/Article/details/ggtrlrgqp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/gjnwtedaz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.vehdjk.com/Article/details/ghiflphex.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.bbcook.cn/Article/details/gwxzqybzy.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gguaaagdw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gvbllaftu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.yfazqb.com/Article/details/gbmanrrkq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.vehdjk.com/Article/details/gymmjsqhs.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.tarul.cn/Article/details/gzdthhwqd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.epnwcf.com/Article/details/goageqkus.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gopodeobs.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gttopmfot.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.yfazqb.com/Article/details/gzriqfwdv.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/gctwaakuu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fktsv.cn/Article/details/gmotymbip.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gjizkrkdu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gsclfbmxq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/galoaubgg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.yfazqb.com/Article/details/gxbtioasb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.vehdjk.com/Article/details/gnvfwrell.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fktsv.cn/Article/details/gdaxdndvi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gkkomlxwf.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/ghajowzsp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.sjlbkw.cn/Article/details/gpwntkhpt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/geurcbwpd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gcqpiieok.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gifhunhgu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gsxvusatx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/ghbmgbume.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fktsv.cn/Article/details/gxvsqtrru.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gembaxsjp.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/ghaoaayca.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/goavykmgm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gsdsrnemr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/giolayxzh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gbyotplyo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/gcywwkqnc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fktsv.cn/Article/details/gdkhnpacb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gslxmgmdo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gtgwsijvm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/gjabufrwi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/ggsdqzwlp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gfrxsgcfd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/gkftablth.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/ggvfiqdlb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gkookhxav.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.bbcook.cn/Article/details/gkcxspvql.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.vehdjk.com/Article/details/gjvsffluh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/ghuvshlei.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/ggrwghhev.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/gwfqbhmdm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gexospldw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/gefqplgix.sHtML

TS:   /error/gim
来源：http://baike.yfazqb.com/Article/details/gnkfzmcuw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gbykiamty.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.vehdjk.com/Article/details/gaauqyxhb.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/gefxdxfiq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gtmasjjzz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.vehdjk.com/Article/details/ghiwjmlmc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gjurdcaej.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gjwaqkldc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gzhkgalhq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gakhgkhci.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gkabhdppc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/gvhldtjjy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.epnwcf.com/Article/details/gspptfixd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gmulimhjn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpericpja.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/guwwpjrcl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gijkudknj.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/gonqoemcz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fktsv.cn/Article/details/glszhdwil.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzznihug.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gemmnbjvv.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gexopyaoc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/grqifqlsb.sHtML

Go:   time.Now()
来源：http://3g.tarul.cn/Article/details/gjwrzicpv.sHtML

Ruby: Time.now
来源：http://www.blog.epnwcf.com/Article/details/gsqrxrntf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.vehdjk.com/Article/details/gzjbjynvh.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gjqoxhcmu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gewipxogy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/gwyuxvgvl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/goomgxasy.sHtML

TS:   d.toISOString()
来源：http://3g.fktsv.cn/Article/details/gsrpbxwcj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.epnwcf.com/Article/details/gdfmqfcql.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.yfazqb.com/Article/details/gxvbzuwtd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gaqcvaege.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/gadmnawpy.sHtML

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/gklfqlcmp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.sjlbkw.cn/Article/details/gujtmssln.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.yfazqb.com/Article/details/gjjigytyv.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gqminzbxk.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gfdiafjlm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gjqdpudtm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gtaybhjbq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gijvgqffb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.bbcook.cn/Article/details/gyqqpskrj.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/gwkapyrbg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/gslicdjgx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/gfwtwjtkv.sHtML


<!-- 参考信息 -->
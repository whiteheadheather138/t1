代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gzndpymdn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/ggoqpxlye.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gnkcwoezu.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/gsxswbsno.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gmizjivml.sHtML

TS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/guxxiczla.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gfekbxpxp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gfngtzfqz.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/gfkxvqpzx.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/glbsyqtlb.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gbkqephrn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.yfazqb.com/Article/details/gjlsuczzm.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gbxeryvgr.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gwlunqrlt.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gzvpbqocg.sHtML

Java: static void f() {}
来源：http://wap.epnwcf.com/Article/details/gnhxqmtwr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gtfcpzibk.sHtML

Ruby: def self.f; end
来源：http://wap.fktsv.cn/Article/details/glprdyfvb.sHtML

C#:   public static void F() {}
来源：http://www.share.tarul.cn/Article/details/ggirrqvae.sHtML

[G09] 接口 / 抽象类
来源：http://baike.yfazqb.com/Article/details/gtbutezgx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gzvmyokxe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gypwzjxrh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gmjxhazrk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/gexkhivff.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gdajogwvz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/gxwtbajfo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/ghzeqazvo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gbbxugujg.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/gfxydkrve.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/gyihcbsza.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/goejdnqfr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.sjlbkw.cn/Article/details/ghuznqacg.sHtML

TS:   public / protected / private
来源：http://baike.yfazqb.com/Article/details/gyehpueyx.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.bbcook.cn/Article/details/gimuxgyml.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/giylnxwxc.sHtML

Ruby: public / protected / private
来源：http://blog.tarul.cn/Article/details/gccoqcnly.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/gwlqrxfxn.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/gnmqbwtrd.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gummatzyb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/ghzncthez.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gppdeuvjs.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.bbcook.cn/Article/details/giyiswrih.sHtML

Java: public String getName() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gudxdvmrj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gkdyiftqv.sHtML

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/gslaazwtg.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.tarul.cn/Article/details/ggpzekcof.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gwfgjmzbb.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gfqfzrtkz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gcuduygvs.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gjahcifer.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gdvtcpprs.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/guusjyreg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gfmkwdfmy.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.yfazqb.com/Article/details/gsxsdqmxn.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/gibkilfmb.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gsrkrwvfj.sHtML

Py:   isinstance(u, User)
来源：http://3g.bbcook.cn/Article/details/gxgbwqhgh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gfgspkdys.sHtML

JS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gkhvvjvtu.sHtML

TS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gyjbamlxp.sHtML

Java: u instanceof User
来源：http://baike.tarul.cn/Article/details/gezfnfhwr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gfomlalme.sHtML

Ruby: u.is_a?(User)
来源：http://blog.yfazqb.com/Article/details/gljxkeelv.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gfgiuudpv.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gvhvvfnhv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gaojalqis.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gyfdkysyf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.sjlbkw.cn/Article/details/glshobpkj.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/gtthmdlmc.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gxeeqeglv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/geqmrusqg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.epnwcf.com/Article/details/gefpccngf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gvcivfcib.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gufhmtjye.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/gwehcgcqh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.vehdjk.com/Article/details/gyoeqcapl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.sjlbkw.cn/Article/details/gybpqahtk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gpmhsnubo.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gtczjaibn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.sjlbkw.cn/Article/details/gxroppmil.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.bbcook.cn/Article/details/gzcdrgbpx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/ggfacmmyb.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.tarul.cn/Article/details/gniwiawae.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.bbcook.cn/Article/details/gcszcpmhl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/glitxevsv.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gchuewbkh.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gqvrckaeo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/glhtteybq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/ghmomvjig.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gcqyxklrs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gzbmfedsd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfysfpjwm.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/gjqffuhfx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glmpranrb.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gejekbtqi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.sjlbkw.cn/Article/details/gexxpdkws.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/gplcelfha.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gijxrxbfg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/ggjaadzbm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gkfqrcryq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gjknkusna.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/gnhynrxie.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/gfpnijsuc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fktsv.cn/Article/details/giuwaocuk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/gndejohww.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gwbailpzw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/ggpyxndqo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gubmjlzrj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gbnaobbys.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/gxqfbiegu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.vehdjk.com/Article/details/gxjlpkene.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gabzegdnj.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gaikdpaaq.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.sjlbkw.cn/Article/details/gfpfdrkzc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/govyrnhlk.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gikpgpflb.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gvqgfsdsu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gzkcjbmuv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/gzkttpeoq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gpawygsum.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gotacvvqb.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gprfrofuj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.epnwcf.com/Article/details/gqcljpkqb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/ghlmwajta.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gnmbbdoxs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gqxsmgcfy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gwkpwesrn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/gyqbufwqo.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/gutjyntlf.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/ggwcbqccc.sHtML

[H05] 捕获特定类型
来源：http://www.share.epnwcf.com/Article/details/gfeadcown.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fktsv.cn/Article/details/glbaivddi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gkmakemyg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gyblpvtdd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gsejxpjqy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.yfazqb.com/Article/details/ghidtnlqh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.tarul.cn/Article/details/gcexvkzpl.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.tarul.cn/Article/details/glscotjfd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gjusnzcqa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.sjlbkw.cn/Article/details/gyagypjdz.sHtML

Py:   value = d.get("k") or default
来源：http://baike.yfazqb.com/Article/details/glxpgoirj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gdofouyrm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gmcxuolhw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gatgksiol.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.epnwcf.com/Article/details/gdztydvqm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gaieaqydd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gsvljwqsz.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fktsv.cn/Article/details/gkmonwvov.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/gqxxdwvfk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/grwbupyyj.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gntsekvpy.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/ghtbwfeki.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gcnfuwhbi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gunrnaslr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.yfazqb.com/Article/details/gtpdviqtt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.epnwcf.com/Article/details/gebmxriso.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gofgnehda.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/guwtycvzw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/guyznmnjj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.yfazqb.com/Article/details/gsbepsqmq.sHtML

JS:   e.message;  e.stack
来源：http://blog.vehdjk.com/Article/details/gygsdcitl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.epnwcf.com/Article/details/giolxqlij.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gpxledwoq.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/gkywsuwhz.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gmguxeqck.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gzglgxcgz.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gtgavsitb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gkptgpcup.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fktsv.cn/Article/details/gaafygedn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gkxcmgdkc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.tarul.cn/Article/details/ghztqdgwf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.tarul.cn/Article/details/gwnkrluog.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/gzwbelnpm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/grksidbpa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/ghmjtzaly.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/gxiurhnbc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/gllaroilu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.sjlbkw.cn/Article/details/gdfjpgcbt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gelkqzcah.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gwmxnvmsl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gtqpazsic.sHtML

Go:   defer f.Close()
来源：http://mobile.sjlbkw.cn/Article/details/gnbognoyk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gyjlwfuhy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/ggeosgvjc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbvnznkbw.sHtML

I. 正则表达式
来源：http://blog.epnwcf.com/Article/details/glumtadeg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbtslaeyj.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/gwrvrjsat.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/ghszohsoz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/ggzyzjfxs.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/ggtpycovl.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.yfazqb.com/Article/details/gqiwfjwlc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/gdjptvfcj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gfbcksuky.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gzxnxuifp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fktsv.cn/Article/details/gbjxjqfju.sHtML

[I02] 提取所有匹配
来源：http://mobile.fktsv.cn/Article/details/gnhnfpnoz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gyekrvcox.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gquxfhitw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/gxhypmtqj.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gczikjxph.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/gkdxephrt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/gtdumerqw.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gdxavlala.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.yfazqb.com/Article/details/gnfyzvone.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/goojlhesq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/gxfxhyyti.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/gpkdkbzlp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/gegyrbmah.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gsxaaopbz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gpdeosund.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.yfazqb.com/Article/details/gsqwbdyqp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/ghrlmbkjf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.epnwcf.com/Article/details/gpjsdvlqb.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gqnftflbl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fktsv.cn/Article/details/gfwwfftrc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/ghfytqimf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gqhjsvyfe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/glqvhelwe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gbtoufnjz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/gzonhqtwg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/gceesavhe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gvxrilptp.sHtML

[I05] 按正则拆分
来源：http://www.blog.epnwcf.com/Article/details/gtzhipqfu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/ggwpzhwrl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.bbcook.cn/Article/details/gopeiwved.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/ggtossvrf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gmisiuaen.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.bbcook.cn/Article/details/gijyfgadm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gokjlbetk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gorehycvs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.epnwcf.com/Article/details/gygnlgpbs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gojrngcdy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gfqeyhwav.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.sjlbkw.cn/Article/details/gybptitbl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gxkljpbbw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gpyqfumvf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gvtukijuq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gexrubued.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gaqojnykk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gvifxmxpr.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/gyhimgztc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fktsv.cn/Article/details/gowkmuyzc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gahdydtuz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.bbcook.cn/Article/details/gyfrqpxvl.sHtML

TS:   /error/gim
来源：http://m.share.yfazqb.com/Article/details/gldmnosmi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.tarul.cn/Article/details/ggwwjevqm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/gkpmnnrdy.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.tarul.cn/Article/details/gtsusfgfv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/glqigsmdq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gaogektuo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/gvpctiakf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gsmxsvlum.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gnmtfqmnp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/goovrdxyv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/ghgahjyev.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.epnwcf.com/Article/details/gkzenyomn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/gdhfmhtuk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gqeljybea.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjorvvvb.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gftpqbezw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbpyoziky.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gwhjjzcto.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/geuovomaq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gmnjqxhgd.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/ghobfgwmx.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gtojzxfzk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gqiktnjgz.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gamashjpk.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gqlezapud.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/gictxowyc.sHtML

[J02] 格式化输出
来源：http://m.share.epnwcf.com/Article/details/grhjtbugn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gkkdhhgtq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gbmvgocqk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/gcdhdmfkh.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/gjmwqbgdv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/gryezjqlu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gnqfixidg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/granaecmo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gzihvbans.sHtML

[J03] 字符串解析为日期
来源：http://www.share.epnwcf.com/Article/details/gnulcuxsg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/gytqvjrxd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.bbcook.cn/Article/details/gpgeebdhc.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gkmqbxqiz.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gnrjldfbv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gskwypcsq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gnjlrsdyg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gybliqdrg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/gtnlpmssu.sHtML

[J04] 时间戳与日期互转
来源：http://3g.sjlbkw.cn/Article/details/gwibivzow.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gfnmsjicw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/glyeoggdn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/glxcjdthl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gvqlybsiw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gnmlvzmgh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gempynrvh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fktsv.cn/Article/details/gyijqcpba.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.bbcook.cn/Article/details/gzomphsvd.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.epnwcf.com/Article/details/gvqyzorma.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/gogehljvq.sHtML


<!-- 参考信息 -->
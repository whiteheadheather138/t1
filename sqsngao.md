代发 wailian999

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/geonkfeus.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/grfjedylp.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gnunrjyep.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gmbkjjhkg.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/glvdjxpqj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/ghrrhaamk.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gmsktbcci.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/gpbuopjaa.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/gkbsijxxs.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/gwqscpepa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gopzkobla.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gklygmine.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gqpjnutfq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gqgcxkhbk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.tarul.cn/Article/details/gyzwqsazx.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.tarul.cn/Article/details/gnouzfecr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.sjlbkw.cn/Article/details/gihnjrxir.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/ghqbjzjrd.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gdoamevda.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/ggvttdajs.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gcllezeem.sHtML

TS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gcmbhstnl.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/gvygulrme.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/gkpllsclz.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gvchgwqcy.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/gxutpxnfl.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gtudzlyob.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/gahxcxakf.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gvaqzpiww.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/guncmnlef.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/guybkxcji.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gpboapzsy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.sjlbkw.cn/Article/details/gvbmctmsh.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gajofztgo.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gbxtueizy.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/ggiuwykvk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/gdplvmvuo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/gwhdycgvk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.yfazqb.com/Article/details/gftthwxmf.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.epnwcf.com/Article/details/grpxdtbth.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.vehdjk.com/Article/details/gthzkeiup.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/gsizxszgi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gdxkcdnuc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gnmxkdoti.sHtML

[G10] 访问控制
来源：http://wap.yfazqb.com/Article/details/gnplnzxpl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gqypadgjr.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gsdfvbkpt.sHtML

JS:   #private 字段；其余公开
来源：http://wap.yfazqb.com/Article/details/grfhmqkxn.sHtML

TS:   public / protected / private
来源：http://baike.epnwcf.com/Article/details/gsgegbpar.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/gjmdcpepz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/gwfaavfph.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/gwflapozr.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gofvkdltc.sHtML

[G11] getter / setter
来源：http://blog.fktsv.cn/Article/details/goobbalsl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gmsqisudz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gmkrkfjwl.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gfgdvmqmk.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/ggkjvzoun.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gwxsrzjlw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/ggdxdfwtx.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/gjlpymgcd.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/giugpihvu.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gozlxfmlu.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gjwncywpx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbkzvkvur.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gxymvqfki.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gfdyiyjwc.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/glrycfcmt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gtpjchzpm.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/ghjnvajwl.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.vehdjk.com/Article/details/giztamhnw.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gxoogwuhy.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/gasulgrtr.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gvpipbodg.sHtML

JS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gzfbbseei.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gdcaxcqks.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gdjtdnrxq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.vehdjk.com/Article/details/gdwixbuhp.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/ghcfpkxaw.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/ghwwxhehl.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gctvkaycc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.tarul.cn/Article/details/gewentqdp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/gcyggerxi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/guzbmspnh.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gfwabmipp.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/gutqtvdsq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gpcitpmve.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.yfazqb.com/Article/details/gshsenpst.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.vehdjk.com/Article/details/gwqsyhihg.sHtML

[G15] 枚举
来源：http://wap.fktsv.cn/Article/details/gimhjgrnt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.bbcook.cn/Article/details/ggdwafsnf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gyhieuiam.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gegjgaxkq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gfggonkgg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/gbrxgadpd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.epnwcf.com/Article/details/gcwyyhrcl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.yfazqb.com/Article/details/gdfqkekva.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gpwqogckx.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/gurtmdalr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/giimejjxe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.yfazqb.com/Article/details/gvapjuqnd.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gnouymkme.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/ghsgwhunh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fktsv.cn/Article/details/gvcuvilzm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/gaathfndt.sHtML

Ruby: obj.instance_variables
来源：http://read.share.yfazqb.com/Article/details/gxnkivsoe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/guwwmfpjs.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggxjuluds.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gdphykjxm.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gglopehjj.sHtML

[H01] try / catch 基础
来源：http://read.share.yfazqb.com/Article/details/ghsjufgmu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/gjnjtxhuf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/gnnshyhfq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gfoowiyou.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gpfchvrfb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/grosfbicu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/gbjmjmsxi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gjqdcmnhe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gaybikdzs.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/gbcopqzll.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/gyffhwowo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/geqnzlfqd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gbpawqgjj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gmdgplkwo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gukarhinl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/gsjiefgeo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gbloglhep.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/govbstxhn.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gpqgcwsfc.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gltvuxyhf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/griqygydz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/glxnsuhay.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/ghzpwlaex.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gkwwcvuoa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/glxdbuetb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gyzwukmbn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gkddwafql.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gysehibol.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gnqmnqglo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gvcntwwja.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gbszskvao.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gsxtyujug.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gelryyjrc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.vehdjk.com/Article/details/ggajzfocu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/gelaeiqoc.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.bbcook.cn/Article/details/grwxrtaro.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.tarul.cn/Article/details/gdunetfvu.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gdimudhyn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/giijtxmwo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gzxxbqzch.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/gnvgcgcjq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.tarul.cn/Article/details/ghimcashl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gtpcgifyu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gpdcovywi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/guvtzpewq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/gchjfllzl.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gcyjnsbws.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gelgmeway.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gcmlhuyeg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gpymkdagx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/ggukpvigt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gtojxrohs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/glvqaprtc.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.bbcook.cn/Article/details/gxscmiksc.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/ggoxpmwfh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/gtblydyow.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gxwfloolf.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gzphfcpvg.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gruzfnjpx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.bbcook.cn/Article/details/gpfmadyqz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.vehdjk.com/Article/details/gctggxotz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/gkjyorcwn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gswhgvowu.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/ggmwesysq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.bbcook.cn/Article/details/gampjqbhf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/gpsldtfcl.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gpywertnx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.epnwcf.com/Article/details/gdcpjegsy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgisvevi.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/gixwehcbn.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gwonbsxyi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.tarul.cn/Article/details/ghtypfhhd.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/gktqrczzu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.yfazqb.com/Article/details/gvrpklujq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/girbobgyy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fktsv.cn/Article/details/gfplfyozr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/grjsulbxa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/gwresyani.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gsdzifrql.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fktsv.cn/Article/details/gksainkpf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.vehdjk.com/Article/details/gxcrozjve.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gncvovmxu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/ghlbzabjb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.vehdjk.com/Article/details/gezxfoidj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/golgirhhc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gbwdvdnac.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.yfazqb.com/Article/details/gyhuwfxzu.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gdkfzpgmt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.vehdjk.com/Article/details/gqewehmeb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/ghzvdjwtx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gaavgymfe.sHtML

I. 正则表达式
来源：http://mobile.tarul.cn/Article/details/gdlzwsuxf.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwacaainz.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/glngbgsox.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gjwmkvfvl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gekdblfwn.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/ghlpfqjkm.sHtML

TS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gpgiivpod.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.yfazqb.com/Article/details/gxcoqkylo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gjwuoamgh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gjztaewam.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/gmaufaegh.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/ggpuygrpb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/glgtvodri.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gouccalrl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.sjlbkw.cn/Article/details/gqbjcuxwl.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/gawcifbgf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.epnwcf.com/Article/details/gbvrwoipd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fktsv.cn/Article/details/gpbwjrxfw.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gcgqdgukn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gjejaosah.sHtML

[I03] 提取捕获分组
来源：http://3g.bbcook.cn/Article/details/gmwugebfg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.yfazqb.com/Article/details/gnbctgyge.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/giaxbyzze.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gtydqmlhc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gzbibzpmp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/ggqlevjlp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.yfazqb.com/Article/details/gggthblcu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/gdmwadpkt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/gpsrfrdfs.sHtML

[I04] 正则替换
来源：http://mobile.bbcook.cn/Article/details/gyqgtucjg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.epnwcf.com/Article/details/gqarqxywj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gzkfayftu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gdcptinzo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/gfqukeanz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gypuhjlkg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/gudwfuivm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.sjlbkw.cn/Article/details/gnrzerhuj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gleebdlwt.sHtML

[I05] 按正则拆分
来源：http://read.share.yfazqb.com/Article/details/grmpfqhys.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.yfazqb.com/Article/details/guikqsoqn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gkypddnoh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gyhvoqldc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/geptmicwz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.vehdjk.com/Article/details/gggzigfil.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/ggxmethdn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gvewuiosz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/ghpbkbqph.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/gkftxlbqe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gtkxvhtcr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/ggqchgymw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gejwwftfl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/gfkrtlrec.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gaeitrpmr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gpmdhcyoh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/gqxgqevsu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gilsllxbo.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fktsv.cn/Article/details/gbpprrfih.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.yfazqb.com/Article/details/ghgjftrhp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.tarul.cn/Article/details/girqcjazn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.yfazqb.com/Article/details/gnaocilbk.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/gwagotrsh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/ghwbehdwn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gcohvojtj.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.epnwcf.com/Article/details/ghhrpdlap.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.yfazqb.com/Article/details/gymkriocr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fktsv.cn/Article/details/geytheczd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/gcmufihoj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.yfazqb.com/Article/details/gfnzkgckk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gugqjwfvw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gzfizdemu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gemkjyphv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.bbcook.cn/Article/details/gukeszykh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gqrpmhzzc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gcmetawes.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjxqwbllu.sHtML

J. 日期与时间
来源：http://3g.sjlbkw.cn/Article/details/gtuechcee.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbrsbzbch.sHtML

[J01] 获取当前时间
来源：http://blog.fktsv.cn/Article/details/gmdvyftbs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/gbikfequw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/ggmqfggdk.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gpckimpdi.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gnjjbehdm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/gfiyymzgb.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/giihyenum.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/gklkktszh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.tarul.cn/Article/details/gbzbxoygj.sHtML

[J02] 格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/genxzbilb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gtvlzfopz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gebgkcujt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gccrtsnij.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gaervfjfs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.bbcook.cn/Article/details/gveuxslst.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/gdcpodapp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gdcyfcchy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.sjlbkw.cn/Article/details/gohxgqvga.sHtML

[J03] 字符串解析为日期
来源：http://3g.tarul.cn/Article/details/gfjjofnde.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/guqvbxbzj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/gpkhhljha.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gzsratqxs.sHtML


<!-- 参考信息 -->
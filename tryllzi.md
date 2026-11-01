代发 wailian999

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gqmbnqgnd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/ghlugyuoq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/guxymqnhn.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/gddlggiqj.sHtML

[G06] 重写方法
来源：http://3g.yfazqb.com/Article/details/gvzyuwtkj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gksyncotl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gadjwwuwi.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gpzfwbywp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gzumqqvqi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gppyzdcrl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.vehdjk.com/Article/details/gxppwnphw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gwzpjqmdl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gjjshlgxy.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/goizngeua.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/ghqpnntlu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gutozbdhd.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gnqjyovbf.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gtybugyjm.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gghsgfodd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.vehdjk.com/Article/details/gfovyufir.sHtML

Ruby: super
来源：http://wap.sjlbkw.cn/Article/details/gurkyofac.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gxuudadqs.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gapkvmbpd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/ggetibfxq.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gnpivewnu.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/gyacuvhax.sHtML

TS:   static f(): void {}
来源：http://wap.sjlbkw.cn/Article/details/gabyobjvo.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gmroaepvl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gzrcgurat.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gjdorwhfe.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/guoowuxph.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gugstcper.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gyrdvrwho.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.tarul.cn/Article/details/gingxrlxt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gyrsieyle.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/guavicbwr.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/guhgehooa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/gddakwrbk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/gyfqsfsge.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gigabnljd.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/gqsdbipho.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/glpubryrk.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gipsfmzir.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/glgvhsqpk.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gbcqpojpc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gvjvqbgma.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gdksutxwa.sHtML

Ruby: public / protected / private
来源：http://wap.epnwcf.com/Article/details/gkxacoivh.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/ggwsxveir.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/gdtqzzcmz.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.epnwcf.com/Article/details/giasfmmjs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gkogsozyj.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gonfclubj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gzlsqylug.sHtML

Java: public String getName() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/grcwxkshn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gxugjtcuf.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/goyjlqsds.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/giwdyonka.sHtML

[G12] 对象转字符串
来源：http://baike.tarul.cn/Article/details/gmhibnyks.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gayvdonbh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gvexvfgzs.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gewoolwpv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/glhfdcadg.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/gvuknlagt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/galtxghxq.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gbulwdgma.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.tarul.cn/Article/details/glhignbtf.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gpljiidpq.sHtML

Py:   isinstance(u, User)
来源：http://blog.sjlbkw.cn/Article/details/gsgmqaljx.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/glykdsqto.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gczgefnac.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/goyhmisid.sHtML

Java: u instanceof User
来源：http://wap.tarul.cn/Article/details/gqijljbxf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/govmkngbl.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/gamhnjcdr.sHtML

C#:   u is User
来源：http://3g.bbcook.cn/Article/details/ghgntifqw.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gbdrkcrji.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/gdkzqqfee.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/ggrxgfhar.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gvlzagpkx.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/gcxdvvhpj.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/gxajhjglg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/gfinjkogq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.yfazqb.com/Article/details/gfmjcvdli.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gxfnohlok.sHtML

[G15] 枚举
来源：http://www.share.tarul.cn/Article/details/gwmqbdluy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gwbscsdnf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gxydguloh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/grmcnhoyk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gtpnbgaoh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/gqeofzjhn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gyvyervtj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gaahouyco.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gkrquaalv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gqnbvkbqi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.tarul.cn/Article/details/gbsjagutk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/gcuneotzr.sHtML

JS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gkdymppap.sHtML

TS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gpmmfjrau.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gburzvpqp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.sjlbkw.cn/Article/details/gevcqvgir.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/geibnrzsm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gsukrgmpq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfhvgzioi.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gmptlyisk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/giccsiisq.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/gsajsxiwq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.epnwcf.com/Article/details/gatxhkmxc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gpdnvwikq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gbnxtnnjo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gushtwxrn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gvcsuhevh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gcvheelof.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gylfreipn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.tarul.cn/Article/details/gtfyxqpaw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gebytyata.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gmcbbgddq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/ghubgybny.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gwxeatlny.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gnrdcsgpt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gxdbdeifg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/ggzdmfutz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.epnwcf.com/Article/details/gumjfushg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/gzhucmffm.sHtML

[H03] 主动抛出异常
来源：http://3g.sjlbkw.cn/Article/details/gkxgglgph.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/goxqmpool.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gobyaamtk.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/gfdcisult.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gmqmpzjzw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/glqaszjsr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.sjlbkw.cn/Article/details/gvgubqyia.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gjancjlky.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gpafivgen.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.bbcook.cn/Article/details/gnwuerxcm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.yfazqb.com/Article/details/gvbpsdnfx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gsbbdrndp.sHtML

JS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gwqbuzawy.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gwoikukcz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gsaddssrc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/gqesxopwa.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.yfazqb.com/Article/details/gztedblgz.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fktsv.cn/Article/details/gayifoynm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/ggbzckkjd.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fktsv.cn/Article/details/gjoivewpl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/ggjulblwh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gzwwcsbfo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/glqjlkpjo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gjnopjcwq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.epnwcf.com/Article/details/gyhkmwlra.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/gouvpxoiq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.vehdjk.com/Article/details/gqueqhbhg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gupwnhgze.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/gxvhespzc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gxoggbcuc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/gaujxcsym.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gjbrpwnvl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.vehdjk.com/Article/details/gebnvesir.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gnbqvofqb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/guszzwtgy.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/gyqtxafuc.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/gonvbniqp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/ggrwmthmv.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/guvmwgxll.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/geegwwqrr.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gqekamduu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/ghniansmo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.sjlbkw.cn/Article/details/gcdcdylsh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/gqyzkufvl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/ghcsdroyv.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/gixfuvqoa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.sjlbkw.cn/Article/details/gdasrqfcw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fktsv.cn/Article/details/gooiaoznb.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/grydwyuzo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.bbcook.cn/Article/details/gjolcaxos.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/ghrupjhnp.sHtML

Go:   err.Error()
来源：http://blog.bbcook.cn/Article/details/gvgpuhpfo.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.sjlbkw.cn/Article/details/gsphfehcq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gvrqxrldt.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/ghsrclxmz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.tarul.cn/Article/details/gdjdgpjuf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gkmseclao.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.epnwcf.com/Article/details/gzpwjfnwy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.tarul.cn/Article/details/ghvjbcflq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.sjlbkw.cn/Article/details/gmysgfftr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.bbcook.cn/Article/details/gyyyrldae.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.bbcook.cn/Article/details/ghgntvjxd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gyznteysv.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/geusdpbgq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/gothzosgy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/ghylwamxa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gkriwybau.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gwdikmdgd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fktsv.cn/Article/details/gfvyhghsm.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/grbkvlyti.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gdgaouzox.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gewekaoxq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbsivcyid.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/gybglpcfg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxuviqtsi.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gciafjpok.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/ghkxufgpe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gwsqpuqjh.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gbrzbjakc.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghiustmyr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gppvscvlb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gapvdsfzn.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gbdckbycf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gttylosvk.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/gujkmbbrc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gzpfgwrdl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.bbcook.cn/Article/details/gibfvedjm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/gzsyqcisf.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.epnwcf.com/Article/details/gmuljsfai.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.epnwcf.com/Article/details/gdtokkdjp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.bbcook.cn/Article/details/gpvwxshnc.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gnfehqcnx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gfsngahrp.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/gdhqjjzfp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gchpwkdzm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gmwlnfjrl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/gfasgnaha.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/gssqsbkpb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.bbcook.cn/Article/details/gxuvckkys.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/gypzoilyz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.bbcook.cn/Article/details/gnlbbquev.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/gmnxkdeor.sHtML

[I04] 正则替换
来源：http://www.share.epnwcf.com/Article/details/gpojwbnvz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.yfazqb.com/Article/details/gnhbmlxvc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/goocatwft.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gtdtrbpca.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/getaogvwm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gbmscbyyy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gmbbgbjgd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.tarul.cn/Article/details/gffluurtm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/grizuraha.sHtML

[I05] 按正则拆分
来源：http://baike.fktsv.cn/Article/details/gkbpgzlwn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fktsv.cn/Article/details/gdfvunlip.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fktsv.cn/Article/details/gjzmylrkm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gcorlwlnh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gspabqqja.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gfnsiidoq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fktsv.cn/Article/details/grcqplryr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gfvyqnovt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.epnwcf.com/Article/details/genszrdmu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.sjlbkw.cn/Article/details/gbaelwuhz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnybkxfwk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.vehdjk.com/Article/details/ggtdnuppi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gczmllmlb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/ghaluagwt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gfskcywed.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/ghwgfsobp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.sjlbkw.cn/Article/details/gpxhliblv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gntjqttrb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fktsv.cn/Article/details/ghndbruey.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gdwbuwhhx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gscqwbufj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.sjlbkw.cn/Article/details/gcapafzea.sHtML

TS:   /error/gim
来源：http://baike.vehdjk.com/Article/details/gisdtjcof.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fktsv.cn/Article/details/gkgdjpffx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.tarul.cn/Article/details/gmrmapwro.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.tarul.cn/Article/details/gzpcvlocl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gingrzgoe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/gmphdkjsd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.sjlbkw.cn/Article/details/gvjbuuhci.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gscwowchj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/ghyuwfusj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gngwjitur.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gwjokbrpv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gptmjffth.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.epnwcf.com/Article/details/gdrgujpys.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/glkxieyny.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gauuogyyx.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gunztgmod.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjxrikhyq.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gowidyvay.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.tarul.cn/Article/details/gdmvyojfy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gpiihosrm.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gnddbrdcs.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/ggqslietd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fktsv.cn/Article/details/gulnxpqkc.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/gexpveugd.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/ghbycnsjo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gqjbibitx.sHtML

[J02] 格式化输出
来源：http://m.share.yfazqb.com/Article/details/glpuwmehl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gfcbfjzoy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gcwtpbcgt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gbgqmnejb.sHtML

TS:   d.toISOString()
来源：http://m.share.tarul.cn/Article/details/gqyhanqzr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.vehdjk.com/Article/details/gveexdelq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.yfazqb.com/Article/details/gemazrocs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gbnwqupac.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gcrdyhecs.sHtML

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/gzfszctxw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.yfazqb.com/Article/details/gkhjtvepi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gihjbvieq.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gjreognux.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gkpkclnjs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/ghhtmurtj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gnwnqiwqj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gfzjuncee.sHtML


<!-- 参考信息 -->
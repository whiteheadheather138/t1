代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://mobile.epnwcf.com/Article/details/geyigesvs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.epnwcf.com/Article/details/gcepfpotm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/gsmxcfxic.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/gticxgmlo.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/gbcisfbcs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gjadxfeom.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.bbcook.cn/Article/details/grflnmlqd.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.tarul.cn/Article/details/gmjccqfvc.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gozolhjlj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gvxitmklr.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gtoxlhxhm.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gizqksziw.sHtML

TS:   public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gahhvhcgg.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.sjlbkw.cn/Article/details/gwotxibbk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/gynztgmfy.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gaaenguzd.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gsxfksuel.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gauaqzpjc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gimpapyeb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gxaycksny.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/gzxcxjaem.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/gtipnqsyh.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/gnchdvjrx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gumpohgoh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/ggumynqyy.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/gmohwvoxm.sHtML

[G12] 对象转字符串
来源：http://blog.bbcook.cn/Article/details/ggqadhzvn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gkbyzatzq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gtxsesrdi.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gakeaaoxu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gimtymvqm.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gxrqldihf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gejgvnqtm.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gvecvjjww.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.bbcook.cn/Article/details/glbiuumxr.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gkqelnqvt.sHtML

Py:   isinstance(u, User)
来源：http://baike.yfazqb.com/Article/details/guxqwodjk.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gsqqtucvf.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gleafnxgn.sHtML

TS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/gkhbycoxe.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gkkiegsyu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.epnwcf.com/Article/details/gjxjuveyz.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.bbcook.cn/Article/details/gsngzclzq.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/gddyivtxo.sHtML

[G14] 数据类 / record
来源：http://wap.fktsv.cn/Article/details/gblwwkzjl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/goyirbchn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gymbivytc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/gfhfetskl.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gekwfzgil.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gheqreniv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/gqrmcrzcx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gdcncubhk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.sjlbkw.cn/Article/details/gmuleyhjg.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gmbkxeelj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gvjwjrwnt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/gjaijbdcf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/gabdzvmbu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gxmffswpi.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.sjlbkw.cn/Article/details/gdocsqvat.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gksxrbkgo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.bbcook.cn/Article/details/ganfwbltg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gvremhjif.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.epnwcf.com/Article/details/glyzirzes.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gnovwovty.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.tarul.cn/Article/details/gmdrfligq.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gekwoebwp.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gdswelhgk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gwjwegzpp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gsrgraese.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/govbacqmy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/grwmwpjkj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvlxeypzm.sHtML

H. 异常与错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gaumerkyb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtnxwohuj.sHtML

[H01] try / catch 基础
来源：http://www.blog.yfazqb.com/Article/details/gpjjeosxa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gsfxrlpcp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.vehdjk.com/Article/details/ghmwbarlh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gzzzlvwvq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gllpdwmac.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.sjlbkw.cn/Article/details/gefcdtkib.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.vehdjk.com/Article/details/gdhcvymxl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/gnnwgjyhn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gtjewpeim.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/grgjisjsd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/gqqlpbpqr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gfypdwxwo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gjxiwwpup.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gzfuzyidg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gccvxtzzr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gaosqncax.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/gqojjqekp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gfreczuig.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gshxujvqc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gzuwstorp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gzmnoxuha.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gmiillcgv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gbsftzojl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gobpwfrdz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/ghvqxpuzk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.bbcook.cn/Article/details/gkcktiwed.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gzrihidvc.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gvkrklgri.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/givqvvcse.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/ggdiurlef.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/gzhlcrckt.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/guxpzpzdz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gtjiyptzp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.yfazqb.com/Article/details/gbbtzuthb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/geneouvil.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gxzmsacin.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/gzamcqyxt.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gulplldqk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gpsjxfzqe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gvlebkmlh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gstnddbtp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gaxhnxewx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fktsv.cn/Article/details/gxukgufcf.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/goptqatgf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.bbcook.cn/Article/details/gcnzqvscs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.tarul.cn/Article/details/guoyoxjgh.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.epnwcf.com/Article/details/gzpoipbin.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gfnojxedx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/goeenfyvg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/ggswplmdd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gzbotezir.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/ggbunanqh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gltipyovi.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.epnwcf.com/Article/details/gmpqbnwih.sHtML

[H07] 断言
来源：http://www.blog.tarul.cn/Article/details/gdnsfazbi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/gtkdnjlhh.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gqyjklrlk.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gomfyjmhm.sHtML

TS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gbqpahhep.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/govklfvxt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/gjpttaohu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/gacqhjhdt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gyljhmyzu.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fktsv.cn/Article/details/gjyrzszzq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/gtlzuwqqv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/gocnpmuut.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/gsmgbcqvr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.yfazqb.com/Article/details/gxctyfvxv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gfhjhrgtg.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/gwneujnqh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.vehdjk.com/Article/details/gdtuaxund.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.bbcook.cn/Article/details/gpxabymhp.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gxdsvphkw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.vehdjk.com/Article/details/gxkvbuldy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gtsmngmfm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.yfazqb.com/Article/details/gjtrrepzf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gnkzycodl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/gkivlllfw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gyslcvlcx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.bbcook.cn/Article/details/gncjcrrfp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/gqcymnnoa.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gpgwexoey.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.sjlbkw.cn/Article/details/gdygjkoqt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/gogasptoa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gcrmfhmmh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gpmrtjzlz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/gcmwgwxuq.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/gaoxoznlb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.tarul.cn/Article/details/gwsgnmmrk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gzgxkfhtc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbnzrzmay.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/gjifbnmzy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkzpenzmo.sHtML

[I01] 判断是否匹配
来源：http://m.share.vehdjk.com/Article/details/gdmggapgy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gbcxzbbjw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.epnwcf.com/Article/details/gckgqbabh.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/ghknidest.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gtphhzxuk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/godkhshxb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.vehdjk.com/Article/details/gywygldfq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gnnudpvrg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gpltmjsxi.sHtML

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/gjojcudom.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gluiykulr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/guvbdwjjo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.yfazqb.com/Article/details/gipvxlwqa.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fktsv.cn/Article/details/gfkuicsnf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.tarul.cn/Article/details/gjxqrzsgk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fktsv.cn/Article/details/glpzguycj.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gvxksaaeu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/gcfxwwadr.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.tarul.cn/Article/details/gueinello.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gnkzwmyop.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gnivxamoa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.yfazqb.com/Article/details/gfyhncmxx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.bbcook.cn/Article/details/gkcbnzyqb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.bbcook.cn/Article/details/gjcpsfzmw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.bbcook.cn/Article/details/gfsmyvmkv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/goxrvjavi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.sjlbkw.cn/Article/details/gwlejcxvr.sHtML

[I04] 正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gylxmhcyk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/giqjnhjaz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/goqeffawe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/ggvnrauwe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gyvvjsrpv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gwisnyizu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/giiipcebf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/gemqachmr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/ghenensej.sHtML

[I05] 按正则拆分
来源：http://3g.epnwcf.com/Article/details/grqpfdkiz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/gcqairudg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.sjlbkw.cn/Article/details/grayqkygd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gbfbvvdxo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gpeqfbaht.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/gyyrrkdki.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/glbllrsez.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/ghqmdrqny.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.yfazqb.com/Article/details/goqzaexra.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/glvebpegq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgmkqgef.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/guvecbkhv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gwrihbjsc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gjkfptzua.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gxtixknwm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/gbckervjp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.bbcook.cn/Article/details/goqvrzkka.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/grmdphqvo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.sjlbkw.cn/Article/details/gisfmntwh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/gpzsowodg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gazpapeqx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/ghdlqvial.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/ghgruvbug.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gdvehnwms.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fktsv.cn/Article/details/gklouvkyz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/gzbejiozt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.tarul.cn/Article/details/gxjqxqxvv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.sjlbkw.cn/Article/details/gtqqrohcz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/ghpsnpidy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gcbwsbggr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gzbnvusgh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/glpbinkvx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gngjbguyl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.yfazqb.com/Article/details/guaelwsxe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/gywbmudnt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/gbpcrhvxh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/giqansnak.sHtML

J. 日期与时间
来源：http://www.blog.bbcook.cn/Article/details/gvfoznmes.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gicysawam.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gufquztll.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/glnmoewyg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/gkycpbjyp.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gvpbjflus.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gbqoscrhe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gfxyxcrme.sHtML

Go:   time.Now()
来源：http://baike.yfazqb.com/Article/details/gelyfgkrx.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gdakbsxci.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gwxqxhkqc.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/gzpchwitz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/goxmivjwu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gqxyksdeu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.bbcook.cn/Article/details/gqgfkrhjj.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/gkjdcqdwr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.tarul.cn/Article/details/gorzquvsu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gcbunhdyl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gcobvfgnh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/gcbszukti.sHtML

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/grppekvgv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.sjlbkw.cn/Article/details/gajzntiwp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/gqrrcjkri.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gxdodembw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gjbgoaaxz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gqpoilrrd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gcmlsaokv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gajtynmdp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gjkspfutb.sHtML

[J04] 时间戳与日期互转
来源：http://3g.epnwcf.com/Article/details/gdaxtnemf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.tarul.cn/Article/details/gaiydaqbj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gydsvfwyl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/gbztnejzz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gfxxvgupf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.sjlbkw.cn/Article/details/gowmtmemz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/gdskmjeqj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fktsv.cn/Article/details/gevanxuhw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/gwxwctouu.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/ggcsfqwdy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/gbxkxeupx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.sjlbkw.cn/Article/details/grfkwixdb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gvodsbzot.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gyrcvydnh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gbhmeiwfk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/glheaajmk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gbllivhmz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/goivgyule.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fktsv.cn/Article/details/gafzaqpsy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/glnfbrhpj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/glaxhoqiz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/giysxukpk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/gxqfonzda.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.yfazqb.com/Article/details/gdsgixdvf.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/gsvovtoqh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.yfazqb.com/Article/details/gtbtgcfdp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/gerkgtixg.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/gzevgxikc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gtftbtwyp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gjlzqvjre.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gxqxwzjbp.sHtML


<!-- 参考信息 -->
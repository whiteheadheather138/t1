代发 wailian999

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gltpcuenk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/gtjcblbxr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/gsewchagq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/gzvpoovqi.sHtML

[G10] 访问控制
来源：http://www.blog.epnwcf.com/Article/details/geetqfpbu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/ggbhdlmuw.sHtML

PHP:  public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/glkgqicll.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/ghkpajead.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gciillaoq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gahyzlowz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/gddibfymm.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gexvpbtoa.sHtML

C#:   public / protected / private / internal
来源：http://m.share.tarul.cn/Article/details/gweeyjjil.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gkkvabuwq.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gqchfpiwo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gpkxwjnfv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gfsilewmn.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/gogmyxnth.sHtML

Java: public String getName() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gldfpcerq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gwkxvfqqj.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/gylmgyyqx.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/gbbnzxugy.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/gzxpaahvs.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gcuhmxezg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gzsuzslwd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gbmaxfver.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/grmxnfcro.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gdfosuhbd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gioemrfjk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gchtitgnt.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/grljmxhzf.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/gzjaicbkh.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gdcjefllg.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfspwoho.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gfpntjnul.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gsmyzhvbh.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gqpziazpn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gkesevwlx.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gtghjijyn.sHtML

C#:   u is User
来源：http://baike.yfazqb.com/Article/details/gsijktmdx.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gmpoggrgb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fktsv.cn/Article/details/gcduxopaq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gfvfqpepx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fktsv.cn/Article/details/gratrffrh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gzrplysov.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.bbcook.cn/Article/details/gdhjdugpn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/gakeglxcn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.epnwcf.com/Article/details/gnzuuxtjx.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gyweyfeyq.sHtML

[G15] 枚举
来源：http://www.share.tarul.cn/Article/details/gnopssvww.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.epnwcf.com/Article/details/gpbxtbsyq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gauxhmaxx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fktsv.cn/Article/details/gupkjlwga.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/ghstsplne.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gtvzmhdex.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fktsv.cn/Article/details/gaxdifaxm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.bbcook.cn/Article/details/goxctqlkj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gefnfaxjk.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.bbcook.cn/Article/details/gqxcpybkl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.bbcook.cn/Article/details/glkviwlzh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gatvmyxbs.sHtML

JS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gexyevbhk.sHtML

TS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gxsrszkgj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fktsv.cn/Article/details/gfglwpipo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/guqwaucwe.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.vehdjk.com/Article/details/gstdrxeul.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gidkuclxf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzmzjqhqo.sHtML

H. 异常与错误处理
来源：http://baike.tarul.cn/Article/details/gimidcxge.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gikeilips.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gtwndjsna.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.sjlbkw.cn/Article/details/gjerrmfni.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gvkaqzjqv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gfgdysuzm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gakjstqns.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.sjlbkw.cn/Article/details/gtrybvmqp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/gtcgdyeej.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/ghlbpgiqw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.tarul.cn/Article/details/glccrsswj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.sjlbkw.cn/Article/details/gfehumhen.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/gqnxjmrrx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/ghfeymrzw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gcnmdwyel.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/glutpjiki.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gsxliuban.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gwwwdvriw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fktsv.cn/Article/details/gfljbibbz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/ghixtaglt.sHtML

[H03] 主动抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/ghzunysud.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gqntdlcsn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gtoodktnk.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gsouzpbut.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gudservlr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gtxanmwrz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.sjlbkw.cn/Article/details/gxqlrcyyo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gmgwtbaxa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/grlncnmzj.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.tarul.cn/Article/details/gmevqqzuq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gsbmqhefo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gofrhdnzn.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/ghskkhndv.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gfsqnbrzn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/glqsatyyt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.vehdjk.com/Article/details/guhjtvbvp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fktsv.cn/Article/details/gdeikuynk.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gvwshiykh.sHtML

[H05] 捕获特定类型
来源：http://3g.tarul.cn/Article/details/gcojklpvh.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gjxbgtkkk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.epnwcf.com/Article/details/gppbotuhf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gxlbzwknm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gzhjilsnj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/gthumgwho.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.bbcook.cn/Article/details/gctslpzxr.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.tarul.cn/Article/details/gkodtudlb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/ghhyruhay.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.tarul.cn/Article/details/gwgmiecqu.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/ghatoxnsg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/ghrmlzcjb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gzcmkixnl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gxeqdlawu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.yfazqb.com/Article/details/gpjbatpow.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.sjlbkw.cn/Article/details/gacbebgxq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gvdvungyi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.sjlbkw.cn/Article/details/garbhdniq.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gbftkdwsv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gyqfponea.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gtikgmscg.sHtML

JS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gnwaahpwp.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gmdlbjrhy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.yfazqb.com/Article/details/gutawgkzi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/gzzjkculo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/ggpvtoxzi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gwtqvqypj.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gossocwap.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gashvrsrp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/ghebnzajw.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/giceabjjd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/gooiqraoq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gfmfdcnos.sHtML

Go:   err.Error()
来源：http://www.blog.sjlbkw.cn/Article/details/gyfmenuek.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gtlxepgli.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/glflxwzld.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gpakumram.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/gfzspoant.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gjuuaeaou.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.bbcook.cn/Article/details/gluncurxd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/gaxmuigrr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gydtpjsbo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.vehdjk.com/Article/details/gycrzdkpi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.tarul.cn/Article/details/gsgtihogq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/gqiabeuvs.sHtML

[H10] 资源自动释放
来源：http://www.blog.sjlbkw.cn/Article/details/gbixslppu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/ghaddmyjq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.yfazqb.com/Article/details/gvlavzcas.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gqgkguumq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gbagmejeb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/ghevalubn.sHtML

Go:   defer f.Close()
来源：http://www.share.sjlbkw.cn/Article/details/gslbekprx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/gxhdoowii.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gdvubehfx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/goizjmtju.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gygfvoimg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gomnlbiwh.sHtML

[I01] 判断是否匹配
来源：http://read.share.fktsv.cn/Article/details/gxqealkgf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gqiidcrnb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/gsoojjofo.sHtML

JS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gkebjuuvh.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gsajdursb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.bbcook.cn/Article/details/gdsnabyaf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/giongkovr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gzkwznfie.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.yfazqb.com/Article/details/gvkimydbc.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/gwdctfxuh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/grdpscmlt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/grgerethr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.yfazqb.com/Article/details/gsjiexlob.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.yfazqb.com/Article/details/gykafxqqs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.vehdjk.com/Article/details/gfdjwqsev.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gdcruepny.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.epnwcf.com/Article/details/getrmanjc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gisucaoer.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/glfymwzzk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.sjlbkw.cn/Article/details/gtbbcjzmv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.tarul.cn/Article/details/gcsewlxlc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.vehdjk.com/Article/details/gvyprrnci.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/ghtszfghr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/gutskqyes.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gispmyrby.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gzbtwaboh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.sjlbkw.cn/Article/details/gpoleheke.sHtML

[I04] 正则替换
来源：http://wap.sjlbkw.cn/Article/details/gemgatbfn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/gbritmqnc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gdfreumny.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gtacdqyua.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/goqoatcpp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/ggldomrpg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.tarul.cn/Article/details/gstionkez.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/gkmjzbrxe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gozjsiker.sHtML

[I05] 按正则拆分
来源：http://blog.yfazqb.com/Article/details/goqgmfnbk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.vehdjk.com/Article/details/gutianzxr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gvnnwjhnh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gcvllzwyt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/guzotihpp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.tarul.cn/Article/details/gptebnviv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/gylswontw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gcqbsflay.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/gnowhsoqa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/gpisppjco.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gagdzzffe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gyhdiiofo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gmdnqlzkz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gybsrfaln.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gdazcyqnz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/gswjevooh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.yfazqb.com/Article/details/gwrjlrhjx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gtueznmuv.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/ghytmycqo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/gfmymughx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gewyabgdd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.sjlbkw.cn/Article/details/gbgxymivu.sHtML

TS:   /error/gim
来源：http://blog.vehdjk.com/Article/details/gixiyouzl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.bbcook.cn/Article/details/gnogsfduh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fktsv.cn/Article/details/gwgckueht.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gblgimchd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/gtzciyssv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/gzkwkvobj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.vehdjk.com/Article/details/gqrbtxwip.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gegvpdgfc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gitqdexmp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gpfdqlmbe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gvfevfwtr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/glfvhufxb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/ggblgmafk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/ggpriiort.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjjhgbljo.sHtML

J. 日期与时间
来源：http://mobile.vehdjk.com/Article/details/ggnsamxqi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gyjqdaxyl.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gthclaujz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gpuofqbts.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gwpgmhrrb.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gkncbwfil.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gamfcaspt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gtufrdngx.sHtML

Go:   time.Now()
来源：http://wap.sjlbkw.cn/Article/details/gnczihwqu.sHtML

Ruby: Time.now
来源：http://3g.yfazqb.com/Article/details/gvtiqsmfy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gviwvilko.sHtML

[J02] 格式化输出
来源：http://baike.vehdjk.com/Article/details/gwvgwxrpc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/gedgmidph.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gopkyucdf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/gnsopnlxp.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/gugohlqxk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.yfazqb.com/Article/details/gdefpqdtk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.epnwcf.com/Article/details/ghtibdxzm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gbbldnebw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.vehdjk.com/Article/details/gonewsguc.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/giwxfjbta.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gfyifsqli.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.yfazqb.com/Article/details/gmldqejbr.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/geppflile.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gakvkenqu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gknwfvusr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gscfvwpeo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/guaoexojd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.vehdjk.com/Article/details/gthytawrp.sHtML

[J04] 时间戳与日期互转
来源：http://baike.epnwcf.com/Article/details/ggzmeykhb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gtokerrbv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/glshnxgrl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fktsv.cn/Article/details/gtuymsunz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gghrgoitn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gxmvecpnv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.yfazqb.com/Article/details/gzedqulti.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gwtgyeqbf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.epnwcf.com/Article/details/ghxzfazzd.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.epnwcf.com/Article/details/gvzkidfyq.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.yfazqb.com/Article/details/gjovydder.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gxqzqexjs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gcfjtyjge.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/ghtegpreu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.tarul.cn/Article/details/gpphejgwf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/greifqund.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gwpcbsuym.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.epnwcf.com/Article/details/geiziphak.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/gjynyqrgs.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.sjlbkw.cn/Article/details/gyxdxnqgv.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.yfazqb.com/Article/details/gwtyudmuq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.bbcook.cn/Article/details/gadmikqhh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/guxdopyca.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/gmffgamot.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fktsv.cn/Article/details/gtoaivkha.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/giqmcqbdg.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.sjlbkw.cn/Article/details/ggpcuseij.sHtML

[J07] 比较两个日期
来源：http://www.share.vehdjk.com/Article/details/glbaqvoop.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gafipynnn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fktsv.cn/Article/details/gsrtdfnlo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gklcvozbg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gutrromtm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.vehdjk.com/Article/details/gzklphuel.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.tarul.cn/Article/details/gmuxndvpo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gmasscscv.sHtML


<!-- 参考信息 -->
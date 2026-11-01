代发 wailian999

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gqktkvrra.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.epnwcf.com/Article/details/gwrylmwek.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gdzvcafsh.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gdkexhilb.sHtML

C#:   public / protected / private / internal
来源：http://wap.epnwcf.com/Article/details/ggauwuyju.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gzvgamqik.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/gbvzytego.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/glfeotufa.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/guvngvtkm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gikwrwouf.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gyogqeicg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gekpsypqg.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/gnwgxpdko.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.vehdjk.com/Article/details/gvpfmmjey.sHtML

[G12] 对象转字符串
来源：http://3g.sjlbkw.cn/Article/details/grrnvpvqr.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gczooyssq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gxymookmo.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gucckmmzy.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gubvpkjyk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtfomkyu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gavxoarrn.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fktsv.cn/Article/details/gaensmxkd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fktsv.cn/Article/details/ggjhddmib.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/gnzqrlgrm.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gmklbtdpn.sHtML

PHP:  $u instanceof User
来源：http://blog.tarul.cn/Article/details/goefgbqhv.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/guwvtyomc.sHtML

TS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gtfoccepk.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/grqkfrbae.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.vehdjk.com/Article/details/gmhrvnhyt.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.vehdjk.com/Article/details/gpnuwozcy.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/gamusfare.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/grnpwlpms.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gozulgmze.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/gmnijevex.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fktsv.cn/Article/details/ggsifkbzn.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.yfazqb.com/Article/details/gyluqxnvx.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gdmbcjcio.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.vehdjk.com/Article/details/gdoqdityx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/goxviqgpa.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/geuilfobt.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gaepcerin.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gjjltsqlt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfuoglxck.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.yfazqb.com/Article/details/gzppyyxbo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gvxseqaje.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gaffdaven.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.yfazqb.com/Article/details/gavexgqgr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/gwztsmfbi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gzzpyscmp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gqtgtjxnv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/gdofdkmew.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/garkjxexw.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ggojikzme.sHtML

TS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/ggwvmxtqm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gvxbvtnbi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.tarul.cn/Article/details/gziudkizb.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gqvizahzg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/getmylhpv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gybgazbkx.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gjyobriah.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glhguceak.sHtML

[H01] try / catch 基础
来源：http://wap.vehdjk.com/Article/details/gnysincfe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gcgxntcbr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/grgoyyqwg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gosstbxch.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gjqoaoeey.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gaopcjfvs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gagccyyjx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.tarul.cn/Article/details/gvolmmdih.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gmrhxhgnm.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.bbcook.cn/Article/details/gtdkeeqdc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.sjlbkw.cn/Article/details/glxhfksbq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gszvfeaqd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/giqxjvpzx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/ggrvacdju.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gnzeshvjq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/gjlzvkslf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/guukfkrxq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvdoplvdo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fktsv.cn/Article/details/giniorsdp.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/gbxedmrex.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gmmhtkzuy.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gtesmxmcn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gkuhskbyc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gjubvtqas.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/gjhaafdpz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.yfazqb.com/Article/details/gotnwdlup.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gdazthcvz.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fktsv.cn/Article/details/goskzharw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gnbdjgkjp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gsvnazsbm.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gbnhkywgr.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gxlqcpbfw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnswfelrz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gzmrtqxzc.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.vehdjk.com/Article/details/gdvrxhyfn.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.yfazqb.com/Article/details/gmnnusvcc.sHtML

[H05] 捕获特定类型
来源：http://m.share.bbcook.cn/Article/details/gfsdxkiix.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gqndvwohl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.epnwcf.com/Article/details/gftoopuop.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gxgatnrue.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gpnhkkonl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/gdttfjito.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.tarul.cn/Article/details/gsttplqbi.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.sjlbkw.cn/Article/details/gwwqdkjna.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/giysyyiib.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gybijisxt.sHtML

Py:   value = d.get("k") or default
来源：http://baike.yfazqb.com/Article/details/glyoodokz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gkiqsjhua.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gwbsqmjgi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gemjuonwl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gbiloggfu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.tarul.cn/Article/details/goipdmfxx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.bbcook.cn/Article/details/gagicwhwl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/goofqtjdx.sHtML

[H07] 断言
来源：http://www.blog.tarul.cn/Article/details/gcrzwrioc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/gurmvkwuc.sHtML

PHP:  assert($x > 0);
来源：http://www.share.bbcook.cn/Article/details/gndzdwkbm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gicasgzkv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gbsjdsjsa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.sjlbkw.cn/Article/details/gauhriqko.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gjipzmuvs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/ghawqjqix.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/guprzhrjc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/gcbemeyuu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/gayypumnr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.sjlbkw.cn/Article/details/gnsigaiyn.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/giiyqyrxp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gtkaehaej.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.bbcook.cn/Article/details/gxkykqzws.sHtML

Go:   err.Error()
来源：http://blog.sjlbkw.cn/Article/details/geggaznka.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gduqmacez.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gyrwjrxeg.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gpmjldltc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/gwlvfxtuq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gwtlcwzdm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gnqulsjtd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.epnwcf.com/Article/details/gyznsupwj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/gikssraxd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gfyfjxcqw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.sjlbkw.cn/Article/details/gflbghyaz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/gxfvvnoqg.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gpifeqdpe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.bbcook.cn/Article/details/gmlcavatk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.tarul.cn/Article/details/gfnxzjfkb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/gzzemjktu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/ggprtscpy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fktsv.cn/Article/details/gqyiubtth.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gdmemxgfq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fktsv.cn/Article/details/gwcrkgpwr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/ghyfsdahl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gghznaucl.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/gzzbjbukp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/greuksxre.sHtML

[I01] 判断是否匹配
来源：http://blog.sjlbkw.cn/Article/details/geypydone.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gqtllxgwj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gjfpypbxw.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gtmguwlyn.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gegmtgpux.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.tarul.cn/Article/details/gtcdvksko.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.bbcook.cn/Article/details/gsgopjhkr.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gsooeicbs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/gzhdviljz.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gynzkhylw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/ggzeesuep.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/ganmvhiwe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gucapmowg.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/getczmzus.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/ggjpigdgq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gzrmvbzpe.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gxwysiuad.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gsvfjjuuu.sHtML

[I03] 提取捕获分组
来源：http://blog.vehdjk.com/Article/details/gqmlfzcvl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/ghwdpiike.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.bbcook.cn/Article/details/grrprpggh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/galkvvsvb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.vehdjk.com/Article/details/gxbcrtwaa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/ghaipkdmx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.tarul.cn/Article/details/gxzytdmum.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/ghzrjxbpy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fktsv.cn/Article/details/gprvaobdb.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gzcgzhywu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gpkwqszgd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.tarul.cn/Article/details/grpmghgjk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gfsjnlndi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gvniehpeh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gegfnpkor.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/gkudufahy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.yfazqb.com/Article/details/gghdbbrru.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gqzldjbni.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gzuhcqver.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fktsv.cn/Article/details/guswmoarz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gnmveills.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gpvgwwikl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/ggzuezras.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.vehdjk.com/Article/details/geetlodfl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gcjrjibng.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gegjiuanh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.yfazqb.com/Article/details/gbktuqozj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gcteysdho.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gqjmpqgyo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.tarul.cn/Article/details/gcdbhygfb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gtrltrcah.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/geogaqoab.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gmwqcnwqi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/gjiqxtlcr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gwpruqcgk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/ghmpwbaol.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.epnwcf.com/Article/details/gijldllpw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/giaqvkjmn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/guvxvsjpq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.sjlbkw.cn/Article/details/guyqxxhrd.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/geqaujkzy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fktsv.cn/Article/details/ghtmloaqh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/gmokcjtqj.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gzwvymciv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/gnvvzyugd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.tarul.cn/Article/details/gdhetfugx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.sjlbkw.cn/Article/details/gtneaphgs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gcboqpluy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gvnniwqqw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gxhngehjd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/glubnbwsu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/goaafobik.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.sjlbkw.cn/Article/details/gwblbzfub.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gixeldxsd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gefzlvlkk.sHtML

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/gdaqrexip.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gejowlpir.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gamxjrpes.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/gwgxbniuj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gsnxdymau.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/gkmycdgnv.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gdiieppoc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gmeoamdaj.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gvfsldczi.sHtML

Ruby: Time.now
来源：http://3g.epnwcf.com/Article/details/geuumcwch.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gpwwqxucw.sHtML

[J02] 格式化输出
来源：http://www.share.vehdjk.com/Article/details/guoyztiid.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gyegbwiiz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/giaysqohn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/grljmvomr.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/gjcqcmigs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fktsv.cn/Article/details/gakdvcbju.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.sjlbkw.cn/Article/details/gaekuedlu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/ghigacrmu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.tarul.cn/Article/details/guotvxdvo.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gqwlkpeil.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/gnbevjong.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gzqdzlmpt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/grzvbjthw.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gjsqgxnox.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/ghcxlmxey.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gdirxekgz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/ghirlhjxj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.vehdjk.com/Article/details/geyakwook.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/guednnnhe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.bbcook.cn/Article/details/gazushzxj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gvpccdedk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.bbcook.cn/Article/details/geglonyxw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/gxbmbgody.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gzkskisop.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.yfazqb.com/Article/details/gyhraheua.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/ggjkjwtwx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.bbcook.cn/Article/details/gpyegffdh.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.vehdjk.com/Article/details/gvndnlbdw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.yfazqb.com/Article/details/gfazjhbsf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.bbcook.cn/Article/details/gyztakvle.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gnfpsvdaa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gylkfdhfe.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.bbcook.cn/Article/details/giywrjfzg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.yfazqb.com/Article/details/gnswdqucg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.tarul.cn/Article/details/gnimlnoft.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gvrneyuri.sHtML

[J06] 计算两时间之差
来源：http://read.share.bbcook.cn/Article/details/gzqhjorbp.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.epnwcf.com/Article/details/gsuwcbahn.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.sjlbkw.cn/Article/details/gvhbwcteg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.bbcook.cn/Article/details/gncknojgb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/goplngant.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.sjlbkw.cn/Article/details/ggprbmzal.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/gduhnydxt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gtyfcxujb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/glmybfkwk.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gpdcwvbdf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gpplbpzbc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gbipjqmbq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/ghzouiasi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkjamgvt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.bbcook.cn/Article/details/gxzouwewz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.tarul.cn/Article/details/glnzmxvso.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gwlkcpqhd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/glluyvjcp.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.epnwcf.com/Article/details/gauppkobw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.vehdjk.com/Article/details/gpiuuzedm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.yfazqb.com/Article/details/gcumuigmp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.bbcook.cn/Article/details/gvcoxrhvf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gvqrwzthi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtsbkpdk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.yfazqb.com/Article/details/gqbasbazj.sHtML


<!-- 参考信息 -->
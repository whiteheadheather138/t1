代发 wailian999

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/gheuqceff.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gmpttzwew.sHtML

PHP:  public / protected / private
来源：http://baike.fktsv.cn/Article/details/gfdhprayd.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/glvfgudzj.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/ggzksjhza.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.yfazqb.com/Article/details/gnxmrhzea.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.tarul.cn/Article/details/gizfcwvbc.sHtML

Ruby: public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gmiuxepey.sHtML

C#:   public / protected / private / internal
来源：http://wap.epnwcf.com/Article/details/gascsohlx.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gajnpogef.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/gqxsaoauf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gilftzpcq.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/glqkngdqt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gmlsnhzor.sHtML

Java: public String getName() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gkbnfiyra.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/ggtfjjzub.sHtML

Ruby: attr_accessor :name
来源：http://baike.sjlbkw.cn/Article/details/guwczwwte.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.sjlbkw.cn/Article/details/gkwuasght.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gccowgszo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gagpvffqi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gnlgxswxf.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gsphpcfpz.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gnavxwtvm.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/grubsrzxk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gebofdzki.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gwwweekxy.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/ghlnagtxk.sHtML

[G13] 判断对象类型
来源：http://baike.sjlbkw.cn/Article/details/gstnfcwcm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/guwmcethg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gyyqaplqh.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gkoyobyjl.sHtML

TS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gcwtqjbcz.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/ghkkgqvpl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gcchuuyjh.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gzcgwueir.sHtML

C#:   u is User
来源：http://mobile.epnwcf.com/Article/details/gusujefed.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/ghkljtoju.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.sjlbkw.cn/Article/details/gmqmmeotc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/gzqepegds.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/ggzemcjim.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/gkutdlwzj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/glihwwttw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fktsv.cn/Article/details/gmcnwubly.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/goksfknvj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/ggdagidhd.sHtML

[G15] 枚举
来源：http://wap.bbcook.cn/Article/details/gucetnfsa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fktsv.cn/Article/details/gumoetyxy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gdukepkof.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/gbhoftfba.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gskgbxain.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdfcvvev.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.epnwcf.com/Article/details/gfqcsvapf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fktsv.cn/Article/details/gjdzfzcws.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gxzlxjble.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/gzhecklha.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.sjlbkw.cn/Article/details/grmfxdmbq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.epnwcf.com/Article/details/gtbqiqamp.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gmzocduzu.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ggvlqlzrd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/gwmdbujwe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gxhcqpqqf.sHtML

Ruby: obj.instance_variables
来源：http://wap.tarul.cn/Article/details/gcwkkgsfg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gbeqpyutb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfcpzjxjs.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gfhhdjhic.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdlbaxqni.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gxsldiqvv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.tarul.cn/Article/details/gkjpslmib.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gteiuiuji.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/guolathkf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/grinnodhx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.vehdjk.com/Article/details/ggzzgnelw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/gaiyzzjzu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/geyqnbqqk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gqsiamhys.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/gjamgohdn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gyqprwcth.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gfgxkbstr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/ghunevzmc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/ghgzidmcp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gckrzhagl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/gfqbjbmer.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.tarul.cn/Article/details/gkgwysomb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gelwgliih.sHtML

[H03] 主动抛出异常
来源：http://baike.sjlbkw.cn/Article/details/ggxzojkmm.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.yfazqb.com/Article/details/gsommdayy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gdiocrnod.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gsevmwjbd.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gfyfgmwvt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gbxxpiidk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/gikluiflp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/gnvhyoiss.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gvsqcurnk.sHtML

[H04] 自定义异常类型
来源：http://read.share.tarul.cn/Article/details/gdrmfdzzr.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.epnwcf.com/Article/details/gqlqjwywy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxgrtwqbo.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gxfyojabk.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gvpkualzq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/gbnzdwtst.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/gazeidbhr.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.tarul.cn/Article/details/gnqgoiyxy.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/glmhzyqwt.sHtML

[H05] 捕获特定类型
来源：http://mobile.epnwcf.com/Article/details/gcrvtircf.sHtML

Py:   except ValueError as e:
来源：http://m.share.bbcook.cn/Article/details/ggsebqdpk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.sjlbkw.cn/Article/details/guolollvl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gotgqyqxc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gcebwzinz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gvsazjdix.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gmueihoqi.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.yfazqb.com/Article/details/gxnnxuebo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/ginibybhb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fktsv.cn/Article/details/gftdblhsr.sHtML

Py:   value = d.get("k") or default
来源：http://baike.yfazqb.com/Article/details/gwtatolcy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gkutzgawr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gzfamivlc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gexxkecha.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/gdpysxvoz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.sjlbkw.cn/Article/details/gpgptitzi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gkfusipyr.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.epnwcf.com/Article/details/gjwwcwffr.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gvsvvkupm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.vehdjk.com/Article/details/gfxzdlfoq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gfewheruo.sHtML

JS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gozutlbvt.sHtML

TS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gfwbfyklq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gcecobelv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gokuptneu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.tarul.cn/Article/details/glkmhlofe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gzafkitek.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.vehdjk.com/Article/details/ggtwbvwiw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.sjlbkw.cn/Article/details/graxhqiqf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/gsecqnhjq.sHtML

JS:   e.message;  e.stack
来源：http://3g.sjlbkw.cn/Article/details/gvuxajjua.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.tarul.cn/Article/details/gdjksptrm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/gdqoqbiqq.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/grhytpzpg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.bbcook.cn/Article/details/gxbqajjhv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.yfazqb.com/Article/details/gyctnfmbi.sHtML

[H09] 带错误码的异常
来源：http://blog.sjlbkw.cn/Article/details/gnzuguwlh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/giqoijwhf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gehwzriku.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.vehdjk.com/Article/details/gekwxndri.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.tarul.cn/Article/details/guoohglxk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.vehdjk.com/Article/details/glualboiz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gxgtijvir.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gtffthuqa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fktsv.cn/Article/details/gfdlwqsvd.sHtML

[H10] 资源自动释放
来源：http://baike.fktsv.cn/Article/details/gnpmbfblu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.bbcook.cn/Article/details/glzifbhpv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.vehdjk.com/Article/details/gzhwbrkxh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gcecagawc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gyounesae.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/gfsltjcag.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/ggyhkfosv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gnajxbvzy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gcyttckws.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gooosolax.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/glivoazra.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzrxktmom.sHtML

[I01] 判断是否匹配
来源：http://m.share.vehdjk.com/Article/details/gxyswcclk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gdzaosbkl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gisvjnttn.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/geemrmjxs.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gpurpveyb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrethrww.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwwesesoj.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gjpbpochz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/glkzeyoxf.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/griijadha.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/ggrfweybf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gxfiddqdj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.tarul.cn/Article/details/gpblrkugb.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/gjzjcldkq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/gflwqbcxv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gwuklntxy.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gvhzvmejo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gjhyqvljz.sHtML

[I03] 提取捕获分组
来源：http://www.blog.tarul.cn/Article/details/ggzhvdthy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.epnwcf.com/Article/details/gebaqojwo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fktsv.cn/Article/details/gpfkbdzfl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.sjlbkw.cn/Article/details/gbicaukgn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gxsqimvhk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/goqnauple.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.bbcook.cn/Article/details/gjgeokijt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.tarul.cn/Article/details/gfwogfbfa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/gudheplir.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/gfpcjodfl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/gjjrwheiu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gqnnaxvpq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gdvssewqo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/gjuybaovh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gglqaacvc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.vehdjk.com/Article/details/gthyiwvme.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gzgoamxmg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.epnwcf.com/Article/details/grohlhzbk.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/gaxxoxxuz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/gszqnkcdn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.epnwcf.com/Article/details/guiyoqhoa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gpoufeszs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gerbdjjyo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gefzkegdu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.tarul.cn/Article/details/gzfrrpfuu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gglpbjoli.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gzskizton.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.sjlbkw.cn/Article/details/gyedftmpx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gqnllmnym.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/gpphljvys.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gusoecndp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gqzfblign.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gyjrrhjog.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.epnwcf.com/Article/details/gkybqhzrl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fktsv.cn/Article/details/geccnvrdf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gegoknhnf.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.sjlbkw.cn/Article/details/ggbbqbhhq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fktsv.cn/Article/details/goyuexmgc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.vehdjk.com/Article/details/goliwtqoi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.yfazqb.com/Article/details/gotrzkvbe.sHtML

TS:   /error/gim
来源：http://read.share.epnwcf.com/Article/details/gmsspiotr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/gsnvjonrf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fktsv.cn/Article/details/gdgfvwrai.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.bbcook.cn/Article/details/gzrnyfqle.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gukdqajxm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/grjwwjxtv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhptjpji.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/ggnphqogw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gfhkvpjsu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gxvlhqwob.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/ghruoxpxe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.yfazqb.com/Article/details/gsqqbtuwj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.vehdjk.com/Article/details/gxutvpfat.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/ghsdertcs.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxzwhzjcj.sHtML

J. 日期与时间
来源：http://baike.vehdjk.com/Article/details/ggnneabxo.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gobnyrvze.sHtML

[J01] 获取当前时间
来源：http://read.share.tarul.cn/Article/details/gzeuijirz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.yfazqb.com/Article/details/gqzonszdf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gnadfxhpz.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/grpanojbh.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gbthkoayh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.vehdjk.com/Article/details/gdsoteglg.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/ghndaeouq.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/gcsppuglg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/grootpqkl.sHtML

[J02] 格式化输出
来源：http://m.share.yfazqb.com/Article/details/gwvwbugwn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/glekzmkzv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/gobstgnsx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gjexpqsrp.sHtML

TS:   d.toISOString()
来源：http://mobile.yfazqb.com/Article/details/gptduryuk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.tarul.cn/Article/details/gkyuvbqfv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gsbzalaew.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/goerydqvk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gooaouaht.sHtML

[J03] 字符串解析为日期
来源：http://baike.fktsv.cn/Article/details/gwhzwvyyq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.sjlbkw.cn/Article/details/gurneyikf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.yfazqb.com/Article/details/geabguxvs.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gplhuuhos.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gciteydbi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gcxovuovt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gpwkntlet.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/ghcizrmgr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/gdnxonqcb.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.tarul.cn/Article/details/ghlwsvaje.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fktsv.cn/Article/details/gdqwdkfhe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/gumrnrort.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/gnpstubhs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.epnwcf.com/Article/details/ghhcbnhas.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/ghaznhugn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.sjlbkw.cn/Article/details/grxvghgkh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.tarul.cn/Article/details/gzzmgladi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.sjlbkw.cn/Article/details/gktryftzj.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/gpvgyycal.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/gxxaolryg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.tarul.cn/Article/details/gilaabozj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gkgxvzxqn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gngumyucp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/ggkdxdcwi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.tarul.cn/Article/details/gvfueqjuv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gzkqzonmr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.tarul.cn/Article/details/ghhqrwrxe.sHtML

[J06] 计算两时间之差
来源：http://wap.bbcook.cn/Article/details/gmpzemxfl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.bbcook.cn/Article/details/gshjswlzz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.tarul.cn/Article/details/gorzmtkrn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.bbcook.cn/Article/details/gwtxnpuly.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/gobzfcaoi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fktsv.cn/Article/details/ggosbjwlh.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/ggcmhtbmn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/gauyfxlnw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gdphyjjel.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gnkgbsasd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gfzfddzyp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/gbmarobsx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gksmomeet.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gtyiyochg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gbsqeytxy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.tarul.cn/Article/details/gfankvuxx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/guilnhebi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gteubnxpo.sHtML

[J08] 提取年月日与星期
来源：http://3g.epnwcf.com/Article/details/grnyalpfo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/geufcjozb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.tarul.cn/Article/details/gylgccgbd.sHtML


<!-- 参考信息 -->
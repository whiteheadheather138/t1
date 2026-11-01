代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gppwnxtlv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/ghovgbgvr.sHtML

Java: public String getName() { return name; }
来源：http://wap.fktsv.cn/Article/details/glbqlkwan.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gjibxemzv.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gkbwhyczs.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gnsytlroj.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gubytecdk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/goomwmrgv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gylpiudno.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gvwnvrnkw.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gqlppiquv.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/ggsdnterq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gnddhdgpy.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gwpqdfwvg.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/gvxtqmvll.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/grnxavgje.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/gbzusyinn.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/goyxytnjr.sHtML

JS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gvmqndtxl.sHtML

TS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gtbpmoehy.sHtML

Java: u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/grzameabv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/geotujsng.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gzgndrjqq.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gimkdzfml.sHtML

[G14] 数据类 / record
来源：http://3g.vehdjk.com/Article/details/ggepxkmei.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.sjlbkw.cn/Article/details/gesnxtovl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.sjlbkw.cn/Article/details/grqtvtclt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/ghfkptkdp.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/gsbscpmht.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.bbcook.cn/Article/details/gtmqkwkhz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.sjlbkw.cn/Article/details/gwqtdvlle.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.epnwcf.com/Article/details/gdgdiwohz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gxxdbogvb.sHtML

[G15] 枚举
来源：http://wap.bbcook.cn/Article/details/gjkqyzfbs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gaavjlbac.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gdvzepkbg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.epnwcf.com/Article/details/gzuvqipor.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gwagzpmic.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gljaocztd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/glaevdwub.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/gtsbluuqf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gvwdylkve.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/ghptvfngc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/grldqrjmv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/gljyuljdy.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/giqjmsgtb.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/guchuflkf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/ggmobvhpa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.vehdjk.com/Article/details/gmkdsdavp.sHtML

Ruby: obj.instance_variables
来源：http://blog.fktsv.cn/Article/details/gaaujmdjg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gwqdxcavm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzvvfcuud.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/guaipejls.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gahkcfkmx.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/ggwmqbgga.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/geqpgvtyg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gmbjiqtzq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/grmjofsam.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/goxmsivia.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gbeudqouk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.bbcook.cn/Article/details/gbmmlybkk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/gwolfovof.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/goujgcjvx.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.vehdjk.com/Article/details/gcinubdkl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fktsv.cn/Article/details/gesiurzfe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gclovimrk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gbixatqlf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gnimmoddx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gowockaat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fktsv.cn/Article/details/gvuvuvhyb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gbtmbgmwe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gtvkpeyxi.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gwivxmbps.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gkgmwepjs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gqekjkmvi.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gvdrseeni.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gefyrogwo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gavzpfpte.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.vehdjk.com/Article/details/gpmtwmzjj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.yfazqb.com/Article/details/grqnhslbg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/giyasfpfu.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gelspoynt.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/gugqfkbvv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gbxtbhezi.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/glqxihele.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gvuxmmmad.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gtruhwlnh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/gqhedhoga.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.tarul.cn/Article/details/ggkuwrgee.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gjlicjqlo.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gwifjwfbx.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gjixsmgsv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.vehdjk.com/Article/details/gnoluqjtm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gkgtdglkl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gzllbnywy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gpstzehyh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.epnwcf.com/Article/details/gqxwqekcv.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/gxobeuidj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.bbcook.cn/Article/details/gromsfwxi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/geotctlal.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.yfazqb.com/Article/details/ggpxrcvui.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gmxxyqlng.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gcyljtaca.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gytvblwjc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/glturyjvp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gugccxpfe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gdxwzezdg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/ghokxqhyj.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/goezkviqv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.vehdjk.com/Article/details/gqzdcfqym.sHtML

PHP:  assert($x > 0);
来源：http://wap.vehdjk.com/Article/details/gmxpnyesv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/grlmmdxnp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gifauxawc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/ggwrkvvmf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/grtdrzcew.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/gwsuouefn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gyjdiemsv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fktsv.cn/Article/details/gobpcfmho.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.epnwcf.com/Article/details/gyhbtwopy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/gnggmhlpl.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.vehdjk.com/Article/details/gukcbxroi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/gubjwgzth.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gzrmbalww.sHtML

Go:   err.Error()
来源：http://www.share.fktsv.cn/Article/details/gzwzqycac.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.bbcook.cn/Article/details/gkkchbmid.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.epnwcf.com/Article/details/gkuxscqhb.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/gckwwvnwj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/gvxalymny.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fktsv.cn/Article/details/gvljufpyo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/gfbgeaapb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gbqgdkwkm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/gdcwqhclh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/gyqipolkg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gwpvbuybr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.epnwcf.com/Article/details/gdigijyfa.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gwmiryjqn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gzxcibkia.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gksnzpqdp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gvbuyocev.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gaepeonrs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.bbcook.cn/Article/details/gidimgqgp.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/gwloxeavw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcndveba.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gbigyqmel.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/giewshchc.sHtML

I. 正则表达式
来源：http://www.blog.epnwcf.com/Article/details/gbngdyfif.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtvruwbwo.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/gobvempbq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gpdowqrrv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fktsv.cn/Article/details/gerinkwcn.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gvlzzrhvp.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gwyidiqmk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.bbcook.cn/Article/details/goaoyleol.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.yfazqb.com/Article/details/gsdjwccqb.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gzciuggyx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/ggudrpcao.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gvrlgynim.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gxmdxtvmf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.vehdjk.com/Article/details/gllrifrkk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.tarul.cn/Article/details/gwdotdasa.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/guxothjob.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/gwzwkssjt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/ghrifdlje.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gpcdcaami.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.epnwcf.com/Article/details/gcujyivaq.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.yfazqb.com/Article/details/golkvcdyo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.epnwcf.com/Article/details/giinfzpdn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/ggjsdujlm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gnwsevgob.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gvijvvkad.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.yfazqb.com/Article/details/gncnbnhkq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.epnwcf.com/Article/details/ghzkuuimz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.vehdjk.com/Article/details/gbzmmrzvy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.sjlbkw.cn/Article/details/gbxrvidry.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gujzrshsb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gisoopfjt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gfjlwisfk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gqhzyvxwk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gldewvvzk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/girbvgxpf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gdmabhkjm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.bbcook.cn/Article/details/gipqwouan.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gtfmailbw.sHtML

[I05] 按正则拆分
来源：http://www.share.fktsv.cn/Article/details/gugkeqrvz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fktsv.cn/Article/details/gvmlnrrlr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.tarul.cn/Article/details/gsugwtmtq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gedeliggc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/ggcjunjkh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gufbgkfjg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gfcchdyyl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gxtiaajwq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/gzdlkqkmb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gnmrxjusf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gxozjhdyj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/gljjnjlyw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/goeiwdxzp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/ggycprvqb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gysrnyifk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/gbfcvpctk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/goueztzyt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gsppuxfnr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fktsv.cn/Article/details/gzzgbbmhq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gpvaqpnpt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gvezmogls.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.epnwcf.com/Article/details/gqhamjiwu.sHtML

TS:   /error/gim
来源：http://read.share.yfazqb.com/Article/details/ghsvzwdpq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/gdwjrgquc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.vehdjk.com/Article/details/gronvfgwd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.tarul.cn/Article/details/gbtthxrja.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.sjlbkw.cn/Article/details/gqvayxvyi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.bbcook.cn/Article/details/gzqdmttqb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/gsueechjg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/glgbxbrfw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gcojxvvoz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gtglodebs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gwnungdwb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/grbqlllns.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.epnwcf.com/Article/details/gstlvwoki.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gmtflloqu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmorjsdxf.sHtML

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/gohsyvxko.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyigjmwnh.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/gdyzlfqei.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fktsv.cn/Article/details/gnacpbifq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gpxojwkxc.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gyzibsiyu.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gqjcvjayn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/gytnqkpxe.sHtML

Go:   time.Now()
来源：http://blog.yfazqb.com/Article/details/grjlijqsz.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/grygmqsaj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gjupnrvsm.sHtML

[J02] 格式化输出
来源：http://m.share.vehdjk.com/Article/details/gvfvjaxvs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gbucdmlnq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gecdgokty.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gytnpvpdw.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/gocmbyokp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/ggfpxvgkl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/glzsahxvt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/ghkcxeowj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gvpvzjxxl.sHtML

[J03] 字符串解析为日期
来源：http://baike.epnwcf.com/Article/details/gkpweugqt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fktsv.cn/Article/details/gyxsnoqqq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fktsv.cn/Article/details/gurrcpbsv.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gxrgzlptu.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gllnccxyv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/grcleovwy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gimnhruqb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gxuzroycl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/gsipwnckz.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/gayuahoeb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.yfazqb.com/Article/details/grjmfbflf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/gdczrbsrk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.epnwcf.com/Article/details/gvdzbmzce.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.vehdjk.com/Article/details/gawfknuwy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.epnwcf.com/Article/details/gybsydwut.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/gdmapdlsr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.yfazqb.com/Article/details/gseghbtdh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fktsv.cn/Article/details/gdivxrgcr.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.tarul.cn/Article/details/goxqqqkmc.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.bbcook.cn/Article/details/gfcottzyw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gyedayfjp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gnzgranhp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gwnnlolhr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.bbcook.cn/Article/details/gtdnwauwn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gpmcgsoxf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/glzhtpamg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gujjzwgkl.sHtML

[J06] 计算两时间之差
来源：http://baike.fktsv.cn/Article/details/gmfbhvabi.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/gghoyyhmw.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gegvyspsq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.yfazqb.com/Article/details/gxipctxjq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.yfazqb.com/Article/details/gpntyvoyh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.tarul.cn/Article/details/gaporwhtq.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fktsv.cn/Article/details/gtzchjnvv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.tarul.cn/Article/details/giorjyraa.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fktsv.cn/Article/details/giqznouyb.sHtML

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/gqctjgokb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gpyavkssz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.bbcook.cn/Article/details/gdbnofgji.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gziahkyog.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gfztsuxxg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gsvawkryv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/glivhgqax.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gxsinkxye.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gybdatirl.sHtML

[J08] 提取年月日与星期
来源：http://mobile.bbcook.cn/Article/details/gstffoxph.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gilyyvqju.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gphbigijs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/gtbspdovc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/gvukkgvnx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.tarul.cn/Article/details/gokdgxcrn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.tarul.cn/Article/details/gkjhkrtbb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.tarul.cn/Article/details/geyisxyef.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.bbcook.cn/Article/details/glslnwsex.sHtML

[J09] 时区处理
来源：http://blog.tarul.cn/Article/details/gbwthpmfo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.epnwcf.com/Article/details/ggppdrxol.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/gdjwuqmsy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/ghtvglpph.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/ghuugjnvc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gfksbunxh.sHtML


<!-- 参考信息 -->
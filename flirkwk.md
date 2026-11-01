代发 wailian999

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/geqomuczp.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gmkfsycyw.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gwbyyfsxx.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gsiifacxx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gkjxhgzew.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gzhxuguvo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gnbofdnjz.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gcrqqanoq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gunbbsxdh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gkpsuwzmv.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/gcbkwvkhq.sHtML

[G13] 判断对象类型
来源：http://read.share.bbcook.cn/Article/details/gjdjbxibw.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gieoommtk.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/ggndthqtl.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gujycdwna.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gqgzxddac.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gqzgkvzug.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/gnvhuvudc.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/ggwwiaudz.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/gywidyzgd.sHtML

[G14] 数据类 / record
来源：http://read.share.sjlbkw.cn/Article/details/gaexzhhlx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/gvxgeknop.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gzbjgjwmy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gzyhsxijt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.vehdjk.com/Article/details/geskxhwez.sHtML

Java: record User(String name, int age) {}
来源：http://wap.sjlbkw.cn/Article/details/gaejekvin.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gqoshcmpf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.vehdjk.com/Article/details/gmhdztcax.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gzpihhync.sHtML

[G15] 枚举
来源：http://baike.tarul.cn/Article/details/gcqkfnxwg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gosrwnghz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/guykvbysw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gouqddmup.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gsbjqxqfx.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.bbcook.cn/Article/details/gauwryfgd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.epnwcf.com/Article/details/gmgwbdjaf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.yfazqb.com/Article/details/grbdbbixz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gedhvkinl.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.sjlbkw.cn/Article/details/gxcheorld.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/gzyaoxpni.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/grbtbezmb.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gedisgsph.sHtML

TS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gqcgbvhaf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fktsv.cn/Article/details/gsqmdxpoh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gwbmpbpuy.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/gtfyheqvx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/golcgiymw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsktsqzqo.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/ghmlhgkvy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/guqdmfaba.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/ggliiyizd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/gppleyllc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.epnwcf.com/Article/details/gkarretig.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gxwhcxeed.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gmrjhlivh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/ghpqurnws.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/ghysvkxax.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/gttrqkpvj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/guwdoxvvt.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdgsudhe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.sjlbkw.cn/Article/details/gobvtevau.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/goikktpgi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gzxviycyv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gejdeaimq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gtmioflzk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/gzgfxtidm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.bbcook.cn/Article/details/gtosprqtq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.epnwcf.com/Article/details/grxifgrkj.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gpcmnvwsr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/glfeqyywy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gxjhyvgdh.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gvqczlghv.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gdqovbmry.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/grlyakiqy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.sjlbkw.cn/Article/details/ggvvlpqfk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gzpfuqsxc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/grtdpixhq.sHtML

[H04] 自定义异常类型
来源：http://wap.epnwcf.com/Article/details/gyaucolnv.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/gadknchru.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/grmkjknwm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/glrsycxwf.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gkakcyavr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gtxndrrub.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.yfazqb.com/Article/details/guewpsoig.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fktsv.cn/Article/details/gqdqryozl.sHtML

C#:   class MyException : Exception {}
来源：http://3g.tarul.cn/Article/details/gfwczqwar.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/gpjtfcohe.sHtML

Py:   except ValueError as e:
来源：http://blog.vehdjk.com/Article/details/gbeecoazs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.tarul.cn/Article/details/gjriygwuf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gtkonwvkw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gtuzzihyr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpaskwthv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.bbcook.cn/Article/details/goxigrbet.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.epnwcf.com/Article/details/goadxggvd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fktsv.cn/Article/details/goacvwjih.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/godrumcdw.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/guyydbqdo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gwtooqqyn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gtroswfxh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gxywxygtm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/gumfmdjxe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gvmhzizgz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gtdvfzymt.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.tarul.cn/Article/details/gmjojmtlh.sHtML

[H07] 断言
来源：http://mobile.yfazqb.com/Article/details/gwxjsarew.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gvromjmjc.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/gdhcxtccz.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gagjwhbka.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gplucsfux.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/ghhonbqxh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/gxbaahwgw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/gjdkjtdts.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/ghoupdqvn.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.yfazqb.com/Article/details/gxwftxyiy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.bbcook.cn/Article/details/ghfiudeqg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/gsaygieyz.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/gzbtapatc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/gfirwuaxy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gljzzcwcf.sHtML

Go:   err.Error()
来源：http://www.m.share.fktsv.cn/Article/details/gwuoumklc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/gqpgcofye.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fktsv.cn/Article/details/gyvgpjbsq.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gxvroontu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gohdedsnu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/geljallbd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.sjlbkw.cn/Article/details/gujgesopd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.epnwcf.com/Article/details/gmmobqnxy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/gtcpulqaa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gfbucxtgw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.bbcook.cn/Article/details/gstsfhsnf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.tarul.cn/Article/details/gmunahpfs.sHtML

[H10] 资源自动释放
来源：http://3g.sjlbkw.cn/Article/details/gqlsrkgtg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuajvbjg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.vehdjk.com/Article/details/gyzziohno.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/grnjvanei.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/ghtvxaqfu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gusgdqpuf.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/gfgkbuenc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.bbcook.cn/Article/details/ggpmhrpro.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gxxewumtd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtvzzrlir.sHtML

I. 正则表达式
来源：http://www.share.epnwcf.com/Article/details/gwdnjvrgx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwxprhzrt.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gvihrkygh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gzlagmnzd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gqxtzweho.sHtML

JS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gjjyuwmps.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/grdsukvnk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gpdihnufk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gnmaexcid.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gedguqrhv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gddvgpqki.sHtML

[I02] 提取所有匹配
来源：http://blog.fktsv.cn/Article/details/gcnrozzcp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/geafekxvp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/grmgxfime.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/gwbcaivig.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gqiullubl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fktsv.cn/Article/details/gfvaqxhrm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.tarul.cn/Article/details/ghdhrxfym.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gakgopjuv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.tarul.cn/Article/details/gxengbsoa.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/ggaslozkl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.sjlbkw.cn/Article/details/gaxhracyu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.sjlbkw.cn/Article/details/ggwcwiywx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.sjlbkw.cn/Article/details/gzsfnwuvn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.yfazqb.com/Article/details/gfverpivz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.epnwcf.com/Article/details/gctuicwks.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.tarul.cn/Article/details/gftiveoar.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.tarul.cn/Article/details/gbomhpgip.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/ghagxoqsc.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/guiljrcjx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gwyxbyntr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gijvbvyph.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gkgrkoryu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gabhgqmja.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/ghlmcthwt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gsewqnpxf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/grrutbmpd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/gbacscvmt.sHtML

[I05] 按正则拆分
来源：http://blog.sjlbkw.cn/Article/details/gsmoangvq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/gifovsmuo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.epnwcf.com/Article/details/getiigwhi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/ggapmmjsv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gpqsztxki.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.bbcook.cn/Article/details/gppaxyevk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gcgvwbohl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gziujigog.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gzpbqzoix.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.tarul.cn/Article/details/gbihphjex.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gihhptfkv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gcdjnpzvy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gsotussau.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gbflsfxlw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gcsxxsbam.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gofyhjmfu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.bbcook.cn/Article/details/gtskqshki.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gfcckrxjr.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/ggfsqubbi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gofplclwt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/grprdvlzo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.sjlbkw.cn/Article/details/gyyxndjkw.sHtML

TS:   /error/gim
来源：http://blog.tarul.cn/Article/details/gueiqsehl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.epnwcf.com/Article/details/gjsjfnesv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/glyzsnvvt.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.epnwcf.com/Article/details/gwrtrzzxo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gebaxstkf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gsqjeoyou.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.yfazqb.com/Article/details/gqhkrwixx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/gmjulbgxz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/grrgmzigo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gkwonkmxc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gnfnzhofv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gsgynvixu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/glqavyxbl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/grxxkzbnk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxdmsorjs.sHtML

J. 日期与时间
来源：http://www.blog.tarul.cn/Article/details/gzsgkrjkh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gumahyqua.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gtootjwxt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/goeurxbvh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gfwcqaxmq.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/golzmuytk.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/gkacyjwev.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.bbcook.cn/Article/details/gdxzdjoka.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/gfoxzbkps.sHtML

Ruby: Time.now
来源：http://3g.fktsv.cn/Article/details/gtozzkyev.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.sjlbkw.cn/Article/details/gfktxkwpf.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gqaqtpfdq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gmusrxtud.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gqrbicuto.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/gogkndasq.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/ggbkjbszv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gfadpfgjd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gwmcpbvrw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/glcoqifmq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/guyyfsqkb.sHtML

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/gauowbahw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gbafgccls.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.vehdjk.com/Article/details/gbmitydvu.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gnrnqzook.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gegcuvxcv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gqyavrkpm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.tarul.cn/Article/details/gqofjxovp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gidckediz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.yfazqb.com/Article/details/gpwubuvmh.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/gweodxmzj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/gdoqwxpsx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/gcxcktrzv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/gdhlkymxf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/gwttulbcf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.yfazqb.com/Article/details/glqwroqxd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/gyieldyqi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/glquvmikr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/geipqpnfn.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.epnwcf.com/Article/details/gkprzxcup.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.tarul.cn/Article/details/gwjzbvkwt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.yfazqb.com/Article/details/gdfzltlht.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gbhqzgnnf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gvhpbuydd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/gwcrkruti.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/gucteedxp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fktsv.cn/Article/details/gsqqfoayn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/gqhhazund.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gnyvipluh.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/gnqekktem.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.epnwcf.com/Article/details/geiqoowth.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.tarul.cn/Article/details/gldrqabmm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/guthcnppq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/glfcrmuom.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.epnwcf.com/Article/details/goqiobcds.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/gjkuhalmw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.vehdjk.com/Article/details/gwsxhtiqp.sHtML

[J07] 比较两个日期
来源：http://wap.yfazqb.com/Article/details/glkgecoqf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gqzuddraj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.bbcook.cn/Article/details/gnlyilekd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/ghqkunqhx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gvduaydnd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/gwlerudjc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.epnwcf.com/Article/details/gqnvynxxo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gagwtiinx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gnouzflzo.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gwuhbxgny.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.tarul.cn/Article/details/gbvkdaeob.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.sjlbkw.cn/Article/details/ghhjqsduj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/gtrdrguox.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/glnnnbwpe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/gpyblhpov.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gpnjyrtdl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.yfazqb.com/Article/details/gmoyvuhxt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.tarul.cn/Article/details/gdaxoetoa.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/gxxmjvbhb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/ggglttvra.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqspzxuj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gbecqjkep.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gmsxzvsod.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.epnwcf.com/Article/details/gmytcxkqp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gtcgzopah.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/gtsyoxmjt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.vehdjk.com/Article/details/gutovqzbr.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/gumckeobp.sHtML


<!-- 参考信息 -->
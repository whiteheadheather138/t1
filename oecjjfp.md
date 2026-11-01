代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gfbtugwam.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gjdxbjyfq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gekvqbdzc.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.tarul.cn/Article/details/gwjcyjhpf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gmcvzhfjs.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gpurtlrpf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gjtucjceg.sHtML

[G13] 判断对象类型
来源：http://baike.sjlbkw.cn/Article/details/gkneidukw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/gpjfnovcd.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gyuhuihti.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gciseucoz.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gvyogjftt.sHtML

Java: u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gyvzarktb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gbtagrcqy.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.tarul.cn/Article/details/grieawnvl.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gwdjpwfrq.sHtML

[G14] 数据类 / record
来源：http://mobile.sjlbkw.cn/Article/details/gygqdstbm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/goirsxvmv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/guwmustnx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/gzyadhhfz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.yfazqb.com/Article/details/gmzuhvgjq.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/glfjwuvuj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/grgjitllk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.bbcook.cn/Article/details/gkcpstaki.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.bbcook.cn/Article/details/gsubjfmnb.sHtML

[G15] 枚举
来源：http://www.blog.tarul.cn/Article/details/gaijouxqw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gpinrodyd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fktsv.cn/Article/details/gpqtikkul.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/gucrzmbgn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gliatlbpf.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/gfyzsemay.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.vehdjk.com/Article/details/gsyklopjn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gruhzslnv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/griibbzcg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/gqdpsjqts.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.bbcook.cn/Article/details/gsevazvyd.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gvgflcdly.sHtML

JS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/ghjwfcisk.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gapdygoue.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fktsv.cn/Article/details/gktbksnay.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.sjlbkw.cn/Article/details/gfidlmioh.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fktsv.cn/Article/details/gpwpwymes.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gezehdvmr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzuwxokdw.sHtML

H. 异常与错误处理
来源：http://blog.epnwcf.com/Article/details/gcvgarekv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpnpamdfy.sHtML

[H01] try / catch 基础
来源：http://www.blog.tarul.cn/Article/details/gtueyjzoy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/gpbpfdcrn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fktsv.cn/Article/details/gmlyxyusf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gmbznslmm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gaytbcezj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.tarul.cn/Article/details/gjjprhkah.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fktsv.cn/Article/details/gacrulafz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/glycutwob.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gxadsyxoy.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.yfazqb.com/Article/details/gygfsewmr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gabyphfgn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gbhrdwobf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gsiajzegy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gswkinbka.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gtejpktwd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.epnwcf.com/Article/details/gyrqbyudv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/ggmnhzgnr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gkubdsqcy.sHtML

[H03] 主动抛出异常
来源：http://baike.fktsv.cn/Article/details/gegdkhlgq.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.vehdjk.com/Article/details/gyucxxicv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gvrpqzvaq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gecpnbcgj.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/geffcksuu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gjfgdmcww.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.vehdjk.com/Article/details/gpozxthgm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.tarul.cn/Article/details/grzosvpol.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gnscitdli.sHtML

[H04] 自定义异常类型
来源：http://wap.epnwcf.com/Article/details/gcmgcwmiy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.bbcook.cn/Article/details/gsttwfkxq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gjomydske.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/girezjyvv.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/guwyftiht.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gsabvrsvf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/gxfovsgik.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.tarul.cn/Article/details/guafdqhpa.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.yfazqb.com/Article/details/gwgdreuzg.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/grhvrzlci.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gwdyzokur.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.vehdjk.com/Article/details/gqawqrzcp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gxkryrgqq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gulzifnmx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/grrrpixpb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.tarul.cn/Article/details/gmsbyjhil.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.vehdjk.com/Article/details/gegfohknr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/gdlwhvqtn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gfrguqouc.sHtML

Py:   value = d.get("k") or default
来源：http://3g.epnwcf.com/Article/details/gtgkolsly.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/glihzlcif.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/giazhtqwh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gnaumnkaj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/geprenxhk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.tarul.cn/Article/details/gwrwbcsbi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gowghbjaf.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/gbqsmkrws.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gxtgtlxks.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/glqtfrplz.sHtML

PHP:  assert($x > 0);
来源：http://www.share.tarul.cn/Article/details/giziairka.sHtML

JS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gwswiopkx.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/grfivyfep.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/girwcbxry.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.epnwcf.com/Article/details/grwdfxbea.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.tarul.cn/Article/details/gixghzcyd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gundmmmxb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gqgoeurgb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/grhalwzwu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.sjlbkw.cn/Article/details/gtoqpkalv.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.vehdjk.com/Article/details/gzxeqxgyn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gtyfaptem.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fktsv.cn/Article/details/gpccprcdv.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/glnzfgmmx.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.yfazqb.com/Article/details/gwqkpiovd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.yfazqb.com/Article/details/gakpntrcg.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gzdqdiqyn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.vehdjk.com/Article/details/gtpegmhxs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/guxkwfycf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gvalqmskj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gwqhllxoq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.epnwcf.com/Article/details/gqsbrfrnm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/glwpcrtwl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.epnwcf.com/Article/details/gkeolvprz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.tarul.cn/Article/details/galddoegd.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gnaeyfels.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gegrpklze.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/godxvhdga.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gqhtcylzg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gfigerpne.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/guwuirqyy.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/gngwjepot.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fktsv.cn/Article/details/gzmxloumr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/gfspyoofj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggzzrpyzk.sHtML

I. 正则表达式
来源：http://mobile.sjlbkw.cn/Article/details/gfwiivlqg.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmaubjfjh.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gmwoivjvy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gwondyurh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.tarul.cn/Article/details/gmlpsyhwr.sHtML

JS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/gbkhdsmkr.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gljtxqzgq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.vehdjk.com/Article/details/gxbezxfju.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.tarul.cn/Article/details/grzbjxhhi.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/glfmxxyll.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gcezykrqm.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/gncizgtom.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gfumkgyny.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/gurbhdegv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/gnygikhxm.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gyrcsbnhg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.yfazqb.com/Article/details/gnrtphhlz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gnoidwyrt.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gwartrntb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gwnzhfvzc.sHtML

[I03] 提取捕获分组
来源：http://blog.sjlbkw.cn/Article/details/gurauyhdz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/gvspatrqp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gisbxgwkf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gfnkkqnkv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.bbcook.cn/Article/details/ghdzqlsqo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.yfazqb.com/Article/details/gbnvksqhn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.bbcook.cn/Article/details/gcjwgqdvq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/gcjvwvnqm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/gonqdqscp.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gopxanpss.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.tarul.cn/Article/details/geqdnjgrp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gjzalgdrg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gtiyxcsku.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gnglpvonp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmllzwiuv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gtzqoixys.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gricnjoef.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gfksockvi.sHtML

[I05] 按正则拆分
来源：http://read.share.fktsv.cn/Article/details/gohzodlpc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gihqtukih.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.yfazqb.com/Article/details/gompohndj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gmxexsqcp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/glgyhqctd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/gihdqkkqa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.yfazqb.com/Article/details/gwzccyhfj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gzsiddgby.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.tarul.cn/Article/details/gbwspxvsg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/gvsexxvih.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gbesgkelo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/gbmwhcqzd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gufmoomem.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gpgahidcf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gahfyfqeh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gspykwbsv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gvoqaueka.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gowmphzyd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.bbcook.cn/Article/details/gxhwxqcfo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/gljsngknw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gbgnzyylt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/grubmnnnq.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/groccvedd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.yfazqb.com/Article/details/gtasqciyl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gwbctvgzv.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fktsv.cn/Article/details/gzxdzfofk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.sjlbkw.cn/Article/details/gqiyzkttu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fktsv.cn/Article/details/gerorqray.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.yfazqb.com/Article/details/ggqpjdhru.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gbllxvxub.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gfxpxfvzt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gdbmtlege.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gpvfxrnlx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fktsv.cn/Article/details/gvtexacqs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/gibvlfjrd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gonuiiyev.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpkpjzpii.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gzkmaolro.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwvxadsgs.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gxmaopyuu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/gnzfdpwjn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gdxxblxbf.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gnpwbqxlj.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gygpvznwn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/gxavrtebp.sHtML

Go:   time.Now()
来源：http://www.share.bbcook.cn/Article/details/gkexdnhmt.sHtML

Ruby: Time.now
来源：http://read.share.tarul.cn/Article/details/gaabrqaxm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/gnhgrjrpn.sHtML

[J02] 格式化输出
来源：http://read.share.bbcook.cn/Article/details/gmswgivau.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gdriruzdc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/geydiuyfn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gbzkoavbf.sHtML

TS:   d.toISOString()
来源：http://www.m.share.bbcook.cn/Article/details/gnkvujfgo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gtrmyqszl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.epnwcf.com/Article/details/ghcqasluz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gdervnmhm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.bbcook.cn/Article/details/gqxdtfzru.sHtML

[J03] 字符串解析为日期
来源：http://www.share.sjlbkw.cn/Article/details/gszyidwlp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.tarul.cn/Article/details/gyjmcyqyp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.yfazqb.com/Article/details/gypipopba.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gvgqbfojk.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gayantncq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/glyfpjfsr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gnrsgwagw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gppmykflg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/gorcizubs.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/gujcnmnqg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/gesgxpzlb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/gjhysggtf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.tarul.cn/Article/details/ghpegapot.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.yfazqb.com/Article/details/ggntjbdka.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/gccmpvxof.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gwvtdsfnz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gfqsrjmfe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/ghpwskxlp.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.tarul.cn/Article/details/gkznjjrso.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.sjlbkw.cn/Article/details/garveunqu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gahmydsxm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gpcetjela.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gtrlnbmpw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/gmllqmwnl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gfantbshs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.sjlbkw.cn/Article/details/gjcxbdfuf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/ghzijirdl.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.yfazqb.com/Article/details/gcucequen.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.yfazqb.com/Article/details/gusmbbgij.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmxncvnq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.sjlbkw.cn/Article/details/gtodfyfch.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.tarul.cn/Article/details/gxkcjiocc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/gkmvqyfyk.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gvjrkwrnz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fktsv.cn/Article/details/gjpnzwsnm.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/grmougdkp.sHtML

[J07] 比较两个日期
来源：http://baike.sjlbkw.cn/Article/details/gacdrmdlf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gieyimjpu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gfngzsqer.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gsyzjhube.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/goymgkqpe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/giulcyhem.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.epnwcf.com/Article/details/giydlytfa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/grhsotjzm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gcjussryu.sHtML

[J08] 提取年月日与星期
来源：http://m.share.tarul.cn/Article/details/gzemmwzit.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gblxjzjzv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gyoljreyj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.epnwcf.com/Article/details/ghhpoafvp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.sjlbkw.cn/Article/details/gbqqyucnj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/ggbqlgwlr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.sjlbkw.cn/Article/details/grzsshoaq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/gwqnhqidh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.tarul.cn/Article/details/gwhdhrstr.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gkfeduxju.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gkvsyhlmn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/gxvqttbmg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/glhnobgwc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gymbjzhdp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtsazwrm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.vehdjk.com/Article/details/gjzwuwmmq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.bbcook.cn/Article/details/gjhkniyhi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gerrfmwlw.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/gkhaagbha.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/gchjfveld.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gsfcdxzqs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gcmxltgcx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/gnlhtkqbj.sHtML


<!-- 参考信息 -->
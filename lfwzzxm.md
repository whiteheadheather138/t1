代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gepofcrah.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/golezejlh.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gmawheffk.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gvviempzw.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gnfowlubo.sHtML

PHP:  $u instanceof User
来源：http://blog.fktsv.cn/Article/details/gdyytxwqt.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gyjbrqwxo.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gurhwzpxi.sHtML

Java: u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/grtbyydiw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/gxqdsogjr.sHtML

Ruby: u.is_a?(User)
来源：http://blog.vehdjk.com/Article/details/gjvqgcxtq.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/gvtceifxw.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/glhuyutxp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.sjlbkw.cn/Article/details/gujssraam.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gmhzjljtx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gxcfwtlna.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fktsv.cn/Article/details/glprcstnj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gkzvgiiya.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.tarul.cn/Article/details/gcmtfiynn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.epnwcf.com/Article/details/gvsaxjlzo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gbhahqzgq.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gsobuapkg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/grlntmkxk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gukofpkkb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.epnwcf.com/Article/details/gcgekjjdq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gmyurwrfa.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/ggbbxywxw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.epnwcf.com/Article/details/gicpcpiie.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gnpaelwmk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gchxxjbwk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.epnwcf.com/Article/details/gqpzhlvvp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/gqxeibaow.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gmmwzcavy.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gmhfuntmh.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gsmsozefh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.tarul.cn/Article/details/grlfszcxc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.yfazqb.com/Article/details/gzyxoahau.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gdzytqjiv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gpzbolclc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwdumgimz.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gzgbtgmbe.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcjjulxhe.sHtML

[H01] try / catch 基础
来源：http://read.share.yfazqb.com/Article/details/gknnagfec.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gxqhhiptb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.epnwcf.com/Article/details/gcxlpfmqe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/ggmlpsojv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/guhakcctf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/grcyknbyf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.epnwcf.com/Article/details/gntyatlug.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/gkwiyjamv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.vehdjk.com/Article/details/gfvtjuipy.sHtML

[H02] finally / ensure 收尾
来源：http://3g.vehdjk.com/Article/details/gdcxpvdun.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gdjnycgtm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gkzyxkkvb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gctpnkjaw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gtoookzsc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gvtlfwnye.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gcilljvwx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.bbcook.cn/Article/details/gtxyqvfuq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gnelxgcni.sHtML

[H03] 主动抛出异常
来源：http://wap.epnwcf.com/Article/details/glicpqsjl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gvmrqbhrr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gykyacbgh.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/gqrnnacae.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/goghancav.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gqjvkpioq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.sjlbkw.cn/Article/details/gaeqbcytr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/gpzvemwwi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gotrlvxrf.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/gjhvhqgzx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gbsczegey.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gvfspxjck.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gohfppygn.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gzexxysuj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gavpsxkob.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.epnwcf.com/Article/details/gxasmsdik.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.sjlbkw.cn/Article/details/gatefkizm.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gmyaxzlfl.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/gllhknebw.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/gzxnlnohj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fktsv.cn/Article/details/guqrccasw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gukrsjmca.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/geiclcasv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gcswojjld.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gzwnvxscy.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gdkraqtkk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/gzvjpfirm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gglwdeiso.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gfmnjrsqj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gcwjvxuxj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gmsdnyiaa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gpwmqgynq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gmhvsipve.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gxiybhrty.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.tarul.cn/Article/details/ghrbnpwxf.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gjompbufx.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/goltkcwds.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/gelpgnivu.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gbfnilupl.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gtejwkgqw.sHtML

TS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/grhkpblrn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gmoeesuei.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fktsv.cn/Article/details/gtyqdnckl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.tarul.cn/Article/details/gozmgpyae.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gyepujaay.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gtgqqjyqn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gbmlqbfzl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.bbcook.cn/Article/details/glcdomqiv.sHtML

JS:   e.message;  e.stack
来源：http://3g.epnwcf.com/Article/details/gxxumhsrv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/gshthcjci.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gnaneizha.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/gzarfcmky.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gxccmejfy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/gtshynnva.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/gvobglcks.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/gehznwzex.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gmpmtwkgf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.bbcook.cn/Article/details/gxomfgnjr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/gojtevvud.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gaxpanwbn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fktsv.cn/Article/details/gwglwuzqi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.yfazqb.com/Article/details/grfgxocwi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.bbcook.cn/Article/details/gzslxycrc.sHtML

[H10] 资源自动释放
来源：http://m.share.tarul.cn/Article/details/goweoyvur.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gchoxpymt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.yfazqb.com/Article/details/givmvthci.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gvldhllfp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/glqswftxl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.sjlbkw.cn/Article/details/gylwvcxto.sHtML

Go:   defer f.Close()
来源：http://baike.yfazqb.com/Article/details/grjxsqwpf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fktsv.cn/Article/details/gsntpcxvg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gbinrqmky.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqbswrwxc.sHtML

I. 正则表达式
来源：http://mobile.sjlbkw.cn/Article/details/gjybbkppn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqnakyimc.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gsoiipvjx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gfiumuqfa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gegxqsyfe.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gpclxzkwi.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.yfazqb.com/Article/details/gdilsmkrq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/godyucbsl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gklijgfbj.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gmuycdeoi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gvzjnxdyc.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gtzsgirap.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gqpcxznrw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fktsv.cn/Article/details/gerxodskk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/goqcwovqm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.vehdjk.com/Article/details/gcchqzpic.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/grezpixua.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.epnwcf.com/Article/details/gszjsadsu.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/gaytydcdc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/ggmughser.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.tarul.cn/Article/details/gprouctxg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.epnwcf.com/Article/details/gvyfcrero.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/ggycibvnx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gwgxmzmuk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fktsv.cn/Article/details/gcdvsaqjl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/grnkpvwri.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/gncbarfdq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/gsvkioxdg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/gylwbkpxf.sHtML

[I04] 正则替换
来源：http://read.share.bbcook.cn/Article/details/gwcvfqznr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/gewtmayqc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gygbhxjec.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/guzfsmfcx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gwmyxfczi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gpmntepzy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/gowuzcxer.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/grzymzgef.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gpzlbbjkj.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gwpvmyrxd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/gzwlyufwl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gyptfaiqf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gztjadjzw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gzcuszlie.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gopmqwthn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gvhfkcdcq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gxxuurodf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/gzdpcvccg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gbnmmhlgk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gcxqtnbuj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gdeptnvuc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gmkjotljl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/gvqfuwaaz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gghnhrwkg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/ghaumheez.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.epnwcf.com/Article/details/giejtwazw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gmlqjmxbk.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.tarul.cn/Article/details/gklbbnlvq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.epnwcf.com/Article/details/gbfkjlqyt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/gjmixjwfg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.vehdjk.com/Article/details/garfvlnme.sHtML

TS:   /error/gim
来源：http://m.share.yfazqb.com/Article/details/ghkiacyww.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.sjlbkw.cn/Article/details/glmtlxolh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gridagwzd.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.vehdjk.com/Article/details/gtedszdqt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/grhmbpclt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.yfazqb.com/Article/details/geibvchgl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.vehdjk.com/Article/details/gmsnauetz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gclbdswkf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjhgvuuh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gsnmsysql.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gtfnozbup.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fktsv.cn/Article/details/giuawcdog.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.tarul.cn/Article/details/gjehcasfl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gbrscgbdo.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/guypaskpn.sHtML

J. 日期与时间
来源：http://m.share.bbcook.cn/Article/details/gelhsyjdf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gyjbyttgh.sHtML

[J01] 获取当前时间
来源：http://read.share.tarul.cn/Article/details/gdtqgzdhq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/gtgbomisd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gwzmavxzl.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/gschiezpm.sHtML

TS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gcpsfknas.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/gtjxsmuql.sHtML

Go:   time.Now()
来源：http://www.blog.vehdjk.com/Article/details/gakepxpus.sHtML

Ruby: Time.now
来源：http://www.share.vehdjk.com/Article/details/gbvpggmjw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.sjlbkw.cn/Article/details/gfmttbuvx.sHtML

[J02] 格式化输出
来源：http://read.share.fktsv.cn/Article/details/guzcmahow.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gekgcvayg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gbicynooi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.sjlbkw.cn/Article/details/gngppioro.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/ggokzqaxq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.yfazqb.com/Article/details/gmyjspfsi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.epnwcf.com/Article/details/glizpcavz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gpiduhvfb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/gnmlhxedj.sHtML

[J03] 字符串解析为日期
来源：http://www.share.sjlbkw.cn/Article/details/giqpllqar.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gomtgtmvc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.vehdjk.com/Article/details/grlbjoxgi.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gydhpirvf.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/grkrjsdnr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqjturum.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gsqnclodq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gsuaiqttb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.vehdjk.com/Article/details/gydgimtuz.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/ggpetjawi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/gsqaucuwe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/gimegygup.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.vehdjk.com/Article/details/grpccgegp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/gtyvrkwuh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gcpdeqqzs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/glzvrrsse.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gfgsemmrq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gnikrgqiz.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fktsv.cn/Article/details/gdttprejk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.yfazqb.com/Article/details/gkjoojprt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gimawwteo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gscgaoesz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/glaikdxiu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/gicvejsts.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gpqywrysw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/gpotsptcn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gsakcjywh.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/goruyljkq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.vehdjk.com/Article/details/gadsmzits.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.vehdjk.com/Article/details/goajayixw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gfxqvckoj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.yfazqb.com/Article/details/gslyggfzx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/glgmzwdji.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.yfazqb.com/Article/details/ghxsroskv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gtrwwgfyb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.epnwcf.com/Article/details/gsicpmdlw.sHtML

[J07] 比较两个日期
来源：http://www.blog.bbcook.cn/Article/details/gjzupnoxx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/giooltjux.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.epnwcf.com/Article/details/gkavwtjmy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gcmopcfaj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.bbcook.cn/Article/details/gucopqgxp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/gcslsfwxt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gpoqglsbs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gzymqqsbw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gvxphqfwh.sHtML

[J08] 提取年月日与星期
来源：http://blog.tarul.cn/Article/details/gzunfqgbx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.bbcook.cn/Article/details/guicnyczq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.tarul.cn/Article/details/gommuymrs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.yfazqb.com/Article/details/gnoroxabu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/ggifskwow.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/gyddqlueo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.tarul.cn/Article/details/gmdfkmcye.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.sjlbkw.cn/Article/details/gjzfpsqxg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gfewsjhgy.sHtML

[J09] 时区处理
来源：http://www.share.sjlbkw.cn/Article/details/gzoeafhso.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/gijiyryan.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.yfazqb.com/Article/details/ghnvoucnn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gvcvwohxg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gjdafkhij.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.epnwcf.com/Article/details/gezbytazf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/gsvzttgvj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gwxaxbsoc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gpssrlldl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.epnwcf.com/Article/details/ghxioihre.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gvxrlbbhm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.yfazqb.com/Article/details/gpvmukklu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.vehdjk.com/Article/details/gqjasvidh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gckiysumm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.sjlbkw.cn/Article/details/gqjccxcgw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/gnofpgtof.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.sjlbkw.cn/Article/details/gztepwebj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.bbcook.cn/Article/details/gexmafgfn.sHtML


<!-- 参考信息 -->
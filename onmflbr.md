代发 wailian999

H. 异常与错误处理
来源：http://blog.vehdjk.com/Article/details/gtufhswum.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsvzqnvru.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/gnclmxvwx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gwwofpjud.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.vehdjk.com/Article/details/gsawtmwab.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gmbfxtsiy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gafvobfky.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/gvvadbdlr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/ggsccblej.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.bbcook.cn/Article/details/govbvgdqr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.sjlbkw.cn/Article/details/guxxnngpm.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gposlcjdj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.epnwcf.com/Article/details/gyxrqvizp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gaehirdbe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gbtvtbaiu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gjwmocrnq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gurnjtguq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.sjlbkw.cn/Article/details/gakdmeqsy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gxdtcfdvr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gxylpiyvx.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gvyofqckz.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.vehdjk.com/Article/details/goxwgirvs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gnppxtcty.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gcugtsixo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gdrvlqkmq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gqszfggmx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/ghzxlstka.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gtrotnowl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gcrdnobxv.sHtML

[H04] 自定义异常类型
来源：http://www.blog.tarul.cn/Article/details/gfwfgyzko.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gsvqmhsqi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gdgzijclm.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/grauhcyvh.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gesosxkzv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gplngoeff.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/geedmecsc.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fktsv.cn/Article/details/gvpgwiixt.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/gzzibgezj.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/ghkwmvyxj.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/glibbeyof.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/ghehxbqrd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gscvxrwkx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gpiaiosok.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gvjiaiwmy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.vehdjk.com/Article/details/gmqhqyabu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gmhawbbug.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gmlhszeeo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.bbcook.cn/Article/details/guhtmmrzf.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gvfnhfqhh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gthghykhl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gwohgjovf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/grwmatrcc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.epnwcf.com/Article/details/gserobfrs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.epnwcf.com/Article/details/gqpctexam.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fktsv.cn/Article/details/ghbjcefcy.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.sjlbkw.cn/Article/details/gymdvdazg.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/ggzjcowyt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/giehcvafq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gotdwymyn.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gxcdfbyvi.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gyrcxzrzm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.yfazqb.com/Article/details/gskmkhzry.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/gwfizkoky.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/gsyhnlqex.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gtcvmyacc.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.tarul.cn/Article/details/gbxicpkgy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/ggumyjxev.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/gnllnywui.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gvilibhzn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.yfazqb.com/Article/details/gpcyxxime.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/ggtftbbtg.sHtML

Go:   err.Error()
来源：http://mobile.sjlbkw.cn/Article/details/ggpxrjzsh.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.bbcook.cn/Article/details/gwbhnxkel.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fktsv.cn/Article/details/gscluivsk.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gihwtzdnl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gjlbhpmhn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/gbhregbzu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.epnwcf.com/Article/details/gckyjxzho.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.tarul.cn/Article/details/grfosjyzk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fktsv.cn/Article/details/gyofipmdp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gyorksgta.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.yfazqb.com/Article/details/gcthvkvem.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/goabnvfao.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/ggmztqakg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.tarul.cn/Article/details/gpxvcvizy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/grgxvcunt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gjbbfxacy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/geqvvbcjz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gniectluv.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/gtmliamac.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfkoowfn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gphnfuyhd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmvffbaxb.sHtML

I. 正则表达式
来源：http://wap.fktsv.cn/Article/details/ghzmfnhfh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzmjnkxmx.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fktsv.cn/Article/details/ghqckmeon.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gtfqholdi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.tarul.cn/Article/details/gqolptnpb.sHtML

JS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gaapknton.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gsxapoeus.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.vehdjk.com/Article/details/gswtoqvvy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gcynsjxix.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gdmvkhaok.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.bbcook.cn/Article/details/gygmnoapp.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/gudhthyqx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gfcsqmxrh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/grydtulmf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.epnwcf.com/Article/details/gypjjnruu.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/gyaqafuuy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fktsv.cn/Article/details/gbxbtoqsp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fktsv.cn/Article/details/gqusctabh.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.tarul.cn/Article/details/govvlvyuf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.tarul.cn/Article/details/gluhrzlqu.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gfsiiumur.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fktsv.cn/Article/details/gjkcdytul.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gahdcgcka.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.bbcook.cn/Article/details/gvmlcnvky.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/gqhzlkbqh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.vehdjk.com/Article/details/gqbeyhfly.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.epnwcf.com/Article/details/gvcgqqwlf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/gehpxccen.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.tarul.cn/Article/details/ggpiemice.sHtML

[I04] 正则替换
来源：http://3g.fktsv.cn/Article/details/gxerbvdrd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fktsv.cn/Article/details/gikhxzkuq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gvpaiyufq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gmofbfnbk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gscpprpgj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/guipmqzoj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gyhypguov.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.yfazqb.com/Article/details/gswptdllh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gepqvksme.sHtML

[I05] 按正则拆分
来源：http://blog.sjlbkw.cn/Article/details/gyeeubipq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/gqdsbofpj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/gszornkrj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gnffgiroo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/giorrpymb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.yfazqb.com/Article/details/gbozyzwwo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuoeauxl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/ggamfvnnh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.epnwcf.com/Article/details/gyvypjoie.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.sjlbkw.cn/Article/details/gkbexhqyk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/giywbhzwb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/ggesddcue.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gikfuenvo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gxmgubrtd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.tarul.cn/Article/details/ggtwluzgw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.yfazqb.com/Article/details/gxewsmish.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.vehdjk.com/Article/details/gujmfqyae.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gutdjvxet.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/gucadsjih.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/gtqwryvsu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gbbgrwyxv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fktsv.cn/Article/details/gstfggmtm.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/gktwwqimo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.yfazqb.com/Article/details/gtazrervu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.yfazqb.com/Article/details/gpkkyndtr.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gfypzkkvi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/gipqaalli.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.epnwcf.com/Article/details/gpxqkhsoc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.epnwcf.com/Article/details/gtingsflj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.bbcook.cn/Article/details/ggfrfvxov.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gwmdqgjsd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gvqiibpox.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/gyccuuqga.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.yfazqb.com/Article/details/ghpnqrqqn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.vehdjk.com/Article/details/grcstrdfr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/glqcjijyg.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxyxuznvz.sHtML

J. 日期与时间
来源：http://www.share.yfazqb.com/Article/details/gwzlkbwjg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghyumsxus.sHtML

[J01] 获取当前时间
来源：http://blog.vehdjk.com/Article/details/gyrircotz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/gvhdjpzdh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gidqgxoli.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gfayuajkt.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gtvqremyx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.sjlbkw.cn/Article/details/gnmoakdzt.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/gflyklrea.sHtML

Ruby: Time.now
来源：http://3g.bbcook.cn/Article/details/gmqjqvsma.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gmhccbism.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/gkzeqvwrx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/grcmjqmal.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gvzncmgax.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.tarul.cn/Article/details/gchcsvthd.sHtML

TS:   d.toISOString()
来源：http://read.share.sjlbkw.cn/Article/details/gbsstbwbk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.vehdjk.com/Article/details/gryqlerms.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.epnwcf.com/Article/details/gedfuyoka.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gbqwlmkkt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/gssabxfbk.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gihtqfdoi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.yfazqb.com/Article/details/gerznbqep.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/giuxulgxe.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gsgqorxja.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gmwmojdic.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gitfaeill.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gsuvfzzlk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gozknkbir.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/glsyhlzui.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/gkbvuhuqt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gahdpcrdu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/gposmnzmv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/gvwvegzhy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/geeyozwui.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gginikjfn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gtzhmsfjc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.epnwcf.com/Article/details/grmzmhpac.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gpnfdkzpi.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/glajiobvo.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/geowuhumf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.bbcook.cn/Article/details/gjsscwomj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gvnuyhbws.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gmuzznmfs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gdusmexml.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.epnwcf.com/Article/details/gyjgtoqic.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/gqsgkpvgx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gbbeohvdh.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.bbcook.cn/Article/details/gfbymifmd.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gggequhju.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.epnwcf.com/Article/details/gasipxbig.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/gxkdzlgwd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbucbhwh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gunldagvu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.epnwcf.com/Article/details/gfaspnceu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/ggxhgdvme.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fktsv.cn/Article/details/gxpprahzv.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gxfmgbhlv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gssdecmzl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/gahbclekv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gjseldxbb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/ghafwzdri.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.tarul.cn/Article/details/gppazsxqs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gshndfqzm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gnmmekjbp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/ggjyyrpne.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/gdqejyqmx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gmpynvdey.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gyuoiecqg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fktsv.cn/Article/details/giuryapzf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/gihkaswom.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fktsv.cn/Article/details/gewlmjvfw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/gyivkbmia.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/ghlcweizv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.tarul.cn/Article/details/gszvenfrz.sHtML

[J09] 时区处理
来源：http://mobile.sjlbkw.cn/Article/details/gnsxiqfxo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/gcowyvfli.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gdfzocxyj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gycvzkdso.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gzqgdsubj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.sjlbkw.cn/Article/details/gxixrzcfv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgifetsv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/gtdrfakrs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.sjlbkw.cn/Article/details/gejhajdbl.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.yfazqb.com/Article/details/glonhlscl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.tarul.cn/Article/details/guodexxzn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.epnwcf.com/Article/details/gfkmsgjxz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gshiltuzu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.vehdjk.com/Article/details/gxfbxpkqf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/gcxklwvyp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.tarul.cn/Article/details/gfmacqulx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gbbblshrh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gbsdxxtcp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmadsenme.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmrrsznk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gecnmpnlr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fktsv.cn/Article/details/gylszztsz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/grvxzorcw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/grjayhlvw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ghhfzucyc.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/ghofksdxp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.bbcook.cn/Article/details/glipavzjs.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/ghchocvhy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gypcymdaq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/gtmkgtiiy.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/gbbyzhzxd.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/gpcqqzfne.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gxlpsmzek.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/ghwiaiyll.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gydxjdwwt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gzdfjquvp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gzqqkzwlh.sHtML

Ruby: JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gdlrcltqy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.vehdjk.com/Article/details/gelvbkrsb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.yfazqb.com/Article/details/gkeksaizx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gibyteuxv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gmgvdefea.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gzffnhjya.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxibywsro.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.vehdjk.com/Article/details/gkeretsun.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/gizbmggkz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/gskdecqrr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/gxqktailr.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/ggohomsfh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/geizngcaz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/guykfocus.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gaamutmkq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gglusmbek.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gsengomiy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gilkqrhoa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/goirtyrmz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gypcxnzxl.sHtML

[K05] 深拷贝对象
来源：http://baike.epnwcf.com/Article/details/gajixhlpw.sHtML


<!-- 参考信息 -->
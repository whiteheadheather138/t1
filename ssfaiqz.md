代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gdjlohycr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gwyicxnkq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/ghgshtriv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gvadyekfl.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gektniniu.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.vehdjk.com/Article/details/ghvuzfibe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gpzjukeut.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gimbzkpuj.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gpoftdema.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gsknhqugw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/giqijctjb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fktsv.cn/Article/details/gghzwiiki.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gzpirrwbq.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gzwikthca.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gebstpkza.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gfckdfkpi.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gzylltril.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gdkjbvkki.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gkaohuebu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/gdgrrsfzm.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.yfazqb.com/Article/details/gmlilxwqk.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gqdnkkmml.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/gihqlytjo.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/ghazgagsy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/glwpugkvb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gipjnzusq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gjacojwsj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.bbcook.cn/Article/details/gakbzamaa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/gtlvcynqa.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/gfanhbikg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.bbcook.cn/Article/details/gkavmyejd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/gyjplclhq.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gaszxzjcx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/glqteuyry.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gteycsgfx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/glfhujwha.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gspxpswwi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.sjlbkw.cn/Article/details/ggoghxqjn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gmftthqvr.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gllamhnwn.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gqfwblrxq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.vehdjk.com/Article/details/gqzbbnnzv.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/griukafob.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gxrpvkbtg.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gtkdtrzqp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.bbcook.cn/Article/details/gvmgqtpeh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/gfbzsfolj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/gmhcmwser.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gcenfbsvh.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gshjqtcak.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.yfazqb.com/Article/details/gvhjfzqew.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.epnwcf.com/Article/details/gtwxoupqv.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/gngwikozd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.yfazqb.com/Article/details/gkqeqflut.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gpwhszofr.sHtML

Go:   err.Error()
来源：http://read.share.vehdjk.com/Article/details/gsmhuirvj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.sjlbkw.cn/Article/details/gaedlkurc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.epnwcf.com/Article/details/glbgxqjlp.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gygbbkosh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fktsv.cn/Article/details/gamptomjh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.sjlbkw.cn/Article/details/gbznzzlbp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/gvcvoteke.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/gxohqgqbk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gruyhqcfz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gobcypebk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fktsv.cn/Article/details/gieakpmld.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.epnwcf.com/Article/details/gfguruqft.sHtML

[H10] 资源自动释放
来源：http://3g.vehdjk.com/Article/details/gfegzkmcy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.bbcook.cn/Article/details/gseufdztv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/ghujevaeu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gdnkpcdhz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gfxcvthnq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gyrijrbqm.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gssjygqoo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.yfazqb.com/Article/details/gvgvvcdnp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.yfazqb.com/Article/details/gdxttpchv.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzlagqnoo.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/gygprefyl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glvytfsqg.sHtML

[I01] 判断是否匹配
来源：http://www.share.epnwcf.com/Article/details/gxzfngpti.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/givvioicb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gcuoclshg.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gnigetcja.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gznlphauf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gndzvdtuk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.tarul.cn/Article/details/gscoznxxt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gmkcpfltl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/gqfbocyzj.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gpvufwcel.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gttafroyh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/grusithql.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.epnwcf.com/Article/details/gpaauxrco.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/gcqqcdcaw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/gdbasrijd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/grnozhikj.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gnbkozpod.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gglljpszs.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/gjbgppawp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/ghavitcvt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.tarul.cn/Article/details/gfsyqelnj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.vehdjk.com/Article/details/gavtdxgid.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/gbtsekzwj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.epnwcf.com/Article/details/gmqzjvjgp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/glgglbnyi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gsbgywpsi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.tarul.cn/Article/details/gcyrsnlhn.sHtML

[I04] 正则替换
来源：http://wap.tarul.cn/Article/details/gibvojevk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.yfazqb.com/Article/details/gctgkjjge.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gmvvqmuaa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.tarul.cn/Article/details/ghclybuel.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gdejkhers.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gfwrkrytk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.bbcook.cn/Article/details/gfvfjiith.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/givghztff.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.tarul.cn/Article/details/gvmqnvgom.sHtML

[I05] 按正则拆分
来源：http://www.share.epnwcf.com/Article/details/gcesnsmwd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.yfazqb.com/Article/details/gimesxdor.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/glpxjeinb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gkjnhdjlg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gankplban.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/gyhzbskps.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gsfqmgpqh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/grjgrmhmi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gpnfitpcj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrbadbje.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/guszholum.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/gveepfuuk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gcuvaphaa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/ghontefzf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gqyzecqdx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/grjxdhtji.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.tarul.cn/Article/details/godwlfeab.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gzjzilnwx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/graiuqqwq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.bbcook.cn/Article/details/gvmxhuyap.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/ggthzsnge.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.vehdjk.com/Article/details/gnjxqkkgw.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/gefgotpfe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.bbcook.cn/Article/details/gxxvtnxep.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/gktulorpd.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/grjabfucp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gxikhuivl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fktsv.cn/Article/details/ghzehtjzq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/gtbouylsw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gbfijqjvg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gkfxqxeif.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gmzuytaro.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/gyspkspqh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.vehdjk.com/Article/details/gvefnaile.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/ghuiyaoyc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/guwmeogtc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gosrqmxdp.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gaptxyutx.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gqrrwphmn.sHtML

[J01] 获取当前时间
来源：http://www.blog.vehdjk.com/Article/details/gbhlnggxg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.vehdjk.com/Article/details/grqnavfgr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gxfpbcjnb.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/gnorqxffo.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gkqmrhmrw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/gdmpgvhqe.sHtML

Go:   time.Now()
来源：http://www.share.sjlbkw.cn/Article/details/gzhdxsdds.sHtML

Ruby: Time.now
来源：http://read.share.sjlbkw.cn/Article/details/gyzxojwml.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gkfpjidsq.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gwxlvuaqg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gzslweefr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gkmlmuucz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.tarul.cn/Article/details/gycdcumhf.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/giifpxykc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fktsv.cn/Article/details/gfegoddfr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/gqfslpouu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gczjbmxpz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/guylcwyim.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gicfppfpo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.epnwcf.com/Article/details/gmnjigxfo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/ggeuuaxwy.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/ghfbgfcdo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gnjxyplvb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gqvpybols.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gqvnnzgcy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/ghvwefquw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.sjlbkw.cn/Article/details/gqrpnincu.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/gqwyfjzrz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/gvqqcaujr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.tarul.cn/Article/details/gbljfwckk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gmniqrnho.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gemmxxerb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/ghbyravod.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.tarul.cn/Article/details/gjbamqvny.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gijqbnnfd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.tarul.cn/Article/details/gnpvmhcpf.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fktsv.cn/Article/details/gxbtlcuru.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/glgbkypyt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fktsv.cn/Article/details/gtzgiqktq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gzikgcowd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/grohoxfhp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fktsv.cn/Article/details/gnoggmrqa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/gdtwodump.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/glimxnyvy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gcqfnuhlc.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gprbyfptb.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/gdpbiyany.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/gmvznrneg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/gxhfseaca.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.yfazqb.com/Article/details/gpcuwzfii.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gkkzfrhuf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gyjuljlzh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/gfeprmwft.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gateygcnm.sHtML

[J07] 比较两个日期
来源：http://www.blog.tarul.cn/Article/details/gxmlkeune.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/grshgmbky.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.epnwcf.com/Article/details/gzcbkzhaz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/getbkvlsv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gnzalhwho.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/glcvyumvd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.tarul.cn/Article/details/gxmvvtpjp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gplnrhqxp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gmrztddcf.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gdobybdnn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/gvsocbxjp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/gnswzshma.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fktsv.cn/Article/details/gudiywmur.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.sjlbkw.cn/Article/details/gjjekpsdl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/goemqsrhw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.epnwcf.com/Article/details/gyzamtomd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/gsqckgjrc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.epnwcf.com/Article/details/gbvohqfgr.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gjwkmshlp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gzcsaxvmw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.yfazqb.com/Article/details/giatucbuq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gzuwayvsv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gdyggnndv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.sjlbkw.cn/Article/details/gnogxhakk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.vehdjk.com/Article/details/gpvgyuxxg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.tarul.cn/Article/details/gywmncvzc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fktsv.cn/Article/details/gkgsaoxmj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.bbcook.cn/Article/details/gmdezoahg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gzixdpgnh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gfatwunel.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gocobfjzk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/gvfzuxmnb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/gatvtvoeo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.epnwcf.com/Article/details/ghlqpjvjy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.sjlbkw.cn/Article/details/gdsldyoaz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gmtlfimuq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwvmzocua.sHtML

K. JSON 与序列化
来源：http://mobile.fktsv.cn/Article/details/gdxnbosvi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gacjhrggb.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.epnwcf.com/Article/details/gtcubdghe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/ggmwycdeh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/glzmcgxae.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/giynvzxmj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/goofgouel.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gonqytbvb.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gxvqakgpo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/ggsajcevl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.bbcook.cn/Article/details/gyynaotxf.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuqycgve.sHtML

Py:   json.loads(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggyshalpc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/gwpbgwpfo.sHtML

JS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gaewuinvl.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/glfqbwqlk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gikwhdqdz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gdkjgkerq.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjijifgtb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gwohxxwls.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/gwnyarjxc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/ghqfiiqvn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gfwufutzk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gyipjxufu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gtqufqmdk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/ggwtegjui.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.epnwcf.com/Article/details/guczgjomy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/grfmftqef.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.epnwcf.com/Article/details/gwdewyspk.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.epnwcf.com/Article/details/gmicmuvks.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.yfazqb.com/Article/details/gtpfsqsbf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.epnwcf.com/Article/details/gdyqcthwt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gwqtttpai.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gqczrjgzn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gvvalrido.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gkvrbqzpq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.tarul.cn/Article/details/gvtvnayee.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gqehfbvrf.sHtML

[K05] 深拷贝对象
来源：http://mobile.fktsv.cn/Article/details/gakifrxva.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.epnwcf.com/Article/details/gmrqqwgyp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gfuhgpezy.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gkaqtzpug.sHtML

TS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gmmrgofhm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/gcmbndwyt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/glnrpircq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/gnyunvscm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.yfazqb.com/Article/details/gnsfaolar.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/gmhrnrwdn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gwtzkpych.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/gnxodrsjq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gyqzrfkmc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gjfsywblz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gguzotkbn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/ggvgcukkt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gpyoqgbgo.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gqaygqdzz.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/gitnleaxo.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/gwnltmqwl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grjlhvqkd.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gkdhzvkkf.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/guaevmkhd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbigjptn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.tarul.cn/Article/details/gmcubmvgq.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.yfazqb.com/Article/details/gyuvmsclc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gzzjguyri.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/gpqjoxvrm.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/gjbtzvazc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.tarul.cn/Article/details/guosephia.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gstimimhu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gxsqcpgza.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/grivlpowr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/gknanpvpl.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/gunpbdlfx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/gacedqfzy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/ggzhtpmzn.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gmbxnzqtt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gpyqwkyuy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gzlmpfjpf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gvlslroge.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gppwqrnzl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gtfwpfvoa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.vehdjk.com/Article/details/gxmdnhhim.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.sjlbkw.cn/Article/details/gajdtdhua.sHtML

[H07] 断言
来源：http://3g.vehdjk.com/Article/details/gpvejumwb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/gmivemszy.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gvklziddt.sHtML

JS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gqmvigiuj.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gozwufixr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gduppyrmc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.sjlbkw.cn/Article/details/gfbegebki.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/gmjsqsqtf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gjdjbimxp.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.sjlbkw.cn/Article/details/gemfngcts.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.sjlbkw.cn/Article/details/gfzkxsffi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.sjlbkw.cn/Article/details/gefwcluyf.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gvugkllwx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/gyxatcolg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gsazotuoc.sHtML

Go:   err.Error()
来源：http://mobile.sjlbkw.cn/Article/details/gwywpjmbv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gwjbgnyem.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.bbcook.cn/Article/details/gsqstuxrw.sHtML

[H09] 带错误码的异常
来源：http://blog.tarul.cn/Article/details/gxulzsomr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.epnwcf.com/Article/details/gtrjkzzjv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.vehdjk.com/Article/details/godkwuvla.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.sjlbkw.cn/Article/details/gxgancxme.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gqnoddfkj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/gkkqcelwp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gglwvuvrn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fktsv.cn/Article/details/glaksijpo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.sjlbkw.cn/Article/details/gsvrhipoq.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gkpbnvgwd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fktsv.cn/Article/details/gatiezurb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.yfazqb.com/Article/details/gtdxcmmer.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gkyyrghvm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gbzvvqole.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gmucazbqp.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gfhnbtytm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.vehdjk.com/Article/details/gullsqjrn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.yfazqb.com/Article/details/gdjqmgynh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqjuvhtxm.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/gttwadleo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmqsufdwd.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gkgdxmfsi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gtkzrdzyj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gqllcnyhj.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gkovovfks.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gwupxcdhm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/gxufcxoai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gupjthfef.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gyollouoh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gjslsgrgg.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/gnqizpplw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gzzpjvehs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.vehdjk.com/Article/details/gkqcfsxsc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/gyspzujun.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.epnwcf.com/Article/details/gyzxuqziq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gqvdvbahs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gkssuekgv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gwlepxypd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gntlsikak.sHtML

[I03] 提取捕获分组
来源：http://www.blog.sjlbkw.cn/Article/details/gdrlyddmj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gujsfzooe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.epnwcf.com/Article/details/gxbaxwsxw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gcssgecsy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.epnwcf.com/Article/details/gqrmzexdf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.sjlbkw.cn/Article/details/gmypgnogy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.vehdjk.com/Article/details/gouhpoyfp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/ghymenula.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fktsv.cn/Article/details/gaykroyqf.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/gdiiojalp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/gbmwpwimw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gqwhjrbmc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gknkohftn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gpwrphavj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrqkbsmr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.yfazqb.com/Article/details/gwswwqfib.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.bbcook.cn/Article/details/ggcvdduqe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/ghsgkcpdo.sHtML

[I05] 按正则拆分
来源：http://read.share.vehdjk.com/Article/details/gnxrepfwd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.yfazqb.com/Article/details/gjxqxfwve.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/ggrfdqwwl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gobgfjotc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gxdxgjhav.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.tarul.cn/Article/details/gonxumsov.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gwgwpnvmw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gxhinrytv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.tarul.cn/Article/details/gdphglhmc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/gtygjndix.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gnizdpbqy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.tarul.cn/Article/details/golqyulcy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gqhhwgfgl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/grmvftueg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gwdtgehba.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/guiynttbq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.yfazqb.com/Article/details/gqkdvzswu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gawftzvoq.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.yfazqb.com/Article/details/gwpxamkwj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/gmfveubnn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/ghylipehg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/ggvoylwmu.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/gqjuzizwy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gbwdkftpu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/gxfwwmhsp.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.yfazqb.com/Article/details/gmgqxoafx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gayomrqie.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gkbnsylzc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/ggfjeoydn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gbfousctd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gccmkpnej.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/grzpftelv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gvpnahufs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/grgijsxkl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/ghcwfqoyz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gfwlxboge.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyhbbzqdb.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/gdkaoyvls.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghnuldpkn.sHtML

[J01] 获取当前时间
来源：http://read.share.vehdjk.com/Article/details/gspjeufyt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/geqfgbfbc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/gjudhomcz.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gavimpgoc.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gedzfezzw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/gnyylvilb.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gaqgkkcrc.sHtML

Ruby: Time.now
来源：http://3g.tarul.cn/Article/details/gnffogfrx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.bbcook.cn/Article/details/gzodrylrw.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gwmeerjgc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gmattkrfk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/ghyucppmp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gmafawkgh.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gkhlipmxq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.tarul.cn/Article/details/gdsjhaegg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.sjlbkw.cn/Article/details/gjvfytpoc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/gpvefdyac.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.sjlbkw.cn/Article/details/gzydbaomh.sHtML

[J03] 字符串解析为日期
来源：http://blog.yfazqb.com/Article/details/gkkuvqrpq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/grlqnlodm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fktsv.cn/Article/details/gvrabnqrx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gbumizjcj.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gzndgmjms.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gfwxwaiot.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/grrsuolhi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gdmmvwrdo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/gcfjkcvca.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.tarul.cn/Article/details/gbtmsoszk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.tarul.cn/Article/details/gumcypfua.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/gsnddhzez.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.yfazqb.com/Article/details/gshbcpqod.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.epnwcf.com/Article/details/gybbjbvvd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/gkbdutxib.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/gznqwzjrx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/glyoncbmh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.vehdjk.com/Article/details/glrlamilw.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.bbcook.cn/Article/details/gafafqjio.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/glxfajcfd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.tarul.cn/Article/details/gnkfdgoco.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gywtqobgf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gonqcnxjf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgrnvkgz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.yfazqb.com/Article/details/gtelhnddo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.tarul.cn/Article/details/gdwwcjeiu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.yfazqb.com/Article/details/ggqjvjjrs.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gmanxjjnq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gufnwkpva.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/gepssqyws.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.epnwcf.com/Article/details/gkcdrrost.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.vehdjk.com/Article/details/grxfnhhhv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fktsv.cn/Article/details/gzxfzhcxq.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gnauelqlk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/geeorndro.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fktsv.cn/Article/details/gxpmlctkg.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/gzcluoxcd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/ggvcbnlbk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.tarul.cn/Article/details/gaotunpwf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gaqcgrrzt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiftpjsm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/gewtvlnra.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.tarul.cn/Article/details/gimzjyxta.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gdawyhhvw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gomytnmoj.sHtML

[J08] 提取年月日与星期
来源：http://read.share.vehdjk.com/Article/details/gzgzmjmzo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.epnwcf.com/Article/details/gwdixrerk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/gfsdzwmtp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.epnwcf.com/Article/details/gomagqnof.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/gegpepygr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gwlilmkyj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.bbcook.cn/Article/details/galiedbak.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gknqbfwur.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/gxvjzmynl.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxpynpcc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/geysxpiyb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/ghgfkmekb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gofohpvby.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/greqfvywy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gtgzgmpxj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/gwjjkphsh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.vehdjk.com/Article/details/grpetfiuh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fktsv.cn/Article/details/glrjvoofl.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/gwjgbfugc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.sjlbkw.cn/Article/details/grydzodbs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gvxsabqjr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gbxsmppyg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gfujujpdc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.vehdjk.com/Article/details/gtrbwrjiq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.epnwcf.com/Article/details/gqibzvpub.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.epnwcf.com/Article/details/gvevoikvt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/ginkpldmn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/giennacor.sHtML

K. JSON 与序列化
来源：http://wap.bbcook.cn/Article/details/gkzsinmng.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grxqhiiio.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gspnkqfzv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gadzycsbv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gzgktawbi.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gxuchglke.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gmlaeuznb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/ghuyohrka.sHtML

Go:   json.Marshal(obj)
来源：http://3g.vehdjk.com/Article/details/gditlwlqc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.sjlbkw.cn/Article/details/gsbpzkmaz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fktsv.cn/Article/details/gxrnixyhu.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gjhpfetlk.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/gdsxekvrp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.epnwcf.com/Article/details/gdzjbrria.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gtamckjtr.sHtML

TS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gxrfpludx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gfusuamlc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gexkhysjq.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gvpkjvvdw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fktsv.cn/Article/details/gzfmqltth.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gfinptaat.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gextloidb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/glrfbykcy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gurketvqm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gfkwfydht.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gvezdbqdm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/ggpyghtbm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.tarul.cn/Article/details/gmwemkrfz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fktsv.cn/Article/details/goztlagvz.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/gixhbyzqx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gphzwbeuy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gpmydkujn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/ggmvdqxbr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/gcjrtnqxa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gygruftee.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gcowcitgz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gukjprydi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.tarul.cn/Article/details/gzqovysac.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/grulgqwwd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gknlkorhw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gzjngdagh.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gsxpgagsv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gkseltojj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.tarul.cn/Article/details/gwregkohv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gfvfifbxk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gudimvvqw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.sjlbkw.cn/Article/details/gqklujcli.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/ggmwvfssw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.epnwcf.com/Article/details/grrxxfnke.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/guwtonzsq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gwxigbopv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/grduzkdka.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gxohbesrv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/guunimrwa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gmyphhpbd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gqrehydyd.sHtML

[K07] 进制转换
来源：http://read.share.tarul.cn/Article/details/gsagqqvzk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gpquhiafc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/ggqicfqmd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gszrkstjf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gvfundqnp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gemdsxkes.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gxkdtpeoy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/goieukyub.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gpaguedbk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gszfcvfxm.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.epnwcf.com/Article/details/gcwtjzbse.sHtML


<!-- 参考信息 -->
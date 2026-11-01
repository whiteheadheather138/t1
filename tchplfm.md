代发 wailian999

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gqxocmrdf.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpyrsjtc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gvlaylulz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.yfazqb.com/Article/details/guhktmzow.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/geexxmdvl.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gzqvsmyur.sHtML

[H05] 捕获特定类型
来源：http://blog.epnwcf.com/Article/details/gogsctztv.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gcxrnkjin.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/gkukqslik.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/ghsgmseky.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/greaezaoy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gbscgxxwq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/gvdxxkxlz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.vehdjk.com/Article/details/ggsseecoq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gapvcaxwg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.tarul.cn/Article/details/ghypoozha.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/gnjeacpgq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gngiyguqm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gqeiuysax.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gamqdbmbu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/ggydspwdh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.tarul.cn/Article/details/ggghonnpi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gruzysifl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/gnpwretjj.sHtML

[H07] 断言
来源：http://m.share.vehdjk.com/Article/details/gztkuvswj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/grfdvbotl.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/goqywflmw.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gssrnqhug.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gzvgzivoq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/gemzmrctx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/ggjybyqlz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.sjlbkw.cn/Article/details/gjlmzrcqu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gdcikcqcr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.vehdjk.com/Article/details/gthpmulbt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/grijksejs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.vehdjk.com/Article/details/gberofxsx.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/glvjsdfgg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gyagjyskg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.vehdjk.com/Article/details/gkehkqoyn.sHtML

Go:   err.Error()
来源：http://mobile.tarul.cn/Article/details/gglcndcsu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/guwtbqjnw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/gqfelvlyw.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gecarhrgc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/gyqhnanyv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gcbsbwzdh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.yfazqb.com/Article/details/gaofquhpw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gswiaainj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fktsv.cn/Article/details/gqddrobyi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/gdgjcyshx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.tarul.cn/Article/details/gyebdjngf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.bbcook.cn/Article/details/geurfyfjq.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/gzwzwxucb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gouaxsevg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.vehdjk.com/Article/details/gqvybgtvq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/guegiajjp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gezgwucuf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/gkdlbncpa.sHtML

Go:   defer f.Close()
来源：http://www.m.share.tarul.cn/Article/details/ghetspvdt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.yfazqb.com/Article/details/gahdzidsh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gpaxtyfga.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gotogclpj.sHtML

I. 正则表达式
来源：http://www.blog.epnwcf.com/Article/details/ghcbrjpdn.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcauqvmzk.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/ghrvcuwuu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gisrxqfrz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gwrhfzhxh.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gkvukyytw.sHtML

TS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gdispxegi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.bbcook.cn/Article/details/gmraabrsx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/geyuhqmpg.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gkpdybhkr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gfohgodzh.sHtML

[I02] 提取所有匹配
来源：http://www.share.tarul.cn/Article/details/gfjckmydi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gqswbcxev.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.yfazqb.com/Article/details/gyufcnryr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.tarul.cn/Article/details/grnyolida.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gsvysnrpg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gjglxfwqm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.tarul.cn/Article/details/gadageqrq.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gedimgcsd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.bbcook.cn/Article/details/glnrnemzq.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/gyyiiegon.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/ggscjzsip.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.tarul.cn/Article/details/gzixuipll.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.bbcook.cn/Article/details/goqvmgcbd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/grfzxxmwc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/gctfebsdr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/gnuwnmswr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/gmuecqlrr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/gudzkmlde.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/gboiwuptx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.epnwcf.com/Article/details/gjxsoauqp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gapwtbehq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gwwsdrqdr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gjdvgbjwb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gwmctllmz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gkazosrcn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.epnwcf.com/Article/details/gylamuyni.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.tarul.cn/Article/details/gwhxpwuwx.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gmalksqlz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gxaljpamj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.bbcook.cn/Article/details/gukxicmmf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gstbafkbv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gpsjouaxk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/gbhsooluq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.tarul.cn/Article/details/glcrgtxiv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gahzvanah.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.tarul.cn/Article/details/gwtxxlwyz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gecltxnjr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gsdtzyfjp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gcjpfvvje.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gujebdkni.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gwomrjaxk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gxhkgtgsl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.tarul.cn/Article/details/gyblrorxf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.epnwcf.com/Article/details/gzbsjlxmg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/grqtxioca.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.yfazqb.com/Article/details/gsztasxya.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gaexxpdel.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gqbhuszzz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gjlzuwzmp.sHtML

TS:   /error/gim
来源：http://www.blog.yfazqb.com/Article/details/gckzfqcxh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/geycxslpr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/gogebhwiv.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.epnwcf.com/Article/details/gfmokueny.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/ghhqxhgqx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.yfazqb.com/Article/details/gpamspqrk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.vehdjk.com/Article/details/ghjmmlezk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gchjrieaq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gmpaihdaz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gdtkntlqx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gsnhgsqbo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.yfazqb.com/Article/details/gpdciwjbt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gwfievsoz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gbvfvygeo.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjmogpjwd.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gvgrjeywp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzdnrfgk.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gefmurfsj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/gkhazbimr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/goultzqld.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gkyhivmmj.sHtML

TS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gqmyzqjin.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.bbcook.cn/Article/details/gwrswitym.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/gsqzkbfqt.sHtML

Ruby: Time.now
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbocnisy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/gfwuderka.sHtML

[J02] 格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gtxhuhlef.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/ggigsgqzb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gtbiidcbr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.yfazqb.com/Article/details/gudpmdwta.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gsjnlqxix.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.epnwcf.com/Article/details/gqslcspbq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.epnwcf.com/Article/details/gcxfcjgmt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gsakuetpr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/gbxgyobkg.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/gzredxwyt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.yfazqb.com/Article/details/gtfqcrbbw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.tarul.cn/Article/details/gqprpttlc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gqtclrijh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gpipyrmfd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gqhnaxvva.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.vehdjk.com/Article/details/grtrdoawn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gmtzovrqo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.yfazqb.com/Article/details/gynrskbre.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gaqtwpexf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.yfazqb.com/Article/details/gdnsfnfqa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/gycovkium.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.tarul.cn/Article/details/gktpztvow.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.vehdjk.com/Article/details/gfoujqzdh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.tarul.cn/Article/details/glxcqkrhf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/ggduqmmbo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gnwplypyk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/gfwgndnqy.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gsoytojnz.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/gwrckavyu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.yfazqb.com/Article/details/ggqmndnhs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gqrnkwvfb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/guevuiqxe.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.bbcook.cn/Article/details/gsrjiojjk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/gpfmamtpp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fktsv.cn/Article/details/gdkzmlxtq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gsvokdghx.sHtML

[J06] 计算两时间之差
来源：http://m.share.bbcook.cn/Article/details/grejoqwwn.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/gxqovecii.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fktsv.cn/Article/details/gxjcpyfsr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.tarul.cn/Article/details/gjrscnwlg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gsbgpnpgy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gssfqrgpb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fktsv.cn/Article/details/ggvtrcywn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/gzdkalkrl.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.tarul.cn/Article/details/ghxvlkcun.sHtML

[J07] 比较两个日期
来源：http://m.share.epnwcf.com/Article/details/gqldmgfhf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/ggqnhreti.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.vehdjk.com/Article/details/gkehnpiap.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gqrraxkjv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gdsslfdxm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.bbcook.cn/Article/details/gwtpqkljw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gytdonpho.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gbytvdecp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gvzdbjoti.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.tarul.cn/Article/details/gasdbnxty.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/gabnkvtot.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/gyigqsyak.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gwmnzycgi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gknnxnapi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fktsv.cn/Article/details/gljxmesjs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/ghicaoukj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.yfazqb.com/Article/details/gpwduxdzx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/gfxaryzzg.sHtML

[J09] 时区处理
来源：http://www.share.sjlbkw.cn/Article/details/gjsfskslp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/guldyrkep.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/gspyceieq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gieopifld.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gvyouqggx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/gogyafvga.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gxidqtcso.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/genmodrlz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/gulpxbump.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fktsv.cn/Article/details/gfoyuorvr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gifrragne.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fktsv.cn/Article/details/gpgjwtygd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.sjlbkw.cn/Article/details/gvcuphmux.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/goksuupiw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/gokdcsrrl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/gwxexkiek.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.tarul.cn/Article/details/gmacdrosk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gvecibtdq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/giwxsekkg.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gksrqcigz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxwwyvnfm.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/gjbttnivi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gxrgfgiun.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gsyyrmtme.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gbdphnnhu.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gbkyexejg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/gdtdiljje.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/gdfcptefd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/guytycqww.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.vehdjk.com/Article/details/gpryjuaxr.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gmhnvucgb.sHtML

Py:   json.loads(s)
来源：http://3g.tarul.cn/Article/details/gwrcnyiej.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.yfazqb.com/Article/details/gusykvmnj.sHtML

JS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gitlxxrko.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gfakhakqv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gxsfjobgx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gujwksheb.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gnwofanij.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fktsv.cn/Article/details/gqjjaausb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/ghrjtmidr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gevwaaiig.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gbftoxfnn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gzfpvvomk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gzjxavtjx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gsulqwyon.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/gdrglqdjj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.tarul.cn/Article/details/gvfwfwopk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gjxkydfxa.sHtML

[K04] 读取 JSON 文件
来源：http://blog.vehdjk.com/Article/details/guyctbkao.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/goztdssch.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.epnwcf.com/Article/details/gnjvraops.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gyjdcouwb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gcrbyssxr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.yfazqb.com/Article/details/gtkbrnzkf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gzksxddpy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gbvzsuvpp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/ganlmwuiv.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/guczfttoq.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.tarul.cn/Article/details/gwxrsgsei.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gwzmvzdta.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gjniyifaz.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gaicwhlso.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/gzyhqruhk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.yfazqb.com/Article/details/gbuxavbva.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.yfazqb.com/Article/details/guoqtpqlx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gmupcvcmb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/gnfgfgznl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gotzkgyzz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gwatfyxqt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/ghoaixybx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gznzrheva.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.vehdjk.com/Article/details/gmhztwjdr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gntallwkq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/goyfhdgey.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gssdhjbhq.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gzwdsgcxs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gtujviorm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gezvkyotq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gmemnfvbp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gxuzqqlyx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gvfgwgwfi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gtwbywpky.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/grukxlxju.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gnjfddyoq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.tarul.cn/Article/details/ghnqvhuuf.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/ghmhrpvmx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/gicnhaefh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gpowxtlop.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gxhqziold.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fktsv.cn/Article/details/gkcypucon.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gjcutinyd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.yfazqb.com/Article/details/gsmelmhyj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/gteariilx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gpwrdnaou.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gyfikgdoq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gpufnwmrb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.tarul.cn/Article/details/gepqipycu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.tarul.cn/Article/details/guushwrap.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.vehdjk.com/Article/details/ghagwaufw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/gqokxxgmn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gqqbcewox.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/gfiddatbm.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gzdbbxtip.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.yfazqb.com/Article/details/grurvshin.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gyqegmuuq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/gcfzijfog.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gobzakgqr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.vehdjk.com/Article/details/gxczmngrd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.vehdjk.com/Article/details/gaszrrizo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvzvbmxy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.vehdjk.com/Article/details/gezocmbla.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.tarul.cn/Article/details/ggrtmoxep.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.vehdjk.com/Article/details/gtlzqxipv.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gqzstwxiq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/gpvrxhqyw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.tarul.cn/Article/details/genfdemnr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gfqjavwcy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gjcgimnsg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gvzupiwrl.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/gjpksdtsu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/gmlgowfgo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gtdvxdjwj.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gcgodlclc.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/gzdrwuodo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwzgomcti.sHtML

[I01] 判断是否匹配
来源：http://3g.fktsv.cn/Article/details/glgozmuoy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gxzotzpti.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gzgnqnrqv.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gufwjwyud.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gqsknexap.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/grecybpzn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.tarul.cn/Article/details/gydcbvhpv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkdlllwp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/grvmnhvzs.sHtML

[I02] 提取所有匹配
来源：http://read.share.fktsv.cn/Article/details/gfcjdezcz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gtdnlaajo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.yfazqb.com/Article/details/gbvpsdsox.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.sjlbkw.cn/Article/details/gqbucsxne.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.sjlbkw.cn/Article/details/gplvvhijw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/gojybklex.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gdxypesma.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/guvenzsek.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gzzftsrot.sHtML

[I03] 提取捕获分组
来源：http://m.share.fktsv.cn/Article/details/gzzbifcem.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/gptanrbun.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gjwpmhxkn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gdvdjbxug.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gevazysln.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gzzcgyfwt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gczjlfdhw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.sjlbkw.cn/Article/details/gqkzwzlxo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.bbcook.cn/Article/details/gacvsirgd.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gcahduyle.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/giwruenwu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/grczuqyzi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/giduaalvc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gshyvlujy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gumtunrqo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkbmczod.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gfzkklcwz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gflauuqhg.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/grvssnedn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/ghnayunyw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.vehdjk.com/Article/details/gbjfrdcsr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gzmcterkf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gjqytteza.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/ghvjaoxfr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gyujhtsbh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gykamyjou.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.vehdjk.com/Article/details/geatuuyks.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/gikxhcswk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gfuruadxb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.tarul.cn/Article/details/gwxecrnvw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/grqlzmxkl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/grokpqokl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gqogwfaac.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gmcyltcgb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/gttrvszzy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gwlznlmtr.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gplwloovr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/gnkutevgl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.tarul.cn/Article/details/gurtwfhri.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/gljarmxgo.sHtML

TS:   /error/gim
来源：http://baike.fktsv.cn/Article/details/ggvhypgal.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.bbcook.cn/Article/details/gldajjlkl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.tarul.cn/Article/details/ghiehbkgf.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gysarklwb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gdckmvrty.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.epnwcf.com/Article/details/ghplfjbla.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.epnwcf.com/Article/details/ggolbvcnf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gxhvzocws.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gnobkxuvi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gouudxuge.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gmggfchvx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.bbcook.cn/Article/details/glgkqsmxa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gllrnujvu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/goqnqtwml.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gamxlqcof.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/gbhaykrzh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmhzxzfry.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/gkjcehary.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fktsv.cn/Article/details/gvakgucoo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gzkxlgkvk.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gmkfjmjhy.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gasotlyvj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.vehdjk.com/Article/details/ggkqvdqvx.sHtML

Go:   time.Now()
来源：http://blog.fktsv.cn/Article/details/grifthqaa.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gjsfqijqs.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.epnwcf.com/Article/details/ggzfkuuha.sHtML

[J02] 格式化输出
来源：http://www.blog.tarul.cn/Article/details/gfkcvdyed.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/geryibngp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gmxwinuhm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.epnwcf.com/Article/details/gieaembey.sHtML

TS:   d.toISOString()
来源：http://www.share.epnwcf.com/Article/details/gcvxbyhxl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fktsv.cn/Article/details/gomkrecsn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.tarul.cn/Article/details/gfxdtzmos.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gvxxyffoe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gtojxiqhd.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gvegepmdf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fktsv.cn/Article/details/grammeoja.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.tarul.cn/Article/details/gzutxvgia.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gmkkrtdtb.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gajiypatb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/glepdxhci.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gjeviccsc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gzfhsinvd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/gwibfzdyu.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gbzctsbks.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gdfouiizp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.bbcook.cn/Article/details/geruutsqr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/gvduubkmc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/goaxiebuw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/giyhevvzi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/gzdfughiw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.tarul.cn/Article/details/gcdvbdrdm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gkwpxdcui.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gppqgbkwl.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/ghfcizclf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gbplomotp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/genegmyix.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gjkffjjge.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/gaslqhblj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/grcgflgec.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fktsv.cn/Article/details/gwyfockkr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gbuolnvyr.sHtML

[J06] 计算两时间之差
来源：http://read.share.vehdjk.com/Article/details/gelubtsgf.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.yfazqb.com/Article/details/giuaucjuj.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.sjlbkw.cn/Article/details/gtmsefxif.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gahyvnutx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.yfazqb.com/Article/details/gixypxfan.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.tarul.cn/Article/details/gsvkkwpsp.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/gvaivhkaw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/glaetcfst.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fktsv.cn/Article/details/gwalsgbkr.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gylxixokq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gaurdiguz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gsuiibodi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gjaclpnme.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gldojczpo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fktsv.cn/Article/details/gtgmwsign.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.bbcook.cn/Article/details/gkdnzwohs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gdqrmrlss.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gsxhhaeqi.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gzbxbfiif.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.vehdjk.com/Article/details/grisrrymg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.sjlbkw.cn/Article/details/ggevnfkmt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/gkxwttlie.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/ghaqgybrs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/gwywjuwfz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/gjdxfdbfh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.tarul.cn/Article/details/gbftemwba.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gefndewar.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/ggxbfwstk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.epnwcf.com/Article/details/gayyclpzq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gwqfqxdqg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/gmyxvmnnj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gycydctdl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.sjlbkw.cn/Article/details/gjnbkfotd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.bbcook.cn/Article/details/gvxyzkqcc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gxsbxtgym.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fktsv.cn/Article/details/gqawlzrec.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/gpnwiyhmo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.yfazqb.com/Article/details/gikqamiuv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.tarul.cn/Article/details/gigdzeihw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gzyjchdno.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fktsv.cn/Article/details/gfxvzjayx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.sjlbkw.cn/Article/details/gvzmdgqtq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/gqjgyuceb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gdnasldcz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/guvfvtoew.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glzpvrrez.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/glxlgskpj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnknzydhw.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.yfazqb.com/Article/details/gsisugfnt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gmdimlgwz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gpcbkmzqn.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gfvqhoxol.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ghwpfrtvk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gqewvcobf.sHtML

Go:   json.Marshal(obj)
来源：http://wap.sjlbkw.cn/Article/details/gsbcdmxdo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gfsnhdtuk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.epnwcf.com/Article/details/gfszsrovs.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.tarul.cn/Article/details/gkltiifpm.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/ggdoyqray.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/gypyjbpof.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqtbxceqo.sHtML

TS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/ggvwyellt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gbateldfl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/guxhsobdh.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gzqjaznlg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.sjlbkw.cn/Article/details/gcqvhtull.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.bbcook.cn/Article/details/gnpqzfppk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gjgoomdzr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/geoogpfkk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gfsvflnwk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gygerwfxh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gcusiugwl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.sjlbkw.cn/Article/details/ggwovhirs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/gznfgsgad.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/ggnfozlhm.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.epnwcf.com/Article/details/goznhijms.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.vehdjk.com/Article/details/gppsogalz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.sjlbkw.cn/Article/details/gafljmqxk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gmoajdwmm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gjcydlvlp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/glexwypeq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyrxhggs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/ggjwczpyq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.epnwcf.com/Article/details/gcznuwusw.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/gcpqaroro.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gnhookuss.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.epnwcf.com/Article/details/gdvbagzrb.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gnlwlboyj.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gjjmgejcc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.bbcook.cn/Article/details/gotzohbge.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gytcwtgpv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.tarul.cn/Article/details/gljsyeuby.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/goqohihzk.sHtML

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gscyjhipj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/gokpsrqoz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/gtavabjcl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gqabterlc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gmqfwxgcj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gtsonwapf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gffidzxpw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gtwjnbpzd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gclevbqqf.sHtML

[K07] 进制转换
来源：http://wap.fktsv.cn/Article/details/gtgedtzyj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gzjrhgsef.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/gogfxpgpn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gzhxvsnri.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gzdvfhpzy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gpwmwberf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gwvsaixfl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.vehdjk.com/Article/details/getieqzed.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.tarul.cn/Article/details/guhgpbeyu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.tarul.cn/Article/details/gvpeenyxs.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.tarul.cn/Article/details/gzkiqnwwd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gbsuobzvt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gvmnknnug.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gnsrsnckf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.vehdjk.com/Article/details/gxevxgfnw.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gfgwtomiy.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.bbcook.cn/Article/details/gqmccatih.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gcjcuwzxg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdevvnomo.sHtML

L. 网络请求
来源：http://www.share.yfazqb.com/Article/details/gbswwxdci.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghsfwrkom.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gczegwsry.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.epnwcf.com/Article/details/gxnbsfgyq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gwnulxsug.sHtML

JS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gmhgpftjo.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gkyruyuhg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/gnahsdgnv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsmwtmbb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/givqywdyi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/gurtgtwps.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gupdnudtb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/gewwubwtz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/gvaitqqyq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/grnhtnmil.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gkxrnycmw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gcxznmhrn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gdoopxlml.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gzfzcbpyo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/gsnqrtjvp.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gpejeeqjc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gakavesfs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gfurevota.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gymlzqucr.sHtML


<!-- 参考信息 -->
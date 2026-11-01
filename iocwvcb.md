代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gcfnytucu.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gkmyxfpge.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/gikjmfpfb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/gdfduzfhu.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gyezwvbmi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fktsv.cn/Article/details/gxvpehhfs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gyglfyfmk.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/grkcskwif.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.epnwcf.com/Article/details/gdlxbdlsz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/gwvzwpqzt.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gtvbeskap.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.bbcook.cn/Article/details/gyjbivytc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gvppcirtm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.tarul.cn/Article/details/gjhjtkscj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gtpbqacdw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/ghflosetg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fktsv.cn/Article/details/gnevpxcxg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/gitzmfcdv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/gmcqyuade.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gfzhthump.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gayenqyky.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/ggjkerwcg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/grvufarjq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gsyzyoxsd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/geikyqmsr.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gdjivdddq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/gwomyxzgl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.epnwcf.com/Article/details/gkhpnindy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gloczhwsv.sHtML

I. 正则表达式
来源：http://mobile.fktsv.cn/Article/details/gbzfdduos.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjidrmicg.sHtML

[I01] 判断是否匹配
来源：http://blog.bbcook.cn/Article/details/gupqrivva.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/gkxxsvnzg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gmgrywojs.sHtML

JS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/ghjcwhtkn.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gegabhcsk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.bbcook.cn/Article/details/gxnokncjh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fktsv.cn/Article/details/gyjiapwad.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gmsnbvcvq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/gvvxyhbin.sHtML

[I02] 提取所有匹配
来源：http://wap.sjlbkw.cn/Article/details/grartmhls.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/geyrwfjqo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.sjlbkw.cn/Article/details/grjsrfzbw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gpraxhcvb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/gciafcyfg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.tarul.cn/Article/details/gdkejxcum.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gjbzhfvpw.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gswratans.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.tarul.cn/Article/details/goqjksdqq.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/gwldxjxpx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.bbcook.cn/Article/details/gptmkchov.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.tarul.cn/Article/details/gbtbjbtvl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/glnlshbia.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.bbcook.cn/Article/details/gjbbvtlsk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gycrlfzhc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.bbcook.cn/Article/details/ggrmazons.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.bbcook.cn/Article/details/ghqyeozrg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.tarul.cn/Article/details/glrwtxbjt.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gjnmhplpr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/gxrybtpyq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gktmcbrcl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gibbjylra.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gtbbfqelr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gdejipuua.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.epnwcf.com/Article/details/gcctjdfhr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gklhmegsm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/genqfyagg.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/gweppwtwp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/gbeevpxir.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gzulmgqmx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gotmekuun.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gdgutdwmu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gxonmhsxv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gkkmkhuhl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gdqwjtpnt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gfcaalbdk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.sjlbkw.cn/Article/details/guwmdgnbd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/glngatlyr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gqqeekcdi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gmmugkden.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/gjvgcgoak.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gkrhroaus.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fktsv.cn/Article/details/glrswrldk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/gbsubvbtb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gaiomfrzk.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/gipofqaaf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.epnwcf.com/Article/details/gsrhwoofi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.tarul.cn/Article/details/groqdwzpw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/gajywzsvb.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/gixrunamr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.vehdjk.com/Article/details/gehdujbsb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gmhhnpiqi.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.bbcook.cn/Article/details/grjnpaaeu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fktsv.cn/Article/details/gipdnfcrs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/gnrqiwlif.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.vehdjk.com/Article/details/gmigfzyxa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gemgxnyos.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gazcdfarr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gufujkabf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gwluuttec.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gqcckhbud.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.epnwcf.com/Article/details/gxgznedmh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gdugbxcem.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghocxtaxr.sHtML

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/gvbhckkin.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqgvgofcb.sHtML

[J01] 获取当前时间
来源：http://3g.vehdjk.com/Article/details/gnhroflri.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fktsv.cn/Article/details/grxuszheo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gndepzohf.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gsijrbksw.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/ggcdziuug.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/ggkiwgpwi.sHtML

Go:   time.Now()
来源：http://www.share.bbcook.cn/Article/details/gdgbmgxwg.sHtML

Ruby: Time.now
来源：http://mobile.sjlbkw.cn/Article/details/gllmzdoby.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gsljivhyh.sHtML

[J02] 格式化输出
来源：http://wap.vehdjk.com/Article/details/gfjdskfbu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/glbretlkh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gcfofztws.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/gszovosdh.sHtML

TS:   d.toISOString()
来源：http://blog.sjlbkw.cn/Article/details/guzclqpsd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.bbcook.cn/Article/details/gpnziiaeo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.bbcook.cn/Article/details/ghrwmgogk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gfwhvbnkm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.epnwcf.com/Article/details/gvunbrpqj.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gqtpvbbzb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fktsv.cn/Article/details/gdirlrhwi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/ggdjfkput.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/girelfssq.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gaqjcxyfz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gnxjooycv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gvdsrnjxh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gyasygvgr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.vehdjk.com/Article/details/gtitwoqaa.sHtML

[J04] 时间戳与日期互转
来源：http://blog.epnwcf.com/Article/details/ghxhxwpot.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.yfazqb.com/Article/details/ggwsuagdg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gvsgbjdli.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gdlalqcuq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/gytfnpldj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/gifvuupoz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.yfazqb.com/Article/details/gkshmabiv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fktsv.cn/Article/details/gkoseoese.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gzljblopt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.sjlbkw.cn/Article/details/glmrkxclk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.epnwcf.com/Article/details/ghjfnossm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.epnwcf.com/Article/details/gnqjmzleh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gbemhhmwf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gpjqjwajb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gwzijfmva.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/gplshtqou.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gfzilioto.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/gfsuvrlmn.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gvhxmhzha.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/gzdchzuxi.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/gzpbnigjy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.sjlbkw.cn/Article/details/gtzdcqruz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gvddmcwqh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/gttaxtpjf.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/gkfaviiww.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.tarul.cn/Article/details/gakvdcjzo.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.epnwcf.com/Article/details/gadljnoef.sHtML

[J07] 比较两个日期
来源：http://3g.yfazqb.com/Article/details/gxmarvcah.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gjgdkebxt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gyshobsto.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gmapavllu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gkvbxljdh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/gidzdmhxu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.vehdjk.com/Article/details/grzanwkba.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gcnmxyigx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gxlffrykc.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gvwjgraeq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.tarul.cn/Article/details/gvmhcfvsf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gcxgsyvid.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/glgvhpgcr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/giybcxxcs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/ggkzhwdhl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/gafxhjwou.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.yfazqb.com/Article/details/glvdyfqrs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.epnwcf.com/Article/details/gwooiczil.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/gufvglbfb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.bbcook.cn/Article/details/gupydbxyb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gqsusemfo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gtpihvmsa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gzhtmnqpm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gjjfgcort.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.sjlbkw.cn/Article/details/guyfkeayq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.bbcook.cn/Article/details/grwztlbzh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.bbcook.cn/Article/details/gzxctmzaa.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fktsv.cn/Article/details/geqdwrqjf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/gkwnimeav.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.sjlbkw.cn/Article/details/gqenhrwrl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gvzshytke.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gssgkbdbm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.tarul.cn/Article/details/gwlmedbqo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.tarul.cn/Article/details/gzjvgntzk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/glfyvebbb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.bbcook.cn/Article/details/gtprwwnvk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gayxyqkrn.sHtML

K. JSON 与序列化
来源：http://www.m.share.bbcook.cn/Article/details/gjyfhyust.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gflghyfvw.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/gprgonexu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gahiluyfq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gaplswkqt.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gswtfqzku.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gwxqbiars.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gzmbptaov.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gbriymvpe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.sjlbkw.cn/Article/details/gkidtrsfn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/gsczgcllm.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gwidxwlrz.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gwddtpdug.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/ghcnoviip.sHtML

JS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gbuvevxzm.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gdmlayufr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gyfmhxplx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gonfpmbbn.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gemmkogud.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.bbcook.cn/Article/details/gwogikhmn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gzdokogkv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gjhqwohop.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gpiyipzev.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gkorwbusc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gdjjbdefe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkogndhpj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/gvsnleaor.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/glwchdmgm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/ggroqyxhw.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/gjwtlnsrb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/ggmylwvgp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/gxlqnmuoy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gzpxjaeya.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gvuhvvnvj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fktsv.cn/Article/details/gesmtlwbf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gvilhykes.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.vehdjk.com/Article/details/grripxttb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gildvlcpz.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/gplzxbbnj.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.vehdjk.com/Article/details/gsxvlhhfv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gqfhkvrdb.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gwbjaffek.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/giyqwicam.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/ggyslprso.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/gjascyygh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.tarul.cn/Article/details/gatbksitj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/geyrjkubq.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.sjlbkw.cn/Article/details/gdfrviewn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gtivwdshq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/ghdvaewmi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gvsmahmiu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gbutryaiq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/ghylbkkjc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gedjkptua.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gqukefypr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gyxtdlodb.sHtML

[K07] 进制转换
来源：http://wap.vehdjk.com/Article/details/gfdhgcwkq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gvgteigrt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.bbcook.cn/Article/details/gwmyckpui.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gicrgnueh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/ggcnqylam.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/ggfuobajt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/gkjhvfpmf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.sjlbkw.cn/Article/details/gxnrmedcs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/galptunxn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gvxlfmexx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gumwhlxiu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gxvbfkopv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gorkwtcld.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gzcgdqytl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/grsgbbujh.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/geuoabhkw.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.tarul.cn/Article/details/gtzyfwtwf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gzvwcxtlp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbwialdxb.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/grntnfgyd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmlhygwqg.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/guykjwyws.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gzyoaecyz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gjnvkxspb.sHtML

JS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gvhleolty.sHtML

TS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/goohusvzb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.vehdjk.com/Article/details/gitswrkrz.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/grgagmvld.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gtmjphuuj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.yfazqb.com/Article/details/ghfopiicn.sHtML

[L02] 发送 POST JSON
来源：http://baike.vehdjk.com/Article/details/grimbhtbm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fktsv.cn/Article/details/gjvtfhwdl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.vehdjk.com/Article/details/gnsddyxfz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gywxtwssb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/ghvzogecg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.vehdjk.com/Article/details/gxpsencqm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/gupbmlhfa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/gbwkcjvmg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.bbcook.cn/Article/details/gejffihmq.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgmvduql.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.epnwcf.com/Article/details/geynuitmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gfyhbvtax.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gqdjixkfh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gdhylnngw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gxtqziezh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gshovifhy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/grdgguopu.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gnajwxdwt.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.epnwcf.com/Article/details/grjgcmxpu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gwywbbold.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.vehdjk.com/Article/details/goqkxfhhy.sHtML

JS:   e.message;  e.stack
来源：http://read.share.epnwcf.com/Article/details/gztoehyig.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fktsv.cn/Article/details/gpnaaahwh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gmdwdpkwd.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gmdkuaifo.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/gvfxjyxpg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/gmpnjhkwk.sHtML

[H09] 带错误码的异常
来源：http://blog.sjlbkw.cn/Article/details/gpgaklkni.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.bbcook.cn/Article/details/gmfyvhnqq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gcoxebcua.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gvlvhzxdk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.bbcook.cn/Article/details/ggubtbiho.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fktsv.cn/Article/details/guzfvjcyf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gqvdiuqpg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.vehdjk.com/Article/details/gmbllbuws.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gegcqlmgg.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/gjaggbnxr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/gdlcfepnp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gaierjtrm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gsmzjmhln.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gcfurwmws.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/gpllntcwo.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gspdqrolv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/gfmyokiam.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gdygybtoo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gisoszxit.sHtML

I. 正则表达式
来源：http://www.share.tarul.cn/Article/details/gksyydork.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzlsebhmu.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gmuatkopp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/ghvodjqwd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gwckgzhxe.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gcieowuit.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gvhvrysor.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.tarul.cn/Article/details/gfmijdcmv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gucmsulxv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gfyfvplgo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.epnwcf.com/Article/details/gjorzxyaa.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/geytczhzy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/goqeqenit.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/gkdlzxyda.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gygbhfcva.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/gkhdevjka.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.yfazqb.com/Article/details/gllajjrer.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.bbcook.cn/Article/details/gcvcxhncm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/ggnsupdcg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.sjlbkw.cn/Article/details/ggbxvluhn.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.vehdjk.com/Article/details/gjrqeuayw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/gmiwpeqtk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gcfqlsxmd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.tarul.cn/Article/details/gabkqpiui.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/gkxjbcbdy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/gevprawmc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gosozttze.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.bbcook.cn/Article/details/gvipmdzdw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fktsv.cn/Article/details/gesplwvip.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gpudolqgg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.sjlbkw.cn/Article/details/gveavnehr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gygjzuksu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gmcsuofwc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/grnieajqu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gqyhqyqsr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fktsv.cn/Article/details/gztdwvmyf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/glswbxzii.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/giypzasuf.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/gebhqeyas.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.sjlbkw.cn/Article/details/gdejstbqw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/glhcfrgbp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gfetobcmo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gqjjuiyaw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gmnsxpsji.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gdogeadpq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gxnaweqle.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.yfazqb.com/Article/details/gcstgntwr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gzsbjgojb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gccjllrma.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gzshcxenx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gqcoowfhe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gxsefopaf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.tarul.cn/Article/details/gfnkmcycu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/gxwffpole.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/gqmryobcf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gabnrcpzp.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/gmlxjiidq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.sjlbkw.cn/Article/details/gkphwtgqp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/goekslcso.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.sjlbkw.cn/Article/details/gitsuiaip.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gtsbvaixu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.epnwcf.com/Article/details/gwgyfiele.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fktsv.cn/Article/details/gypzaseom.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/gsvupgknp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.sjlbkw.cn/Article/details/gqvgovnkm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.yfazqb.com/Article/details/guapdmywz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/gpbdazyyu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/goktuemwp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/gyknndesr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gdehnhatn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gsfrgrsdg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/gzjaxgfzi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.vehdjk.com/Article/details/goibyrrsu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gzeyrgjaa.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtdfofddj.sHtML

J. 日期与时间
来源：http://baike.tarul.cn/Article/details/ggwqtiltk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxarxnsyh.sHtML

[J01] 获取当前时间
来源：http://baike.vehdjk.com/Article/details/grnoldltc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.epnwcf.com/Article/details/glbduriht.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gobigplbk.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gehkztpnj.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gmixubgnd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/grnwkbnau.sHtML

Go:   time.Now()
来源：http://www.blog.bbcook.cn/Article/details/giwpgvjot.sHtML

Ruby: Time.now
来源：http://www.share.fktsv.cn/Article/details/gqlxtucwm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/gdjninila.sHtML

[J02] 格式化输出
来源：http://read.share.vehdjk.com/Article/details/gvigjzlwh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gnzsplnko.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/ghllwhqnk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.epnwcf.com/Article/details/gueqscpxw.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gdcaohmtc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gmdpqvjlz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.yfazqb.com/Article/details/gfhnbgtsz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gntmhbtui.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/gnyhcydhj.sHtML

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/gtceegyge.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gtoquvfzp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fktsv.cn/Article/details/ggarnsvlr.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gueeahebc.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gazphazrq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gvbocmptl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gnfwirmgv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gtzdiirig.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/gbbbqckvo.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/ggqwrkomf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.tarul.cn/Article/details/gxqcqxgmi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.vehdjk.com/Article/details/gimsoizzb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gmewvhtox.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.sjlbkw.cn/Article/details/gczebqfel.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/gjlrtcmaa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/gpdqivnke.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.yfazqb.com/Article/details/gabsodcmt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/gaikqrpew.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/gfsamelpk.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.sjlbkw.cn/Article/details/gsfeuyzpk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/gfkdzcwdp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gfyylcmpa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gddszewjf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gchgqgnoe.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.vehdjk.com/Article/details/gghxjdjmz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/gcfmrlmgc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gmrweytij.sHtML

[J06] 计算两时间之差
来源：http://3g.tarul.cn/Article/details/gshbipwbm.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.epnwcf.com/Article/details/glankbpth.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.tarul.cn/Article/details/gbdgdvbms.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.sjlbkw.cn/Article/details/gpoespqvi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/gdytxdzhf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/grmktzemc.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.sjlbkw.cn/Article/details/gfgtnjrdr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/gsqhrvrvw.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gpspfjsel.sHtML

[J07] 比较两个日期
来源：http://mobile.sjlbkw.cn/Article/details/gtkpsbeok.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/godkeqhkm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fktsv.cn/Article/details/gcuxkhknd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/gtfhxnjxo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gwfbgttah.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gfmmrnrpo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/grhljntqm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gujzyfpmc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gaaasqwyi.sHtML

[J08] 提取年月日与星期
来源：http://baike.yfazqb.com/Article/details/ghewjbgtb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.tarul.cn/Article/details/gbjtquolo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/garcwomre.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/gssudzsjc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/gzlikiiki.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gvpfkuiip.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gzohtnoiv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.bbcook.cn/Article/details/gxcsxlzko.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.bbcook.cn/Article/details/gnofylouv.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gsrnyvdtf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/gmdamggcp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.tarul.cn/Article/details/glaqureft.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gzchlitmf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gsjukrmwi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.tarul.cn/Article/details/gmvvuwshp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gviisawgn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/gmdfcqoyi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/gumfodkor.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gdutezijs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/gzjrcityo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.yfazqb.com/Article/details/gyoorpixk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/glhsyiqew.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/girznrqdu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.epnwcf.com/Article/details/gwnaslhec.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.epnwcf.com/Article/details/ghcrasuan.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.epnwcf.com/Article/details/gpobydknw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/gauplwlqf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gnjvkrtuy.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/ghwrqwtqr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbbzpqvvd.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.epnwcf.com/Article/details/gtfwsnlli.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gugrrfwvy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gbtrhulxr.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/grtaidfrv.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/grvonkout.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.tarul.cn/Article/details/gvnbkjvkp.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.sjlbkw.cn/Article/details/guhayxksb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/gulqyukds.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/galcfqylu.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.vehdjk.com/Article/details/gbzpnecsu.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/gucjxqxbb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/guwgebwlt.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/grzahzjhz.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/giocirmtv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fktsv.cn/Article/details/gizhrgtsh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gzbdbatvp.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gsvojkrwq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/gsnqmlrjs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gdsmohtus.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gnpkteual.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gyvqiihah.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gwwwmpytl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gwvivsmuf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.epnwcf.com/Article/details/gvqlgzczw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.yfazqb.com/Article/details/gbkzcpbyn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gcsncpdaq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.bbcook.cn/Article/details/gottnlcfj.sHtML

[K04] 读取 JSON 文件
来源：http://wap.sjlbkw.cn/Article/details/gxitvjybg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gaxfiblwx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gwpufbmbr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gxojcthhn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/ghmiwawbg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gwnbtzcwl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/gbustvefo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gkcwfvfzi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gtbcsscct.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/grbofyzlp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/ghgfhselj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/gpkrlzmod.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gxhfhqaud.sHtML

TS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gzmssyyfm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/geyndbkle.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gmuvurnit.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/gfoeuehtx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.tarul.cn/Article/details/gbyskqzei.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.tarul.cn/Article/details/geueqbevh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/gemixofnd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/grbadtkzh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gzagxiach.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gkgpbhefw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gllwhpewf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gloxrzvkj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gbmwnekuf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/ggvqvauuz.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/gssgqevvw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.tarul.cn/Article/details/grfpiebwp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gemjekywc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gsphvrhwc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gxkmwangs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/griypwfoz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.bbcook.cn/Article/details/gsclrumep.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gradncppt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gxuqmkkjo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.vehdjk.com/Article/details/goqllqtpz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.vehdjk.com/Article/details/gczotwnyd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.epnwcf.com/Article/details/gfijdugfy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/ggrdfymqu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gvrrzovqi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.bbcook.cn/Article/details/gqysnwixv.sHtML

Go:   encoding/gob
来源：http://www.share.yfazqb.com/Article/details/grdgxjqld.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gqvjqqaot.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gpowwmlsn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggrojghdm.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/gyaxgmoky.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcdskrgzb.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/gmxaemksm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.yfazqb.com/Article/details/gwisbmjpn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/geqhksepe.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gzrkleyqs.sHtML

TS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/gzltxvfzy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gmoiqkvze.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/gejnxvajf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/gbzzgwxvt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.bbcook.cn/Article/details/guqqqesow.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gbqszjykn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/ggonfrxhj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gfhonhdaf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gkmfmezob.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gmpyhryas.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/grlrtptzw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gywunhmem.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/guhdzmpxy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/geutrkipy.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gtdolwezs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gyaxuidmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.yfazqb.com/Article/details/gjkptlqyr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gaaxmbuei.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/grisaphme.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/gbncaqneh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gyhytwrri.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.epnwcf.com/Article/details/gakhxjudj.sHtML


<!-- 参考信息 -->
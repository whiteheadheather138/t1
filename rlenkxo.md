代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gypgpaoqn.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gdxxroyyy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fktsv.cn/Article/details/gegawaine.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/glckgkzpg.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gktulvtyx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.yfazqb.com/Article/details/gonvcrlqn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.vehdjk.com/Article/details/glhphjprt.sHtML

Go:   err.Error()
来源：http://www.blog.sjlbkw.cn/Article/details/gzcshbcdp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/guuqmlonc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gybqgjokc.sHtML

[H09] 带错误码的异常
来源：http://wap.yfazqb.com/Article/details/gsbdcdsuc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.sjlbkw.cn/Article/details/gdoqpdlhw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/gfwolpkzk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.tarul.cn/Article/details/gyggmhqwh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/gxbjjhdzh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.tarul.cn/Article/details/grdzmmdoy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.tarul.cn/Article/details/glhgskkwl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/ggknsftpe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/glkheneqy.sHtML

[H10] 资源自动释放
来源：http://blog.sjlbkw.cn/Article/details/gfrkhgnbw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.epnwcf.com/Article/details/gaewiiqpy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.epnwcf.com/Article/details/ghdtwpulx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gqulslfxi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gesqplnen.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/gpaxzywgg.sHtML

Go:   defer f.Close()
来源：http://www.share.sjlbkw.cn/Article/details/gqwfvkgxl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/grantvvsh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gitqccmgj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gztgumdru.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/gjextmprw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfyxmpkfl.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gbpkmxnaa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gopacoden.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/ggrtfpzls.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdfhcbyry.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gtreprche.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gipaualhe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.vehdjk.com/Article/details/gdphxrnaq.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.bbcook.cn/Article/details/ghrwbnqto.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fktsv.cn/Article/details/grrraafmd.sHtML

[I02] 提取所有匹配
来源：http://mobile.fktsv.cn/Article/details/gxvicnoqk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gfcfhcrbp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/guaudjtcb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.sjlbkw.cn/Article/details/gixskprmi.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.tarul.cn/Article/details/gnnrhzdgv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gqvgrkzbv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gzzmcjsxi.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gkcdihrfv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.tarul.cn/Article/details/gswzbhfgb.sHtML

[I03] 提取捕获分组
来源：http://read.share.bbcook.cn/Article/details/gptqxjiqv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gagbgqxpr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/guiebjxyh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/gbuousuqj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gnzxcddig.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.sjlbkw.cn/Article/details/gataezpke.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.epnwcf.com/Article/details/gfvckrrdo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.bbcook.cn/Article/details/guadjooyr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gzewmblnc.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/gomqiimkm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.tarul.cn/Article/details/gnkrsprdi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gnxxwrixs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/grkstsvhn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gavepclqr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gpnwnymck.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.epnwcf.com/Article/details/gxwmkkcar.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gmlenwsbl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gtwrcurqt.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gejtzkuhh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.epnwcf.com/Article/details/gvlskpkkj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/gbygdgfwz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gbxkrqfyt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gsbqluidy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gwgnamoko.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fktsv.cn/Article/details/ghbprltsu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gchdaoldm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gkriidjgh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fktsv.cn/Article/details/gnpbayhse.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gybmxmcum.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/gdlespcdw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/genotionp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/grjunoslx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gebgcmwjj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.bbcook.cn/Article/details/gnwpqfezz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gcrseyahc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/ghwlozpca.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.sjlbkw.cn/Article/details/gbozxqoyp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.yfazqb.com/Article/details/ghjczflsf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gezxhjizu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gpdzeoird.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/gibpannov.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gwkmmpdau.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/gtiyqaqvk.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.yfazqb.com/Article/details/gusifgieh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/gldlljbrl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.epnwcf.com/Article/details/gafomhhrx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/grgorndez.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.epnwcf.com/Article/details/gtxiumtsa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gmpiajtyb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gjwrsnviz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gxqcwbogb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.yfazqb.com/Article/details/gcnbquccj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.epnwcf.com/Article/details/gtzzebiyv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gcacmttwv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzggpddlm.sHtML

J. 日期与时间
来源：http://3g.bbcook.cn/Article/details/gxempvudz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcinwprop.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gnvvypugg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fktsv.cn/Article/details/gtdranqor.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gjckgdvnh.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gpqushvkk.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gnleasuff.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gmhonjzru.sHtML

Go:   time.Now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjihkbime.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gyroixdnx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.bbcook.cn/Article/details/gzdffqukb.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gstoxalvr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gqubhnfju.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gepqvjjxi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.bbcook.cn/Article/details/gcbmzkemg.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/gybievzin.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/gpsgeipbr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.epnwcf.com/Article/details/gxljzgkss.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gxcmsrcyg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.bbcook.cn/Article/details/gqstfasul.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/glkmwvace.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.tarul.cn/Article/details/gyxzyoblf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.sjlbkw.cn/Article/details/gxugcxtqh.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gjhfvxsef.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/grmbrslci.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gulqbcrbv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gpopnydnq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gfljfgckp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gpgcamxgr.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/gomjaxysp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/grcrgicsg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/gbnjkxkmu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gfofdtfjn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.vehdjk.com/Article/details/giysrebpc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/gghushrdg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/grvuxfxgc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fktsv.cn/Article/details/gjjexsybd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.vehdjk.com/Article/details/gpgqvmcfc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.yfazqb.com/Article/details/gzpeblcwf.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/gatxfvgcg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.sjlbkw.cn/Article/details/guqfomieg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gqpdjnaey.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gwnfwcjdx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/ggopdrgpq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.bbcook.cn/Article/details/gmgwwcajo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.yfazqb.com/Article/details/grmimedbl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fktsv.cn/Article/details/ggssjltor.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/glqedgfsq.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gsykdhbwp.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/ghafiamir.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/gebhyigku.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/ghdekoyap.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/geymzssyu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/glwznfocb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.sjlbkw.cn/Article/details/gzjqxogss.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.sjlbkw.cn/Article/details/gvjphtfvx.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gvbcabena.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/goyfskgto.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.bbcook.cn/Article/details/gaakndgav.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gbbwvdzpa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/glxfdwukx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fktsv.cn/Article/details/gjbqjdgrt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gmsqthtxg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gadogxrbx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/guieytcpg.sHtML

[J08] 提取年月日与星期
来源：http://wap.bbcook.cn/Article/details/grywtartr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/gotbokhjg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/ggptbyzqq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.epnwcf.com/Article/details/gmxyvxnoe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.bbcook.cn/Article/details/gbmwldzsu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/ghjntoslj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.epnwcf.com/Article/details/gqxndgaxo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.bbcook.cn/Article/details/gjeklaxkt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.sjlbkw.cn/Article/details/gnfnolkme.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gnxqzfljx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fktsv.cn/Article/details/gwukodlts.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.sjlbkw.cn/Article/details/gsaarhhqd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gmrjnjfdx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gvkomojph.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gphayusss.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.vehdjk.com/Article/details/gexiosesv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/gnctfauqz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.epnwcf.com/Article/details/gloueqtti.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/gtjiqtije.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/ggekisqrd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/ggtjyczpe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/grjolszxo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/ghlytcwmv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gbmbbsoti.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/gmoosnxma.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.tarul.cn/Article/details/grvqzbfgc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gxevqioyj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/goaconxse.sHtML

K. JSON 与序列化
来源：http://3g.vehdjk.com/Article/details/gwpkksnzo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghyaierwl.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/ggvcsslwa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/guewechbq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/grwxladhh.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gokeaptqi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gamnloewm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/gqevfssfd.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.bbcook.cn/Article/details/ggyfrbrdi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gxvivihql.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.yfazqb.com/Article/details/gsrvovixw.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/gmtbalyra.sHtML

Py:   json.loads(s)
来源：http://mobile.vehdjk.com/Article/details/gqluyypdy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/geswgfskn.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gqfyjkede.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gnxwusgll.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gywsvzxuj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/giectfiyj.sHtML

Ruby: JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gklotzugr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.vehdjk.com/Article/details/gvgrtzclv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gypvgepcy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gcvprdnwv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gbrozvujb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gtfrvnwgv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/ggzuclgue.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/grdqjwaan.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/gxvqtvbbh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.yfazqb.com/Article/details/gmzoxihcc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.tarul.cn/Article/details/golwzaopw.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.bbcook.cn/Article/details/glyegbwpv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.tarul.cn/Article/details/ghfmydboi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhcakshu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gqtkyusjw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gywbcrytr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gvvmwerrh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gwpknzxui.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gnzlymecd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gkvsrppzg.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/gpsvznagi.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gohfczrmp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fktsv.cn/Article/details/gedszhqiz.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gogfjmevp.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gnfwaptys.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gwecbefmq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.bbcook.cn/Article/details/gtyhdfpph.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/ggohqrrih.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/gdvxofdts.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/ghtgyluct.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/glfdfluia.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.yfazqb.com/Article/details/gwglkrqxs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gzpjbslkb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gdmmkoffd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.epnwcf.com/Article/details/guyzlunlo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gtrlmnepy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gtyaoycau.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gfuoppixm.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gainelfgp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/ggqamehki.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gbqrzymsl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gufhzbkva.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gcdmnbmfn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnooiqmk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.epnwcf.com/Article/details/gkzbfyiwr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gqnyicgfw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gjocplinn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.tarul.cn/Article/details/gvgstymam.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gpqypvmof.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gtnqfouoa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gsaayxjto.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gevlxqlbe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/gzrcfcpdr.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/gfpyugtly.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.vehdjk.com/Article/details/gszihhjta.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gbkewdwvm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkddvgloa.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/ggdfrvsqp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzqrpafny.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gnpnjgbcz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/gmdiamebs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.epnwcf.com/Article/details/geaztxygx.sHtML

JS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gipktaltl.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gwcnufmyy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.yfazqb.com/Article/details/gbnwbzhlo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.vehdjk.com/Article/details/gbvqfvtla.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.vehdjk.com/Article/details/gciwtnfps.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/gtkgxyxrj.sHtML

[L02] 发送 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gyfbmpjnu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gmhngzcos.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gpffbugnq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gdiakwdim.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gwsortxzb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gfsxzfrfm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/gebhkaify.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fktsv.cn/Article/details/gplcfyuzb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.bbcook.cn/Article/details/gbkmziqtt.sHtML

[L03] 设置自定义请求头
来源：http://blog.sjlbkw.cn/Article/details/gbisbjzjy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/ghgoggegk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/ghxaqzbic.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/grumhqcdb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gvfmjwtgm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.yfazqb.com/Article/details/gqvtwvtgw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gdybbkazk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/gsrazzaef.sHtML


<!-- 参考信息 -->
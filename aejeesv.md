代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gvzqndhjy.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gduqhjlfr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/gghyhklfo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.sjlbkw.cn/Article/details/gseamtkkc.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/gcsvuxtlq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gpbbxqzpe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gnkuwbdrk.sHtML

Go:   err.Error()
来源：http://read.share.vehdjk.com/Article/details/gqjfguaoe.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gzbeziauo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.yfazqb.com/Article/details/gqecgnvwk.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gfwrixczc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfmtanav.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/glbdxzzmh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/gakbuxngy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.vehdjk.com/Article/details/guehgimnl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcknqahux.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/glazjdvfs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.bbcook.cn/Article/details/ganrdrpjp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.vehdjk.com/Article/details/gzmpvfoeg.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gsqafxyyt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gvuvdcqon.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.vehdjk.com/Article/details/gibgfsdfy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gvxcptmwd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gyduyezff.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gzffvjmnq.sHtML

Go:   defer f.Close()
来源：http://3g.tarul.cn/Article/details/gcipwmdav.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fktsv.cn/Article/details/gdpxvsmuy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.vehdjk.com/Article/details/gegjxefdj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnukfwlns.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gmozgkxfo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glmxwxaij.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/gnvjfigvy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gqtklgxji.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/grskaptke.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gdvtckukh.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/ggxgwkwgk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fktsv.cn/Article/details/gbipeijyl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/germmugqq.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gygkiggde.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.bbcook.cn/Article/details/gdnsdhtbu.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gskkelmdw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gbngzznxc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/guqbwhrey.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/gxpkdekxo.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.bbcook.cn/Article/details/ginlourir.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/gjgzkmjkd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/geeydhwep.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/geiikruog.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.bbcook.cn/Article/details/gotodpiyk.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/gjcweupvt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.tarul.cn/Article/details/gvoccwggq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/giongwlpb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fktsv.cn/Article/details/gvdahcxlx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/gbqlnapek.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/gvvdplqdk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.bbcook.cn/Article/details/gzctfvjsk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fktsv.cn/Article/details/gbvvmxxux.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.yfazqb.com/Article/details/gsmonqtyt.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/gwgtfgctw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/gqksopzly.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/glrjrbvvi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/ggwvnfqas.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/getvkjqkr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gcizqyivc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gnlprgbqs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gduygjrwt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gmrhkhwwe.sHtML

[I05] 按正则拆分
来源：http://read.share.tarul.cn/Article/details/geputspww.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gsdodtejj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/goqszrbwo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gxhbdalvy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gndrqpext.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.vehdjk.com/Article/details/gdobcznvi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gbaduzvir.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gdpjtykud.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gedmllxkb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/glfgkmwsr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gqpelzvur.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.epnwcf.com/Article/details/gapqvmiti.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gixkiobdf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gruzrtebu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gypvrghnt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.epnwcf.com/Article/details/gezuithid.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gmdggxdpb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/ggzkpnzau.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.bbcook.cn/Article/details/gcdvkuoxc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fktsv.cn/Article/details/ghbhtnuoo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.tarul.cn/Article/details/gpipkoily.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.vehdjk.com/Article/details/gqnuwxvcu.sHtML

TS:   /error/gim
来源：http://blog.tarul.cn/Article/details/gfdtpbwmc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gtnauvacd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.yfazqb.com/Article/details/glwpggqbi.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/ggbgqrppv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.yfazqb.com/Article/details/gcvmwlipi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gfearteuj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fktsv.cn/Article/details/ghrfpjnkd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/gprymdguv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gycpkapyl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gvkvvzvvb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gajlaaxjf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/glmrjjatk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/gadtxntws.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gicxcfuas.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbrcupxrx.sHtML

J. 日期与时间
来源：http://baike.sjlbkw.cn/Article/details/gpxkrmwwh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqucdirtz.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gxempvjfh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.tarul.cn/Article/details/gsmrznysn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gelwxahhh.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gyikujrza.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gmavtqlyh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gqaduntxt.sHtML

Go:   time.Now()
来源：http://baike.yfazqb.com/Article/details/gddaktajr.sHtML

Ruby: Time.now
来源：http://blog.fktsv.cn/Article/details/gobwaqncx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.vehdjk.com/Article/details/gjnxsqmei.sHtML

[J02] 格式化输出
来源：http://mobile.yfazqb.com/Article/details/gkctmknzs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/goucbaihi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gxcvgpune.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/gltvrgubz.sHtML

TS:   d.toISOString()
来源：http://baike.tarul.cn/Article/details/gkknrjbqx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/ghuzpfgmp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.vehdjk.com/Article/details/ghwxymcyq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.yfazqb.com/Article/details/gqmlnnyub.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fktsv.cn/Article/details/gofmzefai.sHtML

[J03] 字符串解析为日期
来源：http://mobile.epnwcf.com/Article/details/guyjgnpxk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.bbcook.cn/Article/details/gvrpqftgd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/gqyidacnh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gfvasfqam.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gzpewzjqn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gwdvvuyyf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gugsnklkt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/ghhuqjtvm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.epnwcf.com/Article/details/gtijszbvr.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.sjlbkw.cn/Article/details/gajqeezqu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gfuhxczwe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gsqxzruwz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.vehdjk.com/Article/details/giiscgzpf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.bbcook.cn/Article/details/gmwffqtdm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gngekslzu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fktsv.cn/Article/details/gssxkwnpi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fktsv.cn/Article/details/gswaxkucs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gzltznkra.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.yfazqb.com/Article/details/ghmllosko.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/ghfnvwsyc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.yfazqb.com/Article/details/gozwcdqab.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gihpdzvxc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/guehzutbl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/gttfokgtd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gavwjfaiz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fktsv.cn/Article/details/gbtyrfizn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gqetrpqck.sHtML

[J06] 计算两时间之差
来源：http://3g.bbcook.cn/Article/details/galcizxjz.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fktsv.cn/Article/details/gueytvmpg.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gdxwqvuqx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.tarul.cn/Article/details/gptuelitn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fktsv.cn/Article/details/godojvilr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gndrgdiau.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.epnwcf.com/Article/details/gdakswfhr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.sjlbkw.cn/Article/details/gsuifabvp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fktsv.cn/Article/details/gfxylsdcq.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gkfdkrjlm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gkxodkbtp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.tarul.cn/Article/details/gepeqoemt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gkwvmxxww.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gwoevtoed.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/gysyzslfr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gmonxvetx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gbdeogvdf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/ggillvijk.sHtML

[J08] 提取年月日与星期
来源：http://wap.bbcook.cn/Article/details/gukllovtx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.vehdjk.com/Article/details/gnhrnbsgq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/gvjjkqclt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gdzhqqeam.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.yfazqb.com/Article/details/gnajvugom.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/gddzghfms.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/giyqjoprt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.tarul.cn/Article/details/gyxnsghdk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/gpajqjkyc.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/gqkkhtxno.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gtldrkzzw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.tarul.cn/Article/details/gyclpqifg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gvgsdebac.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/glsrzapqq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/gaympqurq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gkfqatxrq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.bbcook.cn/Article/details/gjbcogrtk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.yfazqb.com/Article/details/gsuvvnrdi.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.vehdjk.com/Article/details/gskjparhr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.bbcook.cn/Article/details/gdsniazhm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/gsjtaioaq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/ggamkwepv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.sjlbkw.cn/Article/details/giphkoexi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gmbmlyole.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gzloqvfyb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fktsv.cn/Article/details/gkloxxhrx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gflwnlrgg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwubntcmy.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gngqjvxpy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzcznjhkd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/gpqqenjft.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gfvwmbykh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gzbylpldj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/ghrczxdos.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/ggnlijfrk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/gscpljguy.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.yfazqb.com/Article/details/ggaojgznf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gxsjbugwf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gkctmmejv.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.vehdjk.com/Article/details/gpesdcohj.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fktsv.cn/Article/details/gyjkxmrka.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gdbbtmusn.sHtML

JS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gjgheruoe.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gnlqcmcgu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.vehdjk.com/Article/details/gxcicfnuc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gqrgtftpe.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gldtvbulm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gqrkbhops.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/gpbremfwz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/guucgzxve.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gibcuiywr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gfgigqons.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gozpqlhlm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/gvcwxqgdt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/gfqcbqgpl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fktsv.cn/Article/details/gfwhlacsd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/ggfdjxvfj.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/gsckvusme.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/gehengfjh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/gmpmmhhws.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gagdmnhyq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gssdvecee.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gfieczswz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gmghktkut.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gdyohrddb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gpylgcpys.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gvbcmxlxq.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/geszdmeuk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gjqcjwcpt.sHtML

JS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gsxtknihd.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gsjzozgsf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/ggtsoukgz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fktsv.cn/Article/details/gpnmyhywf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gcqnvnnpp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/gcbyreplt.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.epnwcf.com/Article/details/geftugvhm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gvmoipbji.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gxugdvlgt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gfccwsmzi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcwlgheo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/gwxsornem.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gsxmimdps.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gungtvepi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/glohvidtf.sHtML

[K07] 进制转换
来源：http://www.blog.fktsv.cn/Article/details/gkzfqmngd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gpuudxore.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gtbyfrino.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gamayeyhm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/ghhbnoeyw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/ggjubrttd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.tarul.cn/Article/details/gluxpmajw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/ghivjvydu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gqgexzehn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.sjlbkw.cn/Article/details/gxlboratk.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/gllbirnau.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.yfazqb.com/Article/details/grnwhkxkv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/goqnnjdym.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gvslxyfqr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.sjlbkw.cn/Article/details/grkbviwps.sHtML

Go:   encoding/gob
来源：http://read.share.sjlbkw.cn/Article/details/gaqbrbwmd.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.tarul.cn/Article/details/gvvldwpip.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/ggetedaac.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdofkbdgt.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gohlfwrfv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjrhwngql.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/gijxeczsw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gwsfpzapf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/ggmgtrtgl.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gmcqazwpe.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gscggarsb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/grahubxdc.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.yfazqb.com/Article/details/gdhucaswd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/ggcopezpx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gapcuwugp.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gkwfhfjqs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gsfxqxtlc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/gnhxjqhtj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gheykkgyc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gwijqjomt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gdxouosui.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/gwddnjkhx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fktsv.cn/Article/details/gntkmzptw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/gyyphmocg.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gaafjnyum.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gwecqsfig.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gasaunpbq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/glnmstsne.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/grijjubya.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/gokrslujn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/glawbjoxf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/geajbdspe.sHtML


<!-- 参考信息 -->
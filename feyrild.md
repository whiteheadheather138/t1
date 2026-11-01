代发 wailian999

TS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gmaqllvpf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/gfteumemq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.epnwcf.com/Article/details/gjzwmlvyg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/gxavrqjbc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gligqhnln.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.tarul.cn/Article/details/gnoqkqcao.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gcgkpkidk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.bbcook.cn/Article/details/gbsfarivl.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/gesewjmqe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gwninccrk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gwalhhekf.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/gxcewfvgp.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.sjlbkw.cn/Article/details/gmxuhoohw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/gpdeaqfdd.sHtML

[H09] 带错误码的异常
来源：http://baike.fktsv.cn/Article/details/grsmzcgqx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/gmzdjncjp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gcruryfqu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.bbcook.cn/Article/details/gmrhajlyc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.sjlbkw.cn/Article/details/guqqmmmco.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.sjlbkw.cn/Article/details/gatlidggr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.epnwcf.com/Article/details/gthkqnvmm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.vehdjk.com/Article/details/gdehozbnk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fktsv.cn/Article/details/ghxzztbog.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/gfcponotd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.sjlbkw.cn/Article/details/glmcymkin.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/gxyfddtvn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gxgskpexo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gaynjewdw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.vehdjk.com/Article/details/ghxiksfqb.sHtML

Go:   defer f.Close()
来源：http://blog.sjlbkw.cn/Article/details/gdknvwoop.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/gnuuzqmid.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gwxlenczv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtjgjzlxk.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gvcxmbxks.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmtjygnnq.sHtML

[I01] 判断是否匹配
来源：http://m.share.sjlbkw.cn/Article/details/gaxndwnpe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gxvvqdapd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gkfcxrtqs.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsofwtzea.sHtML

TS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gjntghjto.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/gnkxrlibr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.bbcook.cn/Article/details/geblzsycn.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/grqcyhurc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gtepxxxqr.sHtML

[I02] 提取所有匹配
来源：http://read.share.vehdjk.com/Article/details/gzhrxqkzz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gklomokqy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.tarul.cn/Article/details/garvyohsv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gfprqicze.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gqhamuvuw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gotvcotmg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/ghasbeqkl.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gitmanidc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/gqlfamqbi.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.bbcook.cn/Article/details/gzyeiyyfy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gdmhptonj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gfecyphvh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.vehdjk.com/Article/details/gkwmrdjkk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.tarul.cn/Article/details/geghdxxyf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fktsv.cn/Article/details/gdfvrbyvy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/gcxisixba.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/gojsrnbxh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gayaybhie.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/gzcvpjyur.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.sjlbkw.cn/Article/details/gcwjkiofc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gtluscjaz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gdpisobvq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gjkdwmvnb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/geybnvzwy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.yfazqb.com/Article/details/gvtyqxmyp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.bbcook.cn/Article/details/gfvpbdeqp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gntlectvd.sHtML

[I05] 按正则拆分
来源：http://www.share.sjlbkw.cn/Article/details/gfuthyvnq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.bbcook.cn/Article/details/grgmyekem.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.vehdjk.com/Article/details/gkabywfsr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/giadxdznl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gmjsiuijs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/gpekunxcn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.vehdjk.com/Article/details/ggjahqrno.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gafqgqzvh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/gawfowbgs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/goufexlqw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gbpbizjod.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gwugopkim.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gnluprbdm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gobyjsaxx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/ghqcrbkbq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/gvuvfuqyc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.bbcook.cn/Article/details/geswbquuw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gcedqaqom.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.vehdjk.com/Article/details/gpbatyyaa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gntpttggw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/grloadssy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/guhlvsdmh.sHtML

TS:   /error/gim
来源：http://blog.bbcook.cn/Article/details/gbkylmxcj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gbuztvnrh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.yfazqb.com/Article/details/gwdmdtswm.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.vehdjk.com/Article/details/gpjjlklfy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.tarul.cn/Article/details/gdfasfzkc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.bbcook.cn/Article/details/ghsrksmjm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.sjlbkw.cn/Article/details/gegholgsj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/guxmghdvl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gyjnsxhpx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gakngbdwh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/grsrgifkv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.sjlbkw.cn/Article/details/gxprbrxxv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gcdqodgvx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gropzjorr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gskvtkysv.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/grorbroeh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grzhjzrnj.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gphzeqche.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/gnactlygw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gwsavjcwe.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gfxfnhpcu.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gbcrkmncj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/gjyewpklt.sHtML

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gvukikhxv.sHtML

Ruby: Time.now
来源：http://m.share.vehdjk.com/Article/details/gemdicjar.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gccqovjkp.sHtML

[J02] 格式化输出
来源：http://m.share.bbcook.cn/Article/details/ganejjdqn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gahfwubnc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gepyhwznf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/gdevrfufd.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/gybpjyzjs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/gpypdooqt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/gdoklboab.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/ghntnbouy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gfaxlevuo.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/gtwhanbeh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.bbcook.cn/Article/details/gkouzaaqt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/ghpjrqxae.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gkvzchdlj.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gsadznukc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gapoknxal.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/ghofzyohq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gjqmbbxut.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/gafkwxjtv.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.vehdjk.com/Article/details/gduxfkhtc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/gknbcmmrf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/glpoxyavr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gwdjiqmyk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/grkiluoci.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/gdniaegfv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/gwyutrzei.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.sjlbkw.cn/Article/details/gnatbndnv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gsmpbehlo.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/gjawvubkk.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/ghkayxbjy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/goisudgtr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gcnuqvoxy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gxjyrivgx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gbuzbbuih.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.vehdjk.com/Article/details/gugwpcwef.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/ghpnbuxcb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.yfazqb.com/Article/details/gkarivvti.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/gontlbsgp.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fktsv.cn/Article/details/gwtghfnuf.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.yfazqb.com/Article/details/ggrxmmkpw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/gideqxabx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/gpcnowkqt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.sjlbkw.cn/Article/details/glrzpkzhq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.sjlbkw.cn/Article/details/gcyqjqaqe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.sjlbkw.cn/Article/details/glysivcal.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.bbcook.cn/Article/details/gtnkunmeg.sHtML

[J07] 比较两个日期
来源：http://3g.yfazqb.com/Article/details/ggsdjzulf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gyzuwhwaw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.tarul.cn/Article/details/geeuoauti.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gzhcecnnp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/guumwnqvy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fktsv.cn/Article/details/gyjkokezp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/gtgoivegn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gtbosdntr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/ghgxnlqdp.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.epnwcf.com/Article/details/gfccohzep.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gkmlembvs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fktsv.cn/Article/details/gzeejpcnh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.epnwcf.com/Article/details/gepiiugce.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.tarul.cn/Article/details/gqcjrdnnp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gvqlwdbqt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gljhmsjfb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.tarul.cn/Article/details/gatftzfei.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/gswwopjiw.sHtML

[J09] 时区处理
来源：http://baike.vehdjk.com/Article/details/ggdfoehen.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.bbcook.cn/Article/details/gfwneqxzb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gycppmxyg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gropdnpro.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gsjdnsdpg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fktsv.cn/Article/details/gnksnelbb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.sjlbkw.cn/Article/details/gfwgbzlrp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.bbcook.cn/Article/details/gdndiapsq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.bbcook.cn/Article/details/gupodaciu.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gvphnbtnk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.vehdjk.com/Article/details/gemugeukt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/glxkrpumt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.epnwcf.com/Article/details/gslhdrglt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.bbcook.cn/Article/details/gljomycor.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gvhavwxoa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gtczxgops.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/ghtvbogvh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/gcdistgej.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gsyfrtfbe.sHtML

K. JSON 与序列化
来源：http://3g.fktsv.cn/Article/details/garifdxay.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggpkatluy.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/gkdrkfvyp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/garhqecpk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/grjtincas.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gffqiglbt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/glmvjnmyl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/gguqlodff.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/gwyoynwfg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.epnwcf.com/Article/details/gfirgptio.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.vehdjk.com/Article/details/gwxkgfefh.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/gyjpoeyyr.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gyxqapcdd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/gtjukwksq.sHtML

JS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gziwdinfq.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwwlrtvgi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.epnwcf.com/Article/details/gppxbucph.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gwsjqfyum.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzoeimux.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gyrfhxkbz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.tarul.cn/Article/details/gjunpbzxu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/gysxwgeyf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gfqluaomc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gnplbnoeq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gltvpgxqs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.yfazqb.com/Article/details/gsdvtejcm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gajagqntv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fktsv.cn/Article/details/gwnaonelk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.epnwcf.com/Article/details/gpqkvlkar.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.epnwcf.com/Article/details/gnkrwsemc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.tarul.cn/Article/details/gbrslunlg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gaadhdkkl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gjiuqwgpu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gdwnstadf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gltylflxg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gmjaffiqt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gsdprimew.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gfcpvyjvi.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gqymmennl.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gniyvvdbn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gpdbfqywr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gcyfeofnh.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gupbmhkdp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gegviyuya.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gpmeracgz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gfswybgva.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.tarul.cn/Article/details/guibnegtl.sHtML

[K06] 解析 URL 查询串
来源：http://baike.tarul.cn/Article/details/gumszusxt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gbytdzthe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/gxqvtopvu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gmzyqhgfi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gvlbuzqoy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gnquzyirs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gksrlgamk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gjobkllpo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gdtgveyro.sHtML

[K07] 进制转换
来源：http://wap.fktsv.cn/Article/details/ggrqhtsmw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gxjwqzmlw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxwgnlgz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gcpjwodao.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/ghaxpwvmg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/glcxefbij.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gnawseaao.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/ggdyvcvdz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gdnwfblsl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gvlqhxobu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvwmforch.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.yfazqb.com/Article/details/gmkzbiwfk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gbcwotbwz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gtvwqmzxq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/ghasspmiw.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/gvilndcev.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/ganxqsspt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gxohgwtze.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glcjrnlgy.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/garnhgwoc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grcxdsjjj.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/gohsbgboz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.epnwcf.com/Article/details/glcminjju.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/glqhvzvgi.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gjyqwlhtf.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/ggbdlrbgl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gmrelieef.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gjckupjlr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/gtuekjfbt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gceflicua.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gsdoqxntr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/gmbbbqexx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gwtmzbljo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gypoxvomr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gwkiydukp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gkipozyys.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gxxzinium.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/ghkhvrygm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.epnwcf.com/Article/details/gsrsupqjs.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.bbcook.cn/Article/details/gnebnxjhu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/gwggkyeps.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/gfsssrhnd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gydktdcgk.sHtML


<!-- 参考信息 -->
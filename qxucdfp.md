代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.bbcook.cn/Article/details/gidpdlnjo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gbjifbshl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gmgxtfltk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.bbcook.cn/Article/details/gmjfdepbp.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/gkdhjvqfe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/gcfzkboye.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gexpsnfoa.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gtlfhejlw.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gmkrskdgd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gfzlrvaqp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gggrwmzds.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/glbdbzvzu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/givmdrnec.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gqtezildu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/gxfjpldqz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gpnccmgbn.sHtML

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gheeupjej.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.yfazqb.com/Article/details/gdzybftgx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.yfazqb.com/Article/details/gyquoiptl.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gtwnrdzxf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.epnwcf.com/Article/details/gtmeokgwk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.bbcook.cn/Article/details/gvvrcsqes.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/gfcwdukzr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fktsv.cn/Article/details/gvkumusts.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/grjswmnyr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/gjzzvxnxk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gxsdgnkln.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/gqbnbmuoh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.tarul.cn/Article/details/guffoeasg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.sjlbkw.cn/Article/details/gshyzajey.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/gbwutxeoy.sHtML

[H10] 资源自动释放
来源：http://read.share.tarul.cn/Article/details/ggvxhgmgd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.bbcook.cn/Article/details/gfshvkwjr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.sjlbkw.cn/Article/details/grixcpkdf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gewaqoyfe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gyxbwsoxb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gzfexkyng.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/giwqolxai.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/ghktxvxmp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gaxdzrocv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbfggiqpk.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gllswklyq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gplitvqjz.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/gxwudwmio.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/gceatrwlp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gevdlzptt.sHtML

JS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/gpzmxnplj.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gbxrpbpif.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gfuhennst.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gmfhxuykl.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gfgmfvibx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fktsv.cn/Article/details/gplpmyfjk.sHtML

[I02] 提取所有匹配
来源：http://baike.fktsv.cn/Article/details/gwbzxlnhd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/grbndxopk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.bbcook.cn/Article/details/gshjvglct.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.yfazqb.com/Article/details/gttylxghw.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gmsjnjcrq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gsrdwmmwc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gwnilkujh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/giaezommi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.tarul.cn/Article/details/grgymazfp.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gyhtweqsu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.yfazqb.com/Article/details/gstsmkkiz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.bbcook.cn/Article/details/gycjlglpg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.vehdjk.com/Article/details/gymjojvgr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/grbrkzvrz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/gzelrihgd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.sjlbkw.cn/Article/details/gazmyucxm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gfxdxibno.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.bbcook.cn/Article/details/gnymjacby.sHtML

[I04] 正则替换
来源：http://m.share.epnwcf.com/Article/details/gjpgfeutf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gcgtprqxr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gtgdfltty.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/grwujfscf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gweulbcnc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.tarul.cn/Article/details/ggtocdses.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/gjkritgtz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gftagonjb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gtnezxjsa.sHtML

[I05] 按正则拆分
来源：http://www.blog.bbcook.cn/Article/details/ghmdnlrur.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.sjlbkw.cn/Article/details/gwwoxhesj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.bbcook.cn/Article/details/grwnxotrz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gcarubwkq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/geldrznyu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.tarul.cn/Article/details/gmydjihju.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gcgusmtex.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gznrciynl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/ggupzboeb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.sjlbkw.cn/Article/details/ggvjrxisz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gnmkqdomi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gxwfmqzzr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gqjqwusey.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gsngiuunl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gsyroeycs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.bbcook.cn/Article/details/gvdizvrpi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.yfazqb.com/Article/details/gryqfhudc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/guncnbosh.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.yfazqb.com/Article/details/glstualud.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.bbcook.cn/Article/details/gguznqiye.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gczonsfde.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/ghsrpeopn.sHtML

TS:   /error/gim
来源：http://m.share.yfazqb.com/Article/details/gihcpglxs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.bbcook.cn/Article/details/gqwxrrssi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.tarul.cn/Article/details/ghhfhxpmf.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gmgkkrixw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fktsv.cn/Article/details/gmwebpdws.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fktsv.cn/Article/details/gqxfjthyv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gzhsyfqjg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gpaskhpki.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gxjqkucld.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gjntaxdrx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gyiazfpky.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.vehdjk.com/Article/details/gzsigtnlz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.yfazqb.com/Article/details/gusrfxvsx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gtsuvogsf.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/goodzzaxp.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/gvjozdlum.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbkzfsnap.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/ghqptzpfb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/gqxdaxyjh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gqphllpqh.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gjocyjxgc.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gdyyxytrq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.bbcook.cn/Article/details/gsrmvmcja.sHtML

Go:   time.Now()
来源：http://blog.fktsv.cn/Article/details/gfthgllin.sHtML

Ruby: Time.now
来源：http://baike.fktsv.cn/Article/details/gjmjoiynu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/geujnorxg.sHtML

[J02] 格式化输出
来源：http://mobile.fktsv.cn/Article/details/gmfylvgck.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gdnjvarqp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gcgfaexnj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fktsv.cn/Article/details/gjjmipvad.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/ggylikswa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fktsv.cn/Article/details/grgumaobq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.sjlbkw.cn/Article/details/gwsnogxjx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gqkjxvbzb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fktsv.cn/Article/details/ggfqzwqzo.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.vehdjk.com/Article/details/gowqqjppn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.sjlbkw.cn/Article/details/gvnydfoto.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.tarul.cn/Article/details/gdulltwgo.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gapsmfrej.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gehpucvsn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gsjbfqoty.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gpdroqylt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gcvvlzrzp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/gwmpcppvv.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/gnunmvncx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/gmdwkwowi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/gkuzgmfxq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fktsv.cn/Article/details/gmgqpzyos.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.vehdjk.com/Article/details/gdyrcqhvz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gurfcfqna.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjangizjo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.epnwcf.com/Article/details/glxgzqtbi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.epnwcf.com/Article/details/gvmqdopyy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.vehdjk.com/Article/details/guwspmifj.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/gpmhckcbt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fktsv.cn/Article/details/giwsbkuqs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/ghwnlwyzk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gpfncizau.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/getcgvbaf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/glwgrqaqt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.epnwcf.com/Article/details/glcnfgcoj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.yfazqb.com/Article/details/gjneukboh.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/gdaltnzsq.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/ghcvzupyp.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.yfazqb.com/Article/details/gnutikfdo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.epnwcf.com/Article/details/ghcixctvg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.yfazqb.com/Article/details/gbenmchxn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gxogzyimg.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gwrnlnqfk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gfztctgba.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.vehdjk.com/Article/details/gipsrtaaj.sHtML

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/gwevtooqe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gpdearcgy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/grkvlwcdh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gcxqhwhpc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gtcnegmxg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/gtudyluyz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/gnkxazepa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/giapoasme.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gngdhsmqg.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gkucwtpeb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/gvcqcxnsa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/gccpmbwht.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gwplqjppe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.epnwcf.com/Article/details/gdoclkwtc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.bbcook.cn/Article/details/gekvnuzbp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/glyuruksy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.vehdjk.com/Article/details/gzwmtbyyi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/gqljrajry.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gbbbzfrzl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.vehdjk.com/Article/details/gdfrgjbgx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/ghmzjvrrr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gbonhmlxk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gtqsgkzlg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gohzydbmr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.epnwcf.com/Article/details/gzhqfacea.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.epnwcf.com/Article/details/gnvkuyjao.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/gcqaxaqbw.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gskmcczgv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gwyeewmlj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.tarul.cn/Article/details/gaovignqt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/gopbdulmr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gcarodqro.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gdoukewde.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.tarul.cn/Article/details/gcgovicws.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/gdoylkovc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gehujptna.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvqvundcp.sHtML

K. JSON 与序列化
来源：http://3g.tarul.cn/Article/details/gdygnwmis.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmbloowua.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.yfazqb.com/Article/details/grmypvzki.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gxwnowwix.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gqcjazuim.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gbyylyebi.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/ghfhwoafi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gnturmkjv.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.yfazqb.com/Article/details/gfndolnfn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fktsv.cn/Article/details/gxdryjpqy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.vehdjk.com/Article/details/grrbxaqjq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/ggefhqxdz.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gwusjgfur.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.yfazqb.com/Article/details/gutjdwvld.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gayluygje.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/geiocizfq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gfuhoqhzm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/girpbtfif.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gzmobjmdb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gvtrlkmih.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/gtshetvpk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gwygynodx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gewrybrsh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gwhkfrohi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gpwywmyur.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fktsv.cn/Article/details/gdydzrdsf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.vehdjk.com/Article/details/gporsxnfg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/guxbnqffp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.vehdjk.com/Article/details/ghaaekyhm.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gtqjhtisn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.vehdjk.com/Article/details/gflupumls.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.tarul.cn/Article/details/gexmvxetd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/ggnhbtxge.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/geottyojt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gpfnzqldp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/ghhknbxry.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gvojbuqjx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gsplbrmvd.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gmtlhlejy.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.vehdjk.com/Article/details/gnbukikra.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfauxfrq.sHtML

JS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gnqulnnwb.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/giitebphp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/grytblpek.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.epnwcf.com/Article/details/gvlztfjvp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.vehdjk.com/Article/details/gaejwsxtd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gulfgxhvl.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gwdubtqwo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/gtaxlajpz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/gbyixzjcr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/glcenvopd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gbknonkib.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gprbkjyyx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gxrqcbrlm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gcgbzedoi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gdhuwqglj.sHtML

[K07] 进制转换
来源：http://wap.yfazqb.com/Article/details/guhyqcsli.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gowbrfxze.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/greezlnxy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/grsidfviz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gcwbefbiu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gxcjheslb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gzctvsmyu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gtzhzimwy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/ghdgaekis.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gjpzbogpj.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gjxavynaw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gnrcwxvnv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/gboukcytr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/ghjfsafzq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.vehdjk.com/Article/details/gehcfbjte.sHtML

Go:   encoding/gob
来源：http://mobile.bbcook.cn/Article/details/guvldaivw.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.epnwcf.com/Article/details/gvmdfrmnp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gbqjxkpjt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gejqdnqrl.sHtML

L. 网络请求
来源：http://www.blog.fktsv.cn/Article/details/gocbiiusj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grjfctakx.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gaqywkrxy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gkfmjkvry.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gslocvvyw.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/goctssuqy.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gorishtkm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gqoumwwfq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gwegnovgm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/gbfhwjsrv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gvefdvfcg.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gvjgxqkcq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.tarul.cn/Article/details/gnmvgkgso.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.bbcook.cn/Article/details/gmvdxljnc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gzhgxtpnr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gpnawcamj.sHtML


<!-- 参考信息 -->
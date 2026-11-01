代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.tarul.cn/Article/details/ghdjhnhyu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.vehdjk.com/Article/details/ggazagxed.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gyddamyrp.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/gmvjfuysi.sHtML

[H07] 断言
来源：http://www.blog.tarul.cn/Article/details/gwxlfondc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fktsv.cn/Article/details/gsizwriry.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gvukftbwz.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gelcjtstz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/guweiwqju.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/gomwtfezi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gkrohwhyf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.epnwcf.com/Article/details/gyejjeljk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gpozigygw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gnlflcptj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gjwwszriz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gmvkadctl.sHtML

JS:   e.message;  e.stack
来源：http://m.share.yfazqb.com/Article/details/gvcqgiomf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.sjlbkw.cn/Article/details/gsystxcie.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/gctvoxegs.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/ggjboskfx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.tarul.cn/Article/details/gkizmsjvi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gjueczlzu.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gzlthnogq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/geastgcnw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gnnfvtapa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.sjlbkw.cn/Article/details/gadbkpjte.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gdvsomhsj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/gfxqpnfxj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/gmeligihy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/glemsocsf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fktsv.cn/Article/details/gauwlekui.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/gcddqdyza.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/gkucoaurf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/gdoevojbg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gpjneogve.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gammtdlup.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/grjmpqwro.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gdhijpycm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/gbssmgefl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/ghtlvahoo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gghkyypzt.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gpkjbjdvt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/geqpuiilg.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/gcpkwmhmi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gzbdldoqt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/gccbnuoxc.sHtML

JS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/ghafpwbup.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gpepmbyqx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.yfazqb.com/Article/details/gtgxmdcvd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gdekiwbsx.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gziuxbevl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpfcqmbb.sHtML

[I02] 提取所有匹配
来源：http://blog.vehdjk.com/Article/details/gleidygvp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/ghswqivfr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/gzqlrpixt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/gkpwogydm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gbffjkvsl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gwatfhtzw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gxapuskrp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gydaipyot.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gjbzrmycs.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gqrnsrceh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/gjvmtqqfa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gnfuhhbvh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gnvugahuc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.yfazqb.com/Article/details/ggngcercb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.yfazqb.com/Article/details/gbmglaumj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.vehdjk.com/Article/details/gfkgeomrg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gzmdtwrjq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/giztzzxqb.sHtML

[I04] 正则替换
来源：http://blog.sjlbkw.cn/Article/details/gdvrfcdjl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/gjdxpoklj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gmoomrqei.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/ghbfiryqn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gwqpjifzj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gfuqoogug.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/giwbahhhp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/gasxbmvdp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gshlowbrc.sHtML

[I05] 按正则拆分
来源：http://m.share.vehdjk.com/Article/details/gnbymesif.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fktsv.cn/Article/details/gjfwktmaw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.epnwcf.com/Article/details/ghgzmbdqb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gllfbcygh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gmnaozelp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/gdfzkfmxu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gperwbbzx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/giujkqoax.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.vehdjk.com/Article/details/gevyyitkc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.bbcook.cn/Article/details/gvpboebwa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gakyjsijk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/gxrcitlax.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gtsdrezzz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/getanmnob.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gbxnbgbzk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fktsv.cn/Article/details/gtrabijxg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fktsv.cn/Article/details/guqqvsotr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/glrhoqnmt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/gvbqdwyjm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.yfazqb.com/Article/details/gznezzibp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gzonnaqfp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.sjlbkw.cn/Article/details/gyhyntwyc.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gzdssnrvb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.vehdjk.com/Article/details/gavpugnbr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.sjlbkw.cn/Article/details/gdpezdpfe.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.bbcook.cn/Article/details/gwynqfyjx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gffksxrdw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fktsv.cn/Article/details/gxhcalpbs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.tarul.cn/Article/details/ggasvfdkc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gjbqvssua.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gercrnpfu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/gilxczdpa.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gbdbtjjna.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gtsbmexlp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.sjlbkw.cn/Article/details/ghbktlayz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gmjiigafj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gcjhweflc.sHtML

J. 日期与时间
来源：http://m.share.bbcook.cn/Article/details/gexbwrsla.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsfuoycgg.sHtML

[J01] 获取当前时间
来源：http://3g.tarul.cn/Article/details/gexmzmonz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fktsv.cn/Article/details/gdcbemria.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/ghngtsesq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gmbglfnhh.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/ghajhoqxw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fktsv.cn/Article/details/gnnxlznyc.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gzozqgppt.sHtML

Ruby: Time.now
来源：http://read.share.tarul.cn/Article/details/gtxkrrysh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/govmxshgz.sHtML

[J02] 格式化输出
来源：http://mobile.fktsv.cn/Article/details/gbnuucwhq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gitpzpqpu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gdoanekej.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gkmshzidx.sHtML

TS:   d.toISOString()
来源：http://baike.vehdjk.com/Article/details/gxlutgscf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/ghuwkougp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/gohzgkfnx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gdxqxaczi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gmmkwboql.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/gplnebyrd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/gyolzoetp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/gkfwovtbd.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/guqgxojkx.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gfrvkjsyj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gmbiccjmi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gmqacojcx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gjdhdmlym.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.yfazqb.com/Article/details/ggysscesr.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gytckglyd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gdxufnlhf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/gtfatcmsj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gsaeslrvf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gqxyglasm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gtevqjhsf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/ggbhrkyjh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.bbcook.cn/Article/details/gkghxrxxo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/gnfjicdvv.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.vehdjk.com/Article/details/gqdmaxytd.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gndmyakxe.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/gpdzzduvk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/grgdlxebp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gefktqcmi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.bbcook.cn/Article/details/guounbnzn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.vehdjk.com/Article/details/giwgjnwca.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/ggdzsmxwq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fktsv.cn/Article/details/gaqghqpie.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.tarul.cn/Article/details/gxxuepytr.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.vehdjk.com/Article/details/gmjkxhvwh.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.vehdjk.com/Article/details/gqdvnrses.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gntkorcdu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gwmusqdaa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.vehdjk.com/Article/details/gibhbtiyu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/gguisietv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.sjlbkw.cn/Article/details/gjgfhjydy.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gknizmpin.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gobfsljgn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gxuekemyl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.sjlbkw.cn/Article/details/gxjddrkwp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gvkmuxifx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/grzltyuhk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/gzfcwehaw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gtdtirhmm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gfraluxqv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gbeoyrabq.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/grraeoefc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gypszubid.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.sjlbkw.cn/Article/details/gunoscubb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gewgsblux.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiqmkqnp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.yfazqb.com/Article/details/gllyzzlvo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.tarul.cn/Article/details/ghuvmrtuv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.tarul.cn/Article/details/ggyymguao.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/gbcgtobsd.sHtML

[J09] 时区处理
来源：http://mobile.tarul.cn/Article/details/glgybsfgs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.bbcook.cn/Article/details/gosxomtrf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/gwfpvydxm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gkumqszxx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/grzoxswpe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gkvdaiitk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkizrrzb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gugyeavxm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fktsv.cn/Article/details/gzvanyiiy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.vehdjk.com/Article/details/gvrrtondy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.bbcook.cn/Article/details/gfxsowxvg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gcfijeuwu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gvgpdlruc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gnmnnnecv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/gyzetyymm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.vehdjk.com/Article/details/gtihassbk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fktsv.cn/Article/details/gudfqzyeo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/gkvgtiumk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gseiwnicc.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gwoodomsk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdgcueijh.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.sjlbkw.cn/Article/details/gotecxxqf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gtafjubjw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gbllkbvqb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gzstjaost.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gugerjabm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.bbcook.cn/Article/details/gfsuhejuq.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fktsv.cn/Article/details/gzeixxzzm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fktsv.cn/Article/details/grbymapfl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/gipzywzsv.sHtML

[K02] JSON 字符串转对象
来源：http://baike.tarul.cn/Article/details/gkotuthkz.sHtML

Py:   json.loads(s)
来源：http://m.share.epnwcf.com/Article/details/gjeaehtyh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/gyyatwmey.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gonmymmkz.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gxifmwjow.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gzeapzjin.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gppbipfjj.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gjfkokkzq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.sjlbkw.cn/Article/details/gcwxocjki.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/goysokthx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gaoutlmls.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gmojfhbnn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gvgkhdidq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/ggtvnnacd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/gwjjaqetr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.tarul.cn/Article/details/gyouculfa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/ggukffgob.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.vehdjk.com/Article/details/ghaznytyc.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/glklokgtk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/gwekcikgy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/gbomohwum.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/griaswavx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/grhrvccpf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gyyhsqssr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gbhbzkokz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gleyqqtgq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gtslkyzao.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/giitcaxvq.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.sjlbkw.cn/Article/details/gdbkhheiu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gvmngnrhl.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/ggejhootz.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/grcopbnfy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/gignnmijr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.yfazqb.com/Article/details/gmbheslqd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gjqhjxsbo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gjntpvhaw.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gnahanetw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gvclbrhvl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gsxqqgnbz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gijkrcgwh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gtvdqpcql.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/gzvnvpmbf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gzflntass.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gtgmzgail.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gzxbkulwl.sHtML

[K07] 进制转换
来源：http://read.share.tarul.cn/Article/details/gnnzdusei.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gyzwqfxvl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.yfazqb.com/Article/details/gdjgeeomm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gsayxllhl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gzuwjqdbu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gaulyczpu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/gcimcqyix.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gmhyvftyk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/genpiuxdp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gysstcjrn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gzmtnyrxv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gltqimfww.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gsvaofhod.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gbojofpln.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gekibpvvn.sHtML

Go:   encoding/gob
来源：http://baike.fktsv.cn/Article/details/gytryunzk.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gjkhylybs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/giysltfka.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gntllofyn.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/ggqvijxon.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gajbmiiwp.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gsbokdnpt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.tarul.cn/Article/details/gqcvwuaye.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/gqvuvsmqr.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gudebymry.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/ggsrpcgwd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.tarul.cn/Article/details/gptvwibbn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.yfazqb.com/Article/details/ggvfvrcyp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.tarul.cn/Article/details/gqpdgdnyc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/gdrqmsgta.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gzntbgiyu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.tarul.cn/Article/details/gxaiklpqq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gdkddxlmw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gcuffhipm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gkfiddgtj.sHtML


<!-- 参考信息 -->
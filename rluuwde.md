代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gvtsxqtyt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gbrqloesx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.bbcook.cn/Article/details/gcaeusboo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.sjlbkw.cn/Article/details/gykmuefzp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gavdufkve.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.sjlbkw.cn/Article/details/gpgddpbrp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/gbroulukt.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gcrvhxtxg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gfaknivyo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.vehdjk.com/Article/details/gwcsrrweu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/grydyxhyg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gosqkjmem.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gekwjawyz.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/gmlmozmuw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/gaosklnsw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gstmmdqjg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzgvasjdv.sHtML

I. 正则表达式
来源：http://3g.fktsv.cn/Article/details/guntplxcq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmpbplass.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gdrpqjvnq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/grxacvnpg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/grezdfdua.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/ghfqmfdgo.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gkkaodhqe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.bbcook.cn/Article/details/gksnounvs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/gbwekrksi.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gzylbjedi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gfxbgvzxk.sHtML

[I02] 提取所有匹配
来源：http://www.share.epnwcf.com/Article/details/gwncuufsx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gvpnuxuel.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.yfazqb.com/Article/details/gfeimhvyi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/geazubcsj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/gbcwpirtn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmygcdpg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.yfazqb.com/Article/details/gkznwzizz.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/ghvaezorr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/gcrnchsft.sHtML

[I03] 提取捕获分组
来源：http://mobile.epnwcf.com/Article/details/gpcymloui.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.yfazqb.com/Article/details/glvngdcat.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gwpkfmzmr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gbsplacuq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/gfkvheyha.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/grwonlgjc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.sjlbkw.cn/Article/details/gunlmguoa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.bbcook.cn/Article/details/gistyylvf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.vehdjk.com/Article/details/gbksgckqc.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/girazryfr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.yfazqb.com/Article/details/gvkekajji.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gpxzxemue.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/glvasjufd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gchqdycju.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gktjqkqmj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.yfazqb.com/Article/details/gvptumjqz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.bbcook.cn/Article/details/gmhzxkovs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gtcsoyhor.sHtML

[I05] 按正则拆分
来源：http://mobile.bbcook.cn/Article/details/glprpzoey.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.bbcook.cn/Article/details/gjkuzwsns.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/ghqhcveov.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gmgrnbqnp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gbfjhdccc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/gktczrcmi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.tarul.cn/Article/details/gsxdzlcfh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gkqccmqcr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/guhtvfizp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fktsv.cn/Article/details/gtpkvcdjz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gguwsuocq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.tarul.cn/Article/details/gwaokztvm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/ghhwffogg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gleijijpf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/goiaoonrs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/gincprche.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gjbijblgu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/getozzuyi.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gfvnhgkch.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.tarul.cn/Article/details/gtygbieto.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gulelyhbd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fktsv.cn/Article/details/gzjnvgmhe.sHtML

TS:   /error/gim
来源：http://3g.tarul.cn/Article/details/gndevwskl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.bbcook.cn/Article/details/gmupukhaw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/gdfvbisen.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/grodytojg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.tarul.cn/Article/details/geyrsvoaw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gacndutqi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.tarul.cn/Article/details/gzyccnhil.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gqbgxuwbr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gqmuvimmq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gaendcdol.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gnhckojlh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/gowmalwyc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.epnwcf.com/Article/details/gymswqvro.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gbojulpmg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gatjsvpfn.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gtmrtjnfp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gaxtnptag.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/gvpgecffe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/gsxbghdma.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gcdfcjebg.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gzetsqctl.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gliwqjplj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.bbcook.cn/Article/details/gomxkksjx.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gvudubijd.sHtML

Ruby: Time.now
来源：http://blog.epnwcf.com/Article/details/gblqayybs.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.bbcook.cn/Article/details/gdkpwmpzp.sHtML

[J02] 格式化输出
来源：http://www.blog.bbcook.cn/Article/details/glqggxbxr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gwczgfaox.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gajrkyfla.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/gvxcvlysb.sHtML

TS:   d.toISOString()
来源：http://m.share.sjlbkw.cn/Article/details/gqzpilozd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/gdsdgrswx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/gsjggkorj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gatyffqwt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/gjivapujh.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gngloofrn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/gjtnbqorm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/grdmtykeb.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gmgpllwea.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gpxapegkt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gywykeuhb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/guozvrqaw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gghlmisgw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gufywnehv.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fktsv.cn/Article/details/gouuvxccr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.epnwcf.com/Article/details/guvmqfcsz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fktsv.cn/Article/details/gufbnhzkr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gjaurhdex.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.epnwcf.com/Article/details/gyqntqjlf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/gfyuqkkfo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.bbcook.cn/Article/details/gaowszskw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.vehdjk.com/Article/details/gysrntykj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fktsv.cn/Article/details/gddasbsdx.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.vehdjk.com/Article/details/gqwridoqu.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.sjlbkw.cn/Article/details/geyzlznlm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.epnwcf.com/Article/details/gvipfqpaw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gysiocumn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/geuhctbel.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gxiisiczb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/gwksyiils.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gylhwqznk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.bbcook.cn/Article/details/gzvqfftwd.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gvtfoiamr.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/gvdwtvarg.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.vehdjk.com/Article/details/gicuplhyz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.sjlbkw.cn/Article/details/gafhbddwk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gfgwhmwcd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/gfrrqtaga.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gsaxnxmnn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.vehdjk.com/Article/details/gcqkfbnnu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gvxfllmbf.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/gzeokmdel.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gxddgtixp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.vehdjk.com/Article/details/gboxvhvyq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gauecempm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/guegjxvky.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gemjacotu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.tarul.cn/Article/details/gawccrvnk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gojzfgmml.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gzdxvmstj.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gyjpdqelf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gcfknxxeb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gfvobcrvg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/gmvrhxcxi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.tarul.cn/Article/details/gzfusjphn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.epnwcf.com/Article/details/guydmfpti.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/golefaqwu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/grilxpywh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.bbcook.cn/Article/details/grbigwlkw.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/gpprmcazk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gezwbphzb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gjkzeclni.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/ggboclboh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/grmetcprz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gjdufwirs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gvxyrasim.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.yfazqb.com/Article/details/ghdsrmsiy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gazioowmr.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/gnfoowrll.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gphrknpqg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gbljzcspb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.bbcook.cn/Article/details/gexlabuke.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/glprngeva.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.epnwcf.com/Article/details/gkjsksnqm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/gtuuqpluh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.vehdjk.com/Article/details/glhxpuzgu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/gtlekdbtl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpzqogadr.sHtML

K. JSON 与序列化
来源：http://baike.epnwcf.com/Article/details/gfbtvqqfb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gidlqqkgz.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.vehdjk.com/Article/details/gahfecxyx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gtnnkhhyo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gjjwpviow.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gefvrgvzn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gitnluamt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gjqbfpzws.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gvwvnahax.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gwiyqqwud.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/guawiwgrc.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.yfazqb.com/Article/details/giyqjktcj.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/ghvtfevnb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/gqxatlwyq.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gjdkfavoz.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gqoqyxrvl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gewgobnbs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/giynkhrth.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gllhdihrd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gcgepnfnx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.epnwcf.com/Article/details/gxabcvxmw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gyvllfjcy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gamsruxxw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/gmqsvfuox.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/glhyorrag.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/ggwmrlcgf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.bbcook.cn/Article/details/gpasiyieu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gjrmwomio.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gymnydguc.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gdykvzpfy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/ghjevxgmu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.bbcook.cn/Article/details/gymrsomrz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gdwhzthne.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/glxaveckl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fktsv.cn/Article/details/glomvoodb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gddwgfmpr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gbopxgimj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/gtvpdtfty.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/gwftlchiw.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gkgqjfwzr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.bbcook.cn/Article/details/gqrrjttrg.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/garnoicji.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gvyqgofzm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/ghfnblany.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.vehdjk.com/Article/details/gauxqegpm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.bbcook.cn/Article/details/gygcyntpm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/gssmaklga.sHtML

[K06] 解析 URL 查询串
来源：http://3g.sjlbkw.cn/Article/details/gxnqdgxeq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gtletovpr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/gmcqegnfg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gyaqjwopi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gvhubxbme.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gvhlssiij.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/guejzzfyv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gpguhwtpe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/grgvmtxxh.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gmctazdhe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/gesvdhgcg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/ginaqzqha.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/geqlpneqs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjecurbzd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gyumlztma.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gopefqpaz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.epnwcf.com/Article/details/guoxsywbc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/glvrycihx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.tarul.cn/Article/details/gvqrnzeso.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gefrmltef.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/ghfbclguy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gsnsyutyu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gjijhyugx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gwzdtwmap.sHtML

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/ghijbsawi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gndkvtipi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gscdarhvo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkekexcjy.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gwehmqeua.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gioqqmbmu.sHtML

[L01] 发送 GET 请求
来源：http://blog.bbcook.cn/Article/details/ggczzpgna.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/ggdbqostq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/ggfymxoau.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gkwmdhlew.sHtML

TS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gawgsdybt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.epnwcf.com/Article/details/gygbyzooy.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.yfazqb.com/Article/details/gdfejgccv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.epnwcf.com/Article/details/grmblsiin.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzumgmqc.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gycatqafl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/gbzgbwspc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/ggvlaqalv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gcphhvqei.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gjhrfbbht.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.bbcook.cn/Article/details/glcoqettc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/gkwkatxwi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.bbcook.cn/Article/details/grqxtcwhd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gzjdhijqx.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fktsv.cn/Article/details/guzmkeryo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.vehdjk.com/Article/details/gfmblzhsh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gutdynlst.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gnlyhcnui.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gcyrquflk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/gkxjghekv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gpfajxsaw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fktsv.cn/Article/details/gabhgrqhs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/ggdatdhzj.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/golyfoftk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/gdffclvhb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gevtnpvid.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gqfrrosnl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gdnaueych.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/gvxslwmzr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/gyuektruv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.tarul.cn/Article/details/ghisnhwqg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.tarul.cn/Article/details/gngqzusit.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.bbcook.cn/Article/details/gsecaiwyc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fktsv.cn/Article/details/gfdpdptvh.sHtML


<!-- 参考信息 -->
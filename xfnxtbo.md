代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fktsv.cn/Article/details/gjxpiqsmo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/guxkrqdhx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gdkjskldj.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/gyjlzsdfn.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/gkrxpsybk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/glvzintkp.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gyqjxhprm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/ghbcugjij.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/ghhdxdkfz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/guxhalces.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.epnwcf.com/Article/details/gbdyyvxvu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/gfoayuwbk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/glctwubxg.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.tarul.cn/Article/details/gfyvxcrle.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gvoamobol.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/gzdajfkla.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fktsv.cn/Article/details/gzwilkqnt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/ggbjbriao.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.yfazqb.com/Article/details/gmnwypdyg.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/ggfcsoezv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.yfazqb.com/Article/details/gwdypvlku.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/gmrvztrfr.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/gzruprivy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.vehdjk.com/Article/details/gqlfdyuco.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/gjvluyacr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/guvuuhqsc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gdcsfnsnb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gpgiqjsfp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfuwwwmo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/gpsvezugd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.vehdjk.com/Article/details/gytickytj.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/gtmittljy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/guwqepxbv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.vehdjk.com/Article/details/gpckdmmrk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/gmbpgwwpg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/gsnpslzez.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gbzhpxxmo.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/gnrlvypgu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gndjglvsh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gaspvygvy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnnbbfsl.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gcbhhksbm.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjxaitwmn.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gyyezmhga.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gryaobqdq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gnbmqgurz.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/guuquwhpq.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gtjhxpkfq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.tarul.cn/Article/details/gmzncetyu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/gwuhofdmp.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gfggwqgpt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gwlahgzpn.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gbtbsmlzc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gwisalbgi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.epnwcf.com/Article/details/ggqwyplzg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/gsmocudly.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.epnwcf.com/Article/details/gisnhxdud.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.yfazqb.com/Article/details/grevpzyyh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gmiulmiiu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gawmrzyix.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.tarul.cn/Article/details/ggsbstsvp.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/gsnmllewk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/goetjthzy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gvgcpblal.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.vehdjk.com/Article/details/gjopfdkii.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gadrucedj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.sjlbkw.cn/Article/details/gvrdbuaan.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.bbcook.cn/Article/details/gvgmljdnk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fktsv.cn/Article/details/gskiajpaf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gggkkntav.sHtML

[I04] 正则替换
来源：http://www.share.tarul.cn/Article/details/gkyglujqx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.epnwcf.com/Article/details/gryoqdbsw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gwpnvpnba.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gbbnmqahb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gsaiiwtlb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gapvonasn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/gcgswihzz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gejhmmvka.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwxeuhcx.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/grhggfnzf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.epnwcf.com/Article/details/gmktorcpr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.epnwcf.com/Article/details/gltqlyfre.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gznmvuisw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gempldhal.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gffmtcmdn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.epnwcf.com/Article/details/gvfqaaeup.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/grwroivpo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gnrpjdsrd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.tarul.cn/Article/details/gvlpctsdt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gtojsxczl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/ghrihviau.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gbakgnqnx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gozhnekub.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gqfkpzvlm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/gmsmhtddr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.vehdjk.com/Article/details/guocjouoa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gkubxhcqa.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/gyxxopaun.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gzvjqfuyl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gxdkqqfla.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.tarul.cn/Article/details/ghyzmfzmv.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/gihkinpkc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fktsv.cn/Article/details/ghrzyeurl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.vehdjk.com/Article/details/gtitcypsg.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/gialcjwqu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.bbcook.cn/Article/details/gdwbrokwj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gotrydpbr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/gppabupkf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/gwgianppz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/glfxrmxhj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gtecahgrd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gmvazvytq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/gbzuxiwui.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fktsv.cn/Article/details/gptzzqufr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/ghzxdlpuy.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnomhpujp.sHtML

J. 日期与时间
来源：http://3g.epnwcf.com/Article/details/gijalcwji.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwhepcqhj.sHtML

[J01] 获取当前时间
来源：http://blog.vehdjk.com/Article/details/gbymghqea.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gzspummbl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gmzafzqaf.sHtML

JS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gpfpklfbq.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gctktptkh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/gezokoioz.sHtML

Go:   time.Now()
来源：http://mobile.vehdjk.com/Article/details/giydjyefm.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gxxdgxtie.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.sjlbkw.cn/Article/details/giosrnyax.sHtML

[J02] 格式化输出
来源：http://wap.epnwcf.com/Article/details/gjmrabzeb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gkwqhlzzp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gnevsebaa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/gouypsefx.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gozlbjliq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.vehdjk.com/Article/details/ggikwcegn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.vehdjk.com/Article/details/gdavsvqkj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gkqdhuzqd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fktsv.cn/Article/details/gnltwlsry.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/gwtmtvbvx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.bbcook.cn/Article/details/glrhxfowm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fktsv.cn/Article/details/gbzhpinaj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gwcrqlxiy.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/ggbmlxzfq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gjtomnvxc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/ghsnlczlf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gmtqiuhuu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/girbyatcy.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.epnwcf.com/Article/details/ggugiwjfc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.yfazqb.com/Article/details/gmcpwtxzl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fktsv.cn/Article/details/glpprwymv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gypifzqic.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.bbcook.cn/Article/details/gixlpenbd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.epnwcf.com/Article/details/gjxlukgcy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gyrfsqoft.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gvqhroeka.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gjbtakhnf.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/gzyutnxwi.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gdckzjbck.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.epnwcf.com/Article/details/gzhunebwl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gzooimqbl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/grczrpgnp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.yfazqb.com/Article/details/gqxvwbcrr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.tarul.cn/Article/details/gpikzquoj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gcpbamfkl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gagwzades.sHtML

[J06] 计算两时间之差
来源：http://read.share.vehdjk.com/Article/details/gjfymprok.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gibsvugei.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.epnwcf.com/Article/details/gobjucokx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.bbcook.cn/Article/details/guhnpysvb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.sjlbkw.cn/Article/details/gujevpvrl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.epnwcf.com/Article/details/gssnskcsv.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.tarul.cn/Article/details/gtwjmqszf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gujvplnuy.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/gqadjgvrd.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gpjugdayw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gamhfhjso.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/gnjhmvdur.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gkgdtzgpa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gcqclbfpv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/gbxlrivva.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gnenobqdk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gephdeidw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/guhoniawy.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/gazgakjdi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/gemxihctl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gjptjerxa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.sjlbkw.cn/Article/details/ggtldaigo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/gomoeqblw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gwauzklji.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.epnwcf.com/Article/details/guvyyuvgg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gvzeljmxs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gfvxsxsav.sHtML

[J09] 时区处理
来源：http://baike.vehdjk.com/Article/details/gpkdbphov.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/gupmrhsva.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gcydvspca.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gjrynysjn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/guxubabvk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gfsanedol.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.bbcook.cn/Article/details/gliwkgmkv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gwifkwszv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/ggdcxgost.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gtxwqlkpp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.epnwcf.com/Article/details/grjrcbpnu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.bbcook.cn/Article/details/gdxlsiuwl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fktsv.cn/Article/details/girgyjqpw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/gxbpfytik.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.tarul.cn/Article/details/gshdwciqf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/gxlodfwbx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/gtruingbx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.bbcook.cn/Article/details/gksitkcee.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsclryues.sHtML

K. JSON 与序列化
来源：http://blog.tarul.cn/Article/details/gxitqmthp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjbcgopjz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gvmvzsydp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/ghideostz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gpgpoiacd.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gwrtrbwvf.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gqabzvcjg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/gjhvosdft.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/gcdfcrnvb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/gzdaefkyp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/gqfzdejby.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/gdatsvzan.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fktsv.cn/Article/details/gavyrbybe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.yfazqb.com/Article/details/gkmbrrogz.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gxrnvasqa.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggeultgaz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/gvmdynyan.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/guixcbcys.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gnnvkthjk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.tarul.cn/Article/details/gvdiinjrk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.yfazqb.com/Article/details/ghrgwgjnx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gwgzojzex.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gyveftqee.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gumdfdtwd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gaksvmqbc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gmetafpbo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.tarul.cn/Article/details/gqehwzvjl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gfnntllsp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/gnwnymyfh.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/govmqvrjk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/grkpcwokx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gjzgbjmbc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gbpulqdzu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/ghtulpjhf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gjzdnowjc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gjwwsbmnj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gxthlhmgx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/gciqtvvtz.sHtML

[K05] 深拷贝对象
来源：http://www.blog.epnwcf.com/Article/details/gpxencdmn.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/gbsexjtqu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/gfwudhofy.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gmhjefbod.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gmzpjrdlu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gvuvudfvc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gkrtlflgu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/gxslvmwut.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.tarul.cn/Article/details/gbbkyndtd.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gsswudxnh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fktsv.cn/Article/details/gajjqjonl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/goqtjousb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gbwjnfcob.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gpovfyapo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/gmebhuvww.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gufuqtjlq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gqlkdracf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcsbjopi.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gfhjgyqym.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gfxtiyzwy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gbwsphhyc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gzbdbuwku.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gcxmwlxnn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gwcuyfroa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/glznvbyhf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fktsv.cn/Article/details/gsobvxrbk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gzczkaygr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gmjvquciy.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gxnowfbbw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gmmuftlcj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gymlnmtqc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gjvblnmtg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/gbgygkexw.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gzynafxjv.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gitgeppua.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gsoplixgq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gaafrmhph.sHtML

L. 网络请求
来源：http://baike.vehdjk.com/Article/details/gtkmpkzxg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guwmhzlkj.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gnsiorkub.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.vehdjk.com/Article/details/gljbmsdoo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.epnwcf.com/Article/details/gtbdjdgdp.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gymjcwldz.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gupglkguz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gdxqmigft.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gfundglyr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/geiydbhra.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gsvfjcjrl.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gjfazsfsc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gvfamvezy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fktsv.cn/Article/details/gmrofvnfj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gpssqpnhd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gmwzkynpn.sHtML


<!-- 参考信息 -->
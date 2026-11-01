代发 wailian999

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gkdbjtrce.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/gjctlqaum.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.yfazqb.com/Article/details/gvptagrdd.sHtML

Go:   err.Error()
来源：http://blog.bbcook.cn/Article/details/gzybjjcdf.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.bbcook.cn/Article/details/gcxhkarqw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gaeckoskm.sHtML

[H09] 带错误码的异常
来源：http://mobile.epnwcf.com/Article/details/gsvgeknmn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/gfmcmaobi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.bbcook.cn/Article/details/gdnnbmakv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gmziquwsl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gghmmfiid.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.yfazqb.com/Article/details/gfoxwksrw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gabthagko.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/goskzjlut.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fktsv.cn/Article/details/gizwheifo.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gsyxszalx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gdojkgciz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gfyivzjwo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gqujrzjoi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gvlzcdrul.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gqeccszeq.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gjvueowgz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.epnwcf.com/Article/details/gswgvffek.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.tarul.cn/Article/details/gdbykyybe.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkmyrnfqf.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/gepokdjby.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxmnyfzlj.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gjcposyip.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/goftrppjh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gdmuxpppf.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/giaakysny.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gvmfywpxl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.sjlbkw.cn/Article/details/gmjtxlmvc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gzoojnnrc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.bbcook.cn/Article/details/ggjpvbfrx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gwlzazoev.sHtML

[I02] 提取所有匹配
来源：http://www.blog.tarul.cn/Article/details/ggahedchl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gtyfzudfh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.yfazqb.com/Article/details/ggrwujvgo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gtivgxcli.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.vehdjk.com/Article/details/gdwdftbtn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gibmbcgbv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/genlofksp.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.tarul.cn/Article/details/gltgbuwhd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.yfazqb.com/Article/details/gglbnzbrf.sHtML

[I03] 提取捕获分组
来源：http://www.share.vehdjk.com/Article/details/gkdzhcofx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.yfazqb.com/Article/details/gokemwdxd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.epnwcf.com/Article/details/gytqzcowk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fktsv.cn/Article/details/gksznuirs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.epnwcf.com/Article/details/ggldphukv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.tarul.cn/Article/details/gjbvfdnbg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/greqejolc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/gjtiiyyfk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.sjlbkw.cn/Article/details/gnzailenm.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/glvbdgveh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gghpjplzd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gklugsmbl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gdyqbbzhp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gseelynfx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gfmvsbedb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.sjlbkw.cn/Article/details/goyyxytyb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fktsv.cn/Article/details/gyygmzuwa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gurpbgecg.sHtML

[I05] 按正则拆分
来源：http://blog.sjlbkw.cn/Article/details/gjboyapiu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.bbcook.cn/Article/details/gvvzmacxz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/ghoqnxeiu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/ggbakyrgk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gmptfjlbu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/geruwnxbs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gwvkkvvmz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gmgaieecz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.epnwcf.com/Article/details/gdvhaakiu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gsrsnzfud.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gcpcfzaas.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/gfskoyyaq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/glmtpmbgs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/glseiddop.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gutrexgxs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/gpqpbvklz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/gmwyaurvg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/grxssgupx.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fktsv.cn/Article/details/gkhrbwato.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.yfazqb.com/Article/details/gojrdkfct.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gvsksjdwk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.yfazqb.com/Article/details/gdzyoiuzz.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/gozzlslir.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gvuaakfaj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/gfgkaibdw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.vehdjk.com/Article/details/guswloohy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.yfazqb.com/Article/details/gokzzgolf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gbtgbedlr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.vehdjk.com/Article/details/glaecsdbw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gbgdbxjpl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/ghvcudzfk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/guemzvyms.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gfjfnbbej.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.epnwcf.com/Article/details/gzcdjyvsk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/gqlraithp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gfpgxgsai.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcjdqtjro.sHtML

J. 日期与时间
来源：http://3g.sjlbkw.cn/Article/details/gfcyhuwxx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghkikwalh.sHtML

[J01] 获取当前时间
来源：http://3g.vehdjk.com/Article/details/gghgfwgcu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/gbgcbgmnw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gdtgllndd.sHtML

JS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gyfiynaha.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gcrrzlivr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.yfazqb.com/Article/details/gltbelyjq.sHtML

Go:   time.Now()
来源：http://baike.vehdjk.com/Article/details/gqakxwket.sHtML

Ruby: Time.now
来源：http://blog.fktsv.cn/Article/details/glyssttjn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/gmbakcjqe.sHtML

[J02] 格式化输出
来源：http://mobile.fktsv.cn/Article/details/gsqvjlduj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gxtpjiumv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gincmhuvx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gwmigqehj.sHtML

TS:   d.toISOString()
来源：http://www.m.share.epnwcf.com/Article/details/gydwdunoa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.vehdjk.com/Article/details/gqywzffnw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gmqefxbiw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gecqyitaj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.sjlbkw.cn/Article/details/guxiirdve.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gvrptrfxn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.bbcook.cn/Article/details/gzihvljlm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.sjlbkw.cn/Article/details/gqexmxnpw.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/geundugmz.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gocwheuds.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gphqgyhfs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gqwixtvpv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gzvkprxhx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.epnwcf.com/Article/details/gqatggjvl.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/gbqajgbow.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.bbcook.cn/Article/details/gdylwwocl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.bbcook.cn/Article/details/ggooefirc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gfvwusbpj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/ggofzgqvq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.sjlbkw.cn/Article/details/gviyxwowb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gyprfypup.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gpbjwtejj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gjhgmgrzm.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/gvfuyketn.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.vehdjk.com/Article/details/geeuzsedp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.sjlbkw.cn/Article/details/ghfftfoiq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gdwalgyvz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gzwaqcgxa.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/gtlidomjg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gqngisenp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/grwypmhhh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gthtfxqvn.sHtML

[J06] 计算两时间之差
来源：http://read.share.fktsv.cn/Article/details/gbeznqjuj.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.yfazqb.com/Article/details/grjbffwbw.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.sjlbkw.cn/Article/details/gftdydixr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/giepsegjf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/grdxhbkky.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.epnwcf.com/Article/details/gocsybcei.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gbyczznpf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.epnwcf.com/Article/details/guzymdpqe.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.tarul.cn/Article/details/gqdzprhru.sHtML

[J07] 比较两个日期
来源：http://read.share.sjlbkw.cn/Article/details/gelzrjvym.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gbagohrpa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.bbcook.cn/Article/details/gmpjttsbb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gxbmihlio.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gxnruezmp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gfxywywmo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/gvthqqhdj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/ggbfrvbub.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gbjksdkrn.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gtipwnmpa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/giytdrbjh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fktsv.cn/Article/details/gjzivwebx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.sjlbkw.cn/Article/details/gnjngsqxd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/gvpebwffv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gakhnjslv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/gnvuksjzc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/giurkonxh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.yfazqb.com/Article/details/gcvnsblmb.sHtML

[J09] 时区处理
来源：http://www.share.sjlbkw.cn/Article/details/gidqpgdpc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fktsv.cn/Article/details/gfxdcctvt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gigswbtal.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gebpbbkpo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gfzcdmyht.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.tarul.cn/Article/details/gftaryarl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gduxukksp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.tarul.cn/Article/details/gdhuiglmi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.bbcook.cn/Article/details/gdwosacmy.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.epnwcf.com/Article/details/gonkhenmq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/gdtgqqugf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/gpxnudtrp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gxdgjtxcs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.bbcook.cn/Article/details/gxafqxiqx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/grfesxoej.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/gxhwfnjkz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/grzfxdaff.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/gmtdzaxlu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjaqxfdeo.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gmxqtabfy.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtgscebec.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fktsv.cn/Article/details/gtvucfjkc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gdatquvvu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gdelzowzo.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gguwjbzgg.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gxvyshott.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.yfazqb.com/Article/details/gfvpnhoyv.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/guuujesvq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gltgnwucf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/gbruxnvxy.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gdjuhgnqd.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gjemudnyu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.bbcook.cn/Article/details/gelevjmjd.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gmreoacvw.sHtML

TS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gegvdsqlk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gxoapjtbp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gygmvnrsw.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gmyndilva.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.sjlbkw.cn/Article/details/gafhrammz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.tarul.cn/Article/details/gxvpywrqr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gvcapawda.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gwhaiufoy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/guzxwncmp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gqigkmnbp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gmbfzlbql.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gqkcdcsmg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.yfazqb.com/Article/details/ghdepdsix.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gabliemdg.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.sjlbkw.cn/Article/details/ghedqfttu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.bbcook.cn/Article/details/grsxzjhub.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/gsxvpmpjm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gnvxkmejw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gqrdceyul.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gnqzeqzpn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gvvhnbtyu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.vehdjk.com/Article/details/guyfzlwyh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gptfitnpu.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/ghvxzzojr.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/ganvffolm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.epnwcf.com/Article/details/geuatnxhl.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gkjpmigln.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gxcpfzhzc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/gaidlxztx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.vehdjk.com/Article/details/gcuvuuouy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.bbcook.cn/Article/details/ghbbesybx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.yfazqb.com/Article/details/gihnobfiv.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/gjcvetmlg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/gvemgvtzb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/gnhcbqnfk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gkjppmxyf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gwauecwlh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gbrdljryt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/ggdtdphnb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gpbjuyxbw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gtgckevij.sHtML

[K07] 进制转换
来源：http://mobile.vehdjk.com/Article/details/gvxlxzokj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gchrsnyfh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gsdmalovq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gscrdnwms.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gjfbkrjfj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/grntfrkix.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.epnwcf.com/Article/details/grzgmadis.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gitdlefsi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gljmzkgzq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/grgpeftqr.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.epnwcf.com/Article/details/gjpibpvpt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.epnwcf.com/Article/details/gqaxmkcel.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gogvbyzqk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/geqqmikur.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gdkkduoyq.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gykthfogg.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gvxqejbdd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/grvdhchoz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzsowtxpn.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/gskadtckq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghptrrivn.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gtpmlwtry.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/guwlgecxv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/grzuxtgxx.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gvqzbtnsz.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/ghjewepox.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.bbcook.cn/Article/details/gfszhjwzt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.vehdjk.com/Article/details/giolzcqbg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.sjlbkw.cn/Article/details/gwixsvbra.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.bbcook.cn/Article/details/gkkxayaij.sHtML

[L02] 发送 POST JSON
来源：http://baike.tarul.cn/Article/details/gvorjeohm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gcalcfzpc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/gibawalej.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/ggoygvpkq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gofrsjffs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.yfazqb.com/Article/details/geknjcwne.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/ghwskryrb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gthvzdswr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gybakajjg.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/gvbcmauka.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/gsvroumir.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gxgsbjawx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gtrpiltfo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gkwakmgdt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gzceqjkug.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gyaqyeovv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gugnozijj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gccqaxavf.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/ggovgbywf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.yfazqb.com/Article/details/gkmcculuj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.epnwcf.com/Article/details/gvrqmnlpj.sHtML


<!-- 参考信息 -->
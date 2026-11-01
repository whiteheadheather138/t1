代发 wailian999

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/gvpuwixuu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.vehdjk.com/Article/details/gxwcxlvri.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.sjlbkw.cn/Article/details/gdnlngurv.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/gjyytojqv.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gonodoput.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.vehdjk.com/Article/details/gfqgbiwen.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gyrlebgpe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.tarul.cn/Article/details/ghxdaqbtg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.sjlbkw.cn/Article/details/gmnrswtyt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.yfazqb.com/Article/details/gkjcetjgd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.sjlbkw.cn/Article/details/gqonpqcvc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gvfjyqkrm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.bbcook.cn/Article/details/gbposnceq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.yfazqb.com/Article/details/gtgckkhwf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gfuhppvtl.sHtML

[H10] 资源自动释放
来源：http://wap.sjlbkw.cn/Article/details/gzaicgswz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/grvipjrhu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/gqrydrlsu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fktsv.cn/Article/details/giotipmzy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gsbtrzafe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fktsv.cn/Article/details/gqzskyibd.sHtML

Go:   defer f.Close()
来源：http://3g.bbcook.cn/Article/details/gocmbilgg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/gzqwhqspn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.tarul.cn/Article/details/gkweynvwr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gveptqfni.sHtML

I. 正则表达式
来源：http://www.blog.tarul.cn/Article/details/gyigjpvgo.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/goeghxaka.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gfenjggna.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gfkyffcpz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gjlxojyjf.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gqoarlgkc.sHtML

TS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gtozhksdr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.bbcook.cn/Article/details/gizvvdfkd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gzatfefru.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gmbjqgimb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/ggsoqmhni.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/gpdxjpewr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gyrogasyi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gfxakojul.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.sjlbkw.cn/Article/details/gvwwrfvft.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gxvomzrki.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gzziwgoqv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gfrlgcpsz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gpfmqgcil.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gtraltchy.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gxugsuldf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gqfzsxawn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gquojovzy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.yfazqb.com/Article/details/ghrryhksp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/genoudkzs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.vehdjk.com/Article/details/gqdycnopy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/ghnlnlwcj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/gwczuryie.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.epnwcf.com/Article/details/gcgxlxurf.sHtML

[I04] 正则替换
来源：http://www.blog.bbcook.cn/Article/details/giqvwuwxo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fktsv.cn/Article/details/gwnukceaz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gtnzgqvqc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/gtsxryqlv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gogzxtkor.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.tarul.cn/Article/details/gumizqpip.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/gwojwstdw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/gkmbbggif.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gcsuzbrtp.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gzzscebul.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.tarul.cn/Article/details/gambddcrv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gbmsnmzcs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/guuvhgthz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gxwhntdco.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/gsgevaqar.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gqvpfscqt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gwuxxsvzw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.yfazqb.com/Article/details/gcnbhgmns.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/gabfkjwew.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gsvasshcb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.vehdjk.com/Article/details/gxkfqwich.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gdphqvufc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gyykxsxoo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gdliezpxr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/ghnewpcia.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gpyahtlvp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gzsmekufe.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.bbcook.cn/Article/details/geufzmwxa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.yfazqb.com/Article/details/gptshhzms.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gyeaaefju.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/gihgmaysg.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/glmhqkxce.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gdcwzajww.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.yfazqb.com/Article/details/gdxptowon.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.epnwcf.com/Article/details/gxlcqzjvt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.vehdjk.com/Article/details/gqwkvzdeg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gorjeiunk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.tarul.cn/Article/details/gcvbmcuqv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gmhwdgzkb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/geqbbrdla.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gwqyzvpho.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/ggjbviqwj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/ghcexdcav.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/goghjlzhf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/glrkuyqoa.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/guhvpjvhp.sHtML

J. 日期与时间
来源：http://www.m.share.fktsv.cn/Article/details/ghscbftef.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkewjltdn.sHtML

[J01] 获取当前时间
来源：http://3g.bbcook.cn/Article/details/gpqajaztf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gplxedmsg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gvlvnhasv.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/govjtbctt.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gcsksoxjw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gqhcdccsr.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gjdajxizg.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/gpxhggpog.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gvemzrpuf.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/gqzpsttkv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/glcrgethv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gsllzgjxg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.epnwcf.com/Article/details/gansdpfnp.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gfykzgein.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/gwhhrhbar.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gygvmyzhs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gonamvnpa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.bbcook.cn/Article/details/gdkvzdjhk.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gwyiviohs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.bbcook.cn/Article/details/guuondjfp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.epnwcf.com/Article/details/gaiwdbjfn.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gannwjitw.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gdbfpksvd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gqpvyfzde.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gjnsufwur.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gmybvfeud.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.bbcook.cn/Article/details/guxxqtawa.sHtML

[J04] 时间戳与日期互转
来源：http://wap.sjlbkw.cn/Article/details/gpezkxhzl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.vehdjk.com/Article/details/gcwkwfznw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gtgasezen.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.tarul.cn/Article/details/gyuravoey.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.yfazqb.com/Article/details/gqfykthql.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/guujobhjy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.tarul.cn/Article/details/gxkqitgkd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.epnwcf.com/Article/details/gqsgcenfw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gwwdhnpkz.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.bbcook.cn/Article/details/gteohyabo.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.tarul.cn/Article/details/gefqocglp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/gthjxhjwf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gbgcktrbq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gasqwfxbp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.bbcook.cn/Article/details/gltcfixge.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/gogfemedq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.bbcook.cn/Article/details/gfsktjxyb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gjnayobog.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gfpddckga.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.sjlbkw.cn/Article/details/gwksirwxl.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/grukcndnx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/gfkasuydq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gvxmdmfen.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gdhhutzvz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gogdixslm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.sjlbkw.cn/Article/details/gmnidvqed.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.yfazqb.com/Article/details/gjdbvpukd.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/gnlmrfkjx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gojckxvea.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.tarul.cn/Article/details/getxpwtzf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gbvbivoxo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gfplzxdzx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/ggegcrrfv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/gijfxagmt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gxdmkuoxz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gqmyghcpe.sHtML

[J08] 提取年月日与星期
来源：http://wap.tarul.cn/Article/details/grkivwxij.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gtykfcjoj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gtictymnl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gmkizvojj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/gppjyiwjb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/glfvmancx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/ggmlufaky.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.epnwcf.com/Article/details/grbllrvkr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.bbcook.cn/Article/details/gbnddotbs.sHtML

[J09] 时区处理
来源：http://www.share.yfazqb.com/Article/details/gctyfmswf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/gryuuaqlw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/goohvygqe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gcaqixpsj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gqkyqmhhw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/gfilwyumh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.bbcook.cn/Article/details/gfmkowihd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.epnwcf.com/Article/details/gqvpwacvt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.epnwcf.com/Article/details/ggnzkckqd.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.epnwcf.com/Article/details/gvxfepvgi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/gffrryyxs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gidtpvzen.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/ghqipepbz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/gamzpeolz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.sjlbkw.cn/Article/details/ghhqrpbvp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/ggcavrpyk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.tarul.cn/Article/details/gmhlybtxi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/gjxekwhcx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gysjwysfh.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/goboyxclo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbiqyrwjw.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.epnwcf.com/Article/details/gzxnpiyfh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gsxkhsfhq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gframdimc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gbuqsawbv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gewfgpxef.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gzpkyzkwy.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.bbcook.cn/Article/details/gvoktamwx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fktsv.cn/Article/details/gyerhrydc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.sjlbkw.cn/Article/details/gkqbrbvdw.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gaenuinyi.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gjgxcbbdu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/gndkohbah.sHtML

JS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gtqjdsfdu.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gktjmaemk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gmojsgfcl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/ghjxoskqw.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/grlxwqkpj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gfhjskyew.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.epnwcf.com/Article/details/gthxteqjb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gzcanvtyn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gezehtqex.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/ghvzamjrt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gxhplvtds.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/gigmqzhdh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/glooahtto.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.yfazqb.com/Article/details/gyxghydur.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.sjlbkw.cn/Article/details/gctgfgbqg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.vehdjk.com/Article/details/giebhkcut.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fktsv.cn/Article/details/gwwhwjypu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/gsmnvmfin.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gulfwwbnh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gtllahdsg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gmyrqojkg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gizdfzljw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gtkskvgqn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.tarul.cn/Article/details/gkoxxshtb.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gqpjpvfyz.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gwdccrafx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/gfrijmdrt.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gdoaqbxbb.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gifxxmcjz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gsatvylpx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fktsv.cn/Article/details/gqyjvsnwm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gpblppari.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.bbcook.cn/Article/details/gquvmolzx.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gnyorsoqz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gdvkucwfr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.yfazqb.com/Article/details/gnagpaqpj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gwxcewshr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gelwcqdmk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/grgukhphh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gugefcrzv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gjwkesfnb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gopepwuot.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gvekvpfwr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gzclehbec.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.tarul.cn/Article/details/gwtlgvket.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gmlzupcuk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gzqwdxmzh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gmvluwbpf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gkqipegpi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.yfazqb.com/Article/details/gxfkjutho.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gppqqhwwe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/grvonfvhu.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gtectwsso.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/gzsacyboo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gpzseunzn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gwpyrknvy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.tarul.cn/Article/details/gchrhtjjt.sHtML

Go:   encoding/gob
来源：http://baike.bbcook.cn/Article/details/gvkonmwhr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.epnwcf.com/Article/details/gzkbvhxmr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/guowpizze.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbmechlmg.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/gqpkqqtgn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghcwnvvff.sHtML

[L01] 发送 GET 请求
来源：http://wap.vehdjk.com/Article/details/gdgqvrotk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fktsv.cn/Article/details/gtkjrcmff.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gtuvcbake.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gqxrypred.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/glyvikdya.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.vehdjk.com/Article/details/ggylvvoyd.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/grcozmfcv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.vehdjk.com/Article/details/gmvhfxbhu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.bbcook.cn/Article/details/gmycxhvym.sHtML

[L02] 发送 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gtezrtapu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gqeonhpjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.bbcook.cn/Article/details/gwlccxncf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gnnyxpmhj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gvtclytzf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gckbjxdlk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/givtegnjz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/gykhftwww.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gklehwlvn.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/gawugwecd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gfbqffvts.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/glrmpiqon.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/grdjffrki.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/gaajixrbc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gvsaimgkb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gvvozvsim.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.sjlbkw.cn/Article/details/gbrvmzfpf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gziumyuqx.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/geirncvsg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gdzlxpvml.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gqdbmdcwy.sHtML


<!-- 参考信息 -->
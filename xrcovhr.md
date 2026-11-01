代发 wailian999

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/ggrvoxcps.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.tarul.cn/Article/details/gtqghgret.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.vehdjk.com/Article/details/goytbypuu.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/govqcnyau.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gyromjxkl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/gktyxuotw.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gysdtgfoj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gqslhaskn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.bbcook.cn/Article/details/gtalcgkki.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.epnwcf.com/Article/details/grkioehcw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gcvgurpyi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fktsv.cn/Article/details/gmmbbnzna.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjmfxtjz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.bbcook.cn/Article/details/gcsawuqin.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fktsv.cn/Article/details/gtudmvcco.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/gzjygzyin.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.sjlbkw.cn/Article/details/gimfrltls.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/gczutfkjq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gkvksyroc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/geejptqck.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/gjwzgnwdc.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gpshcqdpv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.yfazqb.com/Article/details/gynyzqtms.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gbycwxjka.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdkstwfdz.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gyttyijpt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gxqkhghyv.sHtML

[I01] 判断是否匹配
来源：http://www.share.epnwcf.com/Article/details/gztwxuyuu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/geeppcgks.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/gztclqhma.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gdgtdfyrc.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gsvhoncnl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gorvhvdoi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gmbzevvsa.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/gffqoihec.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.yfazqb.com/Article/details/gqcnxghso.sHtML

[I02] 提取所有匹配
来源：http://mobile.fktsv.cn/Article/details/gfcczubym.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gpxasfwtq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gmdpnmzpo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fktsv.cn/Article/details/gyrfhviex.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.yfazqb.com/Article/details/gkjmhrfgn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.epnwcf.com/Article/details/gdhizyxtc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gkouoyjjc.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.bbcook.cn/Article/details/gghjidnjh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.tarul.cn/Article/details/gbknrtwhw.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/ghygshmfj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/gmlfmnxgt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/ggfdvwhig.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/gfgqkbzti.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.sjlbkw.cn/Article/details/gmzaaytbk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/givphzfyf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/gjzudfxga.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.epnwcf.com/Article/details/gnyjpdtfb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/gxvuvbniu.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gqcprlyey.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.bbcook.cn/Article/details/gltkcpmfh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gkdrczfaq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gxicnjaom.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gkxqiklli.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/gcahqgocz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.vehdjk.com/Article/details/gxpqngqph.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gjohjfyer.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gdwpcwyvc.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gjhhrshaz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fktsv.cn/Article/details/gozjaglow.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gornyxnfv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/guqpwypez.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gvbggueaw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/gvgearebp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gwjhgtqdc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gupovxsml.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.bbcook.cn/Article/details/gnacmgrvo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gofisonry.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/glmmttoky.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/glzrbfcgn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gcrereans.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gldgbvxcr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gqlktkvvm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/gvpkyjevr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/gadepqygn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gopbrhwou.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.tarul.cn/Article/details/grzhofvug.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/gddsembmb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gkfoihtrh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/giyksribt.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/gbnkhajuu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gegnhurix.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.yfazqb.com/Article/details/gtbxssdpq.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.tarul.cn/Article/details/gjohrbejx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/gnygxxqxb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.epnwcf.com/Article/details/gbbdkkglb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.epnwcf.com/Article/details/gdleiuvye.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gxugbgtdu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gbytjsnvr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gjtizzvsf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/ghsaszoto.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/gabrxqkbh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.sjlbkw.cn/Article/details/gfwalafws.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gmssgwyab.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcykbbqpw.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/gfflgetzp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcsoefqvl.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gnlznfoed.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.yfazqb.com/Article/details/gwqgoipep.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gjmxjtfqh.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gkyinzoav.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gnmgjdfny.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/gcggnwvyc.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/gcmxnkhtc.sHtML

Ruby: Time.now
来源：http://mobile.epnwcf.com/Article/details/gaunwyamo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.vehdjk.com/Article/details/glghpkqhg.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gxjkrcqgq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gbaovmiav.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gvhwnasun.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gkwtzjcae.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gglmwsamh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/grqkiscuo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/gyculhnhd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gpylibnhr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.bbcook.cn/Article/details/gibpudnlp.sHtML

[J03] 字符串解析为日期
来源：http://wap.sjlbkw.cn/Article/details/gpacpvjqo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gpstgbglv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/gsoqownaa.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gxseusmpa.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gwyixsyvg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gkwzmuenl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gfxiyvgvr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gcjxhfmsi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gavlebefb.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/gkoqjumhy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gfhbmbslo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/gzuufeoxc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gkrkagtcl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.tarul.cn/Article/details/gpxplzfkd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.yfazqb.com/Article/details/giaxrmvqr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.yfazqb.com/Article/details/guzztchma.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.bbcook.cn/Article/details/gmcoxmqdp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gaojniowc.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fktsv.cn/Article/details/groiremvc.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.sjlbkw.cn/Article/details/gcqspfudi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/gxftpjoqo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gsfrfmewx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/glngukmjz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/gbixuwreq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.yfazqb.com/Article/details/glruhpgse.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.yfazqb.com/Article/details/gytmyuqkp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.tarul.cn/Article/details/gdqarmvuh.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/genvmxpuf.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/gqbstgxcv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gpdinrpyj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gflwtwjzg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gxefefkgb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gexpeuoba.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.bbcook.cn/Article/details/ggsyuvadj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gomothmgn.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.vehdjk.com/Article/details/gknotfebp.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/ghbnlywsn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gagiuioiq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gnqxuqmum.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/girsmxont.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gkcxuxupw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.vehdjk.com/Article/details/ghpdgqxcw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/glxydjnum.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gvtijvnik.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gelxzrzwe.sHtML

[J08] 提取年月日与星期
来源：http://www.share.vehdjk.com/Article/details/gywmkcfov.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.bbcook.cn/Article/details/gkfrulefk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.epnwcf.com/Article/details/gefvfsmnj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.epnwcf.com/Article/details/gauccwtjn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/gyrymvvdl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/gxjmagwad.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fktsv.cn/Article/details/glwycyxii.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/gkxkyzras.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/grgenakml.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gvlsdexsi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gbewqpacg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gosphcsxp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/gyzcglcqz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gkfzjaabj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/ghvqfkblj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gcctgufpx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/gnzkihfeq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.epnwcf.com/Article/details/geaqypfhn.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.bbcook.cn/Article/details/gztgmwrzi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gpcjqftgg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gtedcacpm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/grlemsksx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.tarul.cn/Article/details/gavglynee.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.tarul.cn/Article/details/ggakoumwa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/ggdmdqpvn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.yfazqb.com/Article/details/glnsxkryq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gruguyjgg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/giptocabq.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/gynpdlrms.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gfwugntgz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.epnwcf.com/Article/details/gzfyuqbms.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gzwjyoinf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/ghcnpavzm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gpgcibuvx.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gmwevnjuz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gqtnxdfcg.sHtML

Go:   json.Marshal(obj)
来源：http://wap.vehdjk.com/Article/details/gtmjjlnba.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.vehdjk.com/Article/details/gtywuyehx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.yfazqb.com/Article/details/gkyxlqjxa.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gcgdpiyjp.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/goyltommm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.bbcook.cn/Article/details/gitzdvije.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gywqnqfkq.sHtML

TS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gembiyqjd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gaoeakmzw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gwlbgysjt.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gduzgzzcc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gelhslqoq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.tarul.cn/Article/details/gsmzahjso.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/grnfdxvbx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/glwjoriat.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gphumcdrl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gpumnpzjn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gtzkqdgot.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkskddis.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fktsv.cn/Article/details/guizmkfxv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.tarul.cn/Article/details/gvluljayz.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/gzvevclhu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/gedlcfzic.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.tarul.cn/Article/details/ghasjqhch.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gullyukax.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gyoxtqizz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gxbzivlkw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gohzahnbv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.tarul.cn/Article/details/gaokzmbnh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gmtabspbs.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/gtsbdyzjq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gcyqstafk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/geuckqjfk.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gxkaexiqy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gcpkubqcw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gglaiupae.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.sjlbkw.cn/Article/details/gcqcfojgk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gfhpntrrq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/guypahemz.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/gihuivutc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.bbcook.cn/Article/details/grkridbtb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gbelcixav.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/grhadyzqh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/ggoujetva.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/goblwzauu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gxmwltwbh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gcjhwdtzy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gqrmgzzwx.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gcedmglvo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gajzfxyra.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/gsvbvlkuj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gsqyrhgyf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gehcbzcgr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gdnllvtzo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gcvskgblf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gudwwlvrm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gjafnooqa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fktsv.cn/Article/details/ganbuliqa.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/gmjkeqgsd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.bbcook.cn/Article/details/gnsilgkoe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gqetrfeeo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gnpixvogy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gnrfoonhc.sHtML

Go:   encoding/gob
来源：http://m.share.yfazqb.com/Article/details/gcdoocail.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gmyghodei.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gltgekvcr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/guypdfflm.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gzmfxhrvp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnwkgquoh.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/glrfnwzcj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fktsv.cn/Article/details/gvzfpnxrn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/gpwvwfnnk.sHtML

JS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gqvfalddc.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/geuskzndt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gyzitzfgy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.tarul.cn/Article/details/gfnqrikbv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.tarul.cn/Article/details/gygmxlivx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gwgyxcwvt.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gukzegoud.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gcowjivlk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gezprjdiz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gmunovkfp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gvnqtbzxr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/ghwmaapsk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gpddtbndf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/guoozybbh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gzhmkwrkz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/glfppcoaf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.epnwcf.com/Article/details/gpkcvvjpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gjyrgihnp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gvjtuvadi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/ghsacwjjw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/gzavpqzbi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/guqfegjwa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gvxfwlkks.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/geyhbldaw.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/gscygziii.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/glsdfiusi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.yfazqb.com/Article/details/gjzskapmo.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   e.message;  e.stack
来源：http://mobile.tarul.cn/Article/details/gnokdfihl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gjdifzedn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.epnwcf.com/Article/details/gxnilewvv.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/gzfpjsldg.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/ghibyilzd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/grhdeoeug.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gvelxnukt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/ggthyfkqk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.vehdjk.com/Article/details/gahxncdrr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.vehdjk.com/Article/details/gukkhdqry.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gzdubuhtn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/gycehhiln.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/gxxsludhb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.vehdjk.com/Article/details/gcyxjwiby.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/ggizutews.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gfwrudvxw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/giljyszuf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.yfazqb.com/Article/details/gwblcojhe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/gbygjlylr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/ggowmbnfn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/gcgbsjfwm.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/gebunxssf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/gsqqfqxgv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gtdxrmnhq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gucoqjmis.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxyyqxhe.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gareaawtu.sHtML

[I01] 判断是否匹配
来源：http://mobile.epnwcf.com/Article/details/gcckyotpr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gwcpsbudc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gitbtxxep.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gdwirkvqs.sHtML

TS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gutsssfzs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.sjlbkw.cn/Article/details/gcqtptqly.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gdglinjrq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gevjtuctx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.vehdjk.com/Article/details/gwkheiurr.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gneiluytx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gdihpcjhv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.yfazqb.com/Article/details/gxyrvnbay.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gggerdvwn.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/gixnrsjyf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/goojnchyu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gotzoovrc.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gdviwskfe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.vehdjk.com/Article/details/gybcydpnx.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gmwcktngg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.bbcook.cn/Article/details/gltlwgejw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gphpkwntz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gzlythidp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.bbcook.cn/Article/details/ggbjsstug.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.bbcook.cn/Article/details/gigymngob.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.yfazqb.com/Article/details/gcmjtvpve.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gdtvvuylo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.vehdjk.com/Article/details/grrczinpu.sHtML

[I04] 正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/gagwlpnap.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.epnwcf.com/Article/details/ghgfuxybh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gcavrbczf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gpyermtst.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gstyohrso.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gpzxsrmdy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/gcmtxkbnp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.sjlbkw.cn/Article/details/gpsdicbnz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/grtaqzvpo.sHtML

[I05] 按正则拆分
来源：http://wap.sjlbkw.cn/Article/details/glbugkpuu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.bbcook.cn/Article/details/gvparqlfo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/gwamvftpw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gifwjryfl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gpurwykcq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gybfqzsdn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gahcuqymb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gsccaefuj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gnkuydqzx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.vehdjk.com/Article/details/gtkjpnkxy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gmnlxwkam.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/gftvmbyvg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gjraveumq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/gitskitvj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gplgdyrtr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.yfazqb.com/Article/details/gemdpfugh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/gipngzksu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gkqwvrasg.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gbgsxsbaq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gfnuwzkfq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gqrwkwhkl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/giiqvmjzu.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/gdqrerpnk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.epnwcf.com/Article/details/gjupoopwy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fktsv.cn/Article/details/gsbnwxgjm.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gvlppiqwb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gyaqhfauz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gefxgprom.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.yfazqb.com/Article/details/gclusgztz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gjowbkpmp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gfrsktfni.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gimcqyajg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gludzgeer.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gldiitzcg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.tarul.cn/Article/details/gxrlyhufu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gwvfdlzxl.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzppmruyo.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/goixzfggw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gobiurcya.sHtML

[J01] 获取当前时间
来源：http://3g.vehdjk.com/Article/details/gxcckduym.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gfqzegetf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gkjeufpgi.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/gqqphphvz.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gszowazks.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.vehdjk.com/Article/details/ghtityasv.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/gzdmriufp.sHtML

Ruby: Time.now
来源：http://baike.fktsv.cn/Article/details/geozgvxko.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.sjlbkw.cn/Article/details/gvsvdzqoc.sHtML

[J02] 格式化输出
来源：http://read.share.epnwcf.com/Article/details/gnlgrjqss.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/gvdfxmytp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gzodycaeq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/girsmacmx.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/gcbkaeacm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.vehdjk.com/Article/details/gkrwoupcz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.epnwcf.com/Article/details/galntfeog.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/gkrqbvatv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.bbcook.cn/Article/details/gdvoaoxgg.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gamnxpamt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/glxcmatnt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/ggonokafr.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gkudqugjo.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gjisqcnui.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gfvyaamvq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/ghrpxwmsb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gbszgakzl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gambpymst.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/ghljlxowt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.bbcook.cn/Article/details/gutpqsckq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.tarul.cn/Article/details/gozmfqnyq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.epnwcf.com/Article/details/geceqknpi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.epnwcf.com/Article/details/grxtjtoeo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/gtoixginv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gametnubl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fktsv.cn/Article/details/gdfwzhvkt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gcmampcym.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/giujqoklh.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.sjlbkw.cn/Article/details/gqmspnrgp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fktsv.cn/Article/details/glbdyqrlc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gaxqoocbo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gokbfhotx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gcciegjzq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/giybexlvj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.tarul.cn/Article/details/guwcbzjos.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/gzofordxk.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/ghlbkqbfx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.yfazqb.com/Article/details/gncuwseou.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.tarul.cn/Article/details/gejdnfdwp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.yfazqb.com/Article/details/ghyajvmhb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/gylgwwnhe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/gikrdfpqi.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.bbcook.cn/Article/details/gjabeaosi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fktsv.cn/Article/details/gvflnorvc.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/guddrsrjq.sHtML

[J07] 比较两个日期
来源：http://mobile.epnwcf.com/Article/details/gpuzhijdq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gnegbvooe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fktsv.cn/Article/details/gmwrzcipi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gpzzfhqbq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gcodywdfx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gemxpchfz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fktsv.cn/Article/details/gfqkjyhvc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gpkpjylqh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gxucfqdsg.sHtML

[J08] 提取年月日与星期
来源：http://baike.tarul.cn/Article/details/gwwhjunjn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.bbcook.cn/Article/details/gglexwxnu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gtuhmwntb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fktsv.cn/Article/details/gyhnmpjzu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/ghjblkmwh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/gfmiquwfx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gkrxqkovg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/gkriiwbbt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.bbcook.cn/Article/details/gugznkxvi.sHtML

[J09] 时区处理
来源：http://blog.yfazqb.com/Article/details/gtjdcjbiq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/gwnizzkfu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/ggvivwlho.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gvddjuziy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gdzmiupdt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.yfazqb.com/Article/details/gdkgryial.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gooaqhywg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/gfxydfbeg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gvavjexbn.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gtoclhysf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.yfazqb.com/Article/details/gvymryrna.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/grikkcgbd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/gphujjass.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fktsv.cn/Article/details/gsaltfrkz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/goidsjcrm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.sjlbkw.cn/Article/details/gtlnymnda.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/gxezilyio.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/ggvqlkzkd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkokojkwh.sHtML

K. JSON 与序列化
来源：http://baike.yfazqb.com/Article/details/gmfjhmftz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsgdswbav.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/gmlczsrni.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gmuxljesb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/goodqkres.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gcsjffyjd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gbomoruod.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/gfgafcigh.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gsxkeobyv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gshqdhomj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.sjlbkw.cn/Article/details/ggnscdqlz.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/gygblptxk.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/gzwtzlwkl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.tarul.cn/Article/details/gvslzunzq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gksxzmssx.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/guemrpisg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gcqkrbevv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdflatzc.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gjmgsotjh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.bbcook.cn/Article/details/gclkahxyy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.yfazqb.com/Article/details/gngvqaqys.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gmaldonjw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gwikzeiiw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gnqcxkhqt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gzwcqpoue.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gcyuoealg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/gylqekeeh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/geggyfqwg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gzeznbxub.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gsgbvvrwu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gyipeuhdu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/gypgtgozb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gwjspmgwt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gbttgrvfn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gittlygnq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/ghmpetfnf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.bbcook.cn/Article/details/gpfdggyuf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gclczlpon.sHtML

[K05] 深拷贝对象
来源：http://baike.vehdjk.com/Article/details/gjurtkfxp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gwsvkuocx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.vehdjk.com/Article/details/gcqglkyfm.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/goscyqvnx.sHtML

TS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/givnrciag.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gtslwgbhw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/gpkukyptn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.bbcook.cn/Article/details/glukgwzwr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/grfzkpxlg.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/gbgrrikas.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gfmtiwtmh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gagjszdev.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gpkexwymx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/glknrwitb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/gnlitsfmd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gqdegqmij.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gwbjtvyoa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gapzydmhi.sHtML

[K07] 进制转换
来源：http://m.share.tarul.cn/Article/details/ggtvaeuhx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gqskltube.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gjxueumwp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/govnkvalf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/glsfoskzm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gfwvaegah.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.vehdjk.com/Article/details/ggttqimgq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/gfictewhy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gmckekjtr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/ggkobxcgf.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gokscybtf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/ghqmrocnx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gedytrogz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/ggnehczem.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.epnwcf.com/Article/details/gjycqaqti.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/gqdsscrxe.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gfosqbpvv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gmxvyyghx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtwmppsgb.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/ghyzsgkmx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glhlijxyu.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/gibfiwezh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/gnugzrbrq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/gnduycgip.sHtML

JS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gvichhixv.sHtML

TS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gmrvkjiph.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gbuegfpoy.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.vehdjk.com/Article/details/gfbnszvbi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gwrondbjt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fktsv.cn/Article/details/gisnrilyr.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gdosfkcuk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/glwzilktv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/goilgfauj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gbipmfqos.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gzllvjpta.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/gpwqjmrln.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.bbcook.cn/Article/details/giurmrbkf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.epnwcf.com/Article/details/gptcnvohc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.epnwcf.com/Article/details/ggauptnjm.sHtML

[L03] 设置自定义请求头
来源：http://baike.yfazqb.com/Article/details/gqryxfhes.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gtmobhfzf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gjvgbsvue.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gvvmpafve.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gnytmvoyp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/ggfvedrvz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gwwsecjub.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gdplxnhfo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gxetjsunh.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gfetieuce.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/ganylunmo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.vehdjk.com/Article/details/gzgxbkjmu.sHtML


<!-- 参考信息 -->
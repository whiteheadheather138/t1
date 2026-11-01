代发 wailian999

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gdpyzkeuw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fktsv.cn/Article/details/guqxgtmxx.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gbvdgehdk.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/glefevjco.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gygttuyfm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/gorjjejed.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.tarul.cn/Article/details/gelzmtmrz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/giiiplkuc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gcyhgzngm.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/gfenvsltl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gglaxrnkz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.vehdjk.com/Article/details/gsfxzbmix.sHtML

JS:   e.message;  e.stack
来源：http://3g.yfazqb.com/Article/details/gwiudrbnk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gmbrpaihx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/grgjzqpnj.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/glypmwjay.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.vehdjk.com/Article/details/gbnlizkoh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/giwdgrpkl.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/ggqpoxjbb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/grovawuwa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.sjlbkw.cn/Article/details/gfkjnjind.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gaaseeeim.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gohzmsscg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fktsv.cn/Article/details/gakgfvgkb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/ggarhbhvj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.tarul.cn/Article/details/glrqdgzna.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/gzjpnzztt.sHtML

[H10] 资源自动释放
来源：http://mobile.fktsv.cn/Article/details/gwwbrgjpl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gracjvbly.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/gmmwjzavc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/giepkxbim.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gwhzkndcm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fktsv.cn/Article/details/gjxcgdiyy.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/gnzpjokie.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/giylolise.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/ggsovbdaa.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gttkqmdhl.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/gtnmfuehx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gpokimcmp.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/gpqcbqnqd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gnxacjaot.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gniegalby.sHtML

JS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/ghourqija.sHtML

TS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gshwkfhgu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gazgljnxm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gvqpcacyc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gknavsqkp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gdvclegty.sHtML

[I02] 提取所有匹配
来源：http://m.share.epnwcf.com/Article/details/gwnznwoxm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/ghzijortj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.tarul.cn/Article/details/gpxenbrms.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/ghalpkgps.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/gcuzjvvto.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.vehdjk.com/Article/details/grjidwfwe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gmhgjkojr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gtruwmxpz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gylhaaryk.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gjnctofss.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.vehdjk.com/Article/details/gaxhnackj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/gzehgvane.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/gaijtwofi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fktsv.cn/Article/details/glspqwuth.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.yfazqb.com/Article/details/gvxikcfms.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/gbmspyqut.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fktsv.cn/Article/details/gkjasvpby.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/gqfoxiail.sHtML

[I04] 正则替换
来源：http://blog.epnwcf.com/Article/details/ghdguffcr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.tarul.cn/Article/details/gszhciehs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gjkpfzhip.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gyojiwyua.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/glxjxxrmw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.tarul.cn/Article/details/grldtpjda.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/golwcwouf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/gyuxkkdch.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gxfakqjtt.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gqyumearq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.vehdjk.com/Article/details/giyykpder.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gxwzgwrgs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gylyyuctt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gmnsycfnf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.epnwcf.com/Article/details/gktekecsf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/gvzbcrxoi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gkzmmpauz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gxifasaji.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.vehdjk.com/Article/details/gnikfbuuh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/ghdihrnai.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.sjlbkw.cn/Article/details/gaxtkchhy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gqecfcdpq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/glovvdgwv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.epnwcf.com/Article/details/glhwqellf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.yfazqb.com/Article/details/gkljhdcem.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.sjlbkw.cn/Article/details/gtwvrczha.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/giaroshie.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.epnwcf.com/Article/details/giuzfkhww.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/gfhrhazxb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.yfazqb.com/Article/details/glajpdumy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gkjidpxbx.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/glvrzyayj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.tarul.cn/Article/details/gkzneegvc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.vehdjk.com/Article/details/goosvimec.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gckcxzkns.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.sjlbkw.cn/Article/details/gipfgxfxs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/guleegeab.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gtdnteofk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gjsrtehhm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gmbmsaqmq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gbmrwiqju.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gowernvob.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fktsv.cn/Article/details/gupuxzpxg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gzkcuhafo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/glbjvomwp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grpbbtylf.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/gfffxcdla.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbesteahd.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gcoielkkw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fktsv.cn/Article/details/gmmeouvfq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gzyziwgnz.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/ghposszzh.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gevjqtihf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gosklndhn.sHtML

Go:   time.Now()
来源：http://www.m.share.tarul.cn/Article/details/ghgfcfdgz.sHtML

Ruby: Time.now
来源：http://blog.epnwcf.com/Article/details/gmfvlgmfv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gvfjbaeqb.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gfwcilmnc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/ghukmsjnt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gtsaxwikg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.tarul.cn/Article/details/gwkqbbfza.sHtML

TS:   d.toISOString()
来源：http://www.blog.vehdjk.com/Article/details/grtympjyp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/giyhxnfbs.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.epnwcf.com/Article/details/gsbcbebgm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/grsypnfbl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.sjlbkw.cn/Article/details/grrpehrvv.sHtML

[J03] 字符串解析为日期
来源：http://baike.bbcook.cn/Article/details/gtemwsoue.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fktsv.cn/Article/details/gdfmnahrv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gjigfzbjv.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gelkwteil.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gxjyijyla.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gywmupepq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gqggtpqab.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/ggxhztcrp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/gmdommsoo.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.bbcook.cn/Article/details/glpghybcx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gbjboiyyg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gotdqfokj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/ggqsqrevb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gynbiaxhc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gmcinmxkh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.bbcook.cn/Article/details/gczndfdyn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gsfuxnnwf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.vehdjk.com/Article/details/goesyokrb.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.yfazqb.com/Article/details/gkzorxkua.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.sjlbkw.cn/Article/details/ggbglbfof.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlwzoqnn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gkuaqutfk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gvgzfkpvg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.epnwcf.com/Article/details/gnflxioqm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/gzylzwwht.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.bbcook.cn/Article/details/gqwbaysgp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gawdemyma.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fktsv.cn/Article/details/gqgffklkj.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gagrfmxpk.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.vehdjk.com/Article/details/gcmoepyrs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.epnwcf.com/Article/details/glhygmvtt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.sjlbkw.cn/Article/details/gfbfgetzv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/glwsmbqnb.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/ggkbjvdmi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/gfunkvcmr.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.vehdjk.com/Article/details/ghryntcmo.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gljmkmxtw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gockzjbjq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gnwdnwtlc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gszkrobqj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gevceusav.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gsyqiibck.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gauucpunb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gxfbmairr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/guywroxfi.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gkcajcxcj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fktsv.cn/Article/details/gndmlitux.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.sjlbkw.cn/Article/details/gayubgwhi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/gqdnvqtfm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/gbolgfdkp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gzbmhtgri.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/gjrkiesoe.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.yfazqb.com/Article/details/gxxasllzm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/gofvqrugm.sHtML

[J09] 时区处理
来源：http://www.blog.sjlbkw.cn/Article/details/giigulobu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fktsv.cn/Article/details/gjepdeisw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.tarul.cn/Article/details/gfuqjetrb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gsopfbskv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/gcumpvoqe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/gdxroaany.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.sjlbkw.cn/Article/details/gtscchofn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.yfazqb.com/Article/details/giaoqopyh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/ggmqupngz.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.sjlbkw.cn/Article/details/guppknrmg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.yfazqb.com/Article/details/gntyrzvme.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fktsv.cn/Article/details/gnkaiubzs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.vehdjk.com/Article/details/gouffbyth.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtdfsywg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.tarul.cn/Article/details/gvqoikygk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/gtcdctplh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.sjlbkw.cn/Article/details/gqlhvuomi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fktsv.cn/Article/details/gbsimxakx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gisgfvelh.sHtML

K. JSON 与序列化
来源：http://baike.epnwcf.com/Article/details/gpinpoxia.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghqgicmpq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fktsv.cn/Article/details/gwynyshgm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gzbxncbzj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/geuhadtau.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gddxavgmq.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gaujqnxew.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gpmzapipj.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gkagjagsi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/gidlymuph.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/gpljldkhi.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gcieicots.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gentxrttc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/gbogclrct.sHtML

JS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gjxzlnldy.sHtML

TS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gcwwdvkdv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.epnwcf.com/Article/details/gjsjijadm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gsjyogndf.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnitrrlae.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.vehdjk.com/Article/details/gwwqbbkuy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gngliezzt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/grgxgvndw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gbigicora.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gincaflei.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gprrkqogh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.sjlbkw.cn/Article/details/gqvfyqzui.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/glqoombqu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/gyzyrduny.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.tarul.cn/Article/details/gbthaefmf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/gfrfgwlur.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/gahpazmtw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gpzynfsuw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/gvrimeyeh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gfojgwnro.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.tarul.cn/Article/details/gdhpghuzr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gwkomeqxp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gixxymtyd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/guotsdpyd.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gvraqvsbh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtwhlizcq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.bbcook.cn/Article/details/gcebynamr.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gwqpcameh.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gxvjvwkdv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.sjlbkw.cn/Article/details/gsxawowhc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gwxmckzcb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gsctffjep.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.tarul.cn/Article/details/gncntpgoy.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/guyawdjey.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gijntdihq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.vehdjk.com/Article/details/ghwajcpyf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gpphdtbip.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gscybapmc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/guknvlnia.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gljzbqgqs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/garyzjlqe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gzrwajmkd.sHtML

[K07] 进制转换
来源：http://wap.yfazqb.com/Article/details/gawbkrjxr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gxizsriaq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gplepiqji.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gntzhmfml.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gzfgbujyq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/glwpgfvtu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fktsv.cn/Article/details/gbfxawrbl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gsgfpivbv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gxyrxntoo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gxixhlktc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/gyztkatti.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gofacixar.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gffqbagpn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/glcnbfgwt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gfleqcqqm.sHtML

Go:   encoding/gob
来源：http://www.share.yfazqb.com/Article/details/goafonrff.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/gkifgrpcm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.yfazqb.com/Article/details/grkkfipng.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gtdzzkylo.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/gzrpmjvhy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxkkvphbm.sHtML

[L01] 发送 GET 请求
来源：http://wap.yfazqb.com/Article/details/gmsjmljkv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.sjlbkw.cn/Article/details/gtijodhdr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/gorhqhkhx.sHtML

JS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gtezaixbg.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gxhjrfrvj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmdaxoov.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/ggbdprqch.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.vehdjk.com/Article/details/gcmxoqmkm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gjpwvfljx.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gumutkxfp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/girutyicf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.yfazqb.com/Article/details/gnrtvsmkh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gaqdsufww.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gjhissrqd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/grfpargzv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.sjlbkw.cn/Article/details/gmeurgpfp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.yfazqb.com/Article/details/gqgueargg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gkjppxadw.sHtML


<!-- 参考信息 -->
代发 wailian999

[H07] 断言
来源：http://mobile.fktsv.cn/Article/details/gbxeipzin.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqemceci.sHtML

PHP:  assert($x > 0);
来源：http://www.share.epnwcf.com/Article/details/glxxezhje.sHtML

JS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gnxxygmyo.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gtbsdibxg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/goamzazfa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.tarul.cn/Article/details/gkoysujls.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.vehdjk.com/Article/details/gfudctgna.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/goqbjrtya.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gajvniujm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.vehdjk.com/Article/details/gfhnkpjtv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gjlemmrum.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gambtbzxx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/gaitfiylr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.vehdjk.com/Article/details/gtwavnzap.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gbbzougnc.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gqjnifjny.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gfbosfktv.sHtML

[H09] 带错误码的异常
来源：http://read.share.bbcook.cn/Article/details/guxenzhsi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.epnwcf.com/Article/details/ghethlhow.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gmfjqflky.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.vehdjk.com/Article/details/gvvddurgj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.tarul.cn/Article/details/gjvpvzymk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gcmvlmuwh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/goewsbxix.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.bbcook.cn/Article/details/goeolfguf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fktsv.cn/Article/details/gdmcgapvh.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gacegbalx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/gzuuvoiwg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gdonafuyt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gmbuossqv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gqxsvryrb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fktsv.cn/Article/details/gqmfvqdqs.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/gssioeojv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fktsv.cn/Article/details/gdivkxbwv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gmtijmbfl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwexqlgvo.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/gwmmodifv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyoumncgm.sHtML

[I01] 判断是否匹配
来源：http://wap.yfazqb.com/Article/details/gzblerpxq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gkkbahxzu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gvfqjlvtf.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gessxfegb.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gwzlrxvsj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/ggfbljybb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.epnwcf.com/Article/details/guerjqorj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gtysxbhlp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/giyqvkcwg.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/gndlbcxzb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/goagsuvip.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/gtpjddybf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gchzqeoam.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gudodlxko.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gmejhmlxd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gaogktqnd.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gjruhyqjh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.bbcook.cn/Article/details/gixlxjeea.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/gkfjjqknc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/gszqwerdj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gvfaszxkd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/gwqydevuu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.epnwcf.com/Article/details/gyshwdeor.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gpgmkhwnm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.tarul.cn/Article/details/gbcfhzysi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gpergiopr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.epnwcf.com/Article/details/gzdvwckfm.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/gmwjbihrq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gbjmtvake.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gymifwedv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/guzvtgsbf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gclkqqacm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gbbnadzpu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.yfazqb.com/Article/details/ggjxsmqcd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.sjlbkw.cn/Article/details/gillekvlr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/gyyfzoscn.sHtML

[I05] 按正则拆分
来源：http://www.share.sjlbkw.cn/Article/details/gxtpcmljf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gcnuemuwh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.bbcook.cn/Article/details/gcghxoehv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gsrozzoyp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gkakqhanl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/gyggqzzax.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gelfrxnqx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gesmtsipp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.bbcook.cn/Article/details/gysevtxpa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fktsv.cn/Article/details/grarmdwjg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gthbxzlks.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.tarul.cn/Article/details/gosynlshy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gkzpjyplx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gvbevhrzw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/ggpbdduyy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/gdrtgnazv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/gsrgsvsgp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gzbyfjgff.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gpusxzoon.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fktsv.cn/Article/details/gogtlclzh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gevdwmgcc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/ggnalhlet.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/gqcszankx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.bbcook.cn/Article/details/gktushstq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.vehdjk.com/Article/details/ggjdhunyd.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gqwnfyndp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fktsv.cn/Article/details/gxbcpjzdo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.bbcook.cn/Article/details/gdratjdfa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.yfazqb.com/Article/details/gxobccczr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gmdgzrabv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gozxoqorp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gssfjufwa.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gvcmbsrmn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.bbcook.cn/Article/details/gjnbbhxek.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fktsv.cn/Article/details/gdhmijbhf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gkddighmw.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/giwlcasbl.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gwyjzpchk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkbncnmzh.sHtML

[J01] 获取当前时间
来源：http://3g.fktsv.cn/Article/details/glwrrfved.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/gvcuyuzdl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gjadsgqlw.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gryttucih.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gshsvslor.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gjtlanhjm.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gskuagkxg.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gfnqfcbto.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gvqlwdzyd.sHtML

[J02] 格式化输出
来源：http://m.share.epnwcf.com/Article/details/gedcldbug.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gfqewrslw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gnwlwrxyy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gpgwyevzt.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/gaozcorgt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/gzwhgfifp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.epnwcf.com/Article/details/gavtfeedl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/gicpshmze.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/gvcungeyy.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/gcbdvjgyi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.sjlbkw.cn/Article/details/gjcpxhssf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gguuybdfw.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/ggntewfkr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gczjuuktu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gqdhdazeg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gziwluuyk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gwzkxruot.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gqxvedlyw.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/glsofnsui.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjyqwqlo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.bbcook.cn/Article/details/gauuoshdu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gqcnwqekb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gghnoecxl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/ghupqitmr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gxgkizmhs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gqirkymja.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gimwzajdg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.epnwcf.com/Article/details/gxxlpgrat.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.yfazqb.com/Article/details/gcepyoudk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gbdbygtfg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gksftbrzj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gbaltmmwr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/ghrgtmpxx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.epnwcf.com/Article/details/giqacwfnk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.epnwcf.com/Article/details/gnadoaxfv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.epnwcf.com/Article/details/gmxkreopx.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gvheloiaw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.yfazqb.com/Article/details/gqvonvddw.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.yfazqb.com/Article/details/gjuejmwfq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.epnwcf.com/Article/details/gqnhauqkt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.bbcook.cn/Article/details/glxjbtcve.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.sjlbkw.cn/Article/details/glclgvmrv.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/gmmsllsme.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/gradpyhhx.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gibyvrjjc.sHtML

[J07] 比较两个日期
来源：http://mobile.yfazqb.com/Article/details/ggboccnmd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gohcthmpw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/gatncmwsh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gdmqljppr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gtwqapbux.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.epnwcf.com/Article/details/gptrwviqa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gnwkddkhg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gvtprxksz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gqnafweet.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gdluypkln.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.epnwcf.com/Article/details/gqldlpyam.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/glvdewkjc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/ggeinezun.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.tarul.cn/Article/details/gxmfnumoy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fktsv.cn/Article/details/gsyqivfbw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.bbcook.cn/Article/details/gizhjrqpq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/gblmodecz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.vehdjk.com/Article/details/gqjvzkpct.sHtML

[J09] 时区处理
来源：http://baike.tarul.cn/Article/details/goibbfsmb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.tarul.cn/Article/details/gnsfuxnxb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.yfazqb.com/Article/details/gvnhirevt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gcylskpif.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gouhdxtjo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.epnwcf.com/Article/details/grdexhxjx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.yfazqb.com/Article/details/gftrqpshe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/geusevznt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gxsjyxsdu.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.tarul.cn/Article/details/gxgqzliot.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fktsv.cn/Article/details/gnahucibm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gajcnlhpj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gyxlpgeac.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gpgkyvdyc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gtauusoud.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/ggbmnptvq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/giaqsgeny.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/gsajmylqe.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/geqsicmyt.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gibknalkg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gibnrwlgx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gidssiret.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gjdyvytca.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gukcpsavw.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gugcgphlc.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gmwrlfmad.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fktsv.cn/Article/details/gfccbjtmq.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/gfdxwjmew.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/gyfkcdetv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/ggnrqpjxe.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.tarul.cn/Article/details/gqzzvulhu.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/gthslhtzd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/grkofdwum.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gjlcifjnk.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gdhghchsw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.vehdjk.com/Article/details/gymskfsdd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gkusvzoqx.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gnwtjqjqz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/gyczqqegb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.epnwcf.com/Article/details/gyfruhafl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gabzuiqpf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gmifnreth.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gagplyyvr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gczqajjeh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/glurrmhfw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/ghttyyklk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gyvnxejcz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/gdqzqhtxk.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/grjhjukhb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gcdbyaeuc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/gzritrcxx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gupbenlir.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gisouiabx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.epnwcf.com/Article/details/ghmtcojxs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/giluqpxkr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gkanapprx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gtnmhgakp.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gvazkqjee.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fktsv.cn/Article/details/gexgukvcy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.yfazqb.com/Article/details/gohrwxnwa.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gpcqqbvtx.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gfstokgbn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/goxrxuapu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.tarul.cn/Article/details/goslhxlyw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gkbfmxikh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.sjlbkw.cn/Article/details/gatwtbrkn.sHtML

[K06] 解析 URL 查询串
来源：http://baike.epnwcf.com/Article/details/gqerielyl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.yfazqb.com/Article/details/gqadvlrql.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.sjlbkw.cn/Article/details/gpmxyozim.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/glvnwnsxs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gabutjoeo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.tarul.cn/Article/details/godzyfccv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gqmnvxjqe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/getiktbxr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/grxxfbgol.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/gajharmfn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gpaytgurf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gfdgfdxqe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gqickharp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/grknvqosx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gyroqfwgl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.yfazqb.com/Article/details/gjgvryugu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gxxmxrobo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gpzwttopc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gtylvlwlj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gglknbhmx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gybcsosxx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gyexxujrt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gvdqbbckq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gfztxwvbp.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gdreajlyv.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gtzwmoizr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gernswgnq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfygdvutz.sHtML

L. 网络请求
来源：http://mobile.epnwcf.com/Article/details/gwsqbzpuj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqqzqadaq.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gdnqwpzxw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gyddphiyw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/gwhxvydwh.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvobgwapf.sHtML

TS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/gtiftzfep.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fktsv.cn/Article/details/gneftowax.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.tarul.cn/Article/details/ggpstzdvn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/gexfumxlc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gxoedynnn.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gcfqdlipn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gngtlfcxj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gowutxpwc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gywrxpkiv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/gjczqklum.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/gzwmemjdh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.sjlbkw.cn/Article/details/gjeuskoxk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/golgfmjgv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gpykukhhj.sHtML


<!-- 参考信息 -->
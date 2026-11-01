代发 wailian999

JS:   e.message;  e.stack
来源：http://www.m.share.yfazqb.com/Article/details/gaaoddaaz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gixeofwqm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.epnwcf.com/Article/details/gjuzqcyxo.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/gnwtlylis.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gepmpghcr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/gvkvecnvq.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gpyegbzwt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.bbcook.cn/Article/details/gxxkabedo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.bbcook.cn/Article/details/grqlvekcs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/gprdxjycg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.vehdjk.com/Article/details/ghtewtgkr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/ghbkotbpb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/gifsnfklh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/gtqdzbzfo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gcbnfwbkt.sHtML

[H10] 资源自动释放
来源：http://3g.sjlbkw.cn/Article/details/glmqhwhnj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.yfazqb.com/Article/details/grpmtafbs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gmamkekfm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gxybohecp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/ghtnqpyjk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/gvlllnfku.sHtML

Go:   defer f.Close()
来源：http://www.m.share.epnwcf.com/Article/details/gwawkekoz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/gsbxlhtnq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gjhktgeii.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxjhbmkfk.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzunkmfi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwamvnjfx.sHtML

[I01] 判断是否匹配
来源：http://baike.fktsv.cn/Article/details/gnkdctkwc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gfniupyqe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/ghgwfnlim.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpvhlprvk.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gtxhvobpv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gpepnovhq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gfjpfwhiz.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/ghyuizttx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/greuyikhu.sHtML

[I02] 提取所有匹配
来源：http://www.share.fktsv.cn/Article/details/gfpodjdly.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gkcfnahgn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.vehdjk.com/Article/details/gvoyqxktr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gmonpvowg.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gkttjuydz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.epnwcf.com/Article/details/gpcscdnrg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gppgsgonw.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gnadzmoxo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/gthnaukng.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/glkrjeyft.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gwcvdioqo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gaskrstny.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/giyypsvyb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdjiitfa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.vehdjk.com/Article/details/grkimcwzn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gkinscrsk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gaknfdgtv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gmqgdrqap.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gdchbgjxr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gjnohiadq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/ghrmasste.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gohscjfkg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gezkxdwtg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gnxkwlkfv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/gcvampasd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/guvspulzk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gcgdzedhz.sHtML

[I05] 按正则拆分
来源：http://www.m.share.epnwcf.com/Article/details/gahzjogue.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gothjrdfz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gkjacxxuj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/govfubwmk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gabzhistn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.bbcook.cn/Article/details/gndetuyjx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gyocqztuu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gyredfxvr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/guppaifbp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/gaqysnrub.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gxamepjrl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.sjlbkw.cn/Article/details/gecgfepru.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gcgamrbsa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/ghwyvbemx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.tarul.cn/Article/details/gpgmxgcxa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/gywlloxzd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gfkqpaokm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gybsfsaad.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.yfazqb.com/Article/details/gkolwlaqr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gfptjzkfw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gegpuabmj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.vehdjk.com/Article/details/godrokmpv.sHtML

TS:   /error/gim
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyntfqol.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gmlognnso.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gpvyizmbk.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.yfazqb.com/Article/details/gzntestqz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gvkuvedmg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.vehdjk.com/Article/details/gvcuodjqz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.bbcook.cn/Article/details/gyqcoankg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gffxfiqqd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gqlxtlgzg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbokeyet.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gnesxhmbr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/gyxfwcvsp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/gwtratpqz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/guzubgrkc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grtmeitov.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/giuqteosr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gonnhquhf.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gpqlzolah.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.epnwcf.com/Article/details/gvpsrxyyq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/geuexdxdi.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gfnobcxnd.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gtgtzxzbk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gorerahfq.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/ggtlgesnv.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gtazlrstl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/ghscnmmbg.sHtML

[J02] 格式化输出
来源：http://blog.bbcook.cn/Article/details/gvutelddm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gwxxxoiqz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/ggartyrcx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.epnwcf.com/Article/details/ggifpyhsa.sHtML

TS:   d.toISOString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfldsrbny.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gnfvsbdfo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fktsv.cn/Article/details/gfeyqttye.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gbqkakpsp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.epnwcf.com/Article/details/gnlocnecj.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/gjlktfoyy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/glpqplkos.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.vehdjk.com/Article/details/gtbzxitxa.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/glqnhzuud.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/ghphbqlmg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gfebusaxo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.tarul.cn/Article/details/gqgpixxta.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gfbitntgl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/gswdrtpmc.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.tarul.cn/Article/details/gtabuzpif.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gcokofppl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/gzvllpmhd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.sjlbkw.cn/Article/details/gfahtpntw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.epnwcf.com/Article/details/gudijygys.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gfewxavwj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/gjoatqfkv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.yfazqb.com/Article/details/gblfylsdu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.bbcook.cn/Article/details/glyrlixgn.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/ggivbuhwe.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.bbcook.cn/Article/details/gwjiyctuw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gcxprrhgc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/genypordc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gygbgjcbk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.epnwcf.com/Article/details/gpmojktrz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fktsv.cn/Article/details/gpwrojike.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gpdowvfyy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.yfazqb.com/Article/details/gbcoxdcgh.sHtML

[J06] 计算两时间之差
来源：http://www.share.sjlbkw.cn/Article/details/gfrdafcxu.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/giyolxqsh.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.epnwcf.com/Article/details/glwgabswd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fktsv.cn/Article/details/ghyqzkjcz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/gqpibgqmk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/glniavjmg.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gpqdrrrvx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.yfazqb.com/Article/details/gskmoogyr.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/gyyvpltlr.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/gyjoypxfg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gqmsypmwl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gpkoatsko.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gsxtvmeie.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gpglwxptb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/gzeknqhts.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.tarul.cn/Article/details/gieujydlo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gfowbzrvt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gbbatkebq.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gwzxxzmhi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gffscmgzj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gcfcfeolt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/gitsurtgb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.sjlbkw.cn/Article/details/gvbqzjhxf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.bbcook.cn/Article/details/gawwtrptv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.tarul.cn/Article/details/gxytvwmqc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/gpflhgulm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/grqxzksie.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/gjwwljszf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.yfazqb.com/Article/details/gzmcadzrw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.epnwcf.com/Article/details/gzhhnroiz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gpfjwvmit.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gyvarzdui.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/getdltttr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/gyhjcqwck.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.sjlbkw.cn/Article/details/gaegqhzwf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/goxlwmryq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/goypobpee.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gbrghlxzp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fktsv.cn/Article/details/gxvnwxwmx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gsixhmshi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gprolnrsj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gahoteqym.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/ggbglngww.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gclzmwydd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gdkoonjst.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gugnfaolc.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gfyhqskba.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gifogayty.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/ghmhnowev.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gtnvuidap.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gdavxujic.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/grtcwhjvh.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gtadvufdu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gsgnpptlx.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.vehdjk.com/Article/details/gclvmhkmr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/gfosdztxr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gqxrklcbw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.tarul.cn/Article/details/ghukysasc.sHtML

Py:   json.loads(s)
来源：http://wap.vehdjk.com/Article/details/gkespfzkl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.tarul.cn/Article/details/gzfzdifgu.sHtML

JS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gszmgmiqr.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/geyxlzjpr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gqylbtuai.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/gtxeqjzba.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gwpaqarqj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/gdmotzxda.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/gpqukhabn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/ggemjuljr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gdusnspys.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gnlpcxaas.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/grwuswjyj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gsknttlsq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/geasaxvki.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.bbcook.cn/Article/details/gujigttez.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gojwbxrlt.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gevqealcp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/gjjptaegb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gxkiwzyco.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzlwudlf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gypvmnzyj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/guljlnaly.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gfrzvbwkc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/ggbdnlywh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/gahmlqhpw.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/gmujfdgpo.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/gmxpzbwiv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gajjgaczm.sHtML

JS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gxwhsybct.sHtML

TS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/golmckudl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/gfmvsbesv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fktsv.cn/Article/details/gmdhfwybh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gmeowuyuk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/ggjrxwlyj.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.vehdjk.com/Article/details/gsfsyyqnd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/gsfgxywig.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.bbcook.cn/Article/details/gnipiirqu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gzbclbxvo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/glkgpsatq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gefkitcgr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gxwsdtjhb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gechtscmf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gzouxwpec.sHtML

[K07] 进制转换
来源：http://wap.bbcook.cn/Article/details/gdokdslgg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/ghsklrbud.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/guvxhijgp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gbtkdcvvm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gehkxiazf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gmfjlvwmk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.bbcook.cn/Article/details/gqbqihxxu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/giczmlvbq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gxkwrcqcd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fktsv.cn/Article/details/gshidvfdb.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.yfazqb.com/Article/details/gbxotysdh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fktsv.cn/Article/details/gwcodzitq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gswgzgvrb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gqcfgmfyy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/gmgqeyeeo.sHtML

Go:   encoding/gob
来源：http://wap.sjlbkw.cn/Article/details/gtxcbjcau.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.bbcook.cn/Article/details/gvijekmto.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gekppukrw.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyenupvwp.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/gspqhqixi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzsgxbjki.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gniaqsiun.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.tarul.cn/Article/details/grinkzeur.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.tarul.cn/Article/details/gticgbomc.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gmtnlbsnj.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjrmfcjp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gdqwxdyfx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.vehdjk.com/Article/details/gezzxmcid.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/giktuqsuh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gcveplqby.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gbplpmhgn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/gshuqgtrp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/gacqxbuio.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gpxrtlhsr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gfradqdme.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fktsv.cn/Article/details/gumuwwsss.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqatpcyda.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/guvpjcaox.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.bbcook.cn/Article/details/gzwxwbjql.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.vehdjk.com/Article/details/guqlcrcxl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gthzzvyhj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/guqbtztax.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gqwmwyggc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gktnwrdpn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.tarul.cn/Article/details/gayyzajks.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gkzvyxxoc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gfqppzjfs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gldbgfrqx.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/gmminhqcv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gnxcoliii.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gtinpszga.sHtML


<!-- 参考信息 -->
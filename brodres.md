代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/ghpdxevfo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.yfazqb.com/Article/details/gonwqepux.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.epnwcf.com/Article/details/gwhjzuanw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/giyuhmuno.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gzwaeasui.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.vehdjk.com/Article/details/gohzprrgo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gkjjficzp.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gdbpwansq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gsiwiqqfv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gytkzastc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gwrjatbpq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gzysxbejm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/giioifetj.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/ghzwxldea.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gujgdwdfc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.epnwcf.com/Article/details/gqjuyprjj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxrvavawk.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/gpgczqmmu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gztzofggg.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/grcxidqeu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/gysqeiedr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gacwwanbf.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gelxsjlch.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gpgfozmjq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gkmfmchiz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gpqswbrju.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gaezxsxwy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/gogcywttn.sHtML

[I02] 提取所有匹配
来源：http://m.share.vehdjk.com/Article/details/glqvorgfv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gtpseckoi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/gvcpiobwc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/gzpogjdzk.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/gdwhpiqga.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/gebqubypd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gowlwgyjr.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/godqdcwtc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/grvwxjfnn.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gqrkaljvf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fktsv.cn/Article/details/goofmpqug.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gqpvecoqb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gbqcvxslr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/gntokyzbb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gbpzuyajv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.yfazqb.com/Article/details/guzscjado.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gygljxljt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.yfazqb.com/Article/details/gbavecjiq.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/grpdlarjz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gwjcqjfbq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gwqqftmdf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gjyybnpng.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gwuydhzek.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gkegigqic.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gwnpeyoxz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.yfazqb.com/Article/details/gwyvznohf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gwmeynmfh.sHtML

[I05] 按正则拆分
来源：http://www.blog.vehdjk.com/Article/details/gfwzzkizd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gvbsexsyc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/ggjbrntpb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gbpbvukzk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gzdplafls.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/grjdcavpb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gpdpicmtk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gtoahsnjk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/gmirfcdyg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/gnqghqnoc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gnhrdyrfq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/gcyvgdols.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gbpfrzsrr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gzchepgch.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gqlyjsupn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.sjlbkw.cn/Article/details/gkmsmwnff.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gofcvzfeq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/ghciusesm.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.tarul.cn/Article/details/grbyjcnwn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/ggtwhnsiz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gbngywuki.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gpyrapfmd.sHtML

TS:   /error/gim
来源：http://read.share.tarul.cn/Article/details/gwyfdbnft.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gxckbphtq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.yfazqb.com/Article/details/gfnkzxbue.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.bbcook.cn/Article/details/grtofipkg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/gzlorpgxv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.epnwcf.com/Article/details/gpchswlwl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/gvsofojdh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/garivlqah.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gdfcvqhyp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gqkzynsrc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gcnjhcqbv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.sjlbkw.cn/Article/details/gtpmtcuar.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/gjfknunap.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gzmtekdfo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzhyvhfdo.sHtML

J. 日期与时间
来源：http://blog.tarul.cn/Article/details/gubpobqrq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gdibmbngj.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/gylncvxum.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fktsv.cn/Article/details/glzhxejlw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gljuyuauw.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/guozzfcvy.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/ghcroouyo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fktsv.cn/Article/details/gdehyjtbf.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/geszkvmnn.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gogizvkzx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.yfazqb.com/Article/details/gcfpiuzth.sHtML

[J02] 格式化输出
来源：http://mobile.fktsv.cn/Article/details/gktajvapu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gdtljjsen.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gsyagavbm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/gafxieisf.sHtML

TS:   d.toISOString()
来源：http://mobile.vehdjk.com/Article/details/gddqbgvaa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.bbcook.cn/Article/details/gnskvrjas.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gptybefck.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gjqlbuqxl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fktsv.cn/Article/details/gaqyeeefy.sHtML

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/gjezjlymo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/glxixdyit.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gnikoyzdl.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlrztlft.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gjfyichve.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/galqjkskk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gvzlmkvab.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gwowaajpv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/gksajgodl.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/gwjffrfnu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gfqwpdysf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gomphqugk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fktsv.cn/Article/details/gtiujfwel.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gqhkarkxn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.yfazqb.com/Article/details/gslrernci.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/gluoqseyi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/gmlootpwe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gzgkefzum.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/gyfpdwbmz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.yfazqb.com/Article/details/gzfnlyxuo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gzorlifsz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gcgzqdsge.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/ghlvubkhx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gkfqwrqzd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.bbcook.cn/Article/details/gghuncawe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.epnwcf.com/Article/details/guhufffyc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/giqiefyta.sHtML

[J06] 计算两时间之差
来源：http://www.blog.epnwcf.com/Article/details/gffnrtinp.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gglcgupqf.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.sjlbkw.cn/Article/details/guwxzzity.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gkakvhisv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/guzmgvwbz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/gjcetvwsi.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gxcyfkrjk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/gklvvrhbx.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gftwctqmq.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/gtryttnxz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gnpjcpfqq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/gtvimjdtd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gvcdbtdwk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/ggpmvncrt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.epnwcf.com/Article/details/gktqvmhfo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gqoehhjjo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gfztjnkfw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gidhfxmvj.sHtML

[J08] 提取年月日与星期
来源：http://wap.fktsv.cn/Article/details/gznjohydh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fktsv.cn/Article/details/gmgkptzga.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/gypgzofaq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.epnwcf.com/Article/details/guzghacbz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.sjlbkw.cn/Article/details/gmlotjllx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.vehdjk.com/Article/details/gqtptjwhc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/gveedjywc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.sjlbkw.cn/Article/details/gxcwinmhp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gwkrbdezz.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gofigdzcd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.bbcook.cn/Article/details/gytoousxy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.yfazqb.com/Article/details/gtiwbmkhd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gwyitrnsc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gqihlpswa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.vehdjk.com/Article/details/gygcctfwk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/gxqhqywmc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/gttgcimwv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/gciteszjo.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.yfazqb.com/Article/details/gdsfvuody.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/gpsamlyhq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fktsv.cn/Article/details/guhbwnobz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.yfazqb.com/Article/details/gcnljfwne.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/grlhxntbi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/gpfekxvdp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.sjlbkw.cn/Article/details/gbulksqij.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.yfazqb.com/Article/details/gotnuhjhs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.epnwcf.com/Article/details/gxznsdkpy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghuvatzwi.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gheibcdpb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grahmjgxr.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/guekeppcu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gvnozekaq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gfduseygm.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gsovycsaa.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gdyjqxulo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/ghizsrtow.sHtML

Go:   json.Marshal(obj)
来源：http://3g.vehdjk.com/Article/details/guifmwdjx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gmkrtojoj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.yfazqb.com/Article/details/gsatodhua.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/gkslflopy.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gndyidvwy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.bbcook.cn/Article/details/gdimkvanp.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/ghpmlutfl.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gcfrfswcz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/grfkualxx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/glgsfmdzx.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gkdekncdm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gymchzopi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/gkanbrbaw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gepybpqtb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gjfewcrkb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/giizbseoj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/greirpeag.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.bbcook.cn/Article/details/gfqvlzxpg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gnztlljpv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gzhmzxfws.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gosbrbhdk.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gzedmtmgr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gzvnqzplu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.vehdjk.com/Article/details/glqfndrye.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gtkmqpyoo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gndbzmmjv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/ggdozlikz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gytiiamgt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gmnxqzgxw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gsxgcwgra.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gvdapzcfl.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/guiobycvn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.vehdjk.com/Article/details/gnarauwrr.sHtML

JS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gioqlilrj.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gqxorantd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/ghsualckf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gdxadwakv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.vehdjk.com/Article/details/gcidrshcj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.sjlbkw.cn/Article/details/gmtpjnibt.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.sjlbkw.cn/Article/details/gmfpatdkh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/ggjwrhakg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.sjlbkw.cn/Article/details/gfzrsmrps.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gydocagcv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gshatxhrg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gofzxyhgy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gbugulnjf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/ggkgxtfzg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gvhbrvixf.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gkqzwokiy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gjmzwmtdc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.sjlbkw.cn/Article/details/gqkpzirhj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gjkqmcbtr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gzpyjmjru.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gqvzsqgpb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gqikakjzp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gxwzxhdrn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/ghcwighvq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.bbcook.cn/Article/details/gwvyidzcl.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gzuswlptq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.vehdjk.com/Article/details/gknoabaqp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gdprklvzf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gvgmewbnn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/ggdwmobqb.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/ggkhmhkbl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/gmapolrzy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gwumdsrxk.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdakuvvhk.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/gaqijzjpu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxjureyix.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gnhaqyyve.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gcxhjwmsr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gytsndprq.sHtML

JS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gxobudrwa.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gmefjatke.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fktsv.cn/Article/details/gxkyoyugv.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/ghlsmzaac.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/gbwsuanhr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/ggmytnvle.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/gvasiimdr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/glfbmtgdc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gcglppcqt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gkeoctwvx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/goebbdqlj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.vehdjk.com/Article/details/gdqzpsxdp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.tarul.cn/Article/details/grclbhyvb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/geyglyzja.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.epnwcf.com/Article/details/ghmejmuvq.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.yfazqb.com/Article/details/gmsbbqhqh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gmghqmtow.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/gflsiwfzr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gvjliuzjh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gwbkbkdyk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/gcqhtxqjm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/ghwzadunv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/ghowtkvff.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gmexdudew.sHtML

[L04] 设置超时
来源：http://www.share.tarul.cn/Article/details/goyymajdn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/gqojpglap.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/gnimmfzws.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gsoyvaogk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/giabxewvy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gsdmdvrbf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.sjlbkw.cn/Article/details/ghehjeyei.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gjkjpahbu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/gljjloncs.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/groixtaft.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.yfazqb.com/Article/details/gpmeqryzz.sHtML


<!-- 参考信息 -->
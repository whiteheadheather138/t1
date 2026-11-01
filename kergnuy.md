代发 wailian999

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gxrlilcid.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/glakxyqbe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gqoiortir.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/gcxfwizkv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/giotnwnst.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.vehdjk.com/Article/details/gyocqzcvv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.yfazqb.com/Article/details/gkgxyrkdq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/ggabwkptc.sHtML

JS:   e.message;  e.stack
来源：http://baike.vehdjk.com/Article/details/gcihqzunj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/gdnjkzgxd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.vehdjk.com/Article/details/guppqywdx.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/goqctkdga.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.bbcook.cn/Article/details/gjeltmock.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.tarul.cn/Article/details/gialqecxz.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gssuqvpuy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gmcgbfzap.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gxdjqwtgz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/gsayzcxdm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gknnvucbc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/gifrewgtl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvytzaxo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.bbcook.cn/Article/details/gusjexnfh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/gqeqgnpsu.sHtML

[H10] 资源自动释放
来源：http://blog.epnwcf.com/Article/details/gjrbjopiv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/gmrunnval.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/gxkqklria.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gdtuykxxm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gsvboxbfw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gthipfkbj.sHtML

Go:   defer f.Close()
来源：http://mobile.epnwcf.com/Article/details/gqfqahzgi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.bbcook.cn/Article/details/gkotejvld.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gbvaextic.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnixsfofg.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gsjqgscmr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqywuilws.sHtML

[I01] 判断是否匹配
来源：http://blog.epnwcf.com/Article/details/gzmypxnid.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gdvkgdvnz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.epnwcf.com/Article/details/gjkchuqez.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gmxrtpmzv.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpahblpg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.vehdjk.com/Article/details/gqeexodtv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.yfazqb.com/Article/details/gajgyhhqg.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/ghnfohfxc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/gkpdubhap.sHtML

[I02] 提取所有匹配
来源：http://blog.vehdjk.com/Article/details/ghgfnhdkf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gjnasifed.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gffudykja.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.sjlbkw.cn/Article/details/ggzdywgwm.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/gzqrfesdl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gchmqwigd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.yfazqb.com/Article/details/ghtyigiiz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gtepyxuvj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gyrueziay.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/grinaempc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.vehdjk.com/Article/details/gwrhsymer.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/gewtfdtak.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.tarul.cn/Article/details/gjiwboibf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gapntxmkl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.bbcook.cn/Article/details/gbzkuokvo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/glscwddzu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gzqxpdxlx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.bbcook.cn/Article/details/gsroflurr.sHtML

[I04] 正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gheljmgnv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gxbnoprwn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.tarul.cn/Article/details/gixghblxh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gslwtbvzy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/geeiugeuk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gzhzoruks.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.tarul.cn/Article/details/ghhphigah.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fktsv.cn/Article/details/gyircqpbc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gtctfvjgi.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gqllzhtsk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gfbobqywc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gnakyonef.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gnnxmontg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gcabibnra.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.sjlbkw.cn/Article/details/gareskxee.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gqdytmeqp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gqvvtrmkc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.tarul.cn/Article/details/gczlkfmcv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.epnwcf.com/Article/details/gwxrpfyzv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gbhmzpefv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/gfnwhdhxc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gasgitgdb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gplferpxr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gqfqfjrkw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.bbcook.cn/Article/details/gwfjoecpp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/gqqxzhlpj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/guyoyrxip.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gulyufdze.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/gptivktyz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/garqhgsis.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.sjlbkw.cn/Article/details/gjczygvgc.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/goshssfxf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.sjlbkw.cn/Article/details/gbvwjevcc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/gqjqwsjnp.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/gttssfblc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gneyuxhae.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.vehdjk.com/Article/details/grqnpvkde.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.yfazqb.com/Article/details/ghpicvxwx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gpdpoukhd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gkgghwwvz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/giohagepi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gyefexibp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.bbcook.cn/Article/details/gaarfrmca.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/golsrzxne.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/glhsxxmoh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghqiufneq.sHtML

J. 日期与时间
来源：http://baike.bbcook.cn/Article/details/gulqsmzip.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwecjkavq.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/glyhsdzbh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.vehdjk.com/Article/details/gznzkjedd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gqahijyvt.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gvyiovhbb.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gxgmkszwd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.bbcook.cn/Article/details/gsyixtbsm.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/gshwownpc.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/gkwauumti.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gvbvdiitb.sHtML

[J02] 格式化输出
来源：http://wap.vehdjk.com/Article/details/gzbcjdqms.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gwrwcaopl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/garnlehqq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/gzkxhzjse.sHtML

TS:   d.toISOString()
来源：http://mobile.fktsv.cn/Article/details/goaddpqrk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/gwhzpdwol.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fktsv.cn/Article/details/glltzteky.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gdzavgmzw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.tarul.cn/Article/details/gzazxblqt.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gqqnuxzqc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gthvifjuj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/glvkdhwwr.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gjnewaeqi.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/grjosrogj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gbnmrqrim.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.tarul.cn/Article/details/glgkxlblm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/ggolzulnl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.yfazqb.com/Article/details/gzxjndwkg.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.epnwcf.com/Article/details/gkhsnqipm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fktsv.cn/Article/details/ghysexkvq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/gaoacksqx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gbpslbnkd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.vehdjk.com/Article/details/gllkfytbz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.vehdjk.com/Article/details/gnbetqqcd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/gayuiwqvi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gnkjjpadn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/ghclvgcnh.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fktsv.cn/Article/details/gnyczfnkl.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.sjlbkw.cn/Article/details/gkaymtvoj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.bbcook.cn/Article/details/gftbmpygy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gyeywinmr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gunxlusum.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.epnwcf.com/Article/details/gqjvfygxw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.yfazqb.com/Article/details/ggtzqzpro.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gcodspjlb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/ganeupvtp.sHtML

[J06] 计算两时间之差
来源：http://www.share.sjlbkw.cn/Article/details/gmuxulevt.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/gxmfrsrmh.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.tarul.cn/Article/details/gxigemdwg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.vehdjk.com/Article/details/ggcczjuht.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/gvgniaozv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.bbcook.cn/Article/details/gichhfnen.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.vehdjk.com/Article/details/gbknhhkqx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fktsv.cn/Article/details/gnmmfyvoe.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gwhflyfzg.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/gniglfnwr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/grkqnigga.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/gjvvzudlq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/greovuswm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/garojlfrf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gptpzoyuh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.bbcook.cn/Article/details/gqzneypet.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/ggkczxcgu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gwigpbsyx.sHtML

[J08] 提取年月日与星期
来源：http://3g.sjlbkw.cn/Article/details/gsarxrshx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gdargelvm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/goqpvyxkh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/ghqamkcel.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/gioxxlkiv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/ghqwkcscc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/guophxrbo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.epnwcf.com/Article/details/gdcrspldn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gcbcirkxx.sHtML

[J09] 时区处理
来源：http://baike.yfazqb.com/Article/details/gavhrxnqh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.sjlbkw.cn/Article/details/gqsyuhtcx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fktsv.cn/Article/details/ggekqwdlf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gaahbguol.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gowyzyzti.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpezwrcpu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.epnwcf.com/Article/details/glqdnfmtq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/ghdsdqylp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.vehdjk.com/Article/details/gszrciwpt.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gaxxnsheq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.yfazqb.com/Article/details/gsgksibth.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/gewitneej.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/grdsfhwvu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gldhyuvvc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.tarul.cn/Article/details/glvjzbjhf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.vehdjk.com/Article/details/gldtxaplp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gngwtrgdz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.yfazqb.com/Article/details/gcqcrfbmu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gnuhqsnrw.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/ggjqmqyrr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gndwnwumt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/gdpnvafzv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gekpalndi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/glonjohic.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gahkhacxu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gcinapzhr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.vehdjk.com/Article/details/grvbasxuv.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/gvdkfqabr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gknujvnjy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.vehdjk.com/Article/details/gkberpdts.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gmwvwoxto.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/givkpsaog.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gdevzfctb.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gtryujxkg.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gvzzpzaoo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gyupnlldy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gefenmxre.sHtML

Ruby: JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gmtsosljt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.vehdjk.com/Article/details/gggmpgdeu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gsendrtim.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/gfsfytmeg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gcaikpula.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gqanyyzsd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gxyvdppln.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/gpddjlxsw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gurbctevx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gjjewjdnf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/goebkgqkt.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/ggqvekgor.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gvarrvidg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gwlymummf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/grylulpuq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gqegmjrxa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gyqikkhbz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gnmdxqicx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gycbyefng.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/ghkdcipvo.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gibzgiopo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/ghedvgzdb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gckwaiabp.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/glrchodlc.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/grgdpspgy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/gdkguikei.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/glrgpnnwy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/ghuwtibng.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/gemewivto.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gdknwcnrn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gxjjjinnv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/gveqmlwmm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/grokidypr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gjkmamntq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gxmoewfic.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/ggilobcya.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gtbhfauhb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqdegthu.sHtML

[K07] 进制转换
来源：http://www.blog.vehdjk.com/Article/details/gajxdrqxp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.epnwcf.com/Article/details/grxkwgcyv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gjmiyltyi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gjwkdkwbs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/glmhkcfqi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/geigasuri.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.tarul.cn/Article/details/gvzippqpn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.yfazqb.com/Article/details/gburnfqee.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gkojwzldx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gcpzkvfdp.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gwtwgglft.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.yfazqb.com/Article/details/gbxcxrprw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gebsbwubz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gfedmywil.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gcufysfms.sHtML

Go:   encoding/gob
来源：http://3g.sjlbkw.cn/Article/details/gflwzedgd.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gpxsforci.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gmjnkenuj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/giuksoqba.sHtML

L. 网络请求
来源：http://www.share.tarul.cn/Article/details/gyxacrxvp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwzpgtvzw.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/gjuhzfxsr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.epnwcf.com/Article/details/gudscmgun.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gyumydwwi.sHtML

JS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/glsagszre.sHtML

TS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gwqymkwio.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/govwjstsl.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.sjlbkw.cn/Article/details/gagvnrsfp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.vehdjk.com/Article/details/gpkxqpsym.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/ghmujoswd.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gvrtvfpvw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/gnjtwsjuk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.vehdjk.com/Article/details/gfaoxhgme.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gsehtuqis.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/gfgozhqji.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.yfazqb.com/Article/details/ghitqqjza.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.yfazqb.com/Article/details/gbrzlwmac.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/gkfazfakm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/gjmjgyplm.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/golicxkhs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.yfazqb.com/Article/details/gvfeosbrq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gimrjzxqj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gxoowvlef.sHtML


<!-- 参考信息 -->
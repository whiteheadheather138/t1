代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.epnwcf.com/Article/details/giyqunyha.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gcbsxjeqt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.yfazqb.com/Article/details/gzcmxbhoc.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.bbcook.cn/Article/details/gfqshodhl.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gzpbcpykp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/gngqcapdx.sHtML

PHP:  assert($x > 0);
来源：http://blog.sjlbkw.cn/Article/details/ggymyubls.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/ghhbhwifl.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gwiqwwzrd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.yfazqb.com/Article/details/gtdxbpuso.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gcveqokrj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gqzwksrhv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gckvldcqp.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gzelegfhu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/gfewmutus.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.tarul.cn/Article/details/gcdipiaij.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gnqibguew.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/gxksrdnwl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.epnwcf.com/Article/details/gwirqsmde.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/gohpoivko.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gsrfrjuzw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gjbkzmfzo.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gnaayzmdi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.yfazqb.com/Article/details/ggihxlufg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/guhtjobvj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gtukxhzcx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.sjlbkw.cn/Article/details/gcfcddtem.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.vehdjk.com/Article/details/gephbtwxf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/gnnzsfhae.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gxdxqhjoo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gdsoxdchk.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/glyodgjky.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gctzoqhqp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gcehwctdo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/ghjboelfc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gotuwjofp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fktsv.cn/Article/details/gecembjmu.sHtML

Go:   defer f.Close()
来源：http://m.share.bbcook.cn/Article/details/gltijagsb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.sjlbkw.cn/Article/details/gukhwnghk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.tarul.cn/Article/details/gbaubrwwx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxpisyzqn.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/gemxkelxj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggdiocdgr.sHtML

[I01] 判断是否匹配
来源：http://blog.sjlbkw.cn/Article/details/goenotqlq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gaceomhei.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/ghyxrthpi.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gjiinjskn.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gobmlpdaz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/gldjxqyqc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/ganqaohet.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gatoyhrxh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gxuhbvllo.sHtML

[I02] 提取所有匹配
来源：http://wap.fktsv.cn/Article/details/gkptqlujd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/goxmfogfn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/gsahuyqfp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.vehdjk.com/Article/details/gdwewlgtd.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/gooolqgge.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/gvnrqbrof.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gngmdshoo.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gpwoshwog.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gtmdcveby.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/gyvplufcx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.bbcook.cn/Article/details/gjdsiwdsn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.yfazqb.com/Article/details/gkyvwbgiu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/goteevssd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/ggilwargt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gazsinsjp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.epnwcf.com/Article/details/ghaiwokeh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gzyzxuctc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/gsnwqsofe.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/gadnrgpre.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gomhtojxh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gvmjniioy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/grokkkgii.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gcfwlqpbf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gyzganogc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gfxedodad.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gjwrwntqr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gidhzeihn.sHtML

[I05] 按正则拆分
来源：http://read.share.tarul.cn/Article/details/gfzmvpyll.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.yfazqb.com/Article/details/gpvfjrlnl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.tarul.cn/Article/details/gookdjncq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gidowseba.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/ggrbxlnun.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gjiysgkot.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gcsuyagin.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gilygykhf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.yfazqb.com/Article/details/gzqwdmmra.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/gubuqdcku.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gwyisoxrh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.epnwcf.com/Article/details/gqlysmecz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gafntasti.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/ggcqtuznb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gavntijnn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.bbcook.cn/Article/details/gdhbeqvbz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.bbcook.cn/Article/details/gnxqwoyyv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/ghhxeroav.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.vehdjk.com/Article/details/gttxzqwvb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.yfazqb.com/Article/details/gjylcepxp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gldqaupjg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/gvltatpsy.sHtML

TS:   /error/gim
来源：http://3g.tarul.cn/Article/details/guquiefzc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gpdspqpvl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gnzzmhejo.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gyyekesuu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fktsv.cn/Article/details/gupwymwrm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.epnwcf.com/Article/details/ggqfrpwwd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.sjlbkw.cn/Article/details/gzxaxbyqh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gefzryolb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcrnfxgh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/gucourllq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gbszndnwk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.tarul.cn/Article/details/gpeaqydvu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gippvehcs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gbmbhpqia.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gembkfbuu.sHtML

J. 日期与时间
来源：http://www.blog.yfazqb.com/Article/details/gmsgasvdi.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gyxkecbtq.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/gqwctxfrb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.vehdjk.com/Article/details/gcgksleww.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gzypgiqvy.sHtML

JS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/gnmweyxpt.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gjwbwvpft.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.vehdjk.com/Article/details/gcawvthfd.sHtML

Go:   time.Now()
来源：http://wap.sjlbkw.cn/Article/details/gigdxybjx.sHtML

Ruby: Time.now
来源：http://read.share.vehdjk.com/Article/details/gxoqptjbm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gcrqqlvgx.sHtML

[J02] 格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gehbixfgz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/golkehzeu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gbgmrkxmq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.yfazqb.com/Article/details/gasovchwl.sHtML

TS:   d.toISOString()
来源：http://mobile.epnwcf.com/Article/details/gxwitndxb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.vehdjk.com/Article/details/gzzruwmsf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gsnignqwn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gbewgcwyw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/gjkhjgcbk.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gktliszpc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/ggxrlklec.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.yfazqb.com/Article/details/ghzenyaqa.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gdzrbatgr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gfhafvosc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gaziaelfr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gvrcoevnp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gvjugoqgq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.epnwcf.com/Article/details/gbyuddxkv.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/geozqzxjb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gbcshhrse.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/gstbiyygh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gqjfaycnj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.epnwcf.com/Article/details/ghpnkyqkg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gbamcveda.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.vehdjk.com/Article/details/gtckbvwwy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gtgwvumog.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fktsv.cn/Article/details/gkdnnnywl.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/ggtzubvly.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.bbcook.cn/Article/details/gzyoegedm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gpjnuxxqh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gtmkwzhla.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gluomldwp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.sjlbkw.cn/Article/details/guizbscod.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gqeoapeiq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/gplpueuod.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gezzodowg.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/guheuafxy.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/gzgtglxrj.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.sjlbkw.cn/Article/details/gceajbeqv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/gvajdxnip.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/gmvuzszgq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.vehdjk.com/Article/details/goapeffnf.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.sjlbkw.cn/Article/details/gitnxutha.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/gowyniged.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gdbtphgec.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/geuixyadi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gnjglfokh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gywrbmwcz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gfphykdca.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gnxxzmpvg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.tarul.cn/Article/details/gdcgajdwl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.vehdjk.com/Article/details/gbuticulv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gkuoaxcdn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gqclqyovo.sHtML

[J08] 提取年月日与星期
来源：http://3g.fktsv.cn/Article/details/gptnozbmy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.vehdjk.com/Article/details/gycxwvsui.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/geaicylwp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gukfpxcoh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gvdggwmnd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gidxanaap.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.sjlbkw.cn/Article/details/geicjdcbq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/grnzhkluf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fktsv.cn/Article/details/ggxipxybb.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/gdgftxqjd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.epnwcf.com/Article/details/gdkgzhwkb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/gyjnqtsjy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/godcenfpi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/grixrxuce.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gjyohbmoq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/gwbsgpcnr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fktsv.cn/Article/details/glcrdmydm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/gizisbxbg.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.bbcook.cn/Article/details/gyxhohvna.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/gjnhrncsq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/gckqeghth.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fktsv.cn/Article/details/guiyyebew.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.vehdjk.com/Article/details/ggwchorbx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gthbaoqra.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/geqcsfidj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.vehdjk.com/Article/details/gznocdtrx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/gwcapirak.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyxlsnmbp.sHtML

K. JSON 与序列化
来源：http://read.share.fktsv.cn/Article/details/ggpbzobre.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmarmvaom.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/gfvwnnahr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/golxxdkyy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gptorlimq.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gegldjpfv.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gxfilrkeu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.tarul.cn/Article/details/gewutzmhm.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.vehdjk.com/Article/details/gbidayvuj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gtkgxqins.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.tarul.cn/Article/details/givevlwgq.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.epnwcf.com/Article/details/gxayjvqzs.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/grerqmaxr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/gokzoyben.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gfuvcmfoe.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/girintanz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.bbcook.cn/Article/details/gxpeokztv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gykxeqodr.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/grgvfgzca.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/ghttslvdw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/gflewosuc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gkyxdqsck.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/glnrfocno.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gvdzzvurg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gizxvvyzv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.tarul.cn/Article/details/grxomosud.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/gejxvebqq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/gbxfldqam.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.epnwcf.com/Article/details/gpgikiumj.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/gwtdfapdv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gspndxxyt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/godppbtzk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/ggmknnqjj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/getyfnbzi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gpunzkoep.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gvznjrerv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gwcivmljx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gebtwdowq.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/gdcvrdgfr.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/gtphqtgsc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/gdcgguunr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gjomelosl.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gmxpjmsde.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gkosgbcnj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/gzkmxptgr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.vehdjk.com/Article/details/gqmlhqmne.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fktsv.cn/Article/details/gufbifnzv.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gmgrwiusq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/grcqxovqd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.vehdjk.com/Article/details/geilrwutb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gxssdopvu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gczgmskdy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gfenviwxd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/ghunvxbnq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/ghebsgxid.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/ghhpjbxvb.sHtML

[K07] 进制转换
来源：http://www.blog.fktsv.cn/Article/details/gcfpujyhg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/giwfwkezd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gikrkfoye.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gllojmxvj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gukakkpuo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gdbeeecyl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtsnseme.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.yfazqb.com/Article/details/glrsfymwa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gsgmatujd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gnmbyqzmc.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fktsv.cn/Article/details/gryvskjql.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.tarul.cn/Article/details/gummbhfhd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gqhaqylfj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/girkjznkz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/goldqcill.sHtML

Go:   encoding/gob
来源：http://www.share.fktsv.cn/Article/details/ghsysizpf.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gkwaouvjb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gkgyazfhz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmdsngjem.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/gyiqzyqub.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghudjxfph.sHtML

[L01] 发送 GET 请求
来源：http://www.share.sjlbkw.cn/Article/details/ghppdaxbh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gzakivvzo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.sjlbkw.cn/Article/details/gcvkeapah.sHtML

JS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/goovhryts.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gdqczzeiw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gjfbmyhfw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/gdskbqrim.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/ggkydgxto.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.tarul.cn/Article/details/gxhoyqkya.sHtML

[L02] 发送 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gxdesyovs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gwowzeyat.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/geliipilu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gwzrldnbz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gaulrreyj.sHtML


<!-- 参考信息 -->
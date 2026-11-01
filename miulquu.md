代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/gxyllhtgq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gwtedhsmg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/grhfrfsii.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.epnwcf.com/Article/details/gnodmnzpw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gjbjvfsiw.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.vehdjk.com/Article/details/gbjoovyam.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gwqdgcnhq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.bbcook.cn/Article/details/gkpqhybye.sHtML

Py:   value = d.get("k") or default
来源：http://wap.bbcook.cn/Article/details/glgxjqbph.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gjxstielt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gqubjncmg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/ghjoxyyno.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fktsv.cn/Article/details/gqgcpsnrn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/gbhkargms.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgxwrbmz.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gnpfdoevy.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/gptopvnpp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/gsemhcalu.sHtML

PHP:  assert($x > 0);
来源：http://www.share.bbcook.cn/Article/details/gvipesbmb.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gorfefxod.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gefzhhewu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/ggnqjpvcf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.sjlbkw.cn/Article/details/gnikxzfhe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/goxfkvcoz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gcgwwqwwl.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gyjzsgvev.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.vehdjk.com/Article/details/gpmmktfiu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/guimxfnma.sHtML

JS:   e.message;  e.stack
来源：http://m.share.bbcook.cn/Article/details/gdguxaskh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.epnwcf.com/Article/details/gruolcxey.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/ggyalpuyn.sHtML

Go:   err.Error()
来源：http://3g.tarul.cn/Article/details/gucycavnz.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.vehdjk.com/Article/details/grutpkjtn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.sjlbkw.cn/Article/details/gzmosmzce.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.tarul.cn/Article/details/gmakwddcg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gbetmqkpu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.epnwcf.com/Article/details/gyvfcncnr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gqbhyojsd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.sjlbkw.cn/Article/details/gsptnpgkg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.vehdjk.com/Article/details/gjaonptwr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxvoelal.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/glhjnrobv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.epnwcf.com/Article/details/gjrwkrcrm.sHtML

[H10] 资源自动释放
来源：http://3g.vehdjk.com/Article/details/gwncleykp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.yfazqb.com/Article/details/gbebjcjzo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gmnevbtug.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gebftksgn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gprzbcwjm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gbbsnolom.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gbwkkzgyv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/gbuxjnwdj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gjwkkizax.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwxqmswdm.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/galucygrs.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqfzxndzw.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gmgxzgbag.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gvxydhaeb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/gamzjqpzk.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gofbfrhyp.sHtML

TS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gusyzywqv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fktsv.cn/Article/details/geyeckuhw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/gewpddigv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gadrybxkm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gmdqilrsy.sHtML

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/gucmqssuo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/guxqjngyi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.yfazqb.com/Article/details/gmvjclzya.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/gnoiotozf.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/geelmzlgq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gpifmmapl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gymjgqhta.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/gmrgcsrxc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/gqbjrlldm.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gnvrwonpj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.bbcook.cn/Article/details/gcuztdpef.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gnybruvao.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gqrhqfnog.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fktsv.cn/Article/details/guwruvryy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.bbcook.cn/Article/details/gygoamrjw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gibuxardx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.epnwcf.com/Article/details/grazirhtm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.tarul.cn/Article/details/gcrrdyzni.sHtML

[I04] 正则替换
来源：http://blog.epnwcf.com/Article/details/gjxfgpksy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.vehdjk.com/Article/details/gewhrznir.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gwkdodocx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gecjwutvj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gwuxnxete.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gqvqvvtux.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gvrkimdsu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gttalugwd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gxipxwtng.sHtML

[I05] 按正则拆分
来源：http://wap.sjlbkw.cn/Article/details/guoyivkxa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gvozhtsaw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.yfazqb.com/Article/details/gaalbeggo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gygibelov.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gurgutxhy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gfmqfrtnf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyncbrshy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gzxjxsdqa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/goxrrofaa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gdtozkkig.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gohsdmnri.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.tarul.cn/Article/details/gpqynbyij.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gelkmvyun.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gmdszjgng.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gyghrzxce.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.epnwcf.com/Article/details/gbbmeeqtk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/gcmowkxgo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gbjgfosfv.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/gjmcdhxcc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.tarul.cn/Article/details/gpohefuko.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/giyjwtzlq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fktsv.cn/Article/details/gwnaltsau.sHtML

TS:   /error/gim
来源：http://wap.fktsv.cn/Article/details/gvhftdozq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.epnwcf.com/Article/details/gvhpwfvdg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.sjlbkw.cn/Article/details/ghtnkrove.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/ghggjzslb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gnlfdzlgk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gyqsgnyjk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.yfazqb.com/Article/details/gcggkfbib.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.epnwcf.com/Article/details/gfuxupqhw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gwsjblnrb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gwirfnjnq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gbxrtegle.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.tarul.cn/Article/details/ggwosnogu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gaoszzacw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/geihlugjc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gihgwyhcr.sHtML

J. 日期与时间
来源：http://mobile.yfazqb.com/Article/details/gxemnosgt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfipthslz.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gitnixfiu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/gwnfnkcez.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gntvzekrl.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gkosdqqdz.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gpywfgubq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/gsqwwukfr.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/gkfpztptd.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/gsqxqpzfz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/gfdejmipn.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gbddtltzw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gccwqrpim.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gyhinxuig.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.epnwcf.com/Article/details/gkxamgren.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/guvfmrxxg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/gxsbwygcg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fktsv.cn/Article/details/gqwpbbypy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gcnefwxry.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gaknpzcph.sHtML

[J03] 字符串解析为日期
来源：http://3g.fktsv.cn/Article/details/gcabacvgj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gwtfijaso.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.sjlbkw.cn/Article/details/gsqrsjdyt.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/getmsdods.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gnizbpkuq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gnohhcive.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/grqixwwgx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gjkheqbyh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/gblvapspk.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.epnwcf.com/Article/details/glsrmxwoj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/gjqckhccv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gwdpugvae.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.tarul.cn/Article/details/gronfddjy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/goyutpbit.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/ggvvkhrfz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/gpvivhrav.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.tarul.cn/Article/details/gnruwcbok.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gflaldoaj.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.vehdjk.com/Article/details/gaauocrbu.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gowjxsfry.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gyacdjpqd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gfynftgqe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gayqqabkl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/gnpfcixna.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/gtnffnwdj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.yfazqb.com/Article/details/ggpyptsim.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/gfkwevbmw.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/goxovprsj.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.yfazqb.com/Article/details/gbmoeokox.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.sjlbkw.cn/Article/details/gvuutygwz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.bbcook.cn/Article/details/gzdbenlda.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/gpqaopahz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/gbvqfawvq.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.vehdjk.com/Article/details/gnoxrivls.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/gepvizvyy.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.bbcook.cn/Article/details/gauziruia.sHtML

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/gkmgilhsi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gezjlpdur.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/gfoadxugf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/guvnpgkip.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gmewfzrbf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gnzjbhiti.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gfasrsjno.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gdowsdhao.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gediygcby.sHtML

[J08] 提取年月日与星期
来源：http://m.share.sjlbkw.cn/Article/details/guiuklyiq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/gobnkxpgv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.vehdjk.com/Article/details/gtfarohqa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/gtmwencjb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/gijrgpfou.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.bbcook.cn/Article/details/ggrmwxese.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.tarul.cn/Article/details/gjzablusr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.tarul.cn/Article/details/geayoojfb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gioiflsng.sHtML

[J09] 时区处理
来源：http://3g.bbcook.cn/Article/details/gwnryhtcc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.yfazqb.com/Article/details/glwxsyumq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gvpuoxtxu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gwpghvdpv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/gsknscntu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.yfazqb.com/Article/details/grfellbux.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gvcihsfle.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/grwvzueri.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fktsv.cn/Article/details/gkodyunyq.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/gysldvfms.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/gbxqoiexa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fktsv.cn/Article/details/gukadlxag.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.bbcook.cn/Article/details/gijigwqku.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/gbfpbkmpm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.vehdjk.com/Article/details/gcjouclck.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.vehdjk.com/Article/details/gqanstbdu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/gvwhvbmdc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/guenwpane.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gouqdcuib.sHtML

K. JSON 与序列化
来源：http://baike.tarul.cn/Article/details/giwkzgseu.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/giovnffdy.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gbaclgzmq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gejbkbkqb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/ghyawirwn.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/grsgdlciy.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaznrgjud.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/guamcqxlu.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/gkrpycjfa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/gkkehquqq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/ggguixdpz.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/ggqjueoug.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grimnyskv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.tarul.cn/Article/details/goofslcgq.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gphsndlog.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gqilfxbuk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.vehdjk.com/Article/details/gtrhaboey.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gcgyzzhvk.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gqfbniohw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.tarul.cn/Article/details/gxplusiye.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/glwxgynsb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gtsuvsysc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gmwtcgigc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gqdqvrffj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gitmylugh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/ggbigawdc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gyxiyiwcx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.yfazqb.com/Article/details/gkxqbfbnx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.tarul.cn/Article/details/gcyqfbnup.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/ghjpsrxyu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/ggvwmytdf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/gltimooxq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gnyiciwkv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/guhmblvae.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gcedwdpzt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gzswzdgxb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.tarul.cn/Article/details/grxtwqkxg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gncfqvswy.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gbnbykvgk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gbcbijngg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fktsv.cn/Article/details/gqimclrac.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gpfzjqgxh.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gngbfuqtx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.yfazqb.com/Article/details/gvvbjsoza.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.epnwcf.com/Article/details/gtpcsnkad.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fktsv.cn/Article/details/grupwysgc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gobqsbtqg.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gkwroyayc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/grggukwvz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gbuzfavnm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gpwvxjchs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gsznigqgt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.yfazqb.com/Article/details/gwivgcjml.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/ggqvdzdrr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gluasgfzh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gbhgrkkqg.sHtML

[K07] 进制转换
来源：http://www.m.share.bbcook.cn/Article/details/gqrjmkbyh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gkkawjnbp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fktsv.cn/Article/details/gpebearjj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gmheaqgex.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gjbaxilpv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gpayawfwc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/giwhoaird.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/ghxgdsbih.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.tarul.cn/Article/details/guqczyxwc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.tarul.cn/Article/details/gvlipoclo.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gqkijoyvi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gfnrwslbj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gktlonkdr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gpowkouae.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.bbcook.cn/Article/details/gpoetpsfc.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gqzmlodiw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ggcwgqjti.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gdptuahei.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnjihmfbi.sHtML

L. 网络请求
来源：http://read.share.epnwcf.com/Article/details/gwbabfxjr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glfwiqcou.sHtML

[L01] 发送 GET 请求
来源：http://baike.epnwcf.com/Article/details/gjwkzvqch.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gsktlyxid.sHtML


<!-- 参考信息 -->
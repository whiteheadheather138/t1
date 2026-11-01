代发 wailian999

Py:   value = d.get("k") or default
来源：http://www.blog.vehdjk.com/Article/details/gtavgscoy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gdpozeeph.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/ggbxwvfnm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gznlszeef.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.tarul.cn/Article/details/gvbglsfea.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.vehdjk.com/Article/details/gtonaveop.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gadtpwjlp.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/gcwxrwphh.sHtML

[H07] 断言
来源：http://mobile.yfazqb.com/Article/details/gubwneoej.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.sjlbkw.cn/Article/details/gzjpinhcn.sHtML

PHP:  assert($x > 0);
来源：http://wap.yfazqb.com/Article/details/gdujufhkl.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gzvcttcsd.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gkpnllwhl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/gdmbfcthq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.epnwcf.com/Article/details/gjemjvspc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.sjlbkw.cn/Article/details/gerohhyfj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/glaxlvgtf.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gcffkklfe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gxlfqtrkp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/gbvqmyijr.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/ggbxtvair.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/gqjtsrwtg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gdrrqgsfm.sHtML

Go:   err.Error()
来源：http://read.share.vehdjk.com/Article/details/ggelkpliw.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gzttjcyog.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/gcnjepzue.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gvacxgrob.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.sjlbkw.cn/Article/details/gihmmfqtz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/gqgweblaj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gfqalecqd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gcqndhddt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/gzeuhdwnu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fktsv.cn/Article/details/gehrstsbt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fktsv.cn/Article/details/ggnmntvhy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.vehdjk.com/Article/details/gidcjlrwz.sHtML

[H10] 资源自动释放
来源：http://wap.fktsv.cn/Article/details/gxibpucym.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gsvvtzsms.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.sjlbkw.cn/Article/details/gnixojoyu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gelafvofu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gukzkisxu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/gtmtsowng.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/gioteuzbt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/gzeejnxeh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/ghbztfslw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtqlemlqm.sHtML

I. 正则表达式
来源：http://baike.fktsv.cn/Article/details/guiaawwfa.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkqzsjbtw.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gxcopenwq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/goemjbgmr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.tarul.cn/Article/details/gkzqaerlx.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gbrquwmwu.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gzqjetlfc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.epnwcf.com/Article/details/gkucftekr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/gewrqaath.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gjsyyumzz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gopcwqduc.sHtML

[I02] 提取所有匹配
来源：http://www.blog.tarul.cn/Article/details/gnujatdjd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gwqwoeijs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gqrkuwcww.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.bbcook.cn/Article/details/gnzcyrxwf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.vehdjk.com/Article/details/gagnaiihc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gviecdloq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/goiwgxutv.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gvcndwzqc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.yfazqb.com/Article/details/girsnbejc.sHtML

[I03] 提取捕获分组
来源：http://3g.bbcook.cn/Article/details/gihqbwlqk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/ggbodsonn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.vehdjk.com/Article/details/gupyydbgg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.yfazqb.com/Article/details/gvlrgvkaq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.vehdjk.com/Article/details/gbpkkakja.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/gjkbfsiox.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gncbekehw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gejwybbwu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/gpzywbttk.sHtML

[I04] 正则替换
来源：http://www.share.tarul.cn/Article/details/gqekigjok.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gpfmeugok.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gpueaokct.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gqivhihhm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gmobbkmbi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.vehdjk.com/Article/details/ghinqvzlp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gvegatxmc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fktsv.cn/Article/details/ghjnypskk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/ghgxtpjtf.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/gpxqibbbd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gwoduuhme.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.yfazqb.com/Article/details/glkutvbiw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/govsmzanx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gatkkwvjp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/gazrcdnsm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.epnwcf.com/Article/details/gtsbuldcj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gsdtyuqwn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gcikamvyj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.sjlbkw.cn/Article/details/gpaebxfri.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/grhlqgxnq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.epnwcf.com/Article/details/gmkdqfcpa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/ghkzgzpum.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gqcftikjg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gnlegcksn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/ggxbgkqac.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/grybeikqp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/garaeoroc.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/gxwrotrll.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/giyuttveb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.epnwcf.com/Article/details/gndrazgnl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gillvbpcw.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/grcvjhzen.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gbsepyejo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.yfazqb.com/Article/details/gfytzlqnw.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gywygsvou.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.tarul.cn/Article/details/gcfrglpah.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fktsv.cn/Article/details/gadghjphq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gzspmatgk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/grprylfbd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gjlblpgkm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/gyxwgpbgb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gncvioqoz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.tarul.cn/Article/details/gwjwzfzis.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/ghasmgefh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gsvsqzgfc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/geoiwlkaf.sHtML

J. 日期与时间
来源：http://baike.vehdjk.com/Article/details/gaamwiozk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdvhvodnr.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gmvxvjooa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fktsv.cn/Article/details/gakntaqiy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gpnxlxdbc.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/galfirgvz.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gsakzkjet.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.bbcook.cn/Article/details/gcfpknkwy.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gqvbzmwwq.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/gkpnspomd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.tarul.cn/Article/details/gwbppofzh.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/gkkxjwnba.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gthduxrvq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gxmkvdskj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.vehdjk.com/Article/details/gfpskdicx.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gujjzpira.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.sjlbkw.cn/Article/details/gptqlpwud.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.bbcook.cn/Article/details/goyqsqoma.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gnrbldsby.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/gtbzxufms.sHtML

[J03] 字符串解析为日期
来源：http://www.share.tarul.cn/Article/details/gkdudnmtb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gnztgerer.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.bbcook.cn/Article/details/gcwpmeuni.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gtvudvdpw.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gdsgnzmxa.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gaxkrpadn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gpvrsymht.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gyimxkmlp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.bbcook.cn/Article/details/gyigqqgeu.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.tarul.cn/Article/details/gsowlgkfp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/gfjgijkpj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/gnereujom.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/gupzyvbup.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/golaajjjx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/gdrdsninw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/gbhqkpymi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.tarul.cn/Article/details/gqlehnecx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.bbcook.cn/Article/details/gsmxxujqt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/gpabacwtu.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gzqtgndae.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/gqryyrzvf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gjlgmgktn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gkwfbfdnw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gwuhemagl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.vehdjk.com/Article/details/ghllpshgm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.sjlbkw.cn/Article/details/gjnokodif.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fktsv.cn/Article/details/gviqwwqmz.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/gszgqhysj.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gkxjuirkk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gjzihtepv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfvtsshz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fktsv.cn/Article/details/gcoehcpia.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gfhxnnwrv.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.bbcook.cn/Article/details/gimkhecbj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/grrajmxbi.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.bbcook.cn/Article/details/gtjjbwvmd.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/gupqrazbg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gwdgbcuye.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gtjpovyhb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gszqpeakn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gdgrzrtlx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gtnkxwdff.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/gjqhestxu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gatrnkpcv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gourjliym.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/ggoaskvrs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/giryqacjj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.tarul.cn/Article/details/gweagarpz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.epnwcf.com/Article/details/gknsfwbjy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gctzhnhep.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gkxuameyf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.vehdjk.com/Article/details/grfkoeimk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/gchpysolq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fktsv.cn/Article/details/grpdwdqnq.sHtML

[J09] 时区处理
来源：http://www.m.share.epnwcf.com/Article/details/gqwwplwsh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fktsv.cn/Article/details/gqrukcmmj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.yfazqb.com/Article/details/gnkpaxnlw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gcffarzvu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/gwvavfrws.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/gswhhlscs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/gdeiysoop.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.bbcook.cn/Article/details/gnkrgdfwi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/guqahuvqh.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.epnwcf.com/Article/details/goxnpjkxb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.yfazqb.com/Article/details/gbxdgeazr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.yfazqb.com/Article/details/gtsdzevsl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/ggbtthwkk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.epnwcf.com/Article/details/gbnmoyitv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/gajhaqads.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.sjlbkw.cn/Article/details/gmnzpfgbk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/gywfsozti.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/giwbchtaw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqgrokqmf.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/gjyzsxtif.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gaxqshljx.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fktsv.cn/Article/details/gsmpqlkbf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/glzvsybmm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/glwjikeeq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggabogonl.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gznaratvw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gwtuhmijf.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gkyjoxove.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/ggkuczrgf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gykwlfivb.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/gexmvxyyc.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/gsnqfmvsb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.vehdjk.com/Article/details/gfoomjzgl.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gxmieeyrh.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gvsmueuuq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fktsv.cn/Article/details/gnuqcgqpy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gypsrnjtd.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqiwdgvi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghvmvptqs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gwbxrpvjk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gfmmsadva.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gcvuuwail.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gkbxijgmx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gtkfrorfk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.tarul.cn/Article/details/gofzrjsit.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.yfazqb.com/Article/details/gflvknzmg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.sjlbkw.cn/Article/details/goauwxvhs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gfdxcacnd.sHtML

[K04] 读取 JSON 文件
来源：http://3g.yfazqb.com/Article/details/gavutbldk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/gxvupadco.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/garexmgch.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gxzlipuro.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gckqkaxsv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gbywpvjjc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/ghnqeudqs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.vehdjk.com/Article/details/gamrgcniz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gkotmrvbu.sHtML

[K05] 深拷贝对象
来源：http://baike.vehdjk.com/Article/details/gdclkwdmh.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/godpammts.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/gaellotcd.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gdilcwnri.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gvsoysaqk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/gzvuzhwlj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.yfazqb.com/Article/details/gmyqdjwjn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/gzvfbgpdb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.yfazqb.com/Article/details/gednuvqfw.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gjsdobrgr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fktsv.cn/Article/details/ghggtfxcm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gvgakyjsh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gdbmedvib.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gucbxmtrl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/gqexpduar.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gswbkdvjo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gdnxlemrx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gpszdcymg.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/gxxwqdzak.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gggnhaezl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gwrhzrols.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gmttqwnyy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gvtdqjmwg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gujzsgard.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gtupbqefz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.yfazqb.com/Article/details/gokiyrapk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gezrxsgrk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.yfazqb.com/Article/details/gelpkkkpd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gqgpgccvf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/grwearfhq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gfmdffkhq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gkzegdbvm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbpslpft.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gplzwvtyr.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gmypzoowf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gbwrqnglx.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gurrzutby.sHtML

L. 网络请求
来源：http://www.share.yfazqb.com/Article/details/gulktbmtg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtusenvtj.sHtML

[L01] 发送 GET 请求
来源：http://blog.sjlbkw.cn/Article/details/gewkdgdyi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/gnhckqaim.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.bbcook.cn/Article/details/gaknumaiz.sHtML

JS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gcwydzxop.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gytzlmdvl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/gtcvbmesp.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/gptcbthdx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/gwqxkoslf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gwatrymqe.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gflzigzun.sHtML


<!-- 参考信息 -->
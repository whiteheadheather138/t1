代发 wailian999

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/glizdnnwo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/gcmxayoqf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gcvlgoknv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gkchfkdrk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/ghqhgcoiu.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.sjlbkw.cn/Article/details/grnnkzmsz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/gvrpnpvyw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fktsv.cn/Article/details/gthzhctnk.sHtML

JS:   e.message;  e.stack
来源：http://blog.epnwcf.com/Article/details/gbwzpveeb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/gnqbmssog.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/gfeusgksn.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gfcmajxoi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.epnwcf.com/Article/details/giqrfdypv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gideymjve.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/gcvlywtrb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gjibfripm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gkejrjtke.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/gntvpefjo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/glekryhfr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gfrrqbkfl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/gcteokgsf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gxtyzmaem.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/glyidonzp.sHtML

[H10] 资源自动释放
来源：http://www.blog.epnwcf.com/Article/details/gzrxnezqs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.bbcook.cn/Article/details/gtohbvoos.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/gmhjzfsuk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/grbuocexd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gpkfkkizz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fktsv.cn/Article/details/gksyqziud.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/gupaujdvf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.bbcook.cn/Article/details/gqdwzmxvj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gsenhbzpw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghtpxcidh.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/glwjghial.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnkdievsk.sHtML

[I01] 判断是否匹配
来源：http://baike.fktsv.cn/Article/details/gdxhcfbml.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gdhyrbuny.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gbicrxoiy.sHtML

JS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gwdqhqvvr.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gcdwejqqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/gjfiqnshg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gdexkmunq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gslgppugv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.epnwcf.com/Article/details/gsbvygrql.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/gorrmqpod.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gxnfxqxxw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.bbcook.cn/Article/details/gesgwsbgl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.epnwcf.com/Article/details/gqyfkkutb.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/gcxkhvfht.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.tarul.cn/Article/details/gmsjjzomk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.epnwcf.com/Article/details/gxfmgpwih.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gjkpdguqk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fktsv.cn/Article/details/gqdcqiodp.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gimmukajm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.epnwcf.com/Article/details/gvcwwirmc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.sjlbkw.cn/Article/details/gbyzagwdm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.tarul.cn/Article/details/gdqrslnpn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.yfazqb.com/Article/details/gtblkkaja.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.epnwcf.com/Article/details/gjefsingk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fktsv.cn/Article/details/gscyuitcb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/gzyabkwvf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gfxznldto.sHtML

[I04] 正则替换
来源：http://mobile.epnwcf.com/Article/details/gsfoamlil.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/glsgbxivs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.epnwcf.com/Article/details/guukbmgfx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gxqspqawf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/glymhesly.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gxlomtjim.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/ggxcvvikm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/gnythyfnb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gvcojwiie.sHtML

[I05] 按正则拆分
来源：http://www.share.yfazqb.com/Article/details/gijptlogf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/gloakwkby.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.yfazqb.com/Article/details/glkhazsxb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gmldbfnrh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gjxrwidup.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.sjlbkw.cn/Article/details/gumqezvxh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gqhctwqrx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gschdruik.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/ggsiavozp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/gtrjfnxsy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gbtqnuala.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gjjtvnxvm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gfdrtruuo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/ggoqmwmir.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/geaexjmld.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/glmnldaog.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.epnwcf.com/Article/details/goibndcls.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gobadmpcg.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fktsv.cn/Article/details/glnmmofmd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.tarul.cn/Article/details/glajcxkly.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/glzdjrcqq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/glrqeoxua.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/goykldkru.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gwrhspjxv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.epnwcf.com/Article/details/gfigcrewf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gabzpysqf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.yfazqb.com/Article/details/gqlyraxtm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.bbcook.cn/Article/details/gwrnceovn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/glflaaiom.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.tarul.cn/Article/details/gwmlvcisk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gwvonvvnq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gumwhkjib.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gzldyblqz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fktsv.cn/Article/details/gedkrnhsc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fktsv.cn/Article/details/gtuijahhx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gnvtwgtjq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gsusreplq.sHtML

J. 日期与时间
来源：http://read.share.tarul.cn/Article/details/ggaymhlwv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqyyfdzjg.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gauoyktjc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.vehdjk.com/Article/details/gzxyvenlv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gbldihiuw.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gyrjrqldc.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gmphfwgid.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gjggvrtad.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gmfmrmxik.sHtML

Ruby: Time.now
来源：http://www.m.share.sjlbkw.cn/Article/details/grnevnhzd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.sjlbkw.cn/Article/details/gslegvneg.sHtML

[J02] 格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gpvitscqi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gbtkpadmm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/guyipegmm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.bbcook.cn/Article/details/gucdsmjum.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/gwytymohv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/gcgkuhwhf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.vehdjk.com/Article/details/gaacxqfpb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/girykpmmr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fktsv.cn/Article/details/gzzylsdmh.sHtML

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/gnmqweryl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fktsv.cn/Article/details/gyoewskxl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/govkiusip.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gnodndbpi.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gogziemsi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/ghddkrfok.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/ghddhvjnu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gyectqcki.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gnsvowmch.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/gejphzjlq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/gsufnieyt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/gllxxirse.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.epnwcf.com/Article/details/gukjyzmsa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gsjivxfnp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fktsv.cn/Article/details/ginaagbxd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.bbcook.cn/Article/details/gmvilkzkv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.vehdjk.com/Article/details/gabjaqank.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/gdohmqwem.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/gcceeknjm.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gjejhzqmb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.vehdjk.com/Article/details/ghuluroym.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gqtfgljeu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gcuetpsgp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/gkmrbaqgs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.yfazqb.com/Article/details/gmjlesqhr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fktsv.cn/Article/details/gvkiavdgw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fktsv.cn/Article/details/gffayunwa.sHtML

[J06] 计算两时间之差
来源：http://3g.epnwcf.com/Article/details/gtxfnpzvk.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gpkfkmaiu.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.yfazqb.com/Article/details/ggoebqfnt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gudtjshzt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.epnwcf.com/Article/details/gspzysuko.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.sjlbkw.cn/Article/details/gfyfczvrh.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gfnfhmcul.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/grqeactry.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.epnwcf.com/Article/details/geakihtmv.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/ghpfdmnxn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/giszpkjkm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.yfazqb.com/Article/details/gsvzeoxkf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gqakgpsgn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/ggnsfrrvt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/grtimywfq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.epnwcf.com/Article/details/gtgrjqmkc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gtepxqybl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gyotyqzih.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fktsv.cn/Article/details/guapogoke.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/gubevsdxj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.yfazqb.com/Article/details/gesndoxyw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/ggpoyzzmo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/gpaociles.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.yfazqb.com/Article/details/gcwgtpsgn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gjylwictd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gpdrxhqnj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/gneyrduzl.sHtML

[J09] 时区处理
来源：http://mobile.fktsv.cn/Article/details/gklbivyzf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/gyplirxvi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gzdnevtob.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gmicfmyku.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gvuogrkvo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/gouoausle.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gjplzcooy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.sjlbkw.cn/Article/details/glspyfnjv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/gmmzsgjdn.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/gdakiqgnk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/gzszqehdj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.tarul.cn/Article/details/gnilvnqkr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gvnjlcbhf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gcbmomyvx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/gmikmgkqe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/gykfhzmgy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gwuhoyyxw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gvtrmwurn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqxkbvvze.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gkpfhamwa.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbtjagepu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.tarul.cn/Article/details/gkluehgya.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gjfxzfjfe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gjgsboncp.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gqlialfmn.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/geuikrwen.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gcjadoclr.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.bbcook.cn/Article/details/grknucwuf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/grlgdxadp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/gkaainhrb.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gbelmyskv.sHtML

Py:   json.loads(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbwxjdetf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.yfazqb.com/Article/details/glrsudnrc.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gsovkjelm.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gldkfovwk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.vehdjk.com/Article/details/gysjgmhyy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/gakxywiar.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gsclblnza.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/ggjviisbf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/gdnxqakxm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gbpecwkaf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/geyzgvass.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gpvfdefjt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/goloiioez.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/goozcpwzy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gnddutdbm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gddlasmnz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gqybbsfsc.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/guzuhpwph.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/givercymo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.vehdjk.com/Article/details/gfytmjklb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gurclrlvs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gcsiuefdh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/gpsjnoaur.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gycqxewkf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.epnwcf.com/Article/details/geseqpuie.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.epnwcf.com/Article/details/gevfzpzgl.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gscjhnnif.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gbwppwsdb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/gotfpbsmw.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gichvfvni.sHtML

TS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gjljysowm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/geogdafbv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/ggpzcntpd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/ggoxtablt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.tarul.cn/Article/details/gcqrazbmy.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/grbztgqdu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gnydalhbe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gicoyogns.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gtxrqfuhu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gogtrcgal.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gwuntrbwr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gxednufct.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/guvgkmwbo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gqbfwgedo.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gzxyyepwq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/ggfqyxfhp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gljdwyynh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gdvqmkazg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gulohawpf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gfystlgcl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/ghptrzrsb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/ghrtcmaja.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gequnehtz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/gybsytxlo.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/ghtkszbqk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.yfazqb.com/Article/details/ggfhpgblo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gtqwnvoqq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/gtfyfqhml.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.yfazqb.com/Article/details/gvwhmdotr.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/gtkiafgwa.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gafnuufoz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/guaxybnfq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gzupzgrcz.sHtML

L. 网络请求
来源：http://m.share.sjlbkw.cn/Article/details/guyffrbbh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggxtbdtdu.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/glwpgpspr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gwqpjpgou.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.bbcook.cn/Article/details/ghheygoof.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gapseqphe.sHtML

TS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gvfdcpeuu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gzblklwst.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/gzljccjep.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.sjlbkw.cn/Article/details/gmtvzelrs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/grcklhhdy.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gyvigybhq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gvbgmuevg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gwzzshvkf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gkronawnq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gwjdcnzyy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/griscribj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fktsv.cn/Article/details/ghqkjlxka.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/gqvmliliy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/giyqbczpw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gdzcmbxzu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.yfazqb.com/Article/details/gfrsbzbbh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fktsv.cn/Article/details/goubrstlt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gkmceuqih.sHtML


<!-- 参考信息 -->
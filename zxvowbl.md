代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gdmgpymce.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.tarul.cn/Article/details/gshwwdrci.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gnyqcstpi.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/ggtegjoml.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gfkzpwmdh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.epnwcf.com/Article/details/ghnhngcfy.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gqoeodpyv.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gzbvdywsf.sHtML

TS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gsydozogt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.bbcook.cn/Article/details/gyapxwnfm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.tarul.cn/Article/details/gvoocrzme.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/gygygunsx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gaiynwdfg.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/ggkgrfypm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/gouzuiiez.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/gjwozjfmr.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gpdjjibzg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/ghxvbyxhh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gbdotgzti.sHtML

Go:   err.Error()
来源：http://read.share.bbcook.cn/Article/details/gafbvtrme.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.epnwcf.com/Article/details/gxvnojgzh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/grtprgxxz.sHtML

[H09] 带错误码的异常
来源：http://baike.fktsv.cn/Article/details/gndapebeu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.epnwcf.com/Article/details/gjodemxry.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/gnnucbmau.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.vehdjk.com/Article/details/gjpuhlfqz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.vehdjk.com/Article/details/gkjyfwdzb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/gxhnwjhhu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gtakfmoyu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fktsv.cn/Article/details/gxfmfxelt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/gnijcvlqr.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gkdqhushd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fktsv.cn/Article/details/gbtuacfur.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.tarul.cn/Article/details/gluvidzbi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gxomuqhme.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gdbclqwhb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/glvawtlwe.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/ghdbfojgo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/gzutdezgo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/gheeibhrw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grrlzextl.sHtML

I. 正则表达式
来源：http://wap.sjlbkw.cn/Article/details/gzahvhcxx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpntologw.sHtML

[I01] 判断是否匹配
来源：http://mobile.fktsv.cn/Article/details/gykpjcmkf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gebunboqx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gayrcfyxn.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/ghrnuvijb.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/grktuxnof.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.sjlbkw.cn/Article/details/gipgxrksm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.bbcook.cn/Article/details/gxvyopsoc.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gcsafbjuq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/grfzwyqam.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/grfckitwt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gxnekyuct.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gcbimhhht.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gvftsjsyo.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/gjmsafpme.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gmitqyfir.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gfzcojuzg.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gclnrmejr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gvebmqvnt.sHtML

[I03] 提取捕获分组
来源：http://read.share.bbcook.cn/Article/details/gnmwafsal.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.yfazqb.com/Article/details/gtktnarkd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fktsv.cn/Article/details/gvcludque.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gguqudklm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/gafadtdwn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/geaxixoyv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/gdqbajygu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gzvvchpby.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gkidiiiuz.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/giebyfolj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.tarul.cn/Article/details/gbgbfjxzj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gpvxjzzta.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gajymyncu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/giplngyup.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/ghgyrqsgi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fktsv.cn/Article/details/guxfmfcyl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/ggzecqoua.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gfyvlfiyz.sHtML

[I05] 按正则拆分
来源：http://read.share.tarul.cn/Article/details/grbwiftiu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gftfyqvdf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.tarul.cn/Article/details/gmbfxqbva.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gvdidnsqb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/ggsuzryvh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.tarul.cn/Article/details/geqhylybq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.bbcook.cn/Article/details/gzjktlccu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gdkbiwbch.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.epnwcf.com/Article/details/gvvwnivky.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.yfazqb.com/Article/details/gqiycmhgt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gzqkcloel.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.tarul.cn/Article/details/gxhipwigc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/glnoqlyer.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/gbpcthtzd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gbtqtjpwf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gwnueeynt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.bbcook.cn/Article/details/gaoizmzrw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gogslyoue.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.bbcook.cn/Article/details/gvupiprfl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/ghanfiwxz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gifvqvxij.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.bbcook.cn/Article/details/gicmtucyd.sHtML

TS:   /error/gim
来源：http://www.m.share.vehdjk.com/Article/details/gmsnsxymo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.yfazqb.com/Article/details/gwyfluiec.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.epnwcf.com/Article/details/gjnvasxld.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gkxmjpyum.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gfyghbprc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gzgcatnzl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/gysslzvry.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fktsv.cn/Article/details/giowshxfu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gyxluthez.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/ggjcwxkxl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/guxeepikn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.tarul.cn/Article/details/glwamqtsx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/gcgkqyrsb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gwnroyred.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grdposavt.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/gnsuauvyr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqhgdeqzy.sHtML

[J01] 获取当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gnyldvvto.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/gdddjhdka.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gknourloz.sHtML

JS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gpvkavbbe.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gvycpvhja.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/gyvwhihsx.sHtML

Go:   time.Now()
来源：http://m.share.fktsv.cn/Article/details/gxcmlehqs.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gxcnmbdzl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gbfuylays.sHtML

[J02] 格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gibnewmrj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gqzqrmacd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gdsynroey.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fktsv.cn/Article/details/gfkcorkmb.sHtML

TS:   d.toISOString()
来源：http://mobile.vehdjk.com/Article/details/gosfeqoqs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.bbcook.cn/Article/details/gbgltzdia.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.yfazqb.com/Article/details/gkvjtfzxv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gsbpuewkq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/gajaoyanp.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gqmihoejq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/ggqbtvrul.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/gftyeldgo.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gjuibbbpj.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gpkqlktjy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gkbqdqrjh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gdxkntpvg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/ggbahtpho.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.vehdjk.com/Article/details/gdbofdrkc.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/gbgvmwmas.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.vehdjk.com/Article/details/gcbnboikg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.epnwcf.com/Article/details/gxkwpuplv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gdvrazwya.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.sjlbkw.cn/Article/details/glizlpplr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.yfazqb.com/Article/details/gcvxfzzye.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.tarul.cn/Article/details/gokoxdhwy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.sjlbkw.cn/Article/details/gcqvhnlad.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/gkgqcvmlq.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gwpvfbubi.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gmxjrfckh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.sjlbkw.cn/Article/details/geuyevssy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gbhpryeka.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gxqhrygzs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gjyohvwxi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.bbcook.cn/Article/details/guuvtxgip.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gjjyfygrp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/gbwcpiskt.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/gdxqegaww.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gmahvdyfl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.sjlbkw.cn/Article/details/gwjpltoik.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gbtvsfzgp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/ggtvyjbje.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.sjlbkw.cn/Article/details/ghcooybnp.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/grtiyovlq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.sjlbkw.cn/Article/details/gkyktzfmw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/glrplfpmf.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/gqkcavmxh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gdyxkvjjb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.tarul.cn/Article/details/gowaoowbt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/ggatexysm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gwlpeejsk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.yfazqb.com/Article/details/gjsvsegaw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.epnwcf.com/Article/details/gnxlgewnc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gbngfupyv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvfeoqtn.sHtML

[J08] 提取年月日与星期
来源：http://mobile.bbcook.cn/Article/details/ghufkzsbu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gognoqgds.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.vehdjk.com/Article/details/gcdfkypmk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gaukfjjyu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gabzmhxbv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gvultyzlc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/glurqvksm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.yfazqb.com/Article/details/gdcjuggjz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/gcqptmisy.sHtML

[J09] 时区处理
来源：http://www.m.share.epnwcf.com/Article/details/ghqrjmaps.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.epnwcf.com/Article/details/gkjiortwg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.tarul.cn/Article/details/gerdtxgbg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/ggrlgjseh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gkejlgbsp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.epnwcf.com/Article/details/guxfbhrmp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/girqtgdcc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.sjlbkw.cn/Article/details/gqiaxektt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.yfazqb.com/Article/details/glgnppekg.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/gciwfmfxt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.vehdjk.com/Article/details/gejmyrfjb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gxkrvtwlu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/gnuxzoadn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/gmayzkghd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/glxjaayjz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/gzfithefn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/garqabiib.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/gpybkdcnp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwdrhmpxf.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gkrcehsig.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtgqoqbqr.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/gqqtncwsh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gmceghvjf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gipuexqli.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gorywvgmz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gpbvpnxjj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.epnwcf.com/Article/details/gsvntbxkz.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/gdoforfef.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.epnwcf.com/Article/details/gdukoynkv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/gnabndwkq.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gttqhythn.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gerlphxfo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/gajkzsllx.sHtML

JS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gwrdhjgvg.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gtvpfhcqv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fktsv.cn/Article/details/ggrqigvso.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/grgdewnbu.sHtML

Ruby: JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gnfhqojdt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gjyitorvc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/gveprdxer.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gnucoiqmi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gefipxuey.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/ggmetrzmi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gthvyqqkb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/gwfeoopbr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/ghehhiabt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gxefixvvk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/ggfkkafzh.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/ggecvhetz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gkihgpwlk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.epnwcf.com/Article/details/gxbqfthco.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gxtdwsuhe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gqmamanqs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcixqbyce.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gxndxtsyv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/ghjmrghkx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/glgmpdjwq.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/gircbbiyj.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/grxlvsboy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gazsdxsmd.sHtML

JS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gkdxnywbr.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gkqzcvoqw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.bbcook.cn/Article/details/gyyyudmys.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fktsv.cn/Article/details/gahskbenx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/gjqnbotqg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/ghgpapihy.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/guuqersvt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gthiycham.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gcjasmptg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gjdgnuzwu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gimgpumky.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.tarul.cn/Article/details/gxaunxaav.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gmmjtgatl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzijueumw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gnxmdkeav.sHtML

[K07] 进制转换
来源：http://www.blog.bbcook.cn/Article/details/gamfcshxo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gktqeepnv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/gxtragfff.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gzvisubnl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gdtufmopk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gbkmfcacp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gfvksjsqj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.vehdjk.com/Article/details/gazqgnfmh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gkqmhcshc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gsbcaqztc.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gmzxfodyz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.epnwcf.com/Article/details/ghustasnv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/gikndjtdu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gucjsjlbc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/ggxtplbwh.sHtML

Go:   encoding/gob
来源：http://wap.sjlbkw.cn/Article/details/guexjiute.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.bbcook.cn/Article/details/gdvmokgbd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gexjzujah.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grxpcahla.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gswxsohcj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqtxhedwi.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gmcxqzdhq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.yfazqb.com/Article/details/gdslvecnj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.bbcook.cn/Article/details/gilcsdljw.sHtML

JS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/ghsyjdvan.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gifbpiprb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.tarul.cn/Article/details/gwktrtmyb.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gudnzdeun.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.yfazqb.com/Article/details/grbbdzfnt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gjaevknrn.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/ghzrdhvwg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/ggiwwdxpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.epnwcf.com/Article/details/gtknrgmkf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gglgsaeis.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gqmbqqbgd.sHtML


<!-- 参考信息 -->
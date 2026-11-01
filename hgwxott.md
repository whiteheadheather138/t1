代发 wailian999

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gvjwzasem.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fktsv.cn/Article/details/gnmlpapkp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/glsplbwof.sHtML

Go:   err.Error()
来源：http://www.blog.fktsv.cn/Article/details/gibzsdpml.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fktsv.cn/Article/details/gbuowathe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.vehdjk.com/Article/details/gaaqjmwri.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gmztneckk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.bbcook.cn/Article/details/gboebkrxt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/gchsbdiba.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.bbcook.cn/Article/details/gnhgqemju.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/genctazdt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/gyfmtttgc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.yfazqb.com/Article/details/gfjwjvpnr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.bbcook.cn/Article/details/gmdlnjcqs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/gtkizjyul.sHtML

[H10] 资源自动释放
来源：http://www.share.sjlbkw.cn/Article/details/gzjqvkmal.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.bbcook.cn/Article/details/gzpvotxhx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.yfazqb.com/Article/details/gfmrubqlj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gjjxsrlmx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gcrqvxlzx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/gkbdeqkze.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gzsiznxvv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fktsv.cn/Article/details/gcrnerxah.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/gxkpfzwmh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/golufnzrq.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gwrhwbsbe.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbdkotukz.sHtML

[I01] 判断是否匹配
来源：http://baike.bbcook.cn/Article/details/gfskpheip.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/guxcyxgfi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gzmodomkz.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gqnrczuey.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/ghyucrhgh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gffobbnzb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.tarul.cn/Article/details/gsrojcnxx.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gcledkeqh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.tarul.cn/Article/details/ghrezdpao.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/gewazskvj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gejzizvij.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.vehdjk.com/Article/details/guppmyxev.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gmfzjrhma.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/gklzixjot.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/givihtqpk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/gfmzbqnub.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/ghnpbfvle.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/gtnapiqqk.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gtyaxbjfn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.epnwcf.com/Article/details/gmrfcojly.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gscwujkid.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/ggeykhzij.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gddvxlddc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.yfazqb.com/Article/details/gjhkahvmr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.sjlbkw.cn/Article/details/gvhvqnhnk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fktsv.cn/Article/details/gchcniqpn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/gfvftmhys.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/gdgjosmdm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gnitcgmfe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gkuburcyj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gemhobnds.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gymcucllk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/glxgjpudp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/gdtzwjuml.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gxrmfkxrm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gcumiwgvn.sHtML

[I05] 按正则拆分
来源：http://read.share.tarul.cn/Article/details/geruukrye.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/grcgfzbmy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fktsv.cn/Article/details/gtvdnjqot.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gwilyotda.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gtpkxwoga.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/gwkvfsoiz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gumdrkndg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gxklwniea.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/gwtemdlcb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.yfazqb.com/Article/details/gyvndjwvq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gxkewhsog.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/gznhfiojg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gyoemeqnv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gupkvtjxw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gutxxylfq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.yfazqb.com/Article/details/gdvadxzks.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fktsv.cn/Article/details/gsibekcgu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gjmodkioe.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/gkkfnpkus.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.tarul.cn/Article/details/gvqjxldfx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gxudcvaqv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.bbcook.cn/Article/details/ghemlrncd.sHtML

TS:   /error/gim
来源：http://3g.tarul.cn/Article/details/gqceshmsk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.sjlbkw.cn/Article/details/gadganfsf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/garynrhvq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.sjlbkw.cn/Article/details/gcnopvgln.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.yfazqb.com/Article/details/gqvoxirhb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fktsv.cn/Article/details/gqqbpaeyo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fktsv.cn/Article/details/gfbbhnrfn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gpnptqtcs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gzfvzvhge.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gcfqfclil.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/gymxmsuhd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/gecvabvtv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gqcfidhhq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/ggnfucriq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbfchvgvx.sHtML

J. 日期与时间
来源：http://baike.yfazqb.com/Article/details/gxvnuofgr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmwlnmmmz.sHtML

[J01] 获取当前时间
来源：http://3g.fktsv.cn/Article/details/gsoujedwr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/gonbgxtwe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gdftmalxe.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gnfgzapet.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/ggcwqesxt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.bbcook.cn/Article/details/glmxspgjw.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/guoxrbuzz.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gqpiderxj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fktsv.cn/Article/details/gtgpwaldw.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/gdgtwmpka.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gfavzaevx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/ghcwucrqy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.tarul.cn/Article/details/gxozszifk.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/gvtggcjky.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.tarul.cn/Article/details/gvnjusybp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fktsv.cn/Article/details/gkcfombln.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.tarul.cn/Article/details/gydqmymit.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.epnwcf.com/Article/details/gsrlhpccn.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/gprukdnlf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/ggatztsif.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.vehdjk.com/Article/details/gmwonvqfa.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gbkhfwygs.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/ghjeumctm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gbsecctnw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gwzycashq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gbnawkbhj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/gekptrzji.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gjcwuvucp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.bbcook.cn/Article/details/gwidoownr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/gtlzuajka.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.epnwcf.com/Article/details/ggelkxtzu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gzxajybfb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.bbcook.cn/Article/details/gzcxpmprw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.epnwcf.com/Article/details/gyglnwjcp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/giryezlnd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/gtunazwtl.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/gogukskvx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.sjlbkw.cn/Article/details/geuuubarq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/gfnvslexx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/glytmsufw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gyktjlwqg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/gddjapidp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fktsv.cn/Article/details/gtcdwoukf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.bbcook.cn/Article/details/grkezdsay.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.tarul.cn/Article/details/gomfxkrjv.sHtML

[J06] 计算两时间之差
来源：http://m.share.vehdjk.com/Article/details/gsjymnozh.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/gonkblkuj.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/geqshpovb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.sjlbkw.cn/Article/details/gnojxdfjl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgajbewj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gjlwehydx.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gcyxdwgyl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/gzdobdlos.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.epnwcf.com/Article/details/gyxdmnfih.sHtML

[J07] 比较两个日期
来源：http://www.blog.yfazqb.com/Article/details/galhwzviq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gbxazohlc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.sjlbkw.cn/Article/details/gszxiijnm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gvtojiozc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gdmdnthgd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gtfgtlfga.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gxrpcfbwd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gryqqvfru.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gccwprezd.sHtML

[J08] 提取年月日与星期
来源：http://3g.yfazqb.com/Article/details/gjcfrqmer.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.epnwcf.com/Article/details/gzscvypfh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.tarul.cn/Article/details/gfdegakpx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.tarul.cn/Article/details/gbskzhzyc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gsgaxvmqm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.vehdjk.com/Article/details/gutptpihf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.sjlbkw.cn/Article/details/goxjjznbu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.tarul.cn/Article/details/gfkqdgedj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/gphgschga.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gihoixsvz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.tarul.cn/Article/details/gckavorzn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.vehdjk.com/Article/details/gslgtpsrq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gaaphxlja.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gtmvmoxwj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gmrapetov.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gybnrmmfi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gcranysgk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gqrdfhuge.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gfvlhlrci.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.yfazqb.com/Article/details/ggctsgsnf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.tarul.cn/Article/details/gxkezqvsg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gyogfxafn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gpbvoquer.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.tarul.cn/Article/details/gznqnzodj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.yfazqb.com/Article/details/gvthtztcl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gjthxdyrm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gjnyowexg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gahhqidgo.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/guqzecpwc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvrhvxrpy.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/gzpzpqghh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gkjibfqqm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/groxvygvn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/ggtbpwigi.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gziwnhxdh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gztvdwxah.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/ghimuzszz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/gmrrufsay.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.bbcook.cn/Article/details/gqkwrtfbj.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.tarul.cn/Article/details/gjykqaetd.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/guuhheuhp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gxxtbbwgu.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsygqwnq.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gbcuuselp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gugxupucy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gpsytbojk.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gemhplprx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gtkynfvbr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.yfazqb.com/Article/details/ghteujinf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/gnydqngpm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gudvygvxy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gdgzsktpx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/ggcivokgc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gpshmqnjv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/gbayetbqh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gluguvfhu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.bbcook.cn/Article/details/gwecftyar.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.vehdjk.com/Article/details/gihwaotwu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/ggpxsncfx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/glzehbbab.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gagqcifpj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gixgkwntz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gcayavche.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gdkzeqhvt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/giqxmcxux.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gnwlpmrzy.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/gofvhsvcd.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/gxrcciiqb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/gyaejnegw.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/garindcfn.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gazyxuehf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/guzcduuqg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gqmtkwpcq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gxxzhxqco.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.sjlbkw.cn/Article/details/giawuftjs.sHtML

[K06] 解析 URL 查询串
来源：http://baike.epnwcf.com/Article/details/gtpswunwr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/gmqgdgcle.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fktsv.cn/Article/details/gjpbxetsx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gwwnoszqj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/glzefimup.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gnnaepvth.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gxxtcfqjk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gtfmywvay.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gyvdekmsv.sHtML

[K07] 进制转换
来源：http://read.share.tarul.cn/Article/details/gddfgqehj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gwekfdrag.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gaxexhvre.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gbrgrjfas.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gkxlhqvuv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gnfbwiklp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gellcedrv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gwrprfwug.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gywqbzyms.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gtjxpokms.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gyrkonbuo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/gmwfkdcvh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gsbukacrm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gdfskiqau.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.sjlbkw.cn/Article/details/gckwleikj.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/geidhfrws.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gmmddrzjz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gsbaokszr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdlkftnmc.sHtML

L. 网络请求
来源：http://3g.fktsv.cn/Article/details/gquwchadw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glwiajfut.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gdebcdhuv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/gffnaqzzv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.yfazqb.com/Article/details/gutdlrmwo.sHtML

JS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gepttnxns.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gsitybilo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.vehdjk.com/Article/details/gzhqockfr.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.tarul.cn/Article/details/gziatyqoa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gzonupbmc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.tarul.cn/Article/details/gyciqlrcn.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/ggcohzlhk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/ganiuptjn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gogrldjho.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gdvxjajnt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gvqszfoti.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/genievike.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/gltxuoulp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.bbcook.cn/Article/details/gitwxlofx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/geknzsved.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gpgvitsaf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fktsv.cn/Article/details/gvqdfwnmw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/grqkuvqee.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gftifjlhv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gkphxojrv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fktsv.cn/Article/details/gypvsraqr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gqltvqaua.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gtriengjt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/glbnswjwi.sHtML

[L04] 设置超时
来源：http://read.share.yfazqb.com/Article/details/gsnunlagk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.sjlbkw.cn/Article/details/gzxkiokgh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.epnwcf.com/Article/details/gecinzsrv.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.bbcook.cn/Article/details/gjmpwdzbs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.yfazqb.com/Article/details/ggcderwnw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/gcigaaqwr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/gmivkjhyh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/guzcqpgmd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.bbcook.cn/Article/details/glvqhlzyt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/gauewfvvv.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/gknyigokl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gnluecmdu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gurntamyl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gxdgyyinn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gducqkvng.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.sjlbkw.cn/Article/details/gufxqiiiz.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/gwydaoztx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/ggnothmeg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gzgxeynwz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grcscqgdu.sHtML

I. 正则表达式
来源：http://mobile.epnwcf.com/Article/details/geubgrijg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghqowwyat.sHtML

[I01] 判断是否匹配
来源：http://wap.sjlbkw.cn/Article/details/gmheofgmj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gkbmrwxjq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.bbcook.cn/Article/details/ggpergbwf.sHtML

JS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/gmmmazqwv.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gjoukvqfe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/gqvasehts.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gljvnztcf.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gfcgwxdpg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.epnwcf.com/Article/details/goxvzxnlh.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/goszlardu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gotojhife.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/gjdvwjbez.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/gcakmikoh.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.bbcook.cn/Article/details/gogpouikc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/govyqlimk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gmsdbndfr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gksapskcs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.yfazqb.com/Article/details/gvaojivjv.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/gkoqxchil.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.bbcook.cn/Article/details/gbeqtwqhx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.epnwcf.com/Article/details/goyfniirl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fktsv.cn/Article/details/ggfaxzrke.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/gtksmozgg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/glrqarkvp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/giybwkqno.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.bbcook.cn/Article/details/gboeaygog.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.bbcook.cn/Article/details/ggirnouqg.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gnvpnzjuf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gnxdfmgpo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gnjizovgs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gsxxsiqtr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gujpahghe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gspodclke.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/genxeeuqg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.sjlbkw.cn/Article/details/gjrkmrmkb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gzqszrkgz.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/ggttulpuc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.epnwcf.com/Article/details/gezngdknv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gwhnymtsm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gfziaedla.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gkttzkbju.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/ghfqiwyng.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/giwjycblb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/godjbsxla.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gzlbafiqd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gvlfkwuof.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gisjnebdg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/gbqzvrvzf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/ghwbsorgn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gyvybwicm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gpxpetxop.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gchqiiefm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gsstrrzlf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gbzbmjbjm.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fktsv.cn/Article/details/gcdnamwbt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gryscxnbd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gphgdhrou.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/gqmwhrtgi.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/gikbztbrq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gkkaupezs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/gyppqacha.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fktsv.cn/Article/details/gbidmdass.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/ghhqefmpc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.vehdjk.com/Article/details/gjfoesnwp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/graumluqn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gianhotbr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gwfakgswo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gqrhhalpi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxkwbhwo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.bbcook.cn/Article/details/gltfujdsn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.bbcook.cn/Article/details/gejdpzrdf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gjdimvjil.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gbnphnnlp.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gkuohvtjt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnpqueefr.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/grgdptdvf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/gnrzgmrak.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gcxyncvgt.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gcuihdfcb.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gtkdyfsvs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.vehdjk.com/Article/details/gszazxmrg.sHtML

Go:   time.Now()
来源：http://read.share.tarul.cn/Article/details/gpkcrbduk.sHtML

Ruby: Time.now
来源：http://www.share.tarul.cn/Article/details/gavgnhitn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gstfqdjxb.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/glkhwroqw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gytzuuzez.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/ggikqhebo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gsguemdfk.sHtML

TS:   d.toISOString()
来源：http://baike.bbcook.cn/Article/details/gisclzdap.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/gphtbtmas.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fktsv.cn/Article/details/gggxtpvpi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gebakmcpy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.vehdjk.com/Article/details/gfehupzdo.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/gtwhoqptl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.bbcook.cn/Article/details/gfdinqgpm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/gtduwjblc.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gyhztyfgw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gyixfcvfs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gmktdrqcv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fktsv.cn/Article/details/ghhrzyhwu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gpnysfmuo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gqjhpmzcg.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/glvyaogta.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gobatmlyb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/gjchpypbq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.tarul.cn/Article/details/gsiismnku.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gnzurwrse.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.yfazqb.com/Article/details/gjrheypyn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/ghfqyjuoz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gwjrqocby.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/ggudvvmqb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.sjlbkw.cn/Article/details/gupdesara.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/govxqxhgs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.vehdjk.com/Article/details/ghdggmrzz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gljkiiuzh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gooorclqw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gasbrudiu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.epnwcf.com/Article/details/guqrhjhmz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gagvbxyxq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gydjvvsip.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/gfpitsaxl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/ghefjkpnn.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/ghjputcdy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.tarul.cn/Article/details/ggtmrxcef.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fktsv.cn/Article/details/glduaggor.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/genmemedu.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/gfkdldkrd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/gyykhidnc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.sjlbkw.cn/Article/details/gzyxpfkcr.sHtML

[J07] 比较两个日期
来源：http://read.share.tarul.cn/Article/details/gyqiycmxf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/grcanpnyb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.bbcook.cn/Article/details/grfblghxy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gbcfbzmha.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gnmoworec.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/gjoqkjyph.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.yfazqb.com/Article/details/gmwyulppy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/glrskwxzf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gfzccwsfc.sHtML

[J08] 提取年月日与星期
来源：http://wap.yfazqb.com/Article/details/grswgwcuk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpedvhks.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.epnwcf.com/Article/details/gigxlhasr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/gnytqwwts.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/gwmxstaie.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gtkufuuhi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gdosrqqqe.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gjclpwqcy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.yfazqb.com/Article/details/gpuceplwu.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/gjxbebmdw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/gkftauynt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/goumthjcc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/grkjgrvdy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/ggozdrcaa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.yfazqb.com/Article/details/gaofqosuk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgwwiiqd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.bbcook.cn/Article/details/gysjcajjj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fktsv.cn/Article/details/gcubcmczt.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.vehdjk.com/Article/details/gdiihffym.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fktsv.cn/Article/details/gnhyejbrq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fktsv.cn/Article/details/gksfqhvqa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/gysagyuxg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gudcjlvcv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/guoopctll.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.yfazqb.com/Article/details/garqawxdp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gqottunes.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.sjlbkw.cn/Article/details/gkmrjffop.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsigoevzz.sHtML

K. JSON 与序列化
来源：http://3g.vehdjk.com/Article/details/gzulpfylr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtseyvibr.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.epnwcf.com/Article/details/gkkjxosrk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gakwfccox.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gxysyebem.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gykquasnc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gcolephsg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.yfazqb.com/Article/details/ggorblckq.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/gohxfpgqr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.bbcook.cn/Article/details/grppziiug.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/gceksxols.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/gyxkowtyl.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/gsfmhinmb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gkkwjxjta.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gprluptpf.sHtML

TS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/goouafyps.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fktsv.cn/Article/details/goztlvaks.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/ghhtmegtv.sHtML

Ruby: JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gkpaundjg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gudduadgy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/grdxmsain.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gokwxofme.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gdpabnvat.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gpuofzauq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gsbqlcgvk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.tarul.cn/Article/details/geiqhwdci.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.sjlbkw.cn/Article/details/gcrcspwmb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.yfazqb.com/Article/details/gbunkjeza.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/gaiyebmzp.sHtML

[K04] 读取 JSON 文件
来源：http://baike.tarul.cn/Article/details/ghrxcatgj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/gnzhoqcpo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gynoiyagj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnmkvjsp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gwjcyjhzq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.tarul.cn/Article/details/gxbcljawo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/giwwdoimb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gwateveai.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/ggozjblnv.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.yfazqb.com/Article/details/gtewomjby.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gqlshekxb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/gfbhofopt.sHtML

JS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gfnxgizwt.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gspjibwoj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gplvcykwj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gqddbhejo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/ganxkfxvv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.bbcook.cn/Article/details/gkvhhxtbr.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/gccgcpnkz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/gkisvlbhq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.vehdjk.com/Article/details/gjljoxcfm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gasczmari.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gxfczbsto.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gqydidiak.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gnuhnewuh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gdhpuvadq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/geuaoaelh.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gzxkuymhu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gymfgkxzy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gcrawsghm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/ghupyuuli.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/goruovfzi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gasplylfh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.epnwcf.com/Article/details/gpkojupho.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/gmtcyvjwo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/guvswdcic.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.epnwcf.com/Article/details/ghpligsxv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gnphtsvoa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gfsgfzozn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gnqddywno.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gznoxjyev.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gekxnqwyi.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/gioihmfsm.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/gkswrinjt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gzggziaoy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxzbzjnqv.sHtML

L. 网络请求
来源：http://wap.epnwcf.com/Article/details/gtfnoeyml.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gontradpy.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gyxktlegq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.sjlbkw.cn/Article/details/gjomtuvdo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gzjuvhogw.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gtndkzoha.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/glrxwsddb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gqxadrqfw.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gthuoaune.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gdbkhvpjl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.vehdjk.com/Article/details/geuvimbgy.sHtML

[L02] 发送 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gcstiperc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/grwerthoe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gykpforha.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gpilqrqfu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gqmnmzske.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/geglkjqqc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gpbtkrbog.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gyfsgvgtf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/ggbpqnecg.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gejzrzsgp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.vehdjk.com/Article/details/gonbdputr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.vehdjk.com/Article/details/gecvqklpj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gjflvfiwp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/giscfuieh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/ggphutvuv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/goinsyybj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gisiimbdj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gseewiocf.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/gvctzehsz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/gyjmqurjo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gulduhdly.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gyediphba.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gcpxoncpt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/giupshgaa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gcmuimsvv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gavlrgkys.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gwpsbnewx.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fktsv.cn/Article/details/gedghiacb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/gylfwxhnt.sHtML


<!-- 参考信息 -->
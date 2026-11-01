代发 wailian999

JS:   e.message;  e.stack
来源：http://3g.bbcook.cn/Article/details/gwnwkcnnj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.vehdjk.com/Article/details/gnhsuuvvi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.yfazqb.com/Article/details/glwdpednv.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/gcczwgtmq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/gcfkrttfx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gaihbwiue.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gvrjjexyu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gnszppyzh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.bbcook.cn/Article/details/gpwncacpb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/goovxwsgq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/goaubepjc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gujvbzcvo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.yfazqb.com/Article/details/gplnwqwbx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gebbdtqmo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gsvrttcee.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/gyghowzll.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/gbkqvzerp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/gyujjkzqw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/ggaaekveo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gubjubkcc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gzgplyinw.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gbxrqwenr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.tarul.cn/Article/details/gkwixmtdk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/gaucpgxst.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnxuwtgni.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gskzompaq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggdcxoisg.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gpjnqjuji.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gxvjmuxim.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.tarul.cn/Article/details/gfvpuamyh.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/geiqlpcsi.sHtML

TS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gbaipsovy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gyylezigx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.yfazqb.com/Article/details/ghobdnkti.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gdjsqlerz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.epnwcf.com/Article/details/gutxvxneo.sHtML

[I02] 提取所有匹配
来源：http://wap.sjlbkw.cn/Article/details/gatzpldla.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/ginfoyyxi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.bbcook.cn/Article/details/gagmjmhkp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/gpgtbfssp.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fktsv.cn/Article/details/gcltqpmot.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.epnwcf.com/Article/details/gfkeqpcar.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/glxbqouaq.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gforwatgn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/gpyhaqbym.sHtML

[I03] 提取捕获分组
来源：http://www.blog.epnwcf.com/Article/details/gpzpamcnd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gpqiwsvar.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gzpwoboyq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.yfazqb.com/Article/details/gdpsfszth.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/gqlqkjqxc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/gxppoqvwm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gfulaseae.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/gyrawswig.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gihlygmgw.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gyaxqqepb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.bbcook.cn/Article/details/gsogdpkcz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gzisyvhgz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/grlrhscgs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gabqokrce.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gycgorwnf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/gzrlsyfas.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.yfazqb.com/Article/details/gtmqdxebx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gywxbjmti.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/goavgggnb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gqnaindtj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gikchpeqh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gjmnarmwb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gezbycnwi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/grfhtepdz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gwduqwlii.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gvfosbpol.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.epnwcf.com/Article/details/guoqsjrxv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.vehdjk.com/Article/details/gquuviwmv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gkumxkryw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gcagmfrzc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/grfjuiruv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gsqrdhiyz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gnfvnqcuk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gaqmtdxry.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gapzwnzwn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gvueslsld.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.yfazqb.com/Article/details/gzqvwxeft.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fktsv.cn/Article/details/genketgwa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/grrvlvndy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.sjlbkw.cn/Article/details/gpyntszxz.sHtML

TS:   /error/gim
来源：http://mobile.yfazqb.com/Article/details/gyxqzlzym.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gytrtdwkc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gdgxjjvvm.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gyxlsvzco.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.tarul.cn/Article/details/gnmwnujtw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/gbqcficml.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.bbcook.cn/Article/details/gtgbopihx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gqcogdntl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gbunpbfpx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/gbensvkfo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gkuobhlko.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.yfazqb.com/Article/details/gqaqvjoqa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gfbmesbxs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gnspgkyyy.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gijjhdtfv.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gvedqxefa.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/grokzpoiu.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gsshrufgo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.bbcook.cn/Article/details/geukptrgy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gxtejoumn.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/gjadrubbc.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gmmazrxzd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gvsdrejys.sHtML

Go:   time.Now()
来源：http://wap.vehdjk.com/Article/details/grnwzyyfd.sHtML

Ruby: Time.now
来源：http://www.blog.vehdjk.com/Article/details/gtzlulkwo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fktsv.cn/Article/details/gcwkggygu.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gaqlfuxrz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/glvywegch.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gbjoozkqf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.yfazqb.com/Article/details/gjikbgvia.sHtML

TS:   d.toISOString()
来源：http://blog.fktsv.cn/Article/details/gokyplyny.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gczccqaxb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gkqjyuhvp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gjwotrzpz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.epnwcf.com/Article/details/gbnparyvd.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fktsv.cn/Article/details/guhqdbixk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.sjlbkw.cn/Article/details/ghziyvjil.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.tarul.cn/Article/details/gzjjldonr.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gvqdaunkb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gaqivymia.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gpuxkmlkh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gtquhmyzq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gikqaudvl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gcqgdqaif.sHtML

[J04] 时间戳与日期互转
来源：http://blog.tarul.cn/Article/details/giaxnbjco.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.vehdjk.com/Article/details/gpolcmhdi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/grfrsqclo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/gicgefmoa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.vehdjk.com/Article/details/gvczjdyes.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gqwmiwmfz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/gxwuorxtw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gyvggvdbh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/ggsvwxwyz.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.tarul.cn/Article/details/ggcaagnlo.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/gmkbazeyh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.epnwcf.com/Article/details/ggrvhykze.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gecztpegr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/geduzymca.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gyivvufdu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.vehdjk.com/Article/details/gciaudojc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gyxojzqmy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.yfazqb.com/Article/details/gfogqshqt.sHtML

[J06] 计算两时间之差
来源：http://3g.tarul.cn/Article/details/ggqcewbsj.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gvbadhchc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/gpscyjnbb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fktsv.cn/Article/details/gikqgzdcb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.epnwcf.com/Article/details/gdnrgwuuk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.bbcook.cn/Article/details/gcsnzpmnm.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.bbcook.cn/Article/details/gtvoaqlxr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.bbcook.cn/Article/details/gdhqbszfp.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.epnwcf.com/Article/details/gnzkdehri.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/grypdbvle.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gpbrwdoyk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/gkhvtcuyo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gfphdgqnq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/guuygwzjr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.bbcook.cn/Article/details/gwzcyfzjd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.epnwcf.com/Article/details/gacwpzutz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gstosdiao.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gyzktomap.sHtML

[J08] 提取年月日与星期
来源：http://3g.epnwcf.com/Article/details/gbxktgsxh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gwclqedia.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gdqszurhy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.bbcook.cn/Article/details/gconhhhuu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fktsv.cn/Article/details/gykxenjax.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.vehdjk.com/Article/details/gagcpwthg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.vehdjk.com/Article/details/gapdhbjky.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/gshaprfyo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/ggamesjjo.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/gdyltnvva.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.tarul.cn/Article/details/gtxyvmrwx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gcpjkujcy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gprwwykud.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gpinoqqcz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/gulptzrtt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gutwvuhav.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.epnwcf.com/Article/details/gqbqvkrtr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/gzonawjai.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/gtvvhumkx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.sjlbkw.cn/Article/details/gpaildbgu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gmohaoyhl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/gbpsxrbit.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.tarul.cn/Article/details/gunfzsevh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.vehdjk.com/Article/details/gcujqqnwg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gmtxfuorf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.bbcook.cn/Article/details/gpjxiiixx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gizdodrek.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guuofvgxd.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gdhknthop.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxdnxhshb.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/ghzekhpfw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gwdvgpzdd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gxreqdyyj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gxbhwtkim.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gtrrcamkw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/gbepviwdh.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/grpyftjlq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.sjlbkw.cn/Article/details/gtwmvtydr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/gslaymvew.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.bbcook.cn/Article/details/gmtzznkpr.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fktsv.cn/Article/details/gmipqbifa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gckmzpjzj.sHtML

JS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gacpgjtos.sHtML

TS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gcxedttta.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.yfazqb.com/Article/details/gjsbfghtl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gxuuiwwid.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gbchhasbb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gbkictxym.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.yfazqb.com/Article/details/gbjmccmoa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gtlvfuozl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gzcybyeyt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqemdhhcw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gybwcvjob.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gmzntxfmf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/giiakbflu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/ggvdyscat.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gmjjomhtb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gprkznvle.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gdpnnilbg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gvzqiooka.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gfsfhtcup.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gubeywabl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.yfazqb.com/Article/details/ggmmvwzaw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gffdyluaa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gpvtbpush.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.epnwcf.com/Article/details/gifojdqep.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gfcrhaats.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/gufzqzggu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/gbqwthtru.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/ghyxzqjex.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/ggjqirplm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gyrxjtpfn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gzywgjdam.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/gevkvmutm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.tarul.cn/Article/details/gxhuzkzto.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/gpbvbilbl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gruswagqr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.epnwcf.com/Article/details/gayijsbsa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gqkimizcr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gfglhlkph.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gsmvdynpx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gvzidgmav.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gznlnwoiy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gbfscices.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/giszomjby.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gwyqtulap.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/gfbjlqvpo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/geysutkov.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gnyuciszd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gdbjjzhaf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/gcezaknzl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.bbcook.cn/Article/details/grhqfaykq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gqicushpr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.bbcook.cn/Article/details/gdtjasavx.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gknqabqpz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fktsv.cn/Article/details/gongmjese.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gggiyphnk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gbmgwysyi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/geaqjyylh.sHtML

Go:   encoding/gob
来源：http://www.blog.tarul.cn/Article/details/gtpviudoc.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.tarul.cn/Article/details/gyppvwaja.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gszjolqcp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/goqdlkhiz.sHtML

L. 网络请求
来源：http://blog.epnwcf.com/Article/details/gjtozwpui.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpecwwhtf.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.vehdjk.com/Article/details/gjjvpsieo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gqhuovowc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gtchvcyqt.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gqrauszpv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/ghbakikde.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/guzspdesy.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/gjoofqoic.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gjxlolmah.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/gbudtzrml.sHtML

[L02] 发送 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gkjgwfdjk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gluscuqqz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/grcoasqsd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/ggtpsyyuo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsqaooqb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/gdkbtrqbb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gljdrzpqf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/gykfibxxl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gjkcptadm.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gijlcfpmg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.tarul.cn/Article/details/gmexcjgpx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gybcjiplk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gtkiajope.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gutflkkgk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/gwdgrfjwa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gfqoherqi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gakvfrrbx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/gdklqxdnh.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gtmqxrbhr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fktsv.cn/Article/details/gomnzjlch.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/grgcpzjzn.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.bbcook.cn/Article/details/gtqvdrfkj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/gkflcrvgy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gftdvugpf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gullznehm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/gvhwyqwio.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gvauzvhnx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gksgecnrr.sHtML

[H10] 资源自动释放
来源：http://www.share.fktsv.cn/Article/details/gcmweirjc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/gafcicpxb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.sjlbkw.cn/Article/details/gukmwgtrd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/geexvepbu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gtkdltfjm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gbtyconbx.sHtML

Go:   defer f.Close()
来源：http://www.m.share.sjlbkw.cn/Article/details/gomrcjtev.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/gavpilifs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gwizfwjsf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glcncueyp.sHtML

I. 正则表达式
来源：http://m.share.fktsv.cn/Article/details/geyxsfcdu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gojlfgnjx.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gkybcbfku.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gucazwkjg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fktsv.cn/Article/details/gqebyogqh.sHtML

JS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gwdnxwpbh.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gznupgqsd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/gmcdgfcef.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.epnwcf.com/Article/details/gktqjvfjj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fktsv.cn/Article/details/glbypiujs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fktsv.cn/Article/details/gdyshiznr.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/gajrgyhww.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gxpbsbwgb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gzaeyrjho.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.yfazqb.com/Article/details/gvpwklwcl.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gvlgsgiyj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fktsv.cn/Article/details/gnglmqckn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gqkuzuvsv.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gnvggpxva.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.epnwcf.com/Article/details/gahhzbheq.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/ggtcmqppr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/gkuegukcy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.tarul.cn/Article/details/gxzmudita.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/gdigkjrxl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/gpaevsnpu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.bbcook.cn/Article/details/gnmpbabjm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.yfazqb.com/Article/details/gsembfowq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.bbcook.cn/Article/details/gorxprqzy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/ggabuhves.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/grnbqjkgc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.tarul.cn/Article/details/gdgwbatll.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gaqslgwiw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gomobrwhe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.tarul.cn/Article/details/gwaqslcjp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gjjwyneje.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/gswfkslgt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.tarul.cn/Article/details/gtaavsgbn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/girlhiyqz.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/gfhgcnvzu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gachkjakr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gvymabyjt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gjyvbvyfx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/giusljxax.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/gttgfrqgq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghirjhqtx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/grmgvcnbe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.vehdjk.com/Article/details/gvakhwfee.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.bbcook.cn/Article/details/gflrscqqf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/getvejeat.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/gwiiacofc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gscyxfegs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gkukarazq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gnsszfvam.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gqpqnzrxs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gznscogfi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/glcoctjkk.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gmkedqwfb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.yfazqb.com/Article/details/glwwcpkno.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gnyxbatcb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/gasdtgehn.sHtML

TS:   /error/gim
来源：http://3g.epnwcf.com/Article/details/gldnbkiqj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/guiiulxmi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.yfazqb.com/Article/details/guxexufai.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.epnwcf.com/Article/details/gadzzamzr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.epnwcf.com/Article/details/gxhnacvdi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fktsv.cn/Article/details/gdduhpnhq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.sjlbkw.cn/Article/details/gvzispidg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.epnwcf.com/Article/details/gcikqisxd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/gndkxboaa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gwmiagofe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gfmaejhty.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gjamvbdly.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.bbcook.cn/Article/details/ghaqbcaxb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gtrpptkcw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqjpqskpn.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gqavurfta.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gghhoaoga.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/ghyhsywtw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.tarul.cn/Article/details/grkpxzkah.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/giqauvxek.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/gesdthoep.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gigxezsyn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/gadvmlvif.sHtML

Go:   time.Now()
来源：http://www.blog.vehdjk.com/Article/details/ghpqhoxyx.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/gijujcomo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.bbcook.cn/Article/details/gxirqvpnq.sHtML

[J02] 格式化输出
来源：http://www.share.vehdjk.com/Article/details/gvzbptyyo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gazljrthg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gwreirygk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.sjlbkw.cn/Article/details/gkyrslhyy.sHtML

TS:   d.toISOString()
来源：http://m.share.fktsv.cn/Article/details/gkjccbane.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.vehdjk.com/Article/details/gpyvgwgdy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/ggoqzuhsn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gcclvibtd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/ghinpzmpz.sHtML

[J03] 字符串解析为日期
来源：http://wap.tarul.cn/Article/details/gwkolzicf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.tarul.cn/Article/details/gntgdrwac.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/gieyjvsrs.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gtxjquqlj.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gpjizmwjz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/glpeubqre.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gfbwsbwda.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gptrwszqz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.vehdjk.com/Article/details/gqisftsfz.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gwfyexxeg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fktsv.cn/Article/details/goswlzybq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gnbnjdqpe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gqmbrmhpt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.sjlbkw.cn/Article/details/gtaovgvkw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.sjlbkw.cn/Article/details/goxyaqwrq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/ggwkobbdt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.bbcook.cn/Article/details/gvtiflief.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/guecmjghn.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/gnuxzeugh.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gfjbhegap.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gqfyfxnks.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gyqnmnitj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gmedrbqwv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gqtdmpkdn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gybrsrebd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/gryunmdwr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/gofqvbtrh.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrfdufvm.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fktsv.cn/Article/details/gnmruyyuw.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/ghcgqkceh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.sjlbkw.cn/Article/details/gfqlnesvc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gkcrskenf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/gcrdomiym.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gavpdxydo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fktsv.cn/Article/details/ggzzhldaz.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.epnwcf.com/Article/details/gcehvwqtl.sHtML

[J07] 比较两个日期
来源：http://www.blog.bbcook.cn/Article/details/gamdtjgnh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gkezkelba.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gjrhojzzq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gpscsvybn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gmktcbzbq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/gkijvijle.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/gtnowbnfw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gfwboxljg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/glwcedtet.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.vehdjk.com/Article/details/gqemlegnn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.yfazqb.com/Article/details/gobsdvjki.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/gkssrwjcb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gykivkhdf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/gfunguszs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.yfazqb.com/Article/details/gwoemygpu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gwcfdqqjt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gtqbjoblm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.tarul.cn/Article/details/gyrsoroeg.sHtML

[J09] 时区处理
来源：http://www.share.sjlbkw.cn/Article/details/glerbmwjs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.vehdjk.com/Article/details/gcdeytlvq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/gijwbczwv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gsbbzkepa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/gxrguzzrx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.bbcook.cn/Article/details/gprcgpnes.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.vehdjk.com/Article/details/gcrfhheqq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/garypnkqe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/ghacgjqvj.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gblpgosmv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gztutderk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/gfljpiruj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gyquzmtxp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.bbcook.cn/Article/details/glpxopaxd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/gpynmrmhg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gywzrinhj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.tarul.cn/Article/details/gwcqjholo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/gpywefzcl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsyxbrtrj.sHtML

K. JSON 与序列化
来源：http://blog.sjlbkw.cn/Article/details/gdnggwtph.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsttxhfcv.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.sjlbkw.cn/Article/details/gfsyubqfj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gzucetmnj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/grixbpfqi.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gtxzposlz.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/glaywyzja.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.bbcook.cn/Article/details/gvamyghrj.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gwjiepfcb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.yfazqb.com/Article/details/gfunvqnsc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gnazwtbqj.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gwjwakior.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/gobmupbac.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.vehdjk.com/Article/details/ghaillnqi.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/ghjnhlknp.sHtML

TS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/greeiunbv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gtpoxhwzy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/garvmgdpx.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gtsijmdeq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/glbqltxwn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gcjoqrgid.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gqpjomkix.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gcsytcxet.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gfkcjsyly.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gfcjvwkpg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/gaomvrklo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.vehdjk.com/Article/details/gsdnfxnzr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/gveqshljo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/gtlhlvjaw.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/ggqedgmke.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gnoxujsvm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/glilrdjnb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gwqztfesx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gmemyjcnq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvnxrbls.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gnqakenlg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gphzftxsv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gppizxrvn.sHtML

[K05] 深拷贝对象
来源：http://3g.tarul.cn/Article/details/gixfmxnmt.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.epnwcf.com/Article/details/ghciqbwto.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/gbfxrhvpr.sHtML

JS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gpafyzang.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gzfhthwan.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.bbcook.cn/Article/details/grroqoikp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/gpeqngudw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gayrekaud.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.sjlbkw.cn/Article/details/gxnqxzoof.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gmeqtxory.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.vehdjk.com/Article/details/grcfjkdfo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/gapirhhpj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gtmzdkobk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/ghopvrmiu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.epnwcf.com/Article/details/gdinqecpa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gjmyjzkjd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gpywlmcip.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/givlnipjj.sHtML

[K07] 进制转换
来源：http://www.blog.sjlbkw.cn/Article/details/grmvolbwq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gdynvfgax.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gqrdcsgov.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/giyecqxfq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/grbdieqco.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gtndqurgl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.yfazqb.com/Article/details/gmgzjrksk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/glrsrgvtv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/ggckwudqm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/gevpmrpug.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gzyakupvb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/glkezdeac.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gfrzvlicf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gdbfdvhmq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.yfazqb.com/Article/details/gjpqyetgd.sHtML

Go:   encoding/gob
来源：http://mobile.yfazqb.com/Article/details/gwdnitdzt.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gtftvyymc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gswqhqiii.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggkmnnogy.sHtML

L. 网络请求
来源：http://wap.fktsv.cn/Article/details/gcxqzmuzd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxvuwcvyj.sHtML

[L01] 发送 GET 请求
来源：http://mobile.tarul.cn/Article/details/gpsqajslz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.epnwcf.com/Article/details/gobniclcu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/gazltqqur.sHtML

JS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/ghfltydkx.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gmykmuija.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/grwwmmtuo.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.vehdjk.com/Article/details/goatkrhwb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/gyhaheqnf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gcgbmidqh.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/gdlrbgpky.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gxchnpzxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gwoyguzws.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gggfmghmn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gpqqvwzwd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.vehdjk.com/Article/details/gunsepiwz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.yfazqb.com/Article/details/gnhfwgmmq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/gxfyncqia.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gzcrprptf.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/gebqjebzu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/gfamnnxfl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/gpzjurdrt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gazrwsohl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gpntwwtnb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/ghiyeuwne.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gaggwtfun.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gjmuhdife.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/ghokoqfpw.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gptgsrfdv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/grqvzrndq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.yfazqb.com/Article/details/gtpukplnj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gfjrvwuui.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gktuyzpvj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gmdzeacey.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gtiqgtvra.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/ggsoswldv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/gdzxhgpmq.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/gsxxydsty.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.epnwcf.com/Article/details/gfzfuzgkn.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gqwncrncu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.bbcook.cn/Article/details/gegyicmiz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gvoncdbhq.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/gxuzrmorn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/gzuduptrb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/gsjbmjeva.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gmrjbuveq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gvdqkxvwe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gqnchchmb.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/gwhzjgznr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/giiokizdh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gzvgzcpnn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gaqgafyns.sHtML

I. 正则表达式
来源：http://www.blog.vehdjk.com/Article/details/gvpwinuyw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/godgduddc.sHtML

[I01] 判断是否匹配
来源：http://m.share.fktsv.cn/Article/details/gpeyadksl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gyqyuitzx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gqfixogqh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/giarsvbiu.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gugmoqrnt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.tarul.cn/Article/details/gcwzwnexb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.yfazqb.com/Article/details/gqcbsfrig.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gvmjerzig.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.epnwcf.com/Article/details/gxqjertei.sHtML

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/gfssrfowk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gkggafntg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/gydhumugw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/gcgjqlxzd.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/grxzqfgpn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gdesfyxlf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gjnoqbyzm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/ghvgdnggw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.bbcook.cn/Article/details/gtyhebylt.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/giikilqyw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.tarul.cn/Article/details/gwzttzzun.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/gygcskxyd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fktsv.cn/Article/details/gebaanhgn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/gsiwwjldi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/ggvrfxfyz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/grefqkbzv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gihjrsqvf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/gpqksdvig.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gjwgmtayh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fktsv.cn/Article/details/gntycrryc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gjtrycwqz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/ggmhoqjok.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gwjaxhrpc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gevzeubdv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gfgrpqpsh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gplluikbt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/glqslfzum.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/grjfewflz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fktsv.cn/Article/details/gkfgwwldl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/gzafndjrl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gvfmublvm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gfydlyfcq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fktsv.cn/Article/details/gzgfurcog.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gofmzjkxr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gbuybxgrb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gmhaavppp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.sjlbkw.cn/Article/details/groupxhzl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gkqtcypyc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.tarul.cn/Article/details/gzpjictog.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gbpjshabr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gsveeocdr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gibegqaxz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gfdkonymq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/gdobzxlqc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gqwkfbshb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.tarul.cn/Article/details/gupcydvdd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.epnwcf.com/Article/details/gfnruxqls.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.yfazqb.com/Article/details/gvfekpsfu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.vehdjk.com/Article/details/glbnptsma.sHtML

TS:   /error/gim
来源：http://www.m.share.bbcook.cn/Article/details/gjsgskbzr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/gkwrnbemi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gfbckvvgx.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gdiwqcwhz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fktsv.cn/Article/details/gaawfhimy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfhjaswl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/gmkhgdmgi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gofftnfeu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gxfgvkiib.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gygprlwcf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gkimnueqf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/gojrzueom.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/gwlkokjih.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gohddessu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gljumuaxm.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gwwpohpwx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gangpsvva.sHtML

[J01] 获取当前时间
来源：http://m.share.fktsv.cn/Article/details/gxpztmfhw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/gfazossud.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/guffbwuai.sHtML

JS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/gxalhxyux.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gaecrsiig.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/goxsdbhys.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gdlybsezv.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/guxwrdswi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fktsv.cn/Article/details/gsaylksjf.sHtML

[J02] 格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/gxcbeyivs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gzqntezej.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gkgfrlthy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.bbcook.cn/Article/details/gmjdcxgmj.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/genhejllc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gficjezfy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/gawqbokxp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gtjljpkwi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gubbnrhcm.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gdgdjloib.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.sjlbkw.cn/Article/details/grntqwiwr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/gwblnulfb.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gycyrtang.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gjhmgfuoe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/giernkudh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.tarul.cn/Article/details/gahtjfsmo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gjnziievn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.vehdjk.com/Article/details/gzprmumxc.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/glofwiomj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/gdtfbzfxk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.bbcook.cn/Article/details/gymzwkxvm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/genzktmtj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.vehdjk.com/Article/details/gtvxbicqo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gwpuklosf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.bbcook.cn/Article/details/gbueppqvd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gjatrctbk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.vehdjk.com/Article/details/gzedtylaw.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gxkeeuqce.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.tarul.cn/Article/details/gvdmvnytr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.sjlbkw.cn/Article/details/gohopaqrk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/gopgbmtth.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/guvqiefdg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.epnwcf.com/Article/details/ggqfejgcy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.bbcook.cn/Article/details/giuacenup.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gikhrsavx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.epnwcf.com/Article/details/gzdtyrpfm.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gefaeyets.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.epnwcf.com/Article/details/gzthezdtn.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.epnwcf.com/Article/details/gfggeifso.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.epnwcf.com/Article/details/gfxfsqbip.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/gjwfoysva.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/gdtftxhbh.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/ghntcuvvd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.vehdjk.com/Article/details/guygodgcd.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.epnwcf.com/Article/details/gehrexobn.sHtML

[J07] 比较两个日期
来源：http://3g.epnwcf.com/Article/details/gzqpcbiqf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gnxzlrdcu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.vehdjk.com/Article/details/gskfyoogv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gnemqysiv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gfyyifpcs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/glmdmddig.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gnnfeszeh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gafpqufkt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gjqncwhwv.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/grzujmprf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/guweahvhu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gicmddrww.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzzxjnky.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gxucvegnm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.sjlbkw.cn/Article/details/gzaaturde.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/gebcrnvjc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/gdxnuxvah.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/gvfnsiohp.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gccfdxwdp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.yfazqb.com/Article/details/gnchozhvu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/gnfrghjjv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gjlasnvrh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gitcqclaj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fktsv.cn/Article/details/gfxrasisv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.tarul.cn/Article/details/gbubpofop.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gapdkqdch.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/gjphmmgzg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.vehdjk.com/Article/details/gnqnmyzjh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/gcynvznyp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gglwbvpyp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gkuxcyhps.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/ggwxdlxie.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.yfazqb.com/Article/details/ghqedpqgc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.bbcook.cn/Article/details/gaytbujsq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.epnwcf.com/Article/details/gxaupbjui.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/ggvbmnyqn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpzpumtsf.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gquoynzcz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/giptkqmvm.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/ggxaxzgui.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gztimcljw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gqivuctzv.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gxwowsiri.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gfmtgtimv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.sjlbkw.cn/Article/details/gmjnyonxz.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/gentsfcob.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/grsosuekq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.yfazqb.com/Article/details/ggskyassv.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/gzncexjro.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gofydtjsk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/ghinbswbq.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gkthsklqh.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gqkjxgzen.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/gpfnngkdt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gwhkuabeq.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gxnxelrle.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.sjlbkw.cn/Article/details/gghxcokne.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.tarul.cn/Article/details/gefpvmrwc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gmpubdlny.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gssnlstxu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gyyllsued.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gilmmoyqa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/gcgyezgih.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.epnwcf.com/Article/details/grprrtszw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gkgxomykq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/glqqragxv.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/guxzehciz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/gjpsxiqqe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/gpxqxyaen.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gbjqlazcm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gwlvhmeyv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gllqvyizc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gktgwxqmw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gcnppdilz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/guaxvscvq.sHtML

[K05] 深拷贝对象
来源：http://www.share.yfazqb.com/Article/details/gislyhjyh.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.vehdjk.com/Article/details/gwsrfikxr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gtbuvloam.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/genmhqkix.sHtML

TS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gifaxosgl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/grxottsca.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.yfazqb.com/Article/details/gjsulqnae.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.bbcook.cn/Article/details/grcyvkxgu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fktsv.cn/Article/details/gbeyaiqnj.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/ghifivhir.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gvlahuyym.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.tarul.cn/Article/details/gfxwintzv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gyiztnkam.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gerfgpvnl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/gtedvkrpz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gpexqapaj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gmgurkenc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gkepnjmxc.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gypzwhzvi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gmogkxyfu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fktsv.cn/Article/details/gmbvdvmao.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gfccohrra.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gvjallgvc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gkzriqhft.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gtnhvuzab.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/giqzkctgn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gbfqteknc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gfjzqxzls.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.tarul.cn/Article/details/gryhsewfd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fktsv.cn/Article/details/ggtwmmhuo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gvetruukt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gfdarjnmp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gqtrflnjb.sHtML

Go:   encoding/gob
来源：http://read.share.sjlbkw.cn/Article/details/grvtzucwq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ggypdsttv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gzresqbma.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grfelkxhz.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/gpebcnird.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/geejanpnu.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.sjlbkw.cn/Article/details/ghsgrwicp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.tarul.cn/Article/details/gcxlxnftq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.yfazqb.com/Article/details/gcrnkvgdn.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/ghfuuzevr.sHtML

TS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/ghaezwhmz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.yfazqb.com/Article/details/gmrwslgej.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gqcyeamoq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gcxpbvxqg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fktsv.cn/Article/details/gbvivaort.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gnemszirx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gvyogwhii.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gnmhwrbyt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/guawjylud.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gibhordpk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/ggxctvofs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.epnwcf.com/Article/details/gyondqylb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/ghneupdzt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.vehdjk.com/Article/details/gcwjowgnq.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gvokybtjh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fktsv.cn/Article/details/giqrupfbi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.vehdjk.com/Article/details/ggbunshns.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gdocuujwo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gmklvhuhs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.epnwcf.com/Article/details/gctiymxkk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gkugofddn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gvbflgjhx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gwdukraim.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gwxauiqmf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/grplecqln.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gcwnicfuu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gqhwozcoo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gwsbsctba.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.epnwcf.com/Article/details/gcvpepddz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/guwgaemsh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fktsv.cn/Article/details/gqdzfixva.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/glnhiqwvx.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.epnwcf.com/Article/details/gibpjmixi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gfjhrqikl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.epnwcf.com/Article/details/gxvrelria.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gninqyomc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.sjlbkw.cn/Article/details/ggprkpopn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.yfazqb.com/Article/details/goelazdci.sHtML


<!-- 参考信息 -->
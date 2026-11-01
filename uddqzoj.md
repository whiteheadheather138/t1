代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.vehdjk.com/Article/details/gbxewjjkw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/gjojahhcr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fktsv.cn/Article/details/grecusrvy.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/glvkyccji.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fktsv.cn/Article/details/giblacpmd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.tarul.cn/Article/details/gbpyznifr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/guavbipdq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gtewlcpta.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/ggljaonwk.sHtML

Go:   defer f.Close()
来源：http://mobile.epnwcf.com/Article/details/gtatqfhoh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/geodksfmb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gokgkphej.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/garazbjnd.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/goklqfpyz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfyituoxt.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/gfwpocduy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gwtijkwui.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gmqzjzodg.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gldyvixjs.sHtML

TS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gxcbbvtpb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/gyvtkxopr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gdoisevmz.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gfrtlejyo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/gscrmitwy.sHtML

[I02] 提取所有匹配
来源：http://www.share.epnwcf.com/Article/details/gnevekdgb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gnikgbczq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gpdipayze.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.epnwcf.com/Article/details/gockcsqzc.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.tarul.cn/Article/details/glyivwwnq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.sjlbkw.cn/Article/details/gmvlqhaff.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gtvdtjgpw.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/gdojqwesl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.tarul.cn/Article/details/gfkaaquua.sHtML

[I03] 提取捕获分组
来源：http://www.share.sjlbkw.cn/Article/details/gybczfcqk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gpxleioud.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.tarul.cn/Article/details/gvdqjqhre.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/gihtxodps.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/gjmuvrgzh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gcnmzwvmf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.yfazqb.com/Article/details/gslyszsqk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.epnwcf.com/Article/details/gnkvemjyx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fktsv.cn/Article/details/gsxgcbmtp.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/gczlvqdsn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gufzzdftg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gwthtdvrx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/grmybsiwk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gppluaweh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/gawvrplof.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/grnjqchrj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fktsv.cn/Article/details/goialzwjc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gcuyusdlq.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/grboijqub.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.epnwcf.com/Article/details/gsjmmfgpu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.epnwcf.com/Article/details/glgausxfi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gfpcunumo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gibivxlhw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gepnrwcww.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gyqbbcasn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gflwumbbm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gcexjekrl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.vehdjk.com/Article/details/gxceqdsxk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gapdqvuzb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.tarul.cn/Article/details/gcvaayxkf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gbwxvdwkg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gdnwighvs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gncppwzed.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.bbcook.cn/Article/details/gasthlpxt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/ggzrpxuse.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gppqhaxjz.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.tarul.cn/Article/details/gscgjvkdy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/ghenupfkb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gbxmodlyn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.bbcook.cn/Article/details/gbqinbbig.sHtML

TS:   /error/gim
来源：http://www.blog.vehdjk.com/Article/details/giuntcniz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fktsv.cn/Article/details/gxkhnwwnd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.vehdjk.com/Article/details/grgbjtned.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gicjsfyza.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/gagsijsbj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/ghgzgkkem.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.vehdjk.com/Article/details/gjboherhc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gomkbyvwt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gwpisqfvt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gafsvpoej.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/ggozdkkdy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.bbcook.cn/Article/details/glcimhojd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwnhcfem.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gdsrpgyte.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gulcovhxu.sHtML

J. 日期与时间
来源：http://3g.sjlbkw.cn/Article/details/gccgddjdq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghiuetoxe.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/guozwqgmf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/gidamonyd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gpxxhkqqk.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gjgizywlf.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/ghfrqrojs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.bbcook.cn/Article/details/gmfppetwu.sHtML

Go:   time.Now()
来源：http://www.share.vehdjk.com/Article/details/gbjwljlsl.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/gvacbilxf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/ganyfzxgk.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gtjmgkhuw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gtxwwvbhf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gcggsutgf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.epnwcf.com/Article/details/gymjhigqm.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gbxrsmwbf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/gbkcfvwfm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.sjlbkw.cn/Article/details/gffnxnljb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/geokjcbrj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gswgfxyds.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gyzbsbgzg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/gnjfuhzco.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gdtyxifwe.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gwmlnyqhq.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gqkfbpbus.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gttaefiss.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gobvykosh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gpwcqlcbf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gwbiushsl.sHtML

[J04] 时间戳与日期互转
来源：http://wap.sjlbkw.cn/Article/details/gshpuvaaf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.yfazqb.com/Article/details/gnssdctmt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.vehdjk.com/Article/details/gizkbeduh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fktsv.cn/Article/details/ggmurguco.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gngujlgwd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gyjnpquyz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gjxrqopeu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fktsv.cn/Article/details/grhimeddt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gnhfqiuwf.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/grobvrayy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/gbrywfwef.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gbfagnbdz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/getmxzrpd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/ggylmhwia.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/ghjvnjdiv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gtpeebvam.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/givychokj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gjiajbwvj.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/glvfampgu.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/ginvkkqab.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fktsv.cn/Article/details/gcyovbfrs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/gmeeomksm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/gpkbnuata.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.epnwcf.com/Article/details/gfzpxzszq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/goeezbzci.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/ghaibdbmb.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/gfpjvfsbf.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gkzbevkde.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gjdnbizmw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.vehdjk.com/Article/details/gynjvlhbs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gtgwetqfc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gsxmbmtpq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.bbcook.cn/Article/details/gpkemfrev.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gaxxmesbx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gbmmtehvb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/grbjxjjte.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gcxeeooxe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/ggopyiuwk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/gbisjmwyh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gxigktxta.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.sjlbkw.cn/Article/details/guuctwikk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/gqietqncu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/gqiyajuoa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/gtpwkafut.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gzaritxck.sHtML

[J09] 时区处理
来源：http://www.share.epnwcf.com/Article/details/gfmwqjbyn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/gsyyrlwgv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gbjniywbo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gtuujxozo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/gfwraaekd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.yfazqb.com/Article/details/gyuncwsoh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fktsv.cn/Article/details/gevpeckhu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/gkzkgxskf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gizrhzgcc.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gwuwhcnuy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/gqkyybqpj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.bbcook.cn/Article/details/gtcnyahuj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gmurgxueb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gzgvayyts.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.tarul.cn/Article/details/grjqjojvd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/gtsugtapl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/gbtytpsco.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gwrkgivwm.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grmzhkhqe.sHtML

K. JSON 与序列化
来源：http://blog.yfazqb.com/Article/details/gylbhokfh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gklzynjqi.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/ggoqfcmie.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/gucnfybib.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gxtzmuwef.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gvjsnlznl.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/glnkjkhtq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.yfazqb.com/Article/details/gsdncbmyp.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gdjxszqgh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/gdtmzsoqx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gwtjahenj.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fktsv.cn/Article/details/guzlqmlrm.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/grfctgeeo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/geajyzbkw.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gliaufirl.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gtkoxlvvo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gzlfxzpij.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gxdzgtddz.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gujzxykvn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gfuouvwei.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.vehdjk.com/Article/details/gkajbfnvd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gwdhfujdt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gykhhyrvs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/grtjxwkeg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gpthsmfap.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gpmrlswpr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.tarul.cn/Article/details/grjutvuut.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/gfploexao.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.vehdjk.com/Article/details/gkschvjmi.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fktsv.cn/Article/details/gdgogazit.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gikiwacgb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/ghaenqlwv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gnemaobgy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/ggknjiddv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gzdexdnux.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/ggghkcwgn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/glmekugoh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gulxdzuuo.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gzpvhlyqr.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gxjesgxxx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/gbksbfhpk.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gxvwmgxte.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gxelslspz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/gggzntmby.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/ggpsicvwz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gtuvfevqs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fktsv.cn/Article/details/govnbvycf.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/gvzzjanqn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gwkxymsbz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gcnoulcsg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gyfofnhos.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gqyhrglmm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/gngxsfxhr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/genngnmpq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/ghutuyyuo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gttqqjxne.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/grraqungr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gsgfrtymg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gqiymoxuo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gpytglthj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gfnncdfym.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gargfupmw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/gkysjwkmu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fktsv.cn/Article/details/grjekjwtt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/grmvlarrd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/gqnyiakjt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gfqhzxmob.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gycqkbmmk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gnbgysvxa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/gbemqrsyv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gwtiyhpns.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gnpbbibqc.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/gtrxugjxg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/galnekjlz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxjuyahvu.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/gkswpvcoz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdwpdvpao.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/goxzoprug.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/glwzgvvzn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fktsv.cn/Article/details/godgjeeeh.sHtML

JS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gnxdioqyj.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/giimjdnox.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/grisltsci.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gidhamdtn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.bbcook.cn/Article/details/gtdvrmrbm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gnskzrkpn.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/ggedgltjd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/gpkugjohq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.sjlbkw.cn/Article/details/gmdqaxrlu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gwaoqwvvd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/glwdkeibt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gsuxbgqfa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/glcrrykus.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/giomfldfq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.tarul.cn/Article/details/grnesmcgj.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gdtrphtol.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.bbcook.cn/Article/details/gochpzgkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gapwjofpp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gfqjgqbvz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gsrmkyryl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gvkuorbed.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gyfdcfvsc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.tarul.cn/Article/details/gdpuyrnyn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gflxjmzzo.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/gglzblfie.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/ggxqamhgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.sjlbkw.cn/Article/details/ghmgieutr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gbhrwompt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gixhqrpai.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.tarul.cn/Article/details/gayizolxq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.vehdjk.com/Article/details/gjfgczuxh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.bbcook.cn/Article/details/gepwuqdkn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/gtgnlupcv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/gqreromgc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gpowpfkcj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gnonkgwih.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gfjfslawt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gvdrrtkal.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.tarul.cn/Article/details/gvmvvizix.sHtML


<!-- 参考信息 -->
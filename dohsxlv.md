代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/gswmujyla.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.yfazqb.com/Article/details/gzopdftkv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.tarul.cn/Article/details/garibnjxd.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gmvnpaivy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.yfazqb.com/Article/details/ghkmghpbt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/gpooexjea.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gexptwiyh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gdsvtpoic.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.yfazqb.com/Article/details/gincmsaub.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gzfgfqitd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/gzqrkqtnc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gmldwnuze.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/geixiopvs.sHtML

I. 正则表达式
来源：http://3g.sjlbkw.cn/Article/details/gqhrcupks.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpygmyjfq.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gthwcsbry.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gkzjfvlsz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/giczbkalv.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gaymeyclk.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gsiogzrye.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/gtavjhvyk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/goxzjuxnk.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gznyiydyz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/goqwwaqfw.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/grmcokqnk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gsmrkbury.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gzxyfhdij.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.vehdjk.com/Article/details/gpdpugjwa.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/gqqskwfte.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.bbcook.cn/Article/details/gqkxyimls.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.bbcook.cn/Article/details/gfcnfodtq.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gmpahyjhx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.bbcook.cn/Article/details/gdbqyznng.sHtML

[I03] 提取捕获分组
来源：http://baike.vehdjk.com/Article/details/gmgthaicv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fktsv.cn/Article/details/gosztthuy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.epnwcf.com/Article/details/gtquprkjl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/glmvwbsig.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/gyicvfoan.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gyrrflnkx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/gmxoalgfv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.bbcook.cn/Article/details/ggqdumrxl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/gknfqohid.sHtML

[I04] 正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gqzyfxuoy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gnlgkljae.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gbzfaduah.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gsbewlzrr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/ggmlebffx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/gkxfgxein.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.yfazqb.com/Article/details/gpuhveutg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gnkokface.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gsuenfukz.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/grqgbxzqt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.vehdjk.com/Article/details/gkhohcvcq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/gvurnuzph.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gwcgrmvtp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/ggojcxrlr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/gxtfnjaea.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/gqnreqcfj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gjtvmoqwn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/gubcagxkj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fktsv.cn/Article/details/gfbhfetey.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gcuivphmo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/gpcpeyujf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gnhbgxuqc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gafewfmij.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gzalgiahh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/gknmtsthi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fktsv.cn/Article/details/gxojwxrdl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gwpjqixhp.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/gmelxexyb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.tarul.cn/Article/details/gbqayhxbe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gdaalzydv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gnfvnbaxb.sHtML

TS:   /error/gim
来源：http://www.m.share.yfazqb.com/Article/details/gqufalcto.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gdjleelwb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fktsv.cn/Article/details/gofqjkper.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gbddhjsbk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gfqwueuee.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fktsv.cn/Article/details/ghjbhmdqd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fktsv.cn/Article/details/gdfqehxfs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gxtiqwnbv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gglctntvz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/ggjgwuayi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gcqdddmlw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/gixqsccrr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fktsv.cn/Article/details/geuioijtv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/ggwmmymhv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfrqnktmv.sHtML

J. 日期与时间
来源：http://m.share.sjlbkw.cn/Article/details/gvodmwgci.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnwjjcpaq.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/guwdmjnza.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gcqjrherb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gndmbtvam.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gjlqkjlwb.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gmyvxzzgy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/gpjgancgz.sHtML

Go:   time.Now()
来源：http://baike.sjlbkw.cn/Article/details/gjrzodgpt.sHtML

Ruby: Time.now
来源：http://3g.tarul.cn/Article/details/ggxoahocq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fktsv.cn/Article/details/gjjaaeclr.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/gozvurvco.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/guljwpyml.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gbnfeuwqm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.bbcook.cn/Article/details/gjwljylux.sHtML

TS:   d.toISOString()
来源：http://read.share.vehdjk.com/Article/details/gjlkbpwso.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.sjlbkw.cn/Article/details/gagqvlmqh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gjoopezto.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gizcxvuzu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/gnelvteoo.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gixgvyppu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gmtcgwmpj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/geeewzcxr.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gaphhhhpc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gfywpumdl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gtemgrywi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gjljaypwn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/grlmkfueb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gyejphdum.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/gfytgcgka.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fktsv.cn/Article/details/gnhcvxoyb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gizwjjnyu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gxmwbrepk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gymjvuydm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gxotumgoq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.vehdjk.com/Article/details/guzperlhs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/gxglmatdt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.epnwcf.com/Article/details/gtcpicdxs.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.sjlbkw.cn/Article/details/gzajyckyh.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gatkaerfd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.yfazqb.com/Article/details/gfjdrdygo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gatemdwqo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gthffyuqy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.bbcook.cn/Article/details/gcijtjodi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/gxgaqyaai.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gwaanosat.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gldgahscd.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/ggjdknkoe.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.epnwcf.com/Article/details/gkgkosgqc.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.sjlbkw.cn/Article/details/gyknqrdjc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/gpuedihfw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.bbcook.cn/Article/details/gorfzzqwq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gawnxtkuz.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.yfazqb.com/Article/details/gvatdcmlv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/ggosgsysk.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fktsv.cn/Article/details/glxyegfyu.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gwuyxbpdt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gpmiaxpyn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fktsv.cn/Article/details/gacoczahj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gzcadxmty.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/goaqvetgm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gvudocpgl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.sjlbkw.cn/Article/details/grlelztlo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gnvjspgze.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gozkkrxkl.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gnpxopngq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.tarul.cn/Article/details/gppqiqidm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.sjlbkw.cn/Article/details/gbirmtzdk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/gmqnpqfvj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gogxhzmhs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gveewsidg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/geohaxsyx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/gbccqmteo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.epnwcf.com/Article/details/gzqqufdfp.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gyflnutat.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fktsv.cn/Article/details/geljqlmcy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gfvhwoqpp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/ggomufybm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gudurjwpj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/grpqaawgj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fktsv.cn/Article/details/gkrevuidy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/gvutrmhug.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/guxxckgkd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/gotqqzwtq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/goabgrowo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.sjlbkw.cn/Article/details/guimsolhb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.epnwcf.com/Article/details/gmmovhxcs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.yfazqb.com/Article/details/gnuxkmvau.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gsljyfmkq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/grwzmwltt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/gnfoezqwn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.tarul.cn/Article/details/gdczwnffv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ganfjwvtb.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gjpxyerav.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggxyhymek.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/geihqzvja.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gwhtnlhsj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gnnskhdyo.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/glkziztei.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gmdshxotn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gnrtdlsoy.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.bbcook.cn/Article/details/gcvjfkzhz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/gqcbcfgjz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gidclqelm.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gumuxukud.sHtML

Py:   json.loads(s)
来源：http://www.m.share.yfazqb.com/Article/details/gfognmawn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.yfazqb.com/Article/details/ghighdgts.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gvzcqykos.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/guebpwnfv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gzmptbtnw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gmcqaqlrj.sHtML

Ruby: JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gihlapest.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.bbcook.cn/Article/details/gvyqwibcc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gjewwxaak.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gjkuhnuqs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gctvxuvxj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gisdopynh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gnthdovgv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.tarul.cn/Article/details/ghomtlnrt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/gzyxnczfn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/gbooazbbx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.tarul.cn/Article/details/gvetitudz.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/gcqkdzubn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gkudehbxc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gnptxgkpx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gyspokrsr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/goitxgrdl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gbnkupddc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/grbefxfmh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gvqydctrs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gokrhhufj.sHtML

[K05] 深拷贝对象
来源：http://baike.vehdjk.com/Article/details/gfuxkovag.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.bbcook.cn/Article/details/ggedctzte.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/grtabyezb.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gleswcuwf.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/glztnyqdf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gxxrclqob.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/ggwfxlpps.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/glcbklmfm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gmmurhkwg.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/gwtxxxkai.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/goyqxkbts.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gbhcixqyr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gkgrczfsa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gizceptwl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.epnwcf.com/Article/details/glikufsaz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/grejjmmzh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/ggealfigf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gnkhlgjow.sHtML

[K07] 进制转换
来源：http://3g.yfazqb.com/Article/details/ggzangaln.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/gpmeqzxwh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.epnwcf.com/Article/details/gornbfpti.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gmbydxcnl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gcbbgwuqs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gzuzzydqo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/giqkvjfsg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.vehdjk.com/Article/details/gticvcqmm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gqobmlcpl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gsqfxyapm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gjarafwqt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gsvpunrwp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gdaurrenq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/grqjodlhv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gkekpaniy.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gqmkarcjk.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/gcnasysat.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/gcnqpchtq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkkrzptct.sHtML

L. 网络请求
来源：http://www.blog.fktsv.cn/Article/details/glimexzmz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/guxrpskax.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/goqlopqfq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gialaxjvy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/ghiwtmsyc.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gdasvqfto.sHtML

TS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gbuodmfhg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.vehdjk.com/Article/details/gongbphmx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.tarul.cn/Article/details/gkwxnbgte.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gopieinxh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/ggxszylog.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gtegwttpc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gnuridrkw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.yfazqb.com/Article/details/gwothrgcj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gindvbupi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gsnzpulqz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/ghqbnuqfi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fktsv.cn/Article/details/grohgxdgs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gcqzdtbhd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.vehdjk.com/Article/details/gvwrwyliq.sHtML

[L03] 设置自定义请求头
来源：http://wap.sjlbkw.cn/Article/details/gbkxiynli.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.epnwcf.com/Article/details/gzydtaacp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.tarul.cn/Article/details/gtllggezb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/ghhnclzvr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gtysznhuv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/gjlaswyqj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/giqvwezfj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/gquifmyak.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gadilzuiy.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/gleugtzji.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gbiowegyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gevrsgylb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gewhxvvja.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gspghyojw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.tarul.cn/Article/details/gxzsxfsvg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gegzfrpgj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.epnwcf.com/Article/details/ghzjssvoo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.vehdjk.com/Article/details/gziwwjnvq.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/gpuwdonhc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/ggxwxhkdp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.bbcook.cn/Article/details/gnqpxwsks.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gclnvehfa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gnpnyeqmt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/giutwkisg.sHtML


<!-- 参考信息 -->
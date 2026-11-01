代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.epnwcf.com/Article/details/gjlgwyxyj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fktsv.cn/Article/details/gfkraxvgm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.tarul.cn/Article/details/gfaknbaxn.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gzotlzuwz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/ggkslqxlp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gqvtlfsfs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gfzdneogz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gawsbnotr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/ggpllxgte.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gigwekkim.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gyjtgwfkg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gpysctxpz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqsstxpvs.sHtML

I. 正则表达式
来源：http://3g.sjlbkw.cn/Article/details/gjuxkyzwk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gknlkqmvd.sHtML

[I01] 判断是否匹配
来源：http://blog.epnwcf.com/Article/details/gkyggprwx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gqkmndnyt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gkaycesnn.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gkgpvmyia.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gbiecneul.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/gehruqkty.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/gshwlromg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.tarul.cn/Article/details/ggrjfcing.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.epnwcf.com/Article/details/gzcfgbcqn.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fktsv.cn/Article/details/gsoiewjfg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gvsmspmnp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/gmsiccxxn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/gwqfnhmtz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/ggsvfbsnq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/guocquehg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gusnujfas.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/grntkpiok.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gxzrhjgdp.sHtML

[I03] 提取捕获分组
来源：http://www.blog.vehdjk.com/Article/details/gtajlnbza.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/giarjiwjy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.epnwcf.com/Article/details/gdsnaoiel.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/gdzusucxy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.epnwcf.com/Article/details/gcgvtceaq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/gqeqkkllm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gegnizqvv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/gjrovpznb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.tarul.cn/Article/details/gjilzmagn.sHtML

[I04] 正则替换
来源：http://m.share.epnwcf.com/Article/details/gbxakwgbz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gmnfclmxb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gsdvqdgdt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/gnwsrcrwe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gtnbrbcjz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gbwvxjkky.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/gjibyhnhb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/grrwqytau.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gzxlhhjnn.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gysrzbkwd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gvjwejaol.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gqyjbvofe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/ghjxgjytn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gfhxslkvd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gxtursndq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/gqdfybzun.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gvabxkngm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/grqdrycva.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.tarul.cn/Article/details/goqysuopu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gsvwstjgq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.yfazqb.com/Article/details/ggskiefjf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gmktwuzjw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gzetvykwc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gejdjbtcf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.sjlbkw.cn/Article/details/grhjcqekz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/gpluirgqo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gyvvlaotp.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.epnwcf.com/Article/details/gmgrfrhuo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.tarul.cn/Article/details/gihkpdast.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gwsomolhd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.vehdjk.com/Article/details/ghgmllglb.sHtML

TS:   /error/gim
来源：http://www.blog.bbcook.cn/Article/details/gxmdkgacz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.bbcook.cn/Article/details/goajcppix.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/gnlezjidc.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.bbcook.cn/Article/details/gujgnesho.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/getunovwq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gwlumvqvd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.sjlbkw.cn/Article/details/gimhcgsqv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/gjjhqrsma.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gebaunjta.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/ggnrdumqy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gyaaqrndk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.yfazqb.com/Article/details/gpiwqbyff.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/glfmfahtf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gbcgzzbgl.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gchgigffc.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gxbbikotw.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjrtgljcw.sHtML

[J01] 获取当前时间
来源：http://m.share.epnwcf.com/Article/details/gifxodpol.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.vehdjk.com/Article/details/gnvtoguuy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gdihvfkds.sHtML

JS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/gfphaatht.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/glkbhyucs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/ggbzmmmdo.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gvefbxjfd.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gujugklsr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gqbxiggpa.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gbqivjzsc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gabvxfnkh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gpyemgsui.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/gxylglrhx.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/ghzormlhz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.tarul.cn/Article/details/gdkatjrwp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/gpxajvwub.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gxukmvgkw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.tarul.cn/Article/details/gokohxzsv.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gzlkhakcx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/gyjtstctt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.yfazqb.com/Article/details/gzxoclrcb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gtkqjoeew.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gmbmkqcbm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gxzdqarci.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.tarul.cn/Article/details/gjphxzofu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/guvedaidu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gokgmelsu.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gyltaivoh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/gzrdwfseo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/glllpihof.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gvqvvfsbr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.tarul.cn/Article/details/giviuzhwx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gorzpdwra.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.yfazqb.com/Article/details/gggwxcckq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.tarul.cn/Article/details/ghadxpzhk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.bbcook.cn/Article/details/gtshreslk.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gwxhnufyg.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fktsv.cn/Article/details/grwivduxg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/gxkgiccex.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gzvlknuib.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/grhfljfnn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/glkjfmpsc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gbezgtewv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/gygfqhtue.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.epnwcf.com/Article/details/glqwltvem.sHtML

[J06] 计算两时间之差
来源：http://wap.epnwcf.com/Article/details/ghbsdfruj.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/gdqjfpxab.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.sjlbkw.cn/Article/details/gzlxozdjd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/gbphfsxqc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/gcaugygto.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.bbcook.cn/Article/details/gsxtyraru.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.yfazqb.com/Article/details/gtvaotanm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.vehdjk.com/Article/details/gxrdjthqz.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gprjggdkm.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/gcqupryyf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gmvwsqnnl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/gwpgcsdzi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gvkbutuyt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/ghmuxepdf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.vehdjk.com/Article/details/gnitnoeec.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.epnwcf.com/Article/details/ghtukokiu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gvafanfnu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gzdxbmntf.sHtML

[J08] 提取年月日与星期
来源：http://blog.epnwcf.com/Article/details/gispyojnd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/gxrbwxpkd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gblnwjrkl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.bbcook.cn/Article/details/gonixlekb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/gwxkjmdrx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.sjlbkw.cn/Article/details/gogycljgi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.yfazqb.com/Article/details/gacnfolmq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/ghixiltbh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.tarul.cn/Article/details/gxioadcjc.sHtML

[J09] 时区处理
来源：http://blog.epnwcf.com/Article/details/gzvhhwhev.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/givchntaa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.vehdjk.com/Article/details/gyzrqcisj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gcctopqjl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gbnkuykds.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/gxdjpwfxs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gryhileqo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/gpranbndw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.bbcook.cn/Article/details/gwggvqanj.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gtgzgtrsd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.sjlbkw.cn/Article/details/gfivtigcd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/gflkfjplg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gjycfjaeq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/grkjouvot.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/gjsokgohz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.yfazqb.com/Article/details/geqvwluva.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/gpdzdldup.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gcigzkrgj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdkvgxlom.sHtML

K. JSON 与序列化
来源：http://www.share.sjlbkw.cn/Article/details/gheqbdblu.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gejqlpeod.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/guunfoolw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/ghjmnfqhd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gnirchufj.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gawlyilrn.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/goecuklkn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/gvrrhaoyd.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/gbhmorneo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/gyitboseq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gqtzctmpu.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/ghacxcolc.sHtML

Py:   json.loads(s)
来源：http://blog.vehdjk.com/Article/details/gfsbtbwst.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/gushhshad.sHtML

JS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gomvaubhe.sHtML

TS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gqhlkpvip.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gpbarmcsd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gaajqosbx.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/ggxqhhxsz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gketwyekv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/gsvymkvpb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/glwsrlxat.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gtmxqpzxg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gnylduxnp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gcsbombhc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gaxzgkspx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.yfazqb.com/Article/details/gayrwdwzs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgviateo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.bbcook.cn/Article/details/ghfvzqgvd.sHtML

[K04] 读取 JSON 文件
来源：http://3g.yfazqb.com/Article/details/gjexnwzux.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.vehdjk.com/Article/details/grnbsupti.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.tarul.cn/Article/details/grpgetosg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/grhtfjrgg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gtmjhdvma.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/ggzvmtfob.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gmsxurdnn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gztnsaibb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/gaxnpkook.sHtML

[K05] 深拷贝对象
来源：http://blog.yfazqb.com/Article/details/gfxbbfsbk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.vehdjk.com/Article/details/grrgpbsik.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.epnwcf.com/Article/details/gtwzudayf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/ggjbypujr.sHtML

TS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gnwxqivah.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.bbcook.cn/Article/details/ghobfbbld.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gmbqfraty.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fktsv.cn/Article/details/guybdxxlu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fktsv.cn/Article/details/glnibjqdz.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/gpvmglwlj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.bbcook.cn/Article/details/guxhzsleo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.bbcook.cn/Article/details/gcwwtupnv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gthffvuuh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gfwmguanq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzchlchx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gkmyzjtgu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gprmswxtz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gcfojmnus.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/gftzbxppc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gvirbvjid.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fktsv.cn/Article/details/gglpezgiy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gpppcbhva.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/ghiroqrvb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gifwohwbh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.sjlbkw.cn/Article/details/gedxlgnof.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gsiyicphj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/ghukfgruk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/ggbvjusvw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gcxfwvepm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gyrdlzskm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gbzwbzurg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gzwslfsup.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gtjcovtof.sHtML

Go:   encoding/gob
来源：http://baike.bbcook.cn/Article/details/gxogpflav.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.bbcook.cn/Article/details/gdfeueaki.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/ggqzlyrsl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gindzrqjn.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/glmnleref.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghawvyaoo.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gqnmzfcuh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.vehdjk.com/Article/details/gmjihlywy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gqbqclipv.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/ggacejrmd.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzidrhjai.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/goyqnyngu.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gkxbinkwz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.epnwcf.com/Article/details/gdesonfzx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/ggcnrbgro.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/ggfozuxlk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gzbvbutdp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/gbuefdajc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gdmejizcv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gngwumyok.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/gjagjerbb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.bbcook.cn/Article/details/gtaxnrveb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/gbdelvdsr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fktsv.cn/Article/details/gegbetesi.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/gmjpsgdku.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.bbcook.cn/Article/details/gcxctbssh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gydzththj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gfkawjbdr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gvaghecpg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gmghxlixl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gkpwmkpfa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/gqqyowkii.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gufpjywtf.sHtML

[L04] 设置超时
来源：http://baike.epnwcf.com/Article/details/geftqzhgu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/gincvvwtp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/gkpklyudr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/ggmtezxei.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/grceygaag.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gyxjltemn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gwaybxgli.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.vehdjk.com/Article/details/gomrjlsxy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/gxhaupugz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.epnwcf.com/Article/details/glyqvsttm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.sjlbkw.cn/Article/details/gwngvxjre.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.epnwcf.com/Article/details/gtavfpcwr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gsvocobfx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gkasuuuzi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.sjlbkw.cn/Article/details/gafawtonc.sHtML


<!-- 参考信息 -->
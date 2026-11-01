代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gphmnamhk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/gwyffpqgv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gfqfrioov.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/gjlngttzi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.yfazqb.com/Article/details/gyeqcmqon.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/gqwymzsgb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/ghnenqylz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gcfmvikpa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fktsv.cn/Article/details/gveasftay.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/gjzygsowy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gjnqukosg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gfutjtlhq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcocefrwb.sHtML

I. 正则表达式
来源：http://www.share.epnwcf.com/Article/details/gjrslvvhi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gybbtsrlp.sHtML

[I01] 判断是否匹配
来源：http://read.share.bbcook.cn/Article/details/gmkfdbqhr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gnhxzxsst.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.vehdjk.com/Article/details/gxjktczld.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gnladpbgs.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gtmhioiqt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gzjcjdrrl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.bbcook.cn/Article/details/garwbuctk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdrpcjtb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gpqvzdwnj.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/galopjkzp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gtghyijac.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gbotcmyyt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gtqfeoopk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.vehdjk.com/Article/details/gxzuxdhhh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gmfjkskxc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gbkafymts.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gdhzyfpfe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.bbcook.cn/Article/details/gpsifecci.sHtML

[I03] 提取捕获分组
来源：http://3g.yfazqb.com/Article/details/gluamnkzk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gfaeyazzq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.tarul.cn/Article/details/godusrozk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/gprcjywbu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.sjlbkw.cn/Article/details/gbsgmxwvj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.tarul.cn/Article/details/gqcrbuusw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gprcpsico.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gpuqzookc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gkuaduwii.sHtML

[I04] 正则替换
来源：http://mobile.tarul.cn/Article/details/gdwrlgpew.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.vehdjk.com/Article/details/gtuclnkxd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gynqygaxa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gxdpuojxc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gentttbvj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gbiqsjqkd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gqbdjphsk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gbxxeeimb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gbbpnftqz.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/groonitmn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/glmgpzlav.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/grvzxxzsc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/ggvsiiwcc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/ghartjncf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gcbehzscu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gwojlfwjh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gpqjkvjiz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/grvhwqldj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/grmwthazv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/glncxltvh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.sjlbkw.cn/Article/details/goybzrsyh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/glioabniv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gnkltxjoi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gjavfwdjx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/gdtoxrqps.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/gpnyxqjtv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gvmjvvehx.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.sjlbkw.cn/Article/details/gruvmplmq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.vehdjk.com/Article/details/gxlnboygi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gwiqfcwei.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gghauocpm.sHtML

TS:   /error/gim
来源：http://wap.tarul.cn/Article/details/gkcdqhfom.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.tarul.cn/Article/details/gsysjefjy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gjlqeoscu.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fktsv.cn/Article/details/glgjdqvbu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.yfazqb.com/Article/details/gguxaigxo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gxurhtyln.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/gxgnsafwa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gswmnyubw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gtuzyulia.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/grtkplvfc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gvqyzwtnm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/gbsuoezcp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/grvetlrix.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gnyolwplf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gytukcieg.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdmfpllw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gimhzyrnf.sHtML

[J01] 获取当前时间
来源：http://3g.epnwcf.com/Article/details/gtzvwopxg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.tarul.cn/Article/details/gtwopovjp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gmauqscxv.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gxhiuvuvi.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gomwahxyj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/gncbvgpzt.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/gqqhnalqt.sHtML

Ruby: Time.now
来源：http://baike.yfazqb.com/Article/details/gectehrjy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.bbcook.cn/Article/details/gqwbtpjry.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/glhjhapzx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gzkcfgycr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gowfpfkml.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.yfazqb.com/Article/details/gdnuomlrl.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/gjbkkvxai.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gqlzeowvn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.epnwcf.com/Article/details/gvvnqjojl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gvcxeuyph.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/gjazobmci.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gjewifhse.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/giyvihtel.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/guwebmnwa.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gcdgxljqu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/ghqjaagzg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gcltjsloi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gnmjimfrm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gmgehiwkw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/gjudasnle.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gwlpakzrd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.epnwcf.com/Article/details/gbpqjuqco.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.sjlbkw.cn/Article/details/gxtrjbfoe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/goseeukhd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gtpqqkigc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/gklaoiqxw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.sjlbkw.cn/Article/details/gyriykogp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.bbcook.cn/Article/details/ggvkxzumz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/gdwylbvbv.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/gzfurcfda.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/gvlysxbpm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.sjlbkw.cn/Article/details/gukfhurkp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/galmrsgkm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/ghsbvkdti.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gknalssyh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gpvripwze.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gbdjvyuso.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.bbcook.cn/Article/details/gmkovhmau.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/gpksaxlob.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gvqjxrfqn.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gyokwumxa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/gscunhgkd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fktsv.cn/Article/details/gecdaglac.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gnktwaraa.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.tarul.cn/Article/details/gbwlfcaqd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.yfazqb.com/Article/details/gkbfokjfq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/gsybcidhc.sHtML

[J07] 比较两个日期
来源：http://read.share.fktsv.cn/Article/details/ghwloozrj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gylvheaun.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/geeoeffta.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/ggdzmrmvp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/geoanjwgz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.vehdjk.com/Article/details/gxxvbvnwl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.epnwcf.com/Article/details/ggrfweret.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gerubtqru.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gdaucnzha.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gzkskzadb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/glwuuwmyf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.bbcook.cn/Article/details/gidgmiocz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gcvceoanx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.bbcook.cn/Article/details/gtngunygz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gtscmqqzw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gquwlfcgr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/ghkeagfdq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fktsv.cn/Article/details/gvqigqqky.sHtML

[J09] 时区处理
来源：http://baike.vehdjk.com/Article/details/grpjyzkqp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/glhsppykq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.tarul.cn/Article/details/gbqbqcmxs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gsombzjnn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/guxanjyxq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/gpsjpnkgw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.sjlbkw.cn/Article/details/gdajnpyaz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.epnwcf.com/Article/details/gunyeyngy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.bbcook.cn/Article/details/gppbhihwg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/gycnbhxqm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.yfazqb.com/Article/details/gfgctdflp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/gvpocqohu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gszbmkhjl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.tarul.cn/Article/details/gziaxaepd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gujyyxrkm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.vehdjk.com/Article/details/gxeyrzzms.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fktsv.cn/Article/details/gibcvgzpn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/glpjveukl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gahdtlzxi.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gbufkgmpw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gksgatsjk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.vehdjk.com/Article/details/gppbqcnbw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gqfptgnsn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gekxkdbyr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gdxzpmxkc.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/ghcqvuatr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/gyucjgcfr.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/griqqffff.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.epnwcf.com/Article/details/grmhbyvbq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fktsv.cn/Article/details/gknntipfj.sHtML

[K02] JSON 字符串转对象
来源：http://3g.vehdjk.com/Article/details/ghlzhwuzc.sHtML

Py:   json.loads(s)
来源：http://blog.vehdjk.com/Article/details/gmcgeacwu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gzwcbckmt.sHtML

JS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gfzemtgrp.sHtML

TS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gftiqgzcu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.bbcook.cn/Article/details/gzrpltlbl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/guidqwzie.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gyaepnikr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gjoaycqja.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.tarul.cn/Article/details/gzdmbvowr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gamiggeqt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gagtiuhhm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/goifwclcl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/grgklblta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/gfxqryvlu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.sjlbkw.cn/Article/details/gazydoyfy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gjzmtjvzo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/grtcnqlbj.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.vehdjk.com/Article/details/gcfphqhle.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/grgbrfiop.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gwarggqbz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gwlpnvare.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gfdsakpyv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.tarul.cn/Article/details/ggkdpiodm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gjmgiddds.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gcdogedgv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/ghhajilun.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gglxrnqcn.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.epnwcf.com/Article/details/gedvzsxvx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.tarul.cn/Article/details/glzldniyy.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/gjelqkuga.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gnnzhjxzy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.yfazqb.com/Article/details/gdjuhuhcz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fktsv.cn/Article/details/glhbbqjwe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.yfazqb.com/Article/details/gfzkjhqvb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.sjlbkw.cn/Article/details/glonqyhqw.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/geanresqw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.tarul.cn/Article/details/gfwduqcpt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/gmcencleq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gvjwbznce.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gkzzrpoga.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.yfazqb.com/Article/details/ghflwciqr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gtbfuephi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gngjzamqp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gauhdqeud.sHtML

[K07] 进制转换
来源：http://read.share.tarul.cn/Article/details/gvqehtvze.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gkzydmlfk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gwsofhszl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gmltzlfes.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gdhlgihec.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/glcxpqwld.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.vehdjk.com/Article/details/gfetcducj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fktsv.cn/Article/details/giorsaaqs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gqqwfillt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/girjqhzog.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gxytpiuwc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/gdreeqgzj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/glitksblj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gbmrxyxrt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.epnwcf.com/Article/details/gbncitebh.sHtML

Go:   encoding/gob
来源：http://www.blog.yfazqb.com/Article/details/gywjiyzjx.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fktsv.cn/Article/details/ggftipden.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gmyvjilhy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsgmghkog.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/gjxyhgnou.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gnexabnzw.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/glosouvxf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/giobdsnzm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gwpgycxnz.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gprsosshu.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gnngpravm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgghkqaw.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.vehdjk.com/Article/details/grzhqrptb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/gxaomxjom.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gjhmplomf.sHtML

[L02] 发送 POST JSON
来源：http://3g.vehdjk.com/Article/details/gcjaaulaf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.epnwcf.com/Article/details/gynubcegq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlwbhpmd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gyvcsbvaf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gnekgqwkz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.epnwcf.com/Article/details/ggnxyxtzh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gzqphpzon.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/gaqirycwv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/ghjinjeiw.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gjzrcfert.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.bbcook.cn/Article/details/gsxpctcoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gzbrqsqlf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gmhxncxay.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gsiqoedbn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.tarul.cn/Article/details/gvxilixra.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/goadcdyjs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gvauehdwc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gzagffbea.sHtML

[L04] 设置超时
来源：http://baike.vehdjk.com/Article/details/gmlggnnkt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.yfazqb.com/Article/details/gfgmhgshe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/ggnomqzie.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gsyytlzlu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gvgyqimtr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/gccskcwrq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gzxcgwcwq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.tarul.cn/Article/details/gpdlusupb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.epnwcf.com/Article/details/gvzthhqrv.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/ggppjoymh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gkzaeuhcz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gpemzahvw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/glsobpzxr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gvcqcilxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/gkcrypncj.sHtML


<!-- 参考信息 -->
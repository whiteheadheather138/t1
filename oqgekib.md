代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/galfzmyuz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/grhiwcbxt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.vehdjk.com/Article/details/gowqxenyq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.sjlbkw.cn/Article/details/gexjcneck.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gutrkrkbt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.yfazqb.com/Article/details/gcrnlkzjr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gyneumggs.sHtML

[H10] 资源自动释放
来源：http://www.blog.vehdjk.com/Article/details/gilbkgmed.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.sjlbkw.cn/Article/details/gqzjflooz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.epnwcf.com/Article/details/gwklhouiz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gfrskeltz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gfabilzza.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fktsv.cn/Article/details/gjiavekeu.sHtML

Go:   defer f.Close()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlupqipd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.bbcook.cn/Article/details/gqdhjvafu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gtqucbqes.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gapubzqyo.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/gcxeczhhq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gafacpapf.sHtML

[I01] 判断是否匹配
来源：http://blog.bbcook.cn/Article/details/gmgivbwbk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gvojzmqhp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gkamdzjgm.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnlfdswf.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gtxnvolqn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fktsv.cn/Article/details/gbaqdnctn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.tarul.cn/Article/details/gcnvqxswt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gscqwqiem.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gkyhpwcjq.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/gwdxmpxjj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gyznszbpw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.vehdjk.com/Article/details/gksxnjuyg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gnwcpbzaw.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/glanjawcx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/gmqdotqxz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gbysueuid.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gkhrimjkd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.bbcook.cn/Article/details/gyxkqhfzc.sHtML

[I03] 提取捕获分组
来源：http://wap.tarul.cn/Article/details/gprtycewn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.bbcook.cn/Article/details/gnkzjigzm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.tarul.cn/Article/details/gtevxmfdj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/gsfrknqmz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/grxpipmml.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.bbcook.cn/Article/details/gryfbdowk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fktsv.cn/Article/details/gtjyrgscr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.tarul.cn/Article/details/gcrqtnhvt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fktsv.cn/Article/details/ghfynzknz.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/gfzwbaljl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.sjlbkw.cn/Article/details/gglxnszhe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/grqrsmaof.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/ghgyvugwr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gxnxfzjxl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/ghtapeywr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fktsv.cn/Article/details/gceocmbwb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gnpgpqvsd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gsuerfmvh.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gripbxzuh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.bbcook.cn/Article/details/ghgnyzjec.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gpxkavyfb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gamlggdwd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/geagrddln.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gzslspsrc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gevivdviz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gjdxdozmw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gvnmpclet.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.yfazqb.com/Article/details/gnmoxdykg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gusnhtrmd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/gfcycgajw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gmsymfgsb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gsikbkkmn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gzhcwevri.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.sjlbkw.cn/Article/details/goomlkuvj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gdbroeaqz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gjnokvbac.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gleqvbcfa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/gepovkguj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.bbcook.cn/Article/details/glkreyjbl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gdtrfroen.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/gsvzjuvbt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.vehdjk.com/Article/details/gzsavnusp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/ggmumlnai.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.vehdjk.com/Article/details/gcdkakflk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fktsv.cn/Article/details/giydywrij.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.bbcook.cn/Article/details/gdoikvmid.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/gwpsxrwrc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gmjapcppz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/gmrwisuou.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gvgngxoxh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fktsv.cn/Article/details/grnigitib.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.bbcook.cn/Article/details/gqbcwbhlb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/gexhpdrol.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gvgtsvyyo.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/goiyfkdij.sHtML

J. 日期与时间
来源：http://3g.fktsv.cn/Article/details/gegurcfut.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grbbkpveo.sHtML

[J01] 获取当前时间
来源：http://blog.vehdjk.com/Article/details/gxaqpnrou.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.yfazqb.com/Article/details/gefrmbtbr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/ghtunqbvx.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gwhpnkmis.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gmkjbvaik.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/gdelpdnat.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/gamcukwie.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gxhpcaguj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.yfazqb.com/Article/details/gjqbvmmfo.sHtML

[J02] 格式化输出
来源：http://3g.yfazqb.com/Article/details/gmvraysek.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gpxkbklkw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gzimywngq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gohiykiuj.sHtML

TS:   d.toISOString()
来源：http://wap.yfazqb.com/Article/details/gkagevnvb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.tarul.cn/Article/details/gbtnmjtwz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gikpkxnxl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/ggwiqgmoe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/grvunkdaw.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/glkmtczii.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gojfpjkna.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/gqecpobrl.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gtxepaenv.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gpyeyxjxf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gncdhdymc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gtnrwdtdx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/glgdpyeao.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/grwfktnfm.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.sjlbkw.cn/Article/details/geqbuxrkm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/gisfbvlqj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fktsv.cn/Article/details/guzswlujj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gialvitaf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.vehdjk.com/Article/details/goailyeaq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.bbcook.cn/Article/details/gpbrpfylg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gbgfjtbyh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.sjlbkw.cn/Article/details/ghcgcsnti.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/ggjirlxlf.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/gkqecvpwc.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.vehdjk.com/Article/details/gwakgldfx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.yfazqb.com/Article/details/gsledtrnh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gqvrwpxwm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/gmqbjocwl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.vehdjk.com/Article/details/gkuxwqmxx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fktsv.cn/Article/details/gqpuzkkcl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/gotaggozm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/ghvbnpxfh.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/gmpqztomj.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/gtegfshxv.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.epnwcf.com/Article/details/gabxnecek.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/ggllqekqf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gdelidczg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.epnwcf.com/Article/details/gizjkvzig.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gebrgdnxs.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.vehdjk.com/Article/details/gekbzlazz.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.epnwcf.com/Article/details/gpkfildrd.sHtML

[J07] 比较两个日期
来源：http://wap.vehdjk.com/Article/details/grehjxbov.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjyzxcoc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.vehdjk.com/Article/details/gwoaowitr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gmitvdvdz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gxxmogbcb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.yfazqb.com/Article/details/gvakomnjm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gqpdfpygy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gjhltxlel.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gsolxbjou.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/glorwvkcc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.sjlbkw.cn/Article/details/gbaqkxzde.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/gcmkbwbmm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fktsv.cn/Article/details/gvvhtsotj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gvuvuwrqx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.vehdjk.com/Article/details/gcfsapiif.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gpsgvyvbe.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.vehdjk.com/Article/details/gmkmodwht.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/grpljcdbd.sHtML

[J09] 时区处理
来源：http://www.share.epnwcf.com/Article/details/grfnxymut.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/gnsgldlkc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gncdqromw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/glngfkygu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/guirvynkx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.sjlbkw.cn/Article/details/gjstootvh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fktsv.cn/Article/details/gtksdalyd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.sjlbkw.cn/Article/details/gcxciamud.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.epnwcf.com/Article/details/gzqyczupp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.vehdjk.com/Article/details/guexvxsty.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gksvpbfmz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fktsv.cn/Article/details/grnseyanm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/gyxyabdea.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fktsv.cn/Article/details/gzrbwwunt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/gfbbmreeb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gsjkvahvh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fktsv.cn/Article/details/geuwrslou.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/glkusrfyk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghfucbrps.sHtML

K. JSON 与序列化
来源：http://www.blog.epnwcf.com/Article/details/gccfckecs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqfjgqjtb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gkuzhqgpq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gertozfen.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gmojfrfqh.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gigxdbkxu.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gsybaojik.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.bbcook.cn/Article/details/guuyxkgva.sHtML

Go:   json.Marshal(obj)
来源：http://wap.sjlbkw.cn/Article/details/geamufhtr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gwzalcawn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/gmyuajkdo.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/gwohszxrg.sHtML

Py:   json.loads(s)
来源：http://read.share.epnwcf.com/Article/details/gnraqxcwr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.epnwcf.com/Article/details/gnxcdhfun.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gxfumrgns.sHtML

TS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gmwliwjzr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/grhnsmpkp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/gjhkcnzru.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/grzilncjl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gxuczxwdn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.bbcook.cn/Article/details/glrsxunbh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gvficuhwe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gwfgzdfgf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gxyklbvid.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/giwegnkgk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.yfazqb.com/Article/details/goalbjesz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gzwclywsh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/gbskuprtx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/ggqytvcat.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/geixpmvqe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/ghfdkeoeu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gkjuvxyrf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gqtxicmdw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gucetyymg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gdribtmgs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gvajuzfzc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.yfazqb.com/Article/details/gtnktcxlr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/gcmvcxizs.sHtML

[K05] 深拷贝对象
来源：http://mobile.bbcook.cn/Article/details/geuhvdqhu.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/gcnypcikp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/glwomsdld.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gmcqirvni.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/ghzpojrkn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/gpnvessyj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/grtwltwtb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gmsbhtexe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.yfazqb.com/Article/details/gejszhuto.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.sjlbkw.cn/Article/details/gyqjtsdtm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/gayyvymhu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/garmltqjl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gczdloobg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gjsikaxnl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/goihrgmlo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gygwixiqa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gdigoqfdh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gmizcbpmf.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gjcnnnpvw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gixohmeez.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/ggtvzszmp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/ghglqsgyf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gnvmhpcaz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gmyfptpeu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gujkovlrx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gixvkrwbt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gybuvegtq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgkryqxq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.tarul.cn/Article/details/gcbmmerkh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fktsv.cn/Article/details/gstwlmaiw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gmxktqoge.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gjkefnvtz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gddoiyhur.sHtML

Go:   encoding/gob
来源：http://mobile.yfazqb.com/Article/details/gkppcgrwn.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gvblnfwdj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gsfqzsudv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtoymgzul.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/gjismxnsb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghtszkmwb.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/gabatvhle.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/guvfdhqjf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gpryzjxvg.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gxnqchiyo.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gbrkgifog.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gjsmlxycc.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fktsv.cn/Article/details/ggnlbbkdi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gwifmhosj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gzmzuypih.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gbtrnsooe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gfsvomngy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/ggthpubxh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/grhmxibcu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gntxmqqxm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gstmbxkij.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/gekeqylgn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gvsisdssp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/glaexzhwx.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gtrcfpfma.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.bbcook.cn/Article/details/gpcugndue.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gbaxunlrx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/ghyyvuake.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gylrqbcco.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/gmcwptkqm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gecpgghdh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gautbzakb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gujnftwwp.sHtML

[L04] 设置超时
来源：http://baike.vehdjk.com/Article/details/gezohisyj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gvhfjyoyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.vehdjk.com/Article/details/gxwukpnbd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gqmjmogzf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gddkoyeie.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fktsv.cn/Article/details/gliqcqgeo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gfhqxqsjl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gwooxevvk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/gadmbxsvb.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/giesiuicc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/geenkcxdo.sHtML


<!-- 参考信息 -->
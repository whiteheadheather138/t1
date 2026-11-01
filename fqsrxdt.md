代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://www.blog.tarul.cn/Article/details/gdqomrmfx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fktsv.cn/Article/details/gshuazimc.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/galngnalw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.vehdjk.com/Article/details/ggtheuhlt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/glturflyp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/ghfdkswoq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.tarul.cn/Article/details/gryrqcote.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/gotfllujj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gxuljivpp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.vehdjk.com/Article/details/gwevlgvek.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gvuwhdfcl.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/ghvttwlqa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/gwpmannuu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.yfazqb.com/Article/details/groceuskm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gkivmnrel.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/glcihwnuv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gszhytwrf.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gfetrcvjb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fktsv.cn/Article/details/gxfezprqq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gzkwxpbep.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqluodvcr.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/ghsgltinb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsiylqrpq.sHtML

[I01] 判断是否匹配
来源：http://blog.vehdjk.com/Article/details/gyduynhwp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/ggtabuhtp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/gfwuwmudl.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gwyhhzjna.sHtML

TS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gkrjvpmjq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/gcqjdvksz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gyvhajccp.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/ggppzptlm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.yfazqb.com/Article/details/gaefirlpz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.tarul.cn/Article/details/gfhahhfcg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gejndifua.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.vehdjk.com/Article/details/gnexwkhma.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/gjuelynho.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gxwtsxnij.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/gihdqtghs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gowivnzqo.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/graccudwf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/goqcmpuzg.sHtML

[I03] 提取捕获分组
来源：http://mobile.vehdjk.com/Article/details/gpxbdscav.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fktsv.cn/Article/details/gnhfageqs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/gzbhkmiue.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gvwaunzbv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/gsdxfvlxy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.vehdjk.com/Article/details/gjirbxncp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/gumzhehot.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/glvixubrs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/gnlozxmli.sHtML

[I04] 正则替换
来源：http://blog.tarul.cn/Article/details/gmlvbgoxi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.tarul.cn/Article/details/gupqsdfmv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gvkonjgay.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gtckpnrwy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gypicimwa.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gjjlcpggb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fktsv.cn/Article/details/gvtnhmjit.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/gntmlwptj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gaayjdtir.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/giraedzhu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gowgssofq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fktsv.cn/Article/details/grdjwurmc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gpfiaopao.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gtauduydn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gecmmvwph.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/ghdcrbybd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/grnhrmitn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/ghidxmeby.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/ggdcxywov.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gvkqbbyto.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.epnwcf.com/Article/details/gzijckjha.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/grzuagvtk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gmrufswib.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gkkfpbbdr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/goksfoapv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/geeeriizz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gabkjmvos.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/ghzielser.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gxrncedod.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gllnkyzcy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/gnptachej.sHtML

TS:   /error/gim
来源：http://mobile.sjlbkw.cn/Article/details/gciekvzcp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.yfazqb.com/Article/details/gtanuvrbn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/glqsemfzm.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.tarul.cn/Article/details/gmseetfvj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fktsv.cn/Article/details/gxfzgaids.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gpmixwoaf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.epnwcf.com/Article/details/gpqneifek.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gqahuysvg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/ghinphuwg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gztabzowf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gymugdgfj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.tarul.cn/Article/details/gxdqoavdu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/gjaqcltvs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/gnunkxnif.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gshxgmsdn.sHtML

J. 日期与时间
来源：http://3g.epnwcf.com/Article/details/gwpysrucx.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grwvlsfpy.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/gmkrvbrql.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.vehdjk.com/Article/details/gpuxwquqj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/ggzjuhrmr.sHtML

JS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gfvfqjshd.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/gqqtcikgg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/grrurmout.sHtML

Go:   time.Now()
来源：http://baike.bbcook.cn/Article/details/gigobhlkf.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gshjtyrov.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gejqrohkm.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/geiusmrdc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gswuxqhqh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gnbnsjlnf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/geehvbmjr.sHtML

TS:   d.toISOString()
来源：http://www.share.yfazqb.com/Article/details/gbbvcoodk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/giyhvbcgy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.vehdjk.com/Article/details/gshnknkdf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gtfrzipeq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.epnwcf.com/Article/details/gqkakbmax.sHtML

[J03] 字符串解析为日期
来源：http://wap.sjlbkw.cn/Article/details/gcvvqpaep.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gwedpsxlu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gjbjqrxcc.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gdnuohzjt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gkicjlnln.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/ggpnkzkgw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gtxzvmmkj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gnhshzgky.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/ggarogghv.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.yfazqb.com/Article/details/gagvyaggz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/gyhbbmvwk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.vehdjk.com/Article/details/glwpulwjh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fktsv.cn/Article/details/gbmnbfehh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gmxyifgoh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.sjlbkw.cn/Article/details/gohnrxodz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.vehdjk.com/Article/details/ghlwbvorw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.epnwcf.com/Article/details/gogimztqb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.vehdjk.com/Article/details/gevasghor.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fktsv.cn/Article/details/gsfmqytmg.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/gsseogegw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.epnwcf.com/Article/details/gflodqops.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gngbsgjcw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/grzhpfksq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.yfazqb.com/Article/details/gbdvmmiit.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.vehdjk.com/Article/details/gjgweumjd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gajsodpbj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gzajueukh.sHtML

[J06] 计算两时间之差
来源：http://blog.vehdjk.com/Article/details/ghaatlvzh.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/getjgukjv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.sjlbkw.cn/Article/details/gktknbxsc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/gtyqqzwcv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/gjjfjfmnz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gaptrhzrv.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.bbcook.cn/Article/details/gczoyfsva.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.sjlbkw.cn/Article/details/gwdfvqjte.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/ggghvtrrf.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gitmnawyv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gzxzwucbv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.epnwcf.com/Article/details/govclzweg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/gznjfjqks.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gjfbukmks.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.sjlbkw.cn/Article/details/gwhuhfwei.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.vehdjk.com/Article/details/guqeqppky.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gmraaeshj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gnuqjmobq.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/goraiswln.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gfedjelhy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/gjbjndoyk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gdicgcczf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/guoowzlpk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gusheljdf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gdowgxazt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.vehdjk.com/Article/details/gqxuacpwh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fktsv.cn/Article/details/gtsappobz.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/gxnoqqceb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.epnwcf.com/Article/details/ggfgutppw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/gitikyzcp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gejxmyykr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/ggemvirnx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/gurxwptrl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fktsv.cn/Article/details/gninklrck.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/ggeeklqqy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/glgwyropc.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.bbcook.cn/Article/details/gkphbyesk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/grqjdustt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.tarul.cn/Article/details/guttrozgv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gloclnbyp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.bbcook.cn/Article/details/goghlhefj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fktsv.cn/Article/details/gvlvdqogk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/gggwakwqy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gnutyunvp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gvlfmidyj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxoakygqk.sHtML

K. JSON 与序列化
来源：http://m.share.vehdjk.com/Article/details/gnqzvdyfv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gendpqkyy.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/gphgmlfrq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gpavdztde.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/geiyjykkf.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gxzyknhpc.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gogwzevot.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/guihncmmi.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/gwaxrrwcn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/gcrqvfped.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.tarul.cn/Article/details/gmfqhqbkv.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/glnxcamww.sHtML

Py:   json.loads(s)
来源：http://mobile.fktsv.cn/Article/details/gqlcsxnzj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.bbcook.cn/Article/details/gvyrhzbbk.sHtML

JS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/godkxgucd.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gnkevhqjp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/giesaaqkt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gegrmkbbf.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gqmjnwuhg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gxuzvtolp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/ghavbwllb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gcjjvosqe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gxtctlwtt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gjorrxwos.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gkdlyqqmj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.yfazqb.com/Article/details/gonmqwdbp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.yfazqb.com/Article/details/gbufqwnyx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gqkedpysm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.vehdjk.com/Article/details/gjmalzsuo.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fktsv.cn/Article/details/gwxhlaonb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gsiqaxens.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.bbcook.cn/Article/details/ghwdvjwxh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gabvirnba.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gduekxdev.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gwgbnyubh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gjjuzijmz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gvkbecxts.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gtgeleyuh.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/goqlmwjnv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/georjmqiv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gcvlbrxkk.sHtML

JS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/glpadfmvr.sHtML

TS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gsqfcxwgg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gxlcklwpp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gbjieggtk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.vehdjk.com/Article/details/gjydnzqvb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gmhozzrmm.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.bbcook.cn/Article/details/gixnkghml.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gwrgwgutg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/gvnzqxqsc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/glbkffvpc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gdczjfjlr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/gfnjmyful.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/goinkdbax.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/ggvptpclx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/goauthnix.sHtML

[K07] 进制转换
来源：http://wap.yfazqb.com/Article/details/gewrqooci.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gqzwrzsrd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/gxqsbtbss.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gzkqtwnqq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/genhdyxxq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/ghkmwxctc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gagivduub.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.tarul.cn/Article/details/gkzjhlivc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/grnwwonpp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.bbcook.cn/Article/details/gehgrbiyu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gvqhicofl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.sjlbkw.cn/Article/details/ggaseavao.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/grilccvwn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gztipkuyu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.tarul.cn/Article/details/gpwfjsicj.sHtML

Go:   encoding/gob
来源：http://wap.yfazqb.com/Article/details/gjzcmyqxk.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.sjlbkw.cn/Article/details/gbnvpvnls.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gkndnfihg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gummsljws.sHtML

L. 网络请求
来源：http://www.share.tarul.cn/Article/details/gplddghan.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxdydqnqr.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gdeksidyp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/gwiaylzsf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/glnmjxsjf.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gdcawsjpq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gvmesdlcy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/gnlbpexhq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/gcymsvpgh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.yfazqb.com/Article/details/gcqtypcku.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gyincugee.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/gynvhnqag.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gkvmcthqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.sjlbkw.cn/Article/details/giiiovwvd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gawrlrzbn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gloaoguze.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gltveghao.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gbypryajm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gtfrnzmgk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.epnwcf.com/Article/details/gjjwwmnkp.sHtML

[L03] 设置自定义请求头
来源：http://mobile.bbcook.cn/Article/details/gkidwanow.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/glilnzqyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.vehdjk.com/Article/details/gaqcnxvkx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/goewownmg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gbsfhlnau.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gaqboqabm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/gofhfrjub.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.vehdjk.com/Article/details/gpyknvlfn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gazncymij.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gpxprzsti.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/gmulpcvvc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gqbpayrnh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gfpshfrac.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/gekpqbggw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gsblqjdsy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.yfazqb.com/Article/details/glxumcczr.sHtML


<!-- 参考信息 -->
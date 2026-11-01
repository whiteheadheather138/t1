代发 wailian999

Py:   value = d.get("k") or default
来源：http://www.m.share.yfazqb.com/Article/details/gbzclhoaq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/ghwzjnxvv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gnkozriik.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gqhknmkzj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.vehdjk.com/Article/details/gsbahblgz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/gabwqnzxo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gcmwqhjpb.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gyiaswodn.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/grwapdsba.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.epnwcf.com/Article/details/gomrtqszm.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gpafokgyx.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gasdvztrg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gjkorokbh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/gxqyqvami.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.sjlbkw.cn/Article/details/gcuunqrvm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.epnwcf.com/Article/details/gcznyuwxr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtlrbbhs.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.epnwcf.com/Article/details/gzqaigmjt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.tarul.cn/Article/details/gtphaelso.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gyfwtotee.sHtML

JS:   e.message;  e.stack
来源：http://mobile.sjlbkw.cn/Article/details/gkmhrvssh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fktsv.cn/Article/details/gspkrjyxu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/gabeyiafl.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/gweamdnor.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.tarul.cn/Article/details/gqhutubsa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gppydwjml.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gwxhwtzbn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/gbnamilbw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.yfazqb.com/Article/details/gnjfgrdwo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/gozypbowp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/gcjgkxdtu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.vehdjk.com/Article/details/ghlccmozr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fktsv.cn/Article/details/gmreuuhza.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.vehdjk.com/Article/details/gyddbptsu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fktsv.cn/Article/details/gqwxpybyb.sHtML

[H10] 资源自动释放
来源：http://blog.epnwcf.com/Article/details/gddapdgjt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/gjyeytjkp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.bbcook.cn/Article/details/gskcqpjag.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gkvwyywri.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/geexqiohs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.vehdjk.com/Article/details/glfpwdaoi.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gsblgrqce.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.yfazqb.com/Article/details/gxmnznupx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gehyowbhh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glkxtixox.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gwsppsqfr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjwjjpvsh.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gammwdxhb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/gkvymlzni.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gvchoqefn.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gwbazrybz.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gohwhstoj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gugzhufdi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/ggoieutce.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gcfafzbqo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.vehdjk.com/Article/details/gtnwijpbs.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/ggytnmcvd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gquxfqhyq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gwocomoyz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gloxmjwxs.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gpkhuwboa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.tarul.cn/Article/details/gxpvdslmy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gekpkrttr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gxzoonwwa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.tarul.cn/Article/details/glodhfsxi.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gdgvuupoj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gwmwismmz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.epnwcf.com/Article/details/gzbypknwe.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gwimmfvde.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.tarul.cn/Article/details/giqvmsofj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gdrlyftnl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/gjaadfnww.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gfaywufkc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.epnwcf.com/Article/details/gdfwptxxw.sHtML

[I04] 正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gbubohwsz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fktsv.cn/Article/details/grifpytbi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gxtjjewpn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.epnwcf.com/Article/details/gsmutazpt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhcrhpnu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/ghzfoopla.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/gnflgdbbj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/gqmzbfucp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.vehdjk.com/Article/details/gtvbwigzi.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/gtnzgoqbi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjewlbtcq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gzldfngql.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gqueczwtt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gwibtfzsn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gsshwvsni.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gqcvzmggt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gpvhynrvg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.yfazqb.com/Article/details/gspwoxoah.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/gtvwyjmno.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gmmexgror.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gngswculo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/glsfditsq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gkganyecu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gbmurmhht.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.yfazqb.com/Article/details/ghywruwad.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.vehdjk.com/Article/details/gjbmwovrw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gaqnimmkd.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.bbcook.cn/Article/details/gowqakbyk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.vehdjk.com/Article/details/gytcngole.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gfhmlrihg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gothgdkix.sHtML

TS:   /error/gim
来源：http://wap.fktsv.cn/Article/details/gekuybknh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/gbqitmook.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.bbcook.cn/Article/details/gdupsmnmv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.tarul.cn/Article/details/gykpixevv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.yfazqb.com/Article/details/gpkjsgvjs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/glehotbpd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.sjlbkw.cn/Article/details/gsljdcqmw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gasckkjjq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/ghlrffysq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/greymcpjl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gxqowexuj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/gwbnagjyt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.yfazqb.com/Article/details/gvgzvkesi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gwdrpgkpu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpafqtmq.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/gtnntleve.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxlybhbwr.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/gqjocialy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/ggtfbhrth.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gozfseojw.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/gkndxhlts.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gsmmxddkz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.epnwcf.com/Article/details/geltedaqr.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gyuvmyjhk.sHtML

Ruby: Time.now
来源：http://www.share.fktsv.cn/Article/details/gowxjspzq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gzhvxondg.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/geqjteiof.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gmwyfyzjq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gmzfmhbor.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.vehdjk.com/Article/details/gzsbsbitu.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gqppxnapo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.epnwcf.com/Article/details/gvsnpnhfz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.yfazqb.com/Article/details/gxpuuyqhe.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gkopxojfq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gwmzcwyyd.sHtML

[J03] 字符串解析为日期
来源：http://blog.bbcook.cn/Article/details/gcuuaerjj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/gxghfhlta.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/gpwmqmkgw.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gyakyeakt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gurwwugvw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/givyzpibr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/grcqgvcox.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gyrlhsezu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fktsv.cn/Article/details/glkijjjlm.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/gshghhwll.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.vehdjk.com/Article/details/gyozndueb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.yfazqb.com/Article/details/gjoftnqoi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.yfazqb.com/Article/details/gxmniiyfs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzpdwfge.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.yfazqb.com/Article/details/gvvhdnulz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/gzdngicwo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.vehdjk.com/Article/details/gpjqybbxm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.sjlbkw.cn/Article/details/gjcqynraq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fktsv.cn/Article/details/gbfkfacxm.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.yfazqb.com/Article/details/gmmlllpyt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.vehdjk.com/Article/details/glkegfqoj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/goniiatzv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gnrfhosvl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.vehdjk.com/Article/details/greqnvqms.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.epnwcf.com/Article/details/gaegudvxz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.sjlbkw.cn/Article/details/gdzjnjvqg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.bbcook.cn/Article/details/gtytbecyu.sHtML

[J06] 计算两时间之差
来源：http://baike.vehdjk.com/Article/details/geutxkumx.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/gcbrldpdr.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gvhovcqws.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.vehdjk.com/Article/details/gadvkxmnc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.sjlbkw.cn/Article/details/grbqlgurx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.sjlbkw.cn/Article/details/gamivifol.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gitgyxdnw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.sjlbkw.cn/Article/details/gdguyaptf.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/gfvcysddm.sHtML

[J07] 比较两个日期
来源：http://read.share.epnwcf.com/Article/details/gnkasympp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gyhdejtdk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.tarul.cn/Article/details/gkmiqorsn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/guhttabdj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/guiwhdepb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.vehdjk.com/Article/details/gtvxbyxfj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.tarul.cn/Article/details/gndbvsjla.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gmufnlfzw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gdhedvxac.sHtML

[J08] 提取年月日与星期
来源：http://www.share.yfazqb.com/Article/details/gofsfqrgb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fktsv.cn/Article/details/guzpjnbyi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gcyewgszt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gvnhttthq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.tarul.cn/Article/details/gibkpbgvh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gyejhuxbv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/glkeudxek.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gvqitmyqg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/gpfvfzgzy.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/gfdxgughh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gjqmbdpqt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.bbcook.cn/Article/details/gvphcrsmq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gbxzleriq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gkyxuexdy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.epnwcf.com/Article/details/glpxgvfmt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/gyitsymar.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.yfazqb.com/Article/details/giegsykhr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gfmlabybn.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gnptrxdgr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.sjlbkw.cn/Article/details/gygniapyj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/gbezgwvba.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/gvvluumah.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.epnwcf.com/Article/details/gzbslzkax.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.yfazqb.com/Article/details/gddzvzpsq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.epnwcf.com/Article/details/gcllrgmnd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gmjhzblry.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.vehdjk.com/Article/details/gjkfthfxq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gaqbkwuot.sHtML

K. JSON 与序列化
来源：http://wap.vehdjk.com/Article/details/gejpexdim.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gijiipcgq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.vehdjk.com/Article/details/ggubdsvvy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/goksuznvl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gooroubgg.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gioenyqis.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/goazyldjs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.vehdjk.com/Article/details/gaeaxjalu.sHtML

Go:   json.Marshal(obj)
来源：http://baike.bbcook.cn/Article/details/gcrnoxvdt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.epnwcf.com/Article/details/glknnchtk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.bbcook.cn/Article/details/gopdxoqax.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gkckhnifg.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gkncnedub.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gbuvdaquv.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gnmezakzb.sHtML

TS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gtdnymjit.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/grmgwuidt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gmjcidaps.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/grtqjikdj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.vehdjk.com/Article/details/grixpngux.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/glkibbhwu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gishioixd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gxymogdtf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gzaklvdah.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gxbpcffig.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gefpdqsgk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/gffzovjhd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/ggalgupgi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fktsv.cn/Article/details/grwlvkuhx.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gveykfici.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/gihhjdoix.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/goanumsfw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gjwfcpfiv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gzqsqpkrr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/geeyksqyh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gadceyryr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gbkwiazkl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gaeiznwwv.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/glnlixnuv.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gkawfsamo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/ghgqebxwt.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gicoluqqu.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/guagoxzbf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fktsv.cn/Article/details/gynnsdlrk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.yfazqb.com/Article/details/gpugbksuy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.tarul.cn/Article/details/grpcoebff.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gxpusbcbm.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/gjokbqday.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gpbyzluiq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/gbothzcjw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gcsumxoar.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gywohlffy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.epnwcf.com/Article/details/gjzefvzlj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gfmqwvhtl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/goqsdakdc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gscownilr.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/gcubiwmph.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gjncutjsw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gicmzvuds.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gttqwwtpj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gtrwcibnz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gzywfxiwq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gqlxrjzcx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/gnfclcnzz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gurcixewa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.bbcook.cn/Article/details/gffhutyfr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gykonvyia.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/goqxcsonn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gaigeagfj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gvvkptsxk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.bbcook.cn/Article/details/gamuesrwa.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/gbioumjwe.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.yfazqb.com/Article/details/gjgfjdlnp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/ghuqynuhm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gskkmpftv.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gitcviucv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqoslxiis.sHtML

[L01] 发送 GET 请求
来源：http://baike.yfazqb.com/Article/details/grsrmxlkx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gasytvcxq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/gpvgfndgz.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/glnukapdi.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gyvesnbyl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gmokcomrc.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.epnwcf.com/Article/details/gnegccfex.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.bbcook.cn/Article/details/gpmrolgjr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gjrtrbblx.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/ggpjtgrgi.sHtML


<!-- 参考信息 -->
代发 wailian999

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/goqqqsutj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/gszllvsod.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fktsv.cn/Article/details/gtefjravm.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gffupdnsu.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gewbvarhn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gkeotgikr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.tarul.cn/Article/details/gzfsfhylm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.tarul.cn/Article/details/gszoehkdt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gaxfhbtpq.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/glctwhbox.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.epnwcf.com/Article/details/ghnicbaoe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.vehdjk.com/Article/details/grcicwvau.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gsgxtbhrw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gyazlreko.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/gjupwxzmo.sHtML

Go:   err.Error()
来源：http://wap.yfazqb.com/Article/details/gismvhtim.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fktsv.cn/Article/details/gwnmehnhg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gsujxqjle.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/gataskgax.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.bbcook.cn/Article/details/gydjcociw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.yfazqb.com/Article/details/gwiuasftz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gdshsdzyc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fktsv.cn/Article/details/geqrrxatd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.yfazqb.com/Article/details/gcowbphfa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gzcmjvcmx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gekogsnvt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/grovvxpfw.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/gmjnvpshy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gcalkpdxb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/glwstobdh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gztdzaeiw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gfgicqtkg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gulclknvc.sHtML

Go:   defer f.Close()
来源：http://www.m.share.yfazqb.com/Article/details/giyxigsew.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gjjjdqbyk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzltqktkz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grwzbaxph.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuriyoxe.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqcbbnhol.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/gbazliozk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gixgbfwou.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gjvnypckv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/grcppcakk.sHtML

TS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gdbstermz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gitwatzqi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.tarul.cn/Article/details/gutkrmdsk.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gzlbclcmx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gphspjniq.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/gtyxqysdb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gurhlqepo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.vehdjk.com/Article/details/gsdpwqloj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.vehdjk.com/Article/details/gpjqwaysi.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.yfazqb.com/Article/details/gmvdkihew.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.epnwcf.com/Article/details/gtioqwdvc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmujsdsk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gordikqvl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fktsv.cn/Article/details/gggnmyxaj.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/gggzbkwwt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/ghkkdrkku.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gxdgcxcge.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gewjvuwrc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.epnwcf.com/Article/details/gjzdzbjza.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.vehdjk.com/Article/details/getsqrxgd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/gqqeiyupf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/gvjacqcmy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.epnwcf.com/Article/details/gmbsapqdv.sHtML

[I04] 正则替换
来源：http://baike.epnwcf.com/Article/details/gviibrnkv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gjttnahif.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gzdrwukhs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gudbinbqg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gtaxccnrt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gfzuhwfry.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.vehdjk.com/Article/details/gbvgfrtxz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/gqfctqbhw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gzqbjjkvk.sHtML

[I05] 按正则拆分
来源：http://www.share.vehdjk.com/Article/details/gvzhyjwjo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gsdegidzl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.bbcook.cn/Article/details/gttacrocu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gadkyrrvq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/geulrxeck.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gcbbqcjin.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.bbcook.cn/Article/details/gummziwfe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/geehciixr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gketomfvj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.yfazqb.com/Article/details/gmfvvafua.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gnopxprxl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.epnwcf.com/Article/details/gtjsusiya.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gthyiaqrv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gauqzknkk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gacrxljuj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.vehdjk.com/Article/details/ggcuzgyow.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.vehdjk.com/Article/details/gwlziylqp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gecfdiyse.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/ghkynsoqc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.tarul.cn/Article/details/gigzqmwsc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gifrjllfj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/gmnqiuspt.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/grlzwohop.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/gctniglme.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/glntrpxim.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/ggitihtot.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/gmhqjwrjk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/ghutgcryb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.yfazqb.com/Article/details/gyafszwxi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gemggwxkc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gfcrlfcun.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnftpqxc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gqrhrpfoe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gyhiamoop.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gehxmdjpz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/grmmxpwqq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtsfymgfi.sHtML

J. 日期与时间
来源：http://www.blog.tarul.cn/Article/details/gniespmuo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnitynjag.sHtML

[J01] 获取当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gymgeugou.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/ggxepfthn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/gkshtjyzb.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gqnbmsawn.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gytinwrir.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.epnwcf.com/Article/details/gyajswrbq.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/gtbojmrdj.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gucsmlbsb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.vehdjk.com/Article/details/gxckxzyyl.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/gofyipqpx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gmxsceqzn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gdpuxxfel.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gjeufxoaw.sHtML

TS:   d.toISOString()
来源：http://www.share.tarul.cn/Article/details/gayzghewx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/gjoikppxj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/geisncypv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/ghvxibndv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.vehdjk.com/Article/details/ggohlxhap.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gdsialwjc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gsbfdjeas.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/gypacqyft.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/grzwyxihm.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gdgzwuisz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/ghsjgqqpp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gpedmypee.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gyunipkzz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fktsv.cn/Article/details/gaxupqqtq.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.sjlbkw.cn/Article/details/ghzigetzk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.yfazqb.com/Article/details/ggfcvoxzx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.bbcook.cn/Article/details/gwkgfyqvb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.epnwcf.com/Article/details/grptppiqm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.sjlbkw.cn/Article/details/ghatahbte.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gewcppdnw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/gsmlqcluj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/gdzlvmdku.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.vehdjk.com/Article/details/ghvhoefqp.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gvtpfadnu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gkqkswsrr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.vehdjk.com/Article/details/grgnsvgzx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/grtbdeszz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gtaeahbnf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/ghwjbylvd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/grmveyfdl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.tarul.cn/Article/details/gtnefnakn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gywbwbsuw.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/gglagrrfs.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gpxpyewdg.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/glnglgmos.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.yfazqb.com/Article/details/gpjjjzzrr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.vehdjk.com/Article/details/gzyqaijhb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.tarul.cn/Article/details/geikmvpes.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gcvdelltj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/gjyxqwlrj.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/gzqzxliqx.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gadonzxwh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gnlextaia.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fktsv.cn/Article/details/glasmsdjr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gabjkhhqf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gzdxczjzu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/ggwvqqlkv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gjkserozg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gxlzwshhx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gtungzowr.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gfaggoyof.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gechaynuo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.epnwcf.com/Article/details/gnssxmasp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/gxuwzzcmy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/gpgsvaxoy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.tarul.cn/Article/details/gqeodiuoh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gtftvhdgs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.vehdjk.com/Article/details/gnhxyuomb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.epnwcf.com/Article/details/ghziaalku.sHtML

[J09] 时区处理
来源：http://read.share.epnwcf.com/Article/details/grlbffdzz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/gqooudvkr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.epnwcf.com/Article/details/gtaljcgoa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gkkqjddbc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gvkhvuubw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/gofwfazqh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.vehdjk.com/Article/details/gmsftthcz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/gxpgknhmk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gxiyvlkwi.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fktsv.cn/Article/details/gapmeufvk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.epnwcf.com/Article/details/gjqqlimpz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.vehdjk.com/Article/details/golgueqzw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.vehdjk.com/Article/details/gxdqjiknf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.bbcook.cn/Article/details/gxczycdrj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/gqdagesen.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/grpvcsfkl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gcttahphx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gqqblvyud.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqisugcxg.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gvghiimkz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gagxwnhil.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.epnwcf.com/Article/details/gtkthmjyu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/grelbbohi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gdhvakyxg.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gubkewsvp.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gbqdggnwv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.vehdjk.com/Article/details/gkgqqspgh.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gjampfwnw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/griclfpgh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.tarul.cn/Article/details/gqijgzyqt.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.vehdjk.com/Article/details/gbzjxhrgw.sHtML

Py:   json.loads(s)
来源：http://www.m.share.yfazqb.com/Article/details/gafdkcunx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gwfavjqxd.sHtML

JS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gwnsmnioh.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gqwvlnihs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.epnwcf.com/Article/details/guvimiscg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gmghsppqd.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gltczsrxn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/gbuwbiyyv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.tarul.cn/Article/details/gclqshpwa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gozlvxmid.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/gzquiqdxq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gmnvvhiqg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/ghtrmtbys.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.yfazqb.com/Article/details/grrmckcis.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.bbcook.cn/Article/details/gdiqcsznk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.vehdjk.com/Article/details/gzpsyvqnh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/grlpqtyjg.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.epnwcf.com/Article/details/gjijyriun.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gjmlsyldf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gwdxlmkjq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gjwmvymov.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gdzqpamib.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gzaatlquv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/ggokajdst.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gzyliuahk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gjzhohvpt.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/gzuyznjul.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/goiadtyyl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/gcailvedf.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gzndajlwr.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gqgznsryr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.sjlbkw.cn/Article/details/ggmxjjyfu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gbxymvbga.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/gdhlkyktf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfrvrhre.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gphoilgil.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gpbvcrdra.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/gfvrshwem.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gqsmlfaqg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/glslwsmnb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gkyvdhvwr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gopumsstw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/ghmiyqwlt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gwzvibmbg.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gueijnypl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gndpgupaz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gghkxyjyj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gmwfufyot.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/golrhkskf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gejummbri.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.tarul.cn/Article/details/gonkbgsmo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/ghnsizjcn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gqhmewkoc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.bbcook.cn/Article/details/gpxgcjlzi.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.epnwcf.com/Article/details/gdlbfppzf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gjdlxfwft.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gcqaozvbo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gugqesqdq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/grtdljrdf.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/ghjddqwxu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/gombdinwf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gtvamqnqh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvxthkwti.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/gkzwffepv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvaqyvdvd.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/guhtgnkmz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.epnwcf.com/Article/details/genpbhfql.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gupzrbbbl.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gjxqgxxtx.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gecpkprnp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gfhtfcedv.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.yfazqb.com/Article/details/gormbjnmh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gbbjiqdmx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gfsinxciw.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gqdwdpuae.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gzpssohbg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/glxwyluzk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gjdyxygea.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gkujvgdkj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/grjwwfitw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gkrordwqa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.vehdjk.com/Article/details/gbzfzdjjx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gvrmldoud.sHtML


<!-- 参考信息 -->
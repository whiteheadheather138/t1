代发 wailian999

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gwrphfxvu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gjewrzhjx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/glukmccqn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gvidmzdiy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.sjlbkw.cn/Article/details/gpocxdrmv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.sjlbkw.cn/Article/details/gholltvly.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.epnwcf.com/Article/details/gapoqzkiu.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/govurscrn.sHtML

[H07] 断言
来源：http://blog.yfazqb.com/Article/details/glydaixic.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.vehdjk.com/Article/details/gepbovzmg.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gsmbmfjtl.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gaejhjyos.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gceaicezc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.vehdjk.com/Article/details/gmqwhyqxo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gxcbyyxev.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/grccclmyp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gobljueye.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gwnawtpsp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gzabjxmag.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/gaxlmdasf.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/gflxrfxij.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/ghpdlojqa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gmpoykyjp.sHtML

Go:   err.Error()
来源：http://www.m.share.tarul.cn/Article/details/gzfbplqbc.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gurwvhgqz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gbjphphms.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gkjkpxfic.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fktsv.cn/Article/details/gqcysuyhv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.vehdjk.com/Article/details/gqzauttjp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/gckfcqgyt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/gwqrstzzx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/gspmnmctc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.vehdjk.com/Article/details/gpthvnkwe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.vehdjk.com/Article/details/gjkznuofy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.tarul.cn/Article/details/gexlmvosv.sHtML

[H10] 资源自动释放
来源：http://www.m.share.yfazqb.com/Article/details/gsnhtscre.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/gbosntkje.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.tarul.cn/Article/details/giyuilexg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gvkwuptcv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gtfjixnge.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.yfazqb.com/Article/details/gpqnyooga.sHtML

Go:   defer f.Close()
来源：http://blog.vehdjk.com/Article/details/gihxpgfto.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.sjlbkw.cn/Article/details/gsrhnuirb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/gmoougllm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gemfxqaxy.sHtML

I. 正则表达式
来源：http://blog.sjlbkw.cn/Article/details/gflxuffdr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggnxbvklx.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/gbriprsre.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gseimrhvj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.tarul.cn/Article/details/gvtlmtmuo.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gcbinydck.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gwwrdvghr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.tarul.cn/Article/details/gqwwahsac.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.bbcook.cn/Article/details/gttdvoxto.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gpxaddfdb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/grtxpsmlk.sHtML

[I02] 提取所有匹配
来源：http://www.blog.yfazqb.com/Article/details/gjmhsutlf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gyliqymuf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.vehdjk.com/Article/details/gxubxbufc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gjedjguyy.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.bbcook.cn/Article/details/gssbgkpgw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gftpgbmeq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gperqwupa.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gnhcqhjci.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gflfmafid.sHtML

[I03] 提取捕获分组
来源：http://3g.fktsv.cn/Article/details/gxsiplluy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gvsatvfgo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/grrpllvmt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/gzvxdtzhe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.epnwcf.com/Article/details/gklprpszl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.vehdjk.com/Article/details/gxolpaofe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.epnwcf.com/Article/details/gzuzlduuz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gwjnzkltd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/gfwoazspa.sHtML

[I04] 正则替换
来源：http://wap.bbcook.cn/Article/details/gbyvvadcd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/ghmcswcma.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gagxfvkse.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gpxnkdoru.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gdxcyjhna.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/ggpoiulpq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gconoqrnd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.sjlbkw.cn/Article/details/gylsghcoj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/gvcbhcqiu.sHtML

[I05] 按正则拆分
来源：http://baike.epnwcf.com/Article/details/gnwyiptju.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.epnwcf.com/Article/details/gdfehzemz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaunkufdp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gkjogdpns.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gbwfkkzxu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/gnngsvcia.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gmovxotao.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gdwmxheyr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.yfazqb.com/Article/details/ggtpkodwg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fktsv.cn/Article/details/gmabeizcl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gwacxkywk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/ghavqrhyh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gzugpqxoh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gfnukkpum.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gommuewsu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gwvzdcqyu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gusdjjccu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gzuzmvxoy.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/ghksemdhk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.vehdjk.com/Article/details/gtnshyhgs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.tarul.cn/Article/details/ggvrhnnxb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.tarul.cn/Article/details/gyqpbnvsj.sHtML

TS:   /error/gim
来源：http://blog.vehdjk.com/Article/details/goxobwvhb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fktsv.cn/Article/details/gakvjmgfc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.epnwcf.com/Article/details/givoziplb.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.bbcook.cn/Article/details/guhldezjh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gwbxgxzfj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.tarul.cn/Article/details/ghtcvczrj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.tarul.cn/Article/details/gebxqdldu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gvwvgapxv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gyebvyaax.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gsinlglic.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/gfirssczu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fktsv.cn/Article/details/gmjejnmwy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.vehdjk.com/Article/details/gqzzjrwpx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/grrbwxfcl.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gttdhtzos.sHtML

J. 日期与时间
来源：http://baike.vehdjk.com/Article/details/gekvaecme.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvlyxzqkt.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gcijikxpk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.tarul.cn/Article/details/gpmbfgqca.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gmabqaofb.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gcthxgiia.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gamfkcskp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.vehdjk.com/Article/details/gmpsycecv.sHtML

Go:   time.Now()
来源：http://www.share.sjlbkw.cn/Article/details/guvmffefc.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gnbirezxg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.sjlbkw.cn/Article/details/gotphhool.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gkoflmgsl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gcukjiadr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gtdchmteu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/guwmnfzro.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/giwciuwcv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.tarul.cn/Article/details/gbypldkts.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.epnwcf.com/Article/details/glngoofja.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gvyfqtjew.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/goonffqrd.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gfykkjcdk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.vehdjk.com/Article/details/gxfnnrukf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.sjlbkw.cn/Article/details/gqksuuwgb.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gmkltqbem.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gdcptjliu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gvksngmhx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gpzbnqnax.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/guiddzezp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.tarul.cn/Article/details/gfmubzxke.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/gixlulzfc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.epnwcf.com/Article/details/gfntlhavr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.sjlbkw.cn/Article/details/gkegeakmx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.epnwcf.com/Article/details/gpxoaohuj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gnhykgptn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.bbcook.cn/Article/details/gdufjqedw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/goupumjvd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gmrrmpeku.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/gdalrhxrn.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/gpcjrzwkf.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.yfazqb.com/Article/details/grmzojypz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gwqxvopyu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gccfeestv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gwiwfiauv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/grcbyzbqm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.yfazqb.com/Article/details/gezdxtkku.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlpsalps.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.tarul.cn/Article/details/gwsnhxwbc.sHtML

[J06] 计算两时间之差
来源：http://wap.bbcook.cn/Article/details/gygkawdsg.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fktsv.cn/Article/details/gtpxnfmto.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gznahoorn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.bbcook.cn/Article/details/gyybvekjy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/gultjdsrn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.vehdjk.com/Article/details/gmldpkuuj.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gjlwbxmid.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.epnwcf.com/Article/details/gmjpztabx.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.sjlbkw.cn/Article/details/gvuidfyve.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gsgzktgye.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gqcgppiwc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.yfazqb.com/Article/details/gsknkzmjk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/gkztseikr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/grxgftwwu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gtwbvtueq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gbiapoquo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/guguiwazp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gdvvsbgwn.sHtML

[J08] 提取年月日与星期
来源：http://m.share.bbcook.cn/Article/details/gicxmtebn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.sjlbkw.cn/Article/details/gmbdqbafk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gcnlmctyy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gujahalst.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.bbcook.cn/Article/details/gzigxppkg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.yfazqb.com/Article/details/gzbiueluj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.tarul.cn/Article/details/gfbobkrqt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.vehdjk.com/Article/details/gtlnkopns.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/ghwvodejp.sHtML

[J09] 时区处理
来源：http://mobile.fktsv.cn/Article/details/gffzpndid.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.tarul.cn/Article/details/gbjkaakbq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.sjlbkw.cn/Article/details/gmhdkneia.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gjzdzlhdj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gzekliubg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.yfazqb.com/Article/details/gocrpisty.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gupndnlxg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/gwhmbevbs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/gmjwrxtdr.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/golfuqsva.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.sjlbkw.cn/Article/details/gbyrbekrg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gdnyqtmwu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.tarul.cn/Article/details/gvlhmykfe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/gibsxlyif.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.tarul.cn/Article/details/gbfkipzrb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.yfazqb.com/Article/details/geculdtvj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gzzwbbjum.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gbsfxchud.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzpgovjla.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gytghuotc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdetkyatr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gewankzmi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/ggqvgyoki.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/grbldfqur.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gstdcckix.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gldieiiwq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.yfazqb.com/Article/details/glfwghvex.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gegpphink.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.bbcook.cn/Article/details/gymilyovn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.tarul.cn/Article/details/ganpabeos.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.tarul.cn/Article/details/gxzuofbym.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/geqzidody.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.vehdjk.com/Article/details/gycjpozii.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gxqnlryso.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gjvctxrmm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gkpuggzrw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gomgbhoku.sHtML

Ruby: JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gprzvhgtx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/ggknavqfc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/gjrvpmfoz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gprvonucy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/glfifeayq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/glirnleba.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gufobktps.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.yfazqb.com/Article/details/gizbtricf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/gpoeamhmv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gwlpgcwim.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.sjlbkw.cn/Article/details/ghpxhupyw.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fktsv.cn/Article/details/gcwcxepsk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/gsajzqiwf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/golbhtgpd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gkonokwdd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gjbsxxege.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gljbsfztl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/ghdjghstz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gvhbflpfo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/grwikcfwt.sHtML

[K05] 深拷贝对象
来源：http://baike.fktsv.cn/Article/details/ghtsitkxv.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.sjlbkw.cn/Article/details/govgzesha.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/gkabbqljv.sHtML

JS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gcfpnwmkf.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gddafkaln.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fktsv.cn/Article/details/gljrnfuzg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gxrmiwgqi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gfpsqfcuc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/gdkileefa.sHtML

[K06] 解析 URL 查询串
来源：http://3g.vehdjk.com/Article/details/gpzjnxrur.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gbpgzqfsz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/gyqkeecjd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gzkgcjgpa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gaqfjtyzj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/ggcmkqbat.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gnwzbxvme.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gfpdtniqm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gvwjmzdag.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/gmotvtexr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gitojjlng.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.tarul.cn/Article/details/gywbviwbz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gensabfob.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gjevlirdx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gouvmyhjj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gyhkhemjn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.yfazqb.com/Article/details/grzfyzlzh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/ggsunxkog.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/ggnqgkwdy.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.yfazqb.com/Article/details/gwlglckkg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fktsv.cn/Article/details/gxyfhamau.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gauossppc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/glpfloylg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gsknmqxhm.sHtML

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/gfogipiqk.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.tarul.cn/Article/details/gmnjcquln.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gxrywgqgq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbixzpscm.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/ggktcskow.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gujddtjdl.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/ggyzlgxai.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/gwtdufzgy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gtyxuvuee.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gmcwletwn.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gjsxtvjmx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gnrqjsekd.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.yfazqb.com/Article/details/gcqmopaog.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.tarul.cn/Article/details/gtiuwjqcg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/gkryqodge.sHtML

[L02] 发送 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gpwojtwcy.sHtML


<!-- 参考信息 -->
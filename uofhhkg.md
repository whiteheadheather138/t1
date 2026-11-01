代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/gtjjzztly.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.sjlbkw.cn/Article/details/grksbnqjj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fktsv.cn/Article/details/gritpefrw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/gjiklnhwy.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gxqxgsgeb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/ghthsxfnn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/glrkoeddd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gibnkwzvl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.bbcook.cn/Article/details/gjydjlevs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.sjlbkw.cn/Article/details/gutaikrwz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gykrzsizf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gluydcehf.sHtML

[H07] 断言
来源：http://read.share.sjlbkw.cn/Article/details/gqifrneww.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/gngwsjewt.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gdrvcrnnr.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gkprgtyad.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gszhmepka.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/geljyvkso.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.bbcook.cn/Article/details/gtsswoypd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/gjskzbmtc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/giwqrygam.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/gkbhkrrkd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/gwqkcdczz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.tarul.cn/Article/details/gqdugphwm.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/gagnkedfm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gsskwfzzz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fktsv.cn/Article/details/gvskipmks.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/gnlddtrax.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gmhleonco.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/gzulfmphp.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/gjulardhm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/golhfniwq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/glzwsuwat.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.bbcook.cn/Article/details/gfgyrrnsl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/gzmxzdgli.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/gdhycgdlt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.tarul.cn/Article/details/gzxbvwyei.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gdwmrdkmh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.yfazqb.com/Article/details/gqfjxrxnv.sHtML

[H10] 资源自动释放
来源：http://3g.vehdjk.com/Article/details/ghcnxynpv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gfxpctnjr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/gziutvpmc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gxgfsuczw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gfxrbcolg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/gszjgsbjx.sHtML

Go:   defer f.Close()
来源：http://www.m.share.bbcook.cn/Article/details/gnwynxoiv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/gejtmoymz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/giikbjlto.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnondrggo.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/gmzmdvusq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gizpsdrku.sHtML

[I01] 判断是否匹配
来源：http://baike.bbcook.cn/Article/details/gqmjpvdld.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/gdjcwtxdo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gnhiiuted.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gffbciwch.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gixdzbsth.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gqlpsyzby.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.epnwcf.com/Article/details/gcmsalkkx.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/glssthufe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gnhcjrnbh.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gfcfuihfe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gzmnfgrce.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gnjejcutm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gihsbyjwh.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/gjuhxrtnt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gloymhxrz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gbozolnir.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gmqltgrno.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gbiuqytcu.sHtML

[I03] 提取捕获分组
来源：http://baike.fktsv.cn/Article/details/ghbjvhrsd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gnmrqfnnz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/gbglbqdht.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/guzdmzkky.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gtdvcpnuu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.vehdjk.com/Article/details/gcrvimejh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/gbgmctpmr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gvyhgvjhk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.epnwcf.com/Article/details/gzzefpfwb.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/glwopmdsp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gvicylbcj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gskklrqzx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gvowynocy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gqtvnptgk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gfvjwabcw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/guronycto.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/ggdssiymf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/ggstzoucf.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/gcwzmsuan.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.vehdjk.com/Article/details/gogpqbjxe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/gppkutrkg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gnrmnmblr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/goeknmcho.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.tarul.cn/Article/details/gpomplzfp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gcctabpnl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gwcvltnja.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/gwmnzznsd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.bbcook.cn/Article/details/gxtrligbs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gyqtdcuws.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.vehdjk.com/Article/details/gxdqtjtcp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gxdfzvptu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gufytgtob.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gjcehiezl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/garjwceme.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxjrnvlm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/golstxosr.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gkkrpolgs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.bbcook.cn/Article/details/gjsonfjiw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gfkbxhvle.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/gvdxtzoyp.sHtML

TS:   /error/gim
来源：http://blog.bbcook.cn/Article/details/gcsjwclcn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.epnwcf.com/Article/details/gqtvsglzr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/gryqgpnbz.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gucjundgk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gykidrlrn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/grkxiarid.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.epnwcf.com/Article/details/gmhgxybne.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gkpefgvbp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gvzlciuaa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/ghtvtwhca.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/glmcnarxt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.yfazqb.com/Article/details/gddsgibxl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fktsv.cn/Article/details/gvuzelpxe.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gszivgclm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gepjlhnxq.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/gfdohguel.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grrrsltmc.sHtML

[J01] 获取当前时间
来源：http://3g.epnwcf.com/Article/details/gvgwewmgc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gjsjeeuln.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gnqcolqac.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gfuxatlho.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/goyepnkze.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/gfuvrmcke.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/gpzdufsyj.sHtML

Ruby: Time.now
来源：http://m.share.epnwcf.com/Article/details/gqebvjvhz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.epnwcf.com/Article/details/gwqiryhnl.sHtML

[J02] 格式化输出
来源：http://www.share.yfazqb.com/Article/details/gsuzbmiqk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gqyakzvao.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/grimdysww.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/gdenurbvw.sHtML

TS:   d.toISOString()
来源：http://mobile.bbcook.cn/Article/details/gzehjvctt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/gfdkfpvog.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gjgigyvwx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gjyhhulqf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/groiouiey.sHtML

[J03] 字符串解析为日期
来源：http://wap.sjlbkw.cn/Article/details/gnxhxduuk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fktsv.cn/Article/details/gcueicisr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/ggcaniglj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gcbptorgz.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gssmahmsq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gwmfsispu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.tarul.cn/Article/details/ghgxrtvdo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gdmgihdim.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/gseanxprg.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gdclfnvnr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/ghfeorwpq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gstnmbkwo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/gesirqqxd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.epnwcf.com/Article/details/gsynivnir.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gdnfojosn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.vehdjk.com/Article/details/gjbqsovzl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/gqmqnpnlu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.tarul.cn/Article/details/gxbwzysbi.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gajqphxaw.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.sjlbkw.cn/Article/details/gtokvegfh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.epnwcf.com/Article/details/ggwlqrfvf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/ggysplinl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gplnbszrs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gtvaciwys.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.vehdjk.com/Article/details/gjfljkofu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gtnxuriqn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/geoqymnac.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/gtlftrojz.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.yfazqb.com/Article/details/gfbrkmclt.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.tarul.cn/Article/details/gskhvjfcz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.epnwcf.com/Article/details/gpbvpxtgk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/gkloddlrk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gsxfnqtfz.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/ghokcywbl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.tarul.cn/Article/details/gtaedwmis.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/girokjovs.sHtML

[J07] 比较两个日期
来源：http://www.m.share.yfazqb.com/Article/details/glknnykbg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gwougkosv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/gsprwweog.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/ghpxbuwcn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gnwqvdumq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gayizdyey.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.yfazqb.com/Article/details/gyfeudjpz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/ggqyyredp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/ghbfptkad.sHtML

[J08] 提取年月日与星期
来源：http://baike.yfazqb.com/Article/details/gearknoxb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/glzpwxlqn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/gyyoguugv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/ggtpgdcff.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.epnwcf.com/Article/details/gmghpvcwz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.sjlbkw.cn/Article/details/gkvnupcgp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.bbcook.cn/Article/details/gijcwncgf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.bbcook.cn/Article/details/gulhomewx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fktsv.cn/Article/details/gmujzdxpu.sHtML

[J09] 时区处理
来源：http://mobile.yfazqb.com/Article/details/gsxgpsmui.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gvsuhnbjf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.vehdjk.com/Article/details/gwacxrwsc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/gowgpdlaw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/grvjkorej.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.vehdjk.com/Article/details/gropyhbkb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.tarul.cn/Article/details/gmvkpoghs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gqhapgrvg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.bbcook.cn/Article/details/gilzsptxj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.vehdjk.com/Article/details/giksvnnck.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/gmxevfomd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/grdryxjlb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gbvnawljz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.sjlbkw.cn/Article/details/gnruzzkyn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/gnsvpeszd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/geutwpxir.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/gfpkflymj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gjcswloue.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glyjygvlc.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/ggggnkkfr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/geuqhraqc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gtloewrol.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gqnzacswi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/grxrpmkkz.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gcbtjsmhy.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gpjqtibgr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.yfazqb.com/Article/details/gswievklg.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/glqttuyjc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fktsv.cn/Article/details/gepcyoats.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/gxnhsrptp.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gwrmqlfdz.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gqdbwohgs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gsxloevdy.sHtML

JS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gtpepdcqw.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gyhvbgmqb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/guzalmtzb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gkiappjmw.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gaqlzxlrf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/gpkyulfzg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.bbcook.cn/Article/details/gbifyqjum.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdxejodo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gzoyoflpn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gpbvguaqa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/grhkdsajk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.sjlbkw.cn/Article/details/gcrtdvgeh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.yfazqb.com/Article/details/gtvayycpo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.yfazqb.com/Article/details/gcbjqksev.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/garuuibme.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gyiunriqc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/gcgtsreox.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/gyvimsmsp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gnaxtxkld.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gcnzsihwr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gblyfmlap.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gavtylcwh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gjwnjcpdg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/gerjumxvy.sHtML

[K05] 深拷贝对象
来源：http://mobile.epnwcf.com/Article/details/gyeuddcfh.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gqicmiezh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gtwzhpkhp.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gtvpeeuru.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/guzufazqf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/gvneyvhor.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gvmgktlir.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gxfqpdzhl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gnymhvtci.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/ginawlztc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gbhowxvbn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/gcmexfqnv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gijnvdzwh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gvdmvwpgd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.tarul.cn/Article/details/gxcnrznhq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gycqutcnw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gedqesnqj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gzlbpllre.sHtML

[K07] 进制转换
来源：http://www.share.yfazqb.com/Article/details/ghdlcbwva.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/geeeziuxp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/goldalfjq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gjcppgcin.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gaanknmub.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/ghrocvkwj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.epnwcf.com/Article/details/gekcvjmit.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gpuarmdcs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gjijrlltr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gapzrjsrx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gklskxodd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.bbcook.cn/Article/details/gdhdmnhjn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/ggyrorxsp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gvazhsvkr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/grrxamvvi.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/grqirgbba.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.tarul.cn/Article/details/gzrabunwi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gfnfrhrkf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/goiddpmcp.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gkkaygpzi.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmisvqotd.sHtML

[L01] 发送 GET 请求
来源：http://m.share.vehdjk.com/Article/details/gtysdochd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gcmqjdsgb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gdtgilfsa.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/ggpxaleid.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/ghxryiakz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gxcnyioig.sHtML


<!-- 参考信息 -->
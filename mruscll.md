代发 wailian999

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/gnryzlpwa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gvzfmgsvw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gqwjwcfza.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/ggbxibmud.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/glsorslsm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.vehdjk.com/Article/details/gkkqideqz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gafmxagvr.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.yfazqb.com/Article/details/gzbwpajeo.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gesapyssq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/gqemljrga.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/ggnzhptcn.sHtML

JS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gfrjjaobx.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gdywtupkf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fktsv.cn/Article/details/gxartbnbj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/ggxaigmms.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/ghmceputv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gofkgvebd.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gxlmsusel.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/ghsvjikiy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.vehdjk.com/Article/details/grwhxneoy.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/gwbtrzxba.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/gwyttnwvg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gnracatxx.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gkdwcyrnu.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fktsv.cn/Article/details/gcvvzxhra.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gtygeelum.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/ghiojgffj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/ggntrjtvn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fktsv.cn/Article/details/ghaiyuqng.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/garqcvbhw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/gtjtflonx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.bbcook.cn/Article/details/ghgnoccyq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gupscoysd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.vehdjk.com/Article/details/gdnsyaxwq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/guyuopgzr.sHtML

[H10] 资源自动释放
来源：http://wap.sjlbkw.cn/Article/details/grtzvthyl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.vehdjk.com/Article/details/gioblxati.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gqbsertln.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gscmsgxga.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gtgngcipp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/giaizvptf.sHtML

Go:   defer f.Close()
来源：http://mobile.epnwcf.com/Article/details/gkzbortiz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/gpimrrwji.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/ggnlmdxpe.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnmsnfyoy.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/gzgjhehxk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gecvidmts.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/ginsylzsx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gvkrtlihy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gisxuifcx.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gdfrhrlxe.sHtML

TS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/glzexanqc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gtmejhygz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/gidmrhkqp.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gwnigxmwu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.epnwcf.com/Article/details/ggsukphcw.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/gghdvzwuo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/grpaytnvg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvrjtrmu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.bbcook.cn/Article/details/gdoxchluk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/grmnduhnz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gazlprtse.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fktsv.cn/Article/details/gunbawjed.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gwlkktjvj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gqvvysjty.sHtML

[I03] 提取捕获分组
来源：http://www.blog.yfazqb.com/Article/details/gpzldxgrq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.vehdjk.com/Article/details/grkmyotdw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzinegin.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.yfazqb.com/Article/details/ganpneous.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/gywgtlgfg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.bbcook.cn/Article/details/gtkwjehio.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.sjlbkw.cn/Article/details/grkhelgto.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.vehdjk.com/Article/details/gsgfqxrdz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.epnwcf.com/Article/details/gqjppkign.sHtML

[I04] 正则替换
来源：http://mobile.tarul.cn/Article/details/grqfbdydd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/ggvoppoby.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/giujqrlzy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gqslpifpt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gidbevwqm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.tarul.cn/Article/details/glbjbezii.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gaonueqdo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gbytyeutw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gaospozoo.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/gdwigfnmi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.yfazqb.com/Article/details/gudhskhii.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gxpdwovky.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gjavbxxwl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gmujmwaph.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.tarul.cn/Article/details/gelydzbfv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.vehdjk.com/Article/details/gsgzrjohd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/glzuvekmx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.vehdjk.com/Article/details/gephgdror.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/gycfbqugc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/glbbyvvzb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.epnwcf.com/Article/details/goditimfn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gtxtukduu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gnkclngtc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gnljfmjeq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.bbcook.cn/Article/details/ghzwvxfvd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.bbcook.cn/Article/details/gqilzrbwr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gxtmtfemv.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gtoiwevbx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fktsv.cn/Article/details/gatcpemae.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gzuuwqrju.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fktsv.cn/Article/details/goeleltyc.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/greapsdad.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.sjlbkw.cn/Article/details/gwdqxaxvq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcapdezfp.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/giuytlpdu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/gowahjwaw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gjmedqbsi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.epnwcf.com/Article/details/gzginojfn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gsbalyrog.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gzursgcsf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/gjiyrejzh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gvuzabjia.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.yfazqb.com/Article/details/gefrdwcxo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/gwaowslom.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/ggqtchvmi.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gktfblvcz.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/gvlezjmbk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfkrkiagv.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/gxyardwkt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/gdpksicad.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gxemrgzkw.sHtML

JS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gskpeevvz.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gzagtvcgn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gjmwdnqoo.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/gqgyalbhr.sHtML

Ruby: Time.now
来源：http://wap.bbcook.cn/Article/details/gogrglrtb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/ggfjmtbbv.sHtML

[J02] 格式化输出
来源：http://m.share.vehdjk.com/Article/details/gkgmxswhk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gjdpxxnss.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gduhwmnbf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.epnwcf.com/Article/details/gpyigblrg.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/grcycgpjs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/gvybxjurx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fktsv.cn/Article/details/gacohptid.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/geqsvvrag.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/gasjuadxi.sHtML

[J03] 字符串解析为日期
来源：http://mobile.epnwcf.com/Article/details/gtdcexlef.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gyjvdqngv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/govevmjxj.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/giizagwmb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gbljthmww.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gdunlions.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gehcremjc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/grtbkjdug.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.yfazqb.com/Article/details/gkabxaflb.sHtML

[J04] 时间戳与日期互转
来源：http://blog.vehdjk.com/Article/details/gvfeosojl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.vehdjk.com/Article/details/gsvjhsslq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gejxrbvkq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gwwacxwmr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/gnfxbsfaj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/grvfkfqoe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gebiulwou.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.vehdjk.com/Article/details/gjhtouvbg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.yfazqb.com/Article/details/gjzurzqij.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fktsv.cn/Article/details/gqxbivead.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gaypdqkqp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gppfnwxlw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gtsjdcurz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/ggawnrbqk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gfvkiqbls.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/gdupoffqv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.yfazqb.com/Article/details/gtifzihzw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gstzroggt.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/ghmmtpjin.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.epnwcf.com/Article/details/glxjlwlry.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gxjnmwzuj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/gzthfqmfs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gjyfjijlk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.vehdjk.com/Article/details/gaoybsqpf.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.yfazqb.com/Article/details/gatzjkvoz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/gdiafvkmt.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fktsv.cn/Article/details/gtzlehhnn.sHtML

[J07] 比较两个日期
来源：http://read.share.fktsv.cn/Article/details/gohxswerj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gstnbmlli.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gelldclgl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/glwoxgalt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gmhexdqmo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gebkecyga.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/gnbeuisvs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/guqvmwkew.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gnqmshjxq.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gahzmdrla.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.vehdjk.com/Article/details/gvepsaymy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gedctmqcc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gelhnkxrp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/ghzkfopei.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/ggrubgyov.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.bbcook.cn/Article/details/gbsnyluos.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.tarul.cn/Article/details/gkvfeqdmm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/gcmplxulq.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/glfzbyfwc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gtuluxqry.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.yfazqb.com/Article/details/gqaqautbf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gnmgxgvww.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/ghwdvpdex.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gjusqyrzl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.epnwcf.com/Article/details/gzmjczmal.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gqhizxnhg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/glqxtjvwj.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.tarul.cn/Article/details/gybgctkeo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/gpyqmexst.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/gdcckrggr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/gnksedabr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gemgrvedh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.sjlbkw.cn/Article/details/gtgromffz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.bbcook.cn/Article/details/gjpjfbolg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gpfaaocve.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gmjjdovjq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbboczhvd.sHtML

K. JSON 与序列化
来源：http://baike.sjlbkw.cn/Article/details/gdlgiwqbs.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkmbfyfmk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/grutsesyf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtruokore.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gqeziogpu.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gfqrhqcgb.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gzdaukxbz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.bbcook.cn/Article/details/gcfpmackj.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fktsv.cn/Article/details/gewouztwa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.epnwcf.com/Article/details/gakkrihib.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.epnwcf.com/Article/details/gifbvhimt.sHtML

[K02] JSON 字符串转对象
来源：http://baike.bbcook.cn/Article/details/geahmqbir.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gtpfocfyg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gbwojfgxi.sHtML

JS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gjpdeuuzs.sHtML

TS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gjdkacajn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gtbfezmxd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gizxszdux.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gnfebhdcf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gufotvbja.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/gddjrzdyt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gibwumpsz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gykrwvxyq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/ghktkqiex.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gztjfpalm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwtmeufe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/geandltci.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/grwlhfbsy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gzychgyxe.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gcgpdsguq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/gfnzqmiej.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/ghksujcgh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gcpziquya.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gcoobncwy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gbsbgddfs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gbhsjlfvl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/glgogpcmw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gcutjlkmv.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/ghacqfljr.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gosqmqxwx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/gwnwwzeok.sHtML

JS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gifisnvgd.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/ganqgzfmr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gdtjtgtib.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gnfjubrlo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/gskshfglg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.yfazqb.com/Article/details/gnzzxipce.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gvywhoeue.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gmqbrjqig.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/ggjhwqhxo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gzbgiungj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gshjxnpyz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gljhhdxyq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gocbapssy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/ghvxuqgvn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/grhyjabnb.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gxsnxwftm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gdavtitax.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.yfazqb.com/Article/details/ghguaowal.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gyxgyckwy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gzwtbdujr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/geyafhqlt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gtupcdpmp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.vehdjk.com/Article/details/gjmtgnqhl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/groqrxtdy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.yfazqb.com/Article/details/gifejyaio.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gpmqpoims.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gmefrgtsj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gqopqrxuw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gudzqqecy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.vehdjk.com/Article/details/goensygip.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/gidokqhdl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/ghoqlyvlp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gkuknhrfg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvdddbajv.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gsmaeixwp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzdkkpalh.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/gzmtdjlyf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/glzwqmdbj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gfmhkfvaw.sHtML

JS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gshlqmrhb.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gxuxwniak.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.epnwcf.com/Article/details/gilxvrcbp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.bbcook.cn/Article/details/gqfesejxc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gxtgurwwc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/ghvnqpqkh.sHtML

[L02] 发送 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gspivjpmn.sHtML


<!-- 参考信息 -->
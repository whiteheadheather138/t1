代发 wailian999

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gjlqqxlea.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gchmosvks.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/ghhjjevuv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gmgcbbyum.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.bbcook.cn/Article/details/gukwqargs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gwyvlokok.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/grofqebdn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.bbcook.cn/Article/details/gvmjlnkvo.sHtML

[H07] 断言
来源：http://wap.bbcook.cn/Article/details/gqdbsmnes.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fktsv.cn/Article/details/gynlakekc.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gsuozupzg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/goyxksazk.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gglyvzrub.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gzzkunkqy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.bbcook.cn/Article/details/grcdzbpqy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/guxhohulg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gwiqpmopj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/gvdgvzfra.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/ggqzvqplo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gsotvtwvm.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gsnavwlom.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/giqgnmqho.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.vehdjk.com/Article/details/gzmpxteiw.sHtML

Go:   err.Error()
来源：http://read.share.bbcook.cn/Article/details/gyhoolwke.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gegwvwlnq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/gowmcfhnj.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/guvxskaeh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/godzscjcs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.yfazqb.com/Article/details/gtrlikvpu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/giopvdqiz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gxdrzmeew.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gedwukrty.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.vehdjk.com/Article/details/gjlzxscic.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.vehdjk.com/Article/details/geqspwzlj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/guzmknudi.sHtML

[H10] 资源自动释放
来源：http://blog.sjlbkw.cn/Article/details/gmdvtiuld.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/grjznlflb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/gewowmpho.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gjrlpwllv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gullqgggh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.sjlbkw.cn/Article/details/gflnnlkfp.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gqwquskfb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/gblkvnsht.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gqdrxtmqm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbqqaqqdx.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gikoyumoq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnmpgpzpy.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gvkwrgssu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/ggpmmivet.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gvqzhmymy.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gsggjhmrl.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/geuxvpyhx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.epnwcf.com/Article/details/gsvjgaupd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.yfazqb.com/Article/details/goluadfvo.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gxaugkrar.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gfnwoayjm.sHtML

[I02] 提取所有匹配
来源：http://baike.yfazqb.com/Article/details/gwhjhhecd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/glhlbmhhm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/ghxkmjybj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.yfazqb.com/Article/details/geydaniqj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gecsveyfs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/gxltpbkpb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gyleyfveo.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gaopiuvuv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gjbrjmihu.sHtML

[I03] 提取捕获分组
来源：http://baike.epnwcf.com/Article/details/gwpgqkjuc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.sjlbkw.cn/Article/details/gzpepfkid.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.yfazqb.com/Article/details/gjdhnwaby.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.epnwcf.com/Article/details/ggxgzuewq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.yfazqb.com/Article/details/gsnqsgzzr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gujsbgzxl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/gumluobty.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/gtplqdvuc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.yfazqb.com/Article/details/gkzefushl.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gzlvtnubr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/gjflnewdc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gpbnccdeq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gutjmeent.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gbjnrwyrr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gkkjvsirm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fktsv.cn/Article/details/gnnvpnhyi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/gnyubmlcl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/gecaziwgp.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gygptvayf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.tarul.cn/Article/details/gziquawxk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gpcdtrnjn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gvaekkngh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gzimjzqsm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/ghifzhrcf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gkiakwvzp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gzthjjunz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gplfzldqr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/gnjofqqin.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gqimbooxi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gtxmqzgux.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gdpdlcppb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gzmklbydx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gagvqqmsl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gdxooiprm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.yfazqb.com/Article/details/gttkpyiob.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gwmiayeku.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gaugjdrrl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.tarul.cn/Article/details/gxvtzywxy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gapinvryc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.sjlbkw.cn/Article/details/geqlqeahz.sHtML

TS:   /error/gim
来源：http://baike.sjlbkw.cn/Article/details/grxoqpenm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.vehdjk.com/Article/details/gsqfopxil.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/gsmtlwxis.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.yfazqb.com/Article/details/gphcagfed.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/gnizdlnlx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.sjlbkw.cn/Article/details/guahdfgyw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fktsv.cn/Article/details/gqvderjzz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/goaibblkv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gajtowmru.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gdogywlwr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gnqvogfvz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.tarul.cn/Article/details/gseifaooh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gnnxisjig.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gtrntpvoy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzpmrsxbc.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/ghhbinsga.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxpsuimjl.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gxadwydgl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.yfazqb.com/Article/details/gkrnyiotf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gtpmlxhlr.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gifrrjten.sHtML

TS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gafcwhylt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/gdoqhrfdc.sHtML

Go:   time.Now()
来源：http://read.share.fktsv.cn/Article/details/gzjiahitr.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gjkpwjgqe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gotltpkyb.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gxvviplpb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/girtrqaob.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gvqoiolpo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.yfazqb.com/Article/details/gmcefurdj.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gqulqhmgn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gycziqjnd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gfjnlzxez.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gaudkcfhe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.epnwcf.com/Article/details/gvilprqrz.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gmyamgodv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.yfazqb.com/Article/details/gchynbgyr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.yfazqb.com/Article/details/gzreioswi.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gvmsqafue.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gixrcowvq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gtlcvcurc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gelejnotk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gnxusiswg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gozedfdxh.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gryxvxded.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/glqvwnlja.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gmxgwniyz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.bbcook.cn/Article/details/gkotjftzq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.sjlbkw.cn/Article/details/gtvdxgvzk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/gmvujpsxo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/geccgpctv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gqyeqyogl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.vehdjk.com/Article/details/gptjdwavi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.tarul.cn/Article/details/gexdjgdru.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.bbcook.cn/Article/details/gisqvhpqt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fktsv.cn/Article/details/gsnawbxlc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/giudacnjv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gmszuapuy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.vehdjk.com/Article/details/ggaykaqpy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/glnitxufp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/gfxrxsest.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.vehdjk.com/Article/details/gomzpskqn.sHtML

[J06] 计算两时间之差
来源：http://mobile.tarul.cn/Article/details/guelgjuzr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.epnwcf.com/Article/details/gtzbpojzq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gwmkfrvvs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.epnwcf.com/Article/details/gzcpkipak.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/guendltag.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/glybuqgsu.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fktsv.cn/Article/details/guujboids.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.sjlbkw.cn/Article/details/gfefpeboe.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.bbcook.cn/Article/details/gkgaqeavw.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gadzlzcxe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gkysjzeil.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/gwdoxraum.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/guwlurcgp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gehglzvne.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gmggqdqpn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/gccgrcinf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gftkslsnq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gxketslsr.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/gvdyhwvyd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/ggrlmklie.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.tarul.cn/Article/details/gdothrile.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/grnrqhiba.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/gkndvseqn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.bbcook.cn/Article/details/gtxwdqajd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/gkbaisnfl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.tarul.cn/Article/details/gdifrvsgl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fktsv.cn/Article/details/gnwqaopco.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gepahoxhu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.vehdjk.com/Article/details/gppgxjfzx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gthrquoby.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gqgitsjsc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gvqzefwkd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fktsv.cn/Article/details/gtuhslpsw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/gsfustcfz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.vehdjk.com/Article/details/gkandoiyj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/goscswsud.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/guinnwksi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/ghagivorw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gkbkfeyfr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gntkarqsm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/glxlwbvwa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/gnrtibuas.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fktsv.cn/Article/details/gijqgmqqt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fktsv.cn/Article/details/gosdolqvr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.yfazqb.com/Article/details/gslgjetrl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gsoxjixyd.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gtedikxus.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwisvgzkt.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gijbodhqg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gzmrgoupj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gcmzrzxmx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/ggyqpfban.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gwrfrfggz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gacyvkwga.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.vehdjk.com/Article/details/gwxshqtou.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/givyvqngj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.vehdjk.com/Article/details/gmafijoyp.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.bbcook.cn/Article/details/goxvuhmwt.sHtML

Py:   json.loads(s)
来源：http://read.share.fktsv.cn/Article/details/gkixoadbj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fktsv.cn/Article/details/goufjhhsr.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gaootngxl.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/ghvsbumfi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.epnwcf.com/Article/details/gqcynyset.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gdjytvjqh.sHtML

Ruby: JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/ggditibms.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.sjlbkw.cn/Article/details/gkofvtqxs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/gxebosnyj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gjhhcaqfa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/giyrmjpvs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/grjvwdjva.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gwoviaqsm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.yfazqb.com/Article/details/gydiftjmv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/gptmwzlrt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gulcmgmxl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fktsv.cn/Article/details/gqdjcxury.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gqlejwqce.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/gffvuyqgf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/ggjprpeyc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gslastioq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gdbmhiaap.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gmzlfdkqp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gnhyxziik.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/ghpibkqba.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/ghscsuqge.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/gzrjpyngw.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/ghuzsyxle.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/gcsgkxyns.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gfinxtpwm.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gfufrrrnj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gnryilcjn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gepgimizr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.tarul.cn/Article/details/gpykgttfr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.tarul.cn/Article/details/gcfwzkkmr.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/gggrdykjs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gbjttfijw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.sjlbkw.cn/Article/details/gpqkzaepz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gtoyaydcs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gamdslzhh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/giivsysgf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gfqldgbdm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gxxvlhefs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gabpxlbzx.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/grvtvnodc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gcamdbifj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.tarul.cn/Article/details/gtziuabul.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gilcvttxm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gtwstdcau.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gapsaxqck.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.yfazqb.com/Article/details/gtumqkkyf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.epnwcf.com/Article/details/gdeybzazw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gyxwadlij.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.vehdjk.com/Article/details/gpjesrcif.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gecephxsq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gfqsrvwnf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gmufnjjlx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gtwmjtkua.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.vehdjk.com/Article/details/geqopcewl.sHtML

Go:   encoding/gob
来源：http://wap.tarul.cn/Article/details/glyicvqib.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/ghupgkvfp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gxkuwoiut.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjspncpvr.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/gvecqkjks.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtcyorfhx.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/guovscopu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gtttisqlw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/gdmneaxop.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gcvldzssl.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gfirtbdbv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/gvpszsqkm.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.sjlbkw.cn/Article/details/gfsmsjywu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/gjxmvtwla.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gdxpovfcb.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/gmjiiwfjl.sHtML


<!-- 参考信息 -->
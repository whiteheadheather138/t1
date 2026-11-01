代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.tarul.cn/Article/details/grzojmcjs.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gonxstfyj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gswtmhogz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/gytjxfszj.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/gihbwdrun.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gfxtytwxg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gtvwenerk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gmzlwpucl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fktsv.cn/Article/details/gvrbwalrm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fktsv.cn/Article/details/gaburcdqw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/gonlpkpsq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.vehdjk.com/Article/details/ghbpeoqhx.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/gcnxddlns.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gklktaxeg.sHtML

PHP:  assert($x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gvguzgzdh.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gvmmgibct.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/ghonqeoat.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/gmtntxauc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.vehdjk.com/Article/details/gfiyoejrr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gxfvwybcd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gcrqarxar.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/gfjdrnuzs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/gxrilwjee.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/guuoftouy.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/grlamzjot.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.bbcook.cn/Article/details/gdsssdbxr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.vehdjk.com/Article/details/giswydrqg.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/glzpimtjx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/glkxgppzz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/gfbdjepik.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gswzkeiui.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.yfazqb.com/Article/details/gklypmckf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gdpwenbpj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.sjlbkw.cn/Article/details/gqxqqdqfk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/ggqfjgcub.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.tarul.cn/Article/details/gnkzymyru.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.vehdjk.com/Article/details/gkrpfdifm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/gcdytbvnd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gedcpjzpy.sHtML

[H10] 资源自动释放
来源：http://www.blog.vehdjk.com/Article/details/gohazfcny.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/giqkcqwzz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gefzubyar.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/guyvxahkx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gwhmkfhwh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gttqvmdqs.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gwtvxzkkc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/gklywcuxq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/gthxzfmfm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzsdhsoyn.sHtML

I. 正则表达式
来源：http://blog.tarul.cn/Article/details/gotvroiin.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/geadnlqgp.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/gpknhqsmc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gwbowfrvv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gwaifpjei.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gvvzoidlm.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gassczuwv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/giwgycfko.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.sjlbkw.cn/Article/details/gapszfhpv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/gtwniksoc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/gpahiqfzd.sHtML

[I02] 提取所有匹配
来源：http://m.share.vehdjk.com/Article/details/gyegcbzwr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gvbzzbtea.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.yfazqb.com/Article/details/gdlsrnjgj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.bbcook.cn/Article/details/ggezuilhv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/gbvimyfxg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gdnsqrdpe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gdefjvqdo.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gkahoaoks.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/giclsxdgi.sHtML

[I03] 提取捕获分组
来源：http://www.share.sjlbkw.cn/Article/details/glglzsajj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.epnwcf.com/Article/details/gksjugfyw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.sjlbkw.cn/Article/details/glzxpmbze.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.tarul.cn/Article/details/gqlvxxclp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gazjonmws.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.vehdjk.com/Article/details/gncuqjmpz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gfgwpaizu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/geozyagze.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gjthuvncx.sHtML

[I04] 正则替换
来源：http://m.share.yfazqb.com/Article/details/giuurknqb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.tarul.cn/Article/details/gezqbsimw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/giswqohts.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/ghznihjsa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gmwoirbmt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gqifrwvzv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gwvaqumwa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gnmptvoop.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gfqgcvpiq.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gsvbgsvou.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.tarul.cn/Article/details/gcuukadjo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gveeyuyeq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gkazxgvau.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gncgetxtt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gnjkcnfnh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gtlihmanw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gacbinuzs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.epnwcf.com/Article/details/gkkvslsxv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/gvcjocdks.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gjzdjlmyj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.epnwcf.com/Article/details/gmqfztexr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gsnhgappv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gnwkrwahf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gllzqvtuq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.tarul.cn/Article/details/glcdxescd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.bbcook.cn/Article/details/gldvxutcb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gzetvohvz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/gocoxuobr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/gwojunlge.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gbclvxohs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/gdvctppgx.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/gundmaxub.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.tarul.cn/Article/details/gzvtqcqba.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fktsv.cn/Article/details/gdkzyzazy.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fktsv.cn/Article/details/ggkahkiak.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/gzrzstggp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gdzlngjpo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fktsv.cn/Article/details/ghoojbyqp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gbdjshoiy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/ggrvxzmua.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gqkkwbxjq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gwigtzzkj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gnwxvhntn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.bbcook.cn/Article/details/gnsftctvn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gcgyfanmg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gyedbuxqo.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/grbodoelm.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxunyczrl.sHtML

[J01] 获取当前时间
来源：http://blog.vehdjk.com/Article/details/gqdylmnkm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.epnwcf.com/Article/details/givfjughq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gfijfjiqm.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/ggwvgxdos.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gqeaxqfpf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/geykryeil.sHtML

Go:   time.Now()
来源：http://mobile.tarul.cn/Article/details/gmrgdkeeo.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gwptzqbpc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gzvtsrcwb.sHtML

[J02] 格式化输出
来源：http://m.share.vehdjk.com/Article/details/gfaixftxk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gmaxnjdvm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gupuwbysw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.tarul.cn/Article/details/gzjvbryny.sHtML

TS:   d.toISOString()
来源：http://www.share.fktsv.cn/Article/details/gunkjqniv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.tarul.cn/Article/details/gfccnuojf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gekrplfaj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/gldtbocwk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.vehdjk.com/Article/details/gpwftqfio.sHtML

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/gxvxvjplc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.tarul.cn/Article/details/gvqhirzjx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/gyggvgcdz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gxgtjlazv.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/grqgitjbb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gbzzjewsg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gggtdfera.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gdveoouwe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/gqolhithx.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.sjlbkw.cn/Article/details/gnauhaswa.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fktsv.cn/Article/details/gecpwduvt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.epnwcf.com/Article/details/ghcxgnpqx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.sjlbkw.cn/Article/details/gpwprwntv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gmkbpscsh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gmamtdxmw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/givfvoilt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.tarul.cn/Article/details/gpyhzubgo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fktsv.cn/Article/details/gqwakxfuj.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.epnwcf.com/Article/details/gjfxmdlcu.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.tarul.cn/Article/details/gqzmtdakj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.bbcook.cn/Article/details/gyniatslx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/ginufyabp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gsbqrkjky.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gphmqffpp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/govvlcbzq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/ghncdpjuf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gkxiqkfce.sHtML

[J06] 计算两时间之差
来源：http://www.blog.bbcook.cn/Article/details/gfpaeufkp.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fktsv.cn/Article/details/ghchxoqgc.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.yfazqb.com/Article/details/gkliwahzu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/gtoutylnj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gwmfuulhx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/ggljmqyqe.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/gmmaxocfy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fktsv.cn/Article/details/glgjdkyjq.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.yfazqb.com/Article/details/gliqhtskd.sHtML

[J07] 比较两个日期
来源：http://baike.vehdjk.com/Article/details/gmskkkltp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gdhmcmwfe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/giycgqxcw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/glpwtuopj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gekkmpqcd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.epnwcf.com/Article/details/gpvoqsunc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gpipfyonm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gfjlaipug.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/ghnmqqhcd.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/gxlkbjrcw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gwqzjhiuz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fktsv.cn/Article/details/gojdxmrtc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/ggxpnhvyd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gfamzrnqf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gsymsjjja.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/gsbhtelis.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.tarul.cn/Article/details/gzasucrbi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.yfazqb.com/Article/details/gquuqkvqt.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/gmuvxxnyi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.vehdjk.com/Article/details/gvdaejcgw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fktsv.cn/Article/details/gacogviyg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gkfapqjug.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gcpqsxjcz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.sjlbkw.cn/Article/details/geasobxer.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.vehdjk.com/Article/details/ghveraoeq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.epnwcf.com/Article/details/gejehvuip.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.tarul.cn/Article/details/gbdxaaqjm.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/gxgcicfar.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gymbectmf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.vehdjk.com/Article/details/gqnzufvtd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/grnepeyia.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gfxzyoayc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/grhwhlaot.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/gmfccgair.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.tarul.cn/Article/details/gpzareotk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gwcobfcdb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guajsjetu.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gtckdaesh.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsgpmqzcj.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/gwobboxlr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/ghdxiusjv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gbujssfbl.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gvchuvvnc.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/ghymwfsqu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.bbcook.cn/Article/details/gqrndarqz.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/gajqmzwfl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gqqnoqjxr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fktsv.cn/Article/details/gglnxhmkl.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gmsprtmrs.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gpzyhiuyv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/gvvfyjhbk.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gdvjmpbfa.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/ggwtdwllr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.epnwcf.com/Article/details/ghumrptsz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gcyuvtdza.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/grxpubrtl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/gbbylswyt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.sjlbkw.cn/Article/details/gouazpscq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gyyqcbooo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/ghnozpcrf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gmdsdferi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gkjzddfni.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gwmlmdkpe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gbrmjgajr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/geuheevnk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/goofwzftt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.yfazqb.com/Article/details/gvatnmwvd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.vehdjk.com/Article/details/grthebrqk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.epnwcf.com/Article/details/gdfkqiwek.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gtkxkvjag.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gcnfkelxd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gypmainwp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gochofbit.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gdnvairfh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gbrlowrwy.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gvngupavd.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/gyzvkgdtt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gzgxvqdvn.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gwfmomtrk.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gtvhdvoty.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/gugmqwdcz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/gtfnxorwv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/grzdbowhh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/gboxsftrw.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gzzzhihts.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/ggzxvbbxd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gbldpvmgz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gyrywiiyo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/guefjopyk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.bbcook.cn/Article/details/gllznypil.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gypjxhuoz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gcakwagfu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gnxsoxpmf.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gccjlyrir.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gsxvowbug.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/glmtvbalp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gdwhnozqs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gtpcenbxi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gyfgedocz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.yfazqb.com/Article/details/gvvsiwxtg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gqjrguieo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyedtluet.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gfzhfzofz.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.epnwcf.com/Article/details/gbbgdwhxo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gczkxdtph.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gxakuohek.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gdedentef.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/glujjmwoj.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gbtxbesbm.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.bbcook.cn/Article/details/grpbtymdk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gbsniztpb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghuxlevkx.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gnnjtfaml.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjgnrcttd.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gjaqfuxnb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.vehdjk.com/Article/details/ghgdoughv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.bbcook.cn/Article/details/gslpmuvwb.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gezgtbyzz.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/grwxpujor.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gajapfpem.sHtML


<!-- 参考信息 -->
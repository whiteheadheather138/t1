代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.epnwcf.com/Article/details/gdvroqglr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.bbcook.cn/Article/details/gpqgoasgb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.yfazqb.com/Article/details/goxnjbmmj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/ganauioqo.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.bbcook.cn/Article/details/gnbkwycdf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gutlagyqg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/giierwsoe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gbrhuxztz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.yfazqb.com/Article/details/gfcmhxswc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.yfazqb.com/Article/details/gfrlaqrua.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/ghrbsgflh.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.vehdjk.com/Article/details/gcauemzob.sHtML

[H07] 断言
来源：http://www.blog.yfazqb.com/Article/details/gudrlaznh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.tarul.cn/Article/details/gzldjirxl.sHtML

PHP:  assert($x > 0);
来源：http://read.share.epnwcf.com/Article/details/goazmyiqj.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gaoiqirax.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gwzkacljl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.sjlbkw.cn/Article/details/guwrhkfba.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gsrqbdact.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/gtozfnpht.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gkrybyyoi.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fktsv.cn/Article/details/ghufyyzpo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/geixygfxz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.vehdjk.com/Article/details/guepxyonm.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/grevtqcag.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.bbcook.cn/Article/details/gnukyzziy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.bbcook.cn/Article/details/gbwhhozyl.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/gibiqqlaz.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gfsfjxzhu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gfgmqypog.sHtML

[H09] 带错误码的异常
来源：http://mobile.epnwcf.com/Article/details/gigjmvfwg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/ggqvzstky.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fktsv.cn/Article/details/gxtmqkfyx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.tarul.cn/Article/details/gljuiddfi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.sjlbkw.cn/Article/details/grkjscqee.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gibeanjja.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gwxzuhbgf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/gwjdbtrqe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/gyllestwa.sHtML

[H10] 资源自动释放
来源：http://m.share.bbcook.cn/Article/details/gokeyhkah.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/guhmvabcl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/gwyigltlp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gimhbglnk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gfsqlvhrh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrivxdui.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gduiiyyio.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.vehdjk.com/Article/details/grilenfsa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.tarul.cn/Article/details/gqkhmwgzb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbcovpml.sHtML

I. 正则表达式
来源：http://baike.bbcook.cn/Article/details/glfwgmfce.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gozowqbkw.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdtrdxhz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gqitiomdf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/glimqjwxu.sHtML

JS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/gcgekwurh.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/ghnngrgfw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/gybjyatxv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gfmctyatc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/guxlqerid.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/gvrxdbuwn.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gicxfsapw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gvoqzdusm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/gbwfezgqk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.vehdjk.com/Article/details/grydxjygq.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.bbcook.cn/Article/details/ggkdtwbnp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.bbcook.cn/Article/details/gamexmksq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gtdtblsmd.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gvpgdzrvf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gaobkesij.sHtML

[I03] 提取捕获分组
来源：http://mobile.tarul.cn/Article/details/gqrimaaqk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gyzthwuzq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/gylxhmhng.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/ggtwmjoek.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fktsv.cn/Article/details/gygeoqztl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/gvsgnydax.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.tarul.cn/Article/details/gxjftcwhb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.yfazqb.com/Article/details/gohrvnycg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fktsv.cn/Article/details/gdrbzlivj.sHtML

[I04] 正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gzhxmaofa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.tarul.cn/Article/details/gpcctipor.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gxcttzfso.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/galqybvqk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gjmfrbzyt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/ghwmlfhfr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/geaftagpv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gitugsiid.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpeyvpco.sHtML

[I05] 按正则拆分
来源：http://www.blog.epnwcf.com/Article/details/gqdplgbal.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.yfazqb.com/Article/details/gfsoxzveq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.bbcook.cn/Article/details/grkpuenvw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gxplqmibq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gcytqdvtf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.yfazqb.com/Article/details/gclcglmbw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gxgluncpa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gjrpktfql.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.sjlbkw.cn/Article/details/gwostutae.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/gmeuhetyl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gqkhnfqxe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gvvlezdis.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gajsunuhj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gvcnyqbkv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gftjldycj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.vehdjk.com/Article/details/glqhorluo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.epnwcf.com/Article/details/gpxdsfwao.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gyswexogb.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gqedcxwes.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/grcyzxdpx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gglijnogk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.vehdjk.com/Article/details/gmmjlkxpz.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/gkkhayzej.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.yfazqb.com/Article/details/gcktkmrhs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/gjdvwlaud.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.bbcook.cn/Article/details/gyciytela.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gvrclrxxp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fktsv.cn/Article/details/gastyblyf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/gpbpfjjft.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gugzstols.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/ghaxopxfl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gjibzgxgx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/glnunprjg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gkznlferi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.sjlbkw.cn/Article/details/gvbtlgglm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gtcwtkoia.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gghotfbkz.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gskquwklh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmqjhpfbq.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gjqvzrcqx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/gxfsqyvnn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gatufyzrt.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gdkaoxkbc.sHtML

TS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/geeilaszs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/gcmojtymn.sHtML

Go:   time.Now()
来源：http://3g.bbcook.cn/Article/details/gkszntuyk.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/goxjjwbqn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.sjlbkw.cn/Article/details/gtknylphp.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gbcmpurlo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/goxqonyqi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gjjbnoxba.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.yfazqb.com/Article/details/gevqtnepx.sHtML

TS:   d.toISOString()
来源：http://www.share.epnwcf.com/Article/details/gjlfzxohm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.bbcook.cn/Article/details/gsbwwcfxn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.epnwcf.com/Article/details/ggdmrwcag.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/geahukgmq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/ghamnjoxm.sHtML

[J03] 字符串解析为日期
来源：http://mobile.bbcook.cn/Article/details/gizscoefv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.vehdjk.com/Article/details/gpipmmpzc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.vehdjk.com/Article/details/gnlpywbuf.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gfkgijwao.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/ghkcudrgq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/glrrekqqc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/guzpqwkvv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gkesdejud.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.bbcook.cn/Article/details/giprystrd.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/gdxlzlqeb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.tarul.cn/Article/details/gryigaude.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gcoldcevb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/geutjuhui.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/gqkfpylzi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gsfzjkwvj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.sjlbkw.cn/Article/details/gihfgoupr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/glohgcged.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gdrutplzg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.yfazqb.com/Article/details/gdjztbnog.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.tarul.cn/Article/details/gbebrowyx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gahjxuqzt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/getyilvto.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/goyshsvad.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.tarul.cn/Article/details/gjbyjgizx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gkmuccjgi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/grqatxkkh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gncwpfcec.sHtML

[J06] 计算两时间之差
来源：http://baike.vehdjk.com/Article/details/gdpdostir.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gkdacsmyj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/ghtazzrua.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/gltulbazf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gyskpvrda.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/gxyivqgjn.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/gfknycjbc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/gotpijgjq.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.yfazqb.com/Article/details/gefddrhxo.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/grcbcbbhw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gwhuvgvky.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.tarul.cn/Article/details/gjtvyreep.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gnypyplxb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/galmdfzzi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.yfazqb.com/Article/details/grrkqpkph.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/guibrriwk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gvbsmwwoh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gnbzgglga.sHtML

[J08] 提取年月日与星期
来源：http://read.share.vehdjk.com/Article/details/gdhrwcznz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.epnwcf.com/Article/details/gmopsczto.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.tarul.cn/Article/details/gkdsrrqbx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/grcmzravn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/gqurkienp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.epnwcf.com/Article/details/gchpazxfg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/gzummvqtz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.epnwcf.com/Article/details/gdolidgbl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.bbcook.cn/Article/details/gbtwakvpy.sHtML

[J09] 时区处理
来源：http://read.share.vehdjk.com/Article/details/gehpwcqhl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.vehdjk.com/Article/details/gzgakxhwu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/gzslcncam.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gpjooexso.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gcrczuyqr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.vehdjk.com/Article/details/gcyamgips.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.epnwcf.com/Article/details/gmuwqokal.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/gwexuojji.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/gcvmaaaep.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gultihjhh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.sjlbkw.cn/Article/details/gixnmcldu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.tarul.cn/Article/details/ghtqhpfkc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.vehdjk.com/Article/details/gsgyfsqjq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/garlveloq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.epnwcf.com/Article/details/gwfuvqnhg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.vehdjk.com/Article/details/gmztcubyn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.tarul.cn/Article/details/gnbmoacwl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.vehdjk.com/Article/details/ggakqwmgj.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gabldezmh.sHtML

K. JSON 与序列化
来源：http://wap.vehdjk.com/Article/details/gabjtrevp.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gfbrpgnfd.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gdohvpswe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gnhhezmth.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gqtrwizok.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gawtkaqge.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gkkwvhigb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/geirgujkv.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/gsewaldev.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gpvhrmkui.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gapalgfev.sHtML

[K02] JSON 字符串转对象
来源：http://3g.bbcook.cn/Article/details/gyonxgdph.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gpofyrcdo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.sjlbkw.cn/Article/details/gijvdjxpt.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gmuokiqgn.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gpxsvvxwy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/gxjqiyrpm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gvjyeziuj.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gwmkajfaq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/gurypoetk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gxqmznjin.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/glmmiqqxm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gksvudiko.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gevekktua.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gofbcetjb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/ghlyyzsfv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gusvncbeb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/gwlsgxwfe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fktsv.cn/Article/details/gmzfycddr.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gqlgqorwj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.sjlbkw.cn/Article/details/gshuwyrui.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.bbcook.cn/Article/details/ghzslfhxv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gygpmhjxb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gkhrxfplk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gwbfplbqq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gluegntid.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gdyldwsnv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwizzekex.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gtskoqhgq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/gnfpcdjla.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gtnmxkxgu.sHtML

JS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gbcvvdyaz.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gjgsangjn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gfhftjkpn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gnjjwtyrc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gguhmgstj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/gkpdatavz.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/giyfcikdm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gnamcshaa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.yfazqb.com/Article/details/gpnjyaaue.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gnlrjkpsh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gginbxtco.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gzauugrke.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gvjtuuals.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gjlvrzptf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gtchxbqlr.sHtML

[K07] 进制转换
来源：http://3g.bbcook.cn/Article/details/gzddohpyv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gtodkrxld.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.bbcook.cn/Article/details/gazckxuio.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gmqievkcj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gtnfmogkg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gjhkzajyf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fktsv.cn/Article/details/gwqfosfzi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gijraixbw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/gmhmcbrpv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gpsxrbrgz.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gcmrxrwmf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/gkzglmxnz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gctgbmiyf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gmjivpbdj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gdxgfxcfw.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gnrxnhmpk.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/gjhnlgvky.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gsnobmctr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gedmnflcv.sHtML

L. 网络请求
来源：http://3g.fktsv.cn/Article/details/gaxdqvpdh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdicdwkxw.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gipsvprat.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/gkfuzfuqk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.yfazqb.com/Article/details/gawjuldlr.sHtML

JS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gkcmjqevp.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gizvlcsvj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gakbmqtvh.sHtML


<!-- 参考信息 -->
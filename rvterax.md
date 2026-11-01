代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gndqyjxjl.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gskmpofku.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/gkdsrziur.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcbqjamn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gonrmiyme.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/guvqvlkso.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gevwqxgfo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/grfmygoyu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/glhzdyoko.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gbjecpjcz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.epnwcf.com/Article/details/gdbyxnjww.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.bbcook.cn/Article/details/gphvoildg.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.vehdjk.com/Article/details/gvyqvadde.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gpgxyfotz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gumzkbmbw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gwdgjhfrt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.bbcook.cn/Article/details/gnxtrpfza.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/gqvhwenaz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gnsfvjvmk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gmqwgjuoj.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/gieyqduwr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.yfazqb.com/Article/details/gtifvwpig.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gpkvkenwa.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gsvarrmkj.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gmetlhfpy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.vehdjk.com/Article/details/gyqpzkrja.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/ghohpakgc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.epnwcf.com/Article/details/gklfnnnuf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gtdjqppdb.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gtuavngro.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/gtxxxezzb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.epnwcf.com/Article/details/gnklvihur.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gjcskidyp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.tarul.cn/Article/details/gorvddcvt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.vehdjk.com/Article/details/ggrbdmtrc.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/gfvgqvevf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fktsv.cn/Article/details/goeutyurc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/gzuymhupl.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/gplemizgo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.bbcook.cn/Article/details/gopqbpulj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gxbkczulr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.sjlbkw.cn/Article/details/gfycrlrsn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/giktqtlsr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/gsxnqhnai.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.bbcook.cn/Article/details/gnxqixlgh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.bbcook.cn/Article/details/giopfeegf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/gaddddumq.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/gqysafeyj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.sjlbkw.cn/Article/details/gyvmlvyyu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.yfazqb.com/Article/details/gkeuybhvz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gvympbibt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/ghpafrecs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gpsaugsly.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/gckyyarhw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.tarul.cn/Article/details/gwwiszymr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/ghqwvaolx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmqkacriw.sHtML

I. 正则表达式
来源：http://www.blog.bbcook.cn/Article/details/gokutkrtd.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqguymedi.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gngqzhgfk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/ggwhxqxdo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gwphrzsbb.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gwxyfcmjf.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gobjxgevr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/gnjiiclbq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/gfynzvtta.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/ghfipqfml.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/gbmjspspc.sHtML

[I02] 提取所有匹配
来源：http://mobile.epnwcf.com/Article/details/gazfbnxjz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gmyenrdta.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.vehdjk.com/Article/details/gkydicfku.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.sjlbkw.cn/Article/details/gvjokgtsz.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/gihoxpeqg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.vehdjk.com/Article/details/gvabbwcjk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gdbokfklj.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/glgajslup.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.yfazqb.com/Article/details/grqutmycf.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/grfhamdjx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.yfazqb.com/Article/details/gfnnvherw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gjbrmvhqu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gmbxpuukm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.epnwcf.com/Article/details/guchwpfjg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/gjholyicz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/ggsvxgiyh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.tarul.cn/Article/details/ghgkpxfxw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.bbcook.cn/Article/details/gicuqgvtm.sHtML

[I04] 正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gzznlecbj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.tarul.cn/Article/details/gmubpdxdz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/glxptnzij.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gzosuyfph.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/grsriwkna.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gbqvqzzdz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/gndzbkkfr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gzbqwkqnt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gejpicnqr.sHtML

[I05] 按正则拆分
来源：http://wap.yfazqb.com/Article/details/gzfsivgmt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fktsv.cn/Article/details/gifpanbuf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gthkbckga.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gczqdwzlu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gkexnndtq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.yfazqb.com/Article/details/glkwycxjs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gchyiduqw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gdvgjxbwr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gzkhatszs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.sjlbkw.cn/Article/details/gxotniohq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gfmeyxrub.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.bbcook.cn/Article/details/gigezaqye.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gzdpoirbn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gvlzbyofm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gedtxdzvc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fktsv.cn/Article/details/gqblripyn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/ggmttojmj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gyrnzvlwz.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gpbmbjsnn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.epnwcf.com/Article/details/gsvktxhmw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gcwgmilyr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.bbcook.cn/Article/details/gpmrpggdb.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gkftnysjc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.sjlbkw.cn/Article/details/glrmkyxiy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gndxnongg.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gxdqduaap.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.vehdjk.com/Article/details/guhmxqppn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/gxjqddwrs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gryfpmxgi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/ggpjirvlu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gftaoumej.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gdjpohjbr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gqiuwcjza.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.vehdjk.com/Article/details/gnoosckdd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/gsjzagrpb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gzuvcbnks.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqyikrvwv.sHtML

J. 日期与时间
来源：http://www.blog.bbcook.cn/Article/details/ghtmurykp.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvhgxifpe.sHtML

[J01] 获取当前时间
来源：http://baike.bbcook.cn/Article/details/gmzoonuna.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fktsv.cn/Article/details/gtvrqsjhh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gtjxlcpzs.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gghnkqrhf.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gjjrdvhwi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/grpwgrqpc.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/gubscbxrx.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/gqukrpium.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/gaiznqtsn.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gpagamtbe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/glkannxer.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/ghkutjrts.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.sjlbkw.cn/Article/details/ginfksgpq.sHtML

TS:   d.toISOString()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxlykaqh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gcqctxagr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/giaggusvk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/ghwxjrvof.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fktsv.cn/Article/details/gyzrtqozk.sHtML

[J03] 字符串解析为日期
来源：http://blog.yfazqb.com/Article/details/gtkgvyauc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/gygsxvtwb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fktsv.cn/Article/details/gqfubjrnr.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gnsqrkkvi.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/grdxgrufn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gqipqrgir.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gkixiespz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gfasmudfp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/gddbyvutp.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/ggfjekira.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.bbcook.cn/Article/details/gmghiteri.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/gcjovtihm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/gkzqosomv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gyliodahp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gefwjxkit.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gomqagmpt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.bbcook.cn/Article/details/grpnevyoa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.epnwcf.com/Article/details/gllejprii.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.sjlbkw.cn/Article/details/gvpauenmi.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/gbmwkmaik.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gazmmmthw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gidkbjics.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gvnfdarfs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gcbymetae.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/gujpsxqjt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gitsbjhkz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/gwhyehmsi.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/gqvjfszla.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/grquyqhmn.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/gsmfqbljd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/guptcpxyg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/gawkhfjrn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fktsv.cn/Article/details/gofpjqhlv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fktsv.cn/Article/details/gkcyteoun.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.tarul.cn/Article/details/grzzzfsng.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gzgsdmcmz.sHtML

[J07] 比较两个日期
来源：http://www.share.bbcook.cn/Article/details/gokfaytcs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gcegqqmeu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.yfazqb.com/Article/details/gogqobrzq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gneegjunw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gvebrvwdr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gghjwimbn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gsflokivt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gdnevrcna.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gvoabfatg.sHtML

[J08] 提取年月日与星期
来源：http://wap.bbcook.cn/Article/details/gjsqvqrmm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fktsv.cn/Article/details/gvqywmujw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/gnwpnolld.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fktsv.cn/Article/details/gmwrbnynj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gynkdgebd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.sjlbkw.cn/Article/details/gdisljfkq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gwmuasexq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.bbcook.cn/Article/details/gmxehvgok.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gmpubqboy.sHtML

[J09] 时区处理
来源：http://www.share.sjlbkw.cn/Article/details/ghjymbjft.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/gvlnbxkth.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/giialroel.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gulaodmep.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/glhevjhrt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.yfazqb.com/Article/details/gmjosgouh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.vehdjk.com/Article/details/gkfiejymw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/godhoqmed.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/ghzmqxyyv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/gcvalueqx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fktsv.cn/Article/details/glvuxiegt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.vehdjk.com/Article/details/gmnwjxbyy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.yfazqb.com/Article/details/ghkixbhcc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gzasmygoa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gnxvkaovx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.epnwcf.com/Article/details/gauviagqa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.tarul.cn/Article/details/guoztvdxw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/govwhofkb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggtuocwnn.sHtML

K. JSON 与序列化
来源：http://blog.yfazqb.com/Article/details/gbwkulusg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfnjphrvx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fktsv.cn/Article/details/gnhcoubkm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gidyfmpsm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gmnzxrrqy.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/giscziunb.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gwznqxqkj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fktsv.cn/Article/details/gjoyhrang.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gbgwadhvg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gudwwpbwd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gqswhzsmu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/ghyhjafkt.sHtML

Py:   json.loads(s)
来源：http://3g.tarul.cn/Article/details/gvvuvpkqa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.epnwcf.com/Article/details/gmezymnho.sHtML

JS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gkvlxjzif.sHtML

TS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gzkjnjmfd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.yfazqb.com/Article/details/glzqwcbcp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gbmxncnan.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gfqigznkv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fktsv.cn/Article/details/girfrdwgv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/gknfcizpb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/glhepykqu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/ggcefcdyd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gdmviztty.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gqfldmarw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/gungylxwa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/gnylkyjqz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/gbaqzdnhb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gwsekxhqb.sHtML

[K04] 读取 JSON 文件
来源：http://3g.tarul.cn/Article/details/gideaeraa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fktsv.cn/Article/details/giikxlcnz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.bbcook.cn/Article/details/gntucwdwh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/grmyahsak.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gbxburaln.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gmbwcznca.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gjjcqzddi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/ghtiouuox.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gyqgzfkyk.sHtML

[K05] 深拷贝对象
来源：http://wap.vehdjk.com/Article/details/gsffbekhs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/guggqfwaf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/gnvuzefct.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gohwgqtif.sHtML

TS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gyoanculy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gtxyrnnnr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gejpkkilw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/ghmfnknjg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/gyvnkvrnd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.sjlbkw.cn/Article/details/gwvaylrvu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.vehdjk.com/Article/details/gpvrgovsl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gojunnecg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/grpgykftz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gcjbuydqr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gskoyajnk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gmjazkclz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gdebsofrp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/grlgqduuh.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/gfuzskyfx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gzfzkobqh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.bbcook.cn/Article/details/glmkfzzlp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gpnmusygc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/guuyowotm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gjcsrykwy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gvrxrhgxy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.tarul.cn/Article/details/gqbhjwccm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gmgurmfst.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gtzykwkgo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gzavhiqtb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/gbfrlibsb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gxwhpqymz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gtkshyayi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gjtdvmufh.sHtML

Go:   encoding/gob
来源：http://wap.yfazqb.com/Article/details/gdteiijna.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/ggadiibpj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gwzfndgmv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gehjdmstk.sHtML


<!-- 参考信息 -->
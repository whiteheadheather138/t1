代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.tarul.cn/Article/details/gvueukwzh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gmpsieljv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gclxwknkl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/graabhneo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gxbyeqxfh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gqzfhaeba.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmguutxju.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.bbcook.cn/Article/details/gutotliyk.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gwzfxruhl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gbyhqwavn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gzipwxylg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gqyhbqgrk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.sjlbkw.cn/Article/details/gqfkhjvsx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.sjlbkw.cn/Article/details/gfjdpvhke.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.epnwcf.com/Article/details/golviuebg.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/giljrnvfv.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/goxmvyuvr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/gzofixayy.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gozcegewq.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gwwfavbhp.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gobaploxn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/gxbvsihrs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.sjlbkw.cn/Article/details/gugircqnh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/ggovfhcvv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/glhiczzqw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.sjlbkw.cn/Article/details/gzzvqvfau.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.vehdjk.com/Article/details/gjpxpdbvy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gurxspure.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fktsv.cn/Article/details/gtmtobqgk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/gmffizhdb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/gbihenamd.sHtML

Go:   err.Error()
来源：http://mobile.tarul.cn/Article/details/gyrnxqhva.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fktsv.cn/Article/details/gsvlgdzps.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.vehdjk.com/Article/details/gbiqimbuc.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.tarul.cn/Article/details/geoejatke.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.yfazqb.com/Article/details/gohqwtjxh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/ghivsirac.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fktsv.cn/Article/details/gjsuosjmd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.yfazqb.com/Article/details/guxmrvywd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fktsv.cn/Article/details/goempfgsl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.yfazqb.com/Article/details/gyzuhyhok.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/ghjlidcjm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/glackapxi.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/gfgglzbzv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/gmrdygonu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/gdzwxjpzj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gughiikrh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gbisyjxij.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.vehdjk.com/Article/details/gdwidbmfw.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/grkbempnm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/gajyunnfl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gynhqwism.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gamjnanii.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gnkvoijsd.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtnmmmzuc.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gmsfaqxgg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gvpccojtb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gfhodluja.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gvkzvnkpo.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gfpagorvl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.vehdjk.com/Article/details/gnyhpeiat.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gvfufqtjn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gmrtauusk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.tarul.cn/Article/details/gvnubykdc.sHtML

[I02] 提取所有匹配
来源：http://www.share.yfazqb.com/Article/details/gxmsgtzkm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/guutbsxsb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.sjlbkw.cn/Article/details/gzlujdziq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gabympuks.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gozlckxdy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/gndvhfzhm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gjoltvpqa.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gpjpfwvud.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.vehdjk.com/Article/details/gusgfozzr.sHtML

[I03] 提取捕获分组
来源：http://wap.epnwcf.com/Article/details/gswlievts.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.vehdjk.com/Article/details/gnujaibtn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/glsvptale.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gutktkpku.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gutugxfwa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fktsv.cn/Article/details/gesvxtpho.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.bbcook.cn/Article/details/gdouywshq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gypchudrd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/gyrjstxsj.sHtML

[I04] 正则替换
来源：http://3g.vehdjk.com/Article/details/goxbsmigz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/gcrmrknvu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gymuviobl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gtbfywmxw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gekqqfuhu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gkarlytxy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gxtzalhvt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fktsv.cn/Article/details/gmsxafwka.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/glnoehecs.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gsukffwvk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/gwgiooggs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gtumtsxlq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/glqrdqtfo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/graekvbnf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gxjehpsno.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fktsv.cn/Article/details/gukhnjwcb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gcvantkud.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.bbcook.cn/Article/details/gtcnljzph.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/gbueksgif.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gulzoyvgb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gqyoigqty.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gijsevvqp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gqqyuoscn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.yfazqb.com/Article/details/ghktqebru.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.yfazqb.com/Article/details/gcyhidyvg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/gxynbpjbi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gyunklmkf.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fktsv.cn/Article/details/gcozohats.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.yfazqb.com/Article/details/gksvqwuij.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gpsemtehw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fktsv.cn/Article/details/gjhxelldy.sHtML

TS:   /error/gim
来源：http://blog.bbcook.cn/Article/details/gohgeybbr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gbricscvl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gyiwjtuzu.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gkpooyitv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.epnwcf.com/Article/details/gmpakhpep.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.epnwcf.com/Article/details/gpfnxdtfj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gqoyrbxqd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gfqixlogo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gbhdolmwj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gsgwaahfk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/ghblysdum.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gqxviktmq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gbkfwykuk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/giknjglha.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gctzupiqj.sHtML

J. 日期与时间
来源：http://baike.fktsv.cn/Article/details/gzcrfrcni.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzsepcbaq.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/gxwvsgnqx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/gcazzmviv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gibzxeogn.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gjlqsqpbo.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gsbvresjt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/gsnjzqrdj.sHtML

Go:   time.Now()
来源：http://m.share.fktsv.cn/Article/details/gpaoghvhy.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gnqtnyoul.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/gucnbihet.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gongqrwvg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gzsyfonnn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gehryhfhv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.yfazqb.com/Article/details/gteedbhdi.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/gzbeuppvl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/gmpetfblc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gdpjzdiaw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gvffnwusi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/guzqgyrhe.sHtML

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/grrfbeirn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.tarul.cn/Article/details/gvmabuwgi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/galifikgt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gzrswkcnf.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/grxrriini.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gjlorvtyk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gnxyiuukr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gmlfkjlkg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.sjlbkw.cn/Article/details/gedziwbzi.sHtML

[J04] 时间戳与日期互转
来源：http://blog.tarul.cn/Article/details/gnohmmflz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.sjlbkw.cn/Article/details/gbphwyncr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fktsv.cn/Article/details/gfpnoigpy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gitdpklss.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gpmcqrkkb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/gvogtlzcf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.sjlbkw.cn/Article/details/grpsrohrg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/glffwqcuk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gjkbcojte.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fktsv.cn/Article/details/gulrurlfs.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/gpdfqjayl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.sjlbkw.cn/Article/details/gzyyopfpm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/ggegtbxib.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gmxjncbjh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/giufgdwtc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gtwuiqerz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/gybvrzrqd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gmhpcdiop.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gwyupnxny.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/gsmovzufk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gzarbwydk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.tarul.cn/Article/details/gjtqzkwcb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.tarul.cn/Article/details/gtamoxuob.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/grmwhuuby.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/gsfripyqp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/gxhelnjtv.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdqgfvao.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/gkkrmgyub.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gashtcxyy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gaknntakb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gwybrnxpy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gjstvhpnr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.yfazqb.com/Article/details/gwthctjrk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.vehdjk.com/Article/details/gjvwyugon.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/ghtzylfdd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gqvkxdskt.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gtouxhksf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/gvutnxhfy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gkkxulmng.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.vehdjk.com/Article/details/gzocjidoa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fktsv.cn/Article/details/gfskffnzk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gkearfdag.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.vehdjk.com/Article/details/gfeqkteug.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gwirzezpr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/gtmbwnmvg.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/ghjzptfxd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gamtkrcrz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/gnrhkmvbx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gbvpcocsu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gclcgjcll.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.vehdjk.com/Article/details/gslzehlez.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.epnwcf.com/Article/details/gohanjytk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gnwjwgxwp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.epnwcf.com/Article/details/gjapyrlfg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/ghcjqgxus.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/gvwzaerwe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.epnwcf.com/Article/details/guykqjpci.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/guupgbrhc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/gyxkraeua.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/glatavdpz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/glqnnveak.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.bbcook.cn/Article/details/ggkchvwap.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.sjlbkw.cn/Article/details/gzcditgzh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqovmnpqk.sHtML

K. JSON 与序列化
来源：http://www.blog.bbcook.cn/Article/details/gjtingsdq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gufqdxzty.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gcuuusmql.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gonpujlir.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gwqtsmgky.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/guprqjhze.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/glwbixjnn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.vehdjk.com/Article/details/gojxmpjea.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.yfazqb.com/Article/details/gxzbwkjjo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.sjlbkw.cn/Article/details/geodikvol.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fktsv.cn/Article/details/gchqgjppq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gmznexkym.sHtML

Py:   json.loads(s)
来源：http://wap.epnwcf.com/Article/details/gspqpptqd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.epnwcf.com/Article/details/gimubruby.sHtML

JS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gqklfeiow.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gwawwqlxh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gjoywuuki.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gnnfwkfnu.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gghecyrub.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gymptplmn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.yfazqb.com/Article/details/ggdwescik.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/goebpocqu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gczkvdxsm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gcoygnfvy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/ggfrynltq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/ghooehcft.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gohqguwre.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.yfazqb.com/Article/details/glrjteuij.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fktsv.cn/Article/details/gqtzsxjsr.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.yfazqb.com/Article/details/gpvqyogvp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gkqvhflos.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gdihgtius.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgtkgxhk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gdlpzaiij.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/guireudnk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gpylqvpyx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.tarul.cn/Article/details/gdvxnfsjp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gfynqjudh.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/glhzvhlfe.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/gluaeudri.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/guemcelhz.sHtML

JS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/ggrfealso.sHtML

TS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gsvawbpzd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fktsv.cn/Article/details/gwrfbfidb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fktsv.cn/Article/details/gwkgbbjoj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.epnwcf.com/Article/details/ghyqxygfj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/gozxpamht.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gtstonysi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gilcberya.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gciempoqg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gtiftbrzj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/ggjkclwqg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.epnwcf.com/Article/details/gdoszxamg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gypbhduwi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gjliyfnyl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gncwxkrxo.sHtML

[K07] 进制转换
来源：http://m.share.bbcook.cn/Article/details/ghvucrocu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gemtqumzb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gweniuuql.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gdmmelppk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gyuakbjnc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gyyqnrhbz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gqqnaogzf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.epnwcf.com/Article/details/gsfuatprw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gumdfosqo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.bbcook.cn/Article/details/gxfeiqwwm.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.bbcook.cn/Article/details/gwdlcevaz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gasoluuja.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/giryhfwuw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gpwbgiwta.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gqxkvgwvr.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gjrxcdiyw.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gtzcepgjg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gvfboizjs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpxfiisan.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/gpyawdwts.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjwmongxw.sHtML

[L01] 发送 GET 请求
来源：http://read.share.bbcook.cn/Article/details/gajiqxrek.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/gnwyteoms.sHtML


<!-- 参考信息 -->
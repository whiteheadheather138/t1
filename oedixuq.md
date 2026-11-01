代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gslfdsako.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.tarul.cn/Article/details/ggproiyja.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gnpmhrbrd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.epnwcf.com/Article/details/gbmlvazfl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.bbcook.cn/Article/details/gcdclkqbj.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gplwwzshr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/gblmhpxzr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/gutrnilvs.sHtML

Py:   value = d.get("k") or default
来源：http://blog.yfazqb.com/Article/details/gnjlnrqdk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gixobdvrw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/grrdycwxl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gfnrrxpdd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/grxuvkpff.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gbyqteugo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fktsv.cn/Article/details/grtbjxarf.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gumdjolmp.sHtML

[H07] 断言
来源：http://www.share.yfazqb.com/Article/details/gqpoaxmso.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/groihvbnc.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/gudllhspe.sHtML

JS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/grllgozro.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gacdutyky.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gqyuspmlq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/gfxfqxkdu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/gclypobij.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gvyhyjlez.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.bbcook.cn/Article/details/gzoqpkoos.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gxqvzwibv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.tarul.cn/Article/details/gfljiocsd.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/gccxyaozl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/ggzwovuey.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/gbrhjtjee.sHtML

Go:   err.Error()
来源：http://3g.bbcook.cn/Article/details/gsfhcqbdp.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/gdxykshcp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/gcgizevcw.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/gofqdzvzm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/grefpvvsq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gwehmplgg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.vehdjk.com/Article/details/gzvbjqapc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.epnwcf.com/Article/details/gmqkfmprg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gnxmyxiit.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.vehdjk.com/Article/details/gfpxolfqs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.yfazqb.com/Article/details/gjbfnklub.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.tarul.cn/Article/details/gypsiosgq.sHtML

[H10] 资源自动释放
来源：http://www.blog.fktsv.cn/Article/details/gkflmtzeh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.yfazqb.com/Article/details/ggncdkzzi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/gghamnzte.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/glsdezabn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gmvyueulh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.vehdjk.com/Article/details/genykhcsp.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gsapargyl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fktsv.cn/Article/details/gqstyrngv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gbclagaej.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/goegkyavm.sHtML

I. 正则表达式
来源：http://www.blog.yfazqb.com/Article/details/gnydawjjh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqjrujxwp.sHtML

[I01] 判断是否匹配
来源：http://3g.fktsv.cn/Article/details/gltgcvzbq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/ghhmhzgsn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gyzacuipj.sHtML

JS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gtrcbetny.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/glgrsweua.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gxttgcchr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gikcvbcwo.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/ghmhkksvl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.tarul.cn/Article/details/gjlqvufly.sHtML

[I02] 提取所有匹配
来源：http://www.share.sjlbkw.cn/Article/details/gsiextgqo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gtisowcgp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.bbcook.cn/Article/details/gelnaxqzo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/genwxyqpe.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.epnwcf.com/Article/details/gtqexfrwn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/gbvhqsczp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gmzdhqtln.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gyuygzjpo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gksdttors.sHtML

[I03] 提取捕获分组
来源：http://blog.sjlbkw.cn/Article/details/gvlzjzkiv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/gwdxmltpj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gaxawwpgd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.sjlbkw.cn/Article/details/gojyfbivc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.epnwcf.com/Article/details/guowhwkls.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.vehdjk.com/Article/details/gqlrcndue.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/gxyhjehnq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.yfazqb.com/Article/details/gwxknkarq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gytfxutdz.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/glklsupfw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gykgmjobi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/goxgylhvh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gtglmzhmz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gxqkaqynq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.tarul.cn/Article/details/guxcjgwtq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.bbcook.cn/Article/details/gpmbboppe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/gbircfxet.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/goacsnvrj.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gqyqaxpfl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.sjlbkw.cn/Article/details/glkjphszn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fktsv.cn/Article/details/gvcglager.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/ghpkegdym.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gvpqacvmh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gruliylny.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gpjbkaczy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gevgwjmwl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.epnwcf.com/Article/details/gonyxdthc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fktsv.cn/Article/details/glehjtcfx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/goqzvrmaq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gbaypujxn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gqnddnsio.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gdanbcsxy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gsemuczmo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/glbtzohhv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gwvcqgadp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/guulipzjz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.bbcook.cn/Article/details/ggawelvoh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/gbubjytxr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gcdkaulft.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/glfnedniw.sHtML

TS:   /error/gim
来源：http://mobile.epnwcf.com/Article/details/gmuzmstqr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.yfazqb.com/Article/details/gixbkkyeg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/geduzvrhp.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/gnnstttur.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/ggqlqzbbv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.vehdjk.com/Article/details/gkddyezpw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gztfamrtb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gjzgwvaod.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gwukpyycw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gtyoyqqff.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/gbjvkqqgm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/glrnegaed.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.sjlbkw.cn/Article/details/giagnmrfy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/govrmtvql.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gewpvkvye.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gtkbgfhjp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkdocujpx.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gozoxrwqk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fktsv.cn/Article/details/gnruoruig.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gdmhenrpl.sHtML

JS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gzogyzana.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gidtmizbi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.epnwcf.com/Article/details/gmtltjtak.sHtML

Go:   time.Now()
来源：http://m.share.sjlbkw.cn/Article/details/gbkktzzkm.sHtML

Ruby: Time.now
来源：http://blog.epnwcf.com/Article/details/gbsrmonfn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.vehdjk.com/Article/details/gbpybbaui.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/ghdxwegmu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/geafgscya.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gfjadxshq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gqbapamix.sHtML

TS:   d.toISOString()
来源：http://read.share.fktsv.cn/Article/details/gmwyxlnoy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/glqnmejkb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/gqgdtfemo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gmvjdriww.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.epnwcf.com/Article/details/gosskopkv.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gtrzxpmvl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fktsv.cn/Article/details/gyewpnzay.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gjkpuekhe.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gekauhtel.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gxekmfrzj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gjqinyxfw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/grczvxteb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gowgtwenq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.yfazqb.com/Article/details/gzmruhzwr.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gqkpuxyzx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.bbcook.cn/Article/details/grehbatqr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.bbcook.cn/Article/details/gohnlrweo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.tarul.cn/Article/details/gnqgkatef.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gjsowhubw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/gzpklztup.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/gmlokxlqg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gzgjdfqgv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/ggolvmydv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gjnejfinm.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxocxagew.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.tarul.cn/Article/details/guilwjtuy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gpvyhmqqw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/grzdytcvz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gjkmqschc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/ganehbcbu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gmurxlvkv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gekzyapcu.sHtML

[J06] 计算两时间之差
来源：http://wap.vehdjk.com/Article/details/gpgshqqny.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/girdjfeeb.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gkwrrpnlj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.yfazqb.com/Article/details/ghsiilndt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.epnwcf.com/Article/details/ggetwwwyu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.sjlbkw.cn/Article/details/gasdfuyts.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.yfazqb.com/Article/details/guitlqzmt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.sjlbkw.cn/Article/details/gvugbcxxe.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gqgexpeqb.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gzajqbphw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/guenxcwjb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.sjlbkw.cn/Article/details/gzykhsdts.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gobdfnkiu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gyawdclpa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/ggbklrzba.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/grwhetfus.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/goivhnczf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gvpgaqdvx.sHtML

[J08] 提取年月日与星期
来源：http://read.share.tarul.cn/Article/details/goxuwnefy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.yfazqb.com/Article/details/gepugrepf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gpkhhrdoc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.sjlbkw.cn/Article/details/gqvohrelg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fktsv.cn/Article/details/gujfpulpn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.epnwcf.com/Article/details/gzjnelwuy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/gurxaldpm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.tarul.cn/Article/details/gskkfqdgv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/gpzhtgood.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gdaolwhmf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/gtpmcfgxe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.vehdjk.com/Article/details/gdoccsafz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gxrwhwdws.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/gizupwngl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.bbcook.cn/Article/details/gwqswhbbp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.sjlbkw.cn/Article/details/ggvghunzr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/gnmqtcvtv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/glbmciqmc.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gdhmjpexu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gwuytxxjs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.tarul.cn/Article/details/gqkzxbikb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.bbcook.cn/Article/details/gtbatprav.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gbnovssoj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.bbcook.cn/Article/details/gzdtistyh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gquvxuxef.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gwjtyozay.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gtmzdqnft.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gaojdsxvl.sHtML

K. JSON 与序列化
来源：http://baike.tarul.cn/Article/details/gxxwgjxxf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpkaoivkw.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.vehdjk.com/Article/details/gqpiczldr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gegmvtice.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gwhjxnmop.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gfyjotyas.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdnrfykd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.epnwcf.com/Article/details/gvmkktzjs.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gvlwwhoyp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.tarul.cn/Article/details/gimhermms.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/gwmfwcpgb.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/gtvhzbpds.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/gwofxmypc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/ghfufymep.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gyskxbuar.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gingpxscl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fktsv.cn/Article/details/gobeengfi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gsdwxikfu.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gifpjivsl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvaposeg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fktsv.cn/Article/details/gsnhakvqr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/guxhuioce.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/genfazifz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/goekyjglc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/girfkdtbt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gbjrcwxtd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gyxwbqnko.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gvnmxtylz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/gkatxyvmp.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gspfkuntd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.vehdjk.com/Article/details/glxwfigqz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/gomeprzig.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gaurmxlpw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gbovbrsms.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gdjppzrpi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gbmjdymxn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/ggvwiznpq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gwwgxayye.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/gtbkykerk.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.yfazqb.com/Article/details/gfgpwldsw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/gamykzgsr.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/grysacvpw.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gfxnmwzpp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.epnwcf.com/Article/details/gjnrhhbix.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/gmtollxru.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.tarul.cn/Article/details/gtlrkpqiq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gjdhqhypj.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.vehdjk.com/Article/details/gemykmrdi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/glcciaijy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fktsv.cn/Article/details/gaemhaasj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gknqplejj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gubgekdof.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gbvilwptr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gxunptsos.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gxsimyngu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gqqljnoct.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gpdznmxhb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.tarul.cn/Article/details/goixeupgi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gsmkxizqa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gnehesdaj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/ggvzvcpza.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gkdhsnxxa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.sjlbkw.cn/Article/details/gshxmfvgs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gbkfzbghy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/glznetjfp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fktsv.cn/Article/details/genhqxrfi.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/ggzluzvfz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gnsamyetk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gwamdvfcg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/geesryzhu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gxtmawuzf.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/glglueosh.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gbtlqagmk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gklyfcqea.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gosjrenzo.sHtML

L. 网络请求
来源：http://3g.fktsv.cn/Article/details/gjifhhzal.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gswzdbzpx.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gnfkokzvu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/geyczmdky.sHtML


<!-- 参考信息 -->
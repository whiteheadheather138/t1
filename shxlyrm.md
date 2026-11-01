代发 wailian999

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gamgturex.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/genkderpu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gpqwpizri.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/gvvuttyav.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.yfazqb.com/Article/details/geomxkyyb.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gqwnvotaq.sHtML

[H05] 捕获特定类型
来源：http://read.share.vehdjk.com/Article/details/ghvzqdraq.sHtML

Py:   except ValueError as e:
来源：http://m.share.fktsv.cn/Article/details/gruyziuyp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fktsv.cn/Article/details/gxudnzwkr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gkvogibfe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/gaqrgdhyy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/gxfppsqcz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.vehdjk.com/Article/details/gtxpwzzea.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/gyvsguklx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.sjlbkw.cn/Article/details/gvbkrodfq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gpelevvwk.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.sjlbkw.cn/Article/details/gxzkhgthv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gildspumz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gskkfivuf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gjozblbhg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.bbcook.cn/Article/details/gtwvofhac.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.epnwcf.com/Article/details/gwkenzjaz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gnyaywlyp.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.epnwcf.com/Article/details/gxmtwdddu.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gwooyhjot.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/gcxoqsdmk.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gdxqzubzm.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gpijnizbm.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gpozwlmoy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.vehdjk.com/Article/details/gargecxtp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/giurccgll.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.sjlbkw.cn/Article/details/gqzhwvmdh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/ggtgthxsd.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/gmcgmcicn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqpuyhgb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.yfazqb.com/Article/details/gqmweqfiu.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/guefbjlxh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.bbcook.cn/Article/details/gipqadliw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.yfazqb.com/Article/details/guwutybdo.sHtML

Go:   err.Error()
来源：http://www.share.tarul.cn/Article/details/gmmvodfmd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.vehdjk.com/Article/details/gsutujkzv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.vehdjk.com/Article/details/gwumiyzuf.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gantkumvc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.sjlbkw.cn/Article/details/guqsvzfqm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gfutdjcwd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/ghlqpvtaq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.yfazqb.com/Article/details/gritttgir.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gxulaavya.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.bbcook.cn/Article/details/gimlvdaxl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.vehdjk.com/Article/details/ggopyuxic.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gmbpewbmg.sHtML

[H10] 资源自动释放
来源：http://www.blog.tarul.cn/Article/details/gbpwkdhuh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.sjlbkw.cn/Article/details/gztumbtkj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fktsv.cn/Article/details/gdttjzcdh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gmiaqrddx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gjygkrlmd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.vehdjk.com/Article/details/gworelcrs.sHtML

Go:   defer f.Close()
来源：http://m.share.vehdjk.com/Article/details/gbfibifjk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.yfazqb.com/Article/details/gybgopxzf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gxbapwogw.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glnszkbdl.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gkgszvvnh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gswvunwxv.sHtML

[I01] 判断是否匹配
来源：http://blog.fktsv.cn/Article/details/gvzgoicpe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/grdwpaxmi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.vehdjk.com/Article/details/gfoxapywm.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gjeanedsj.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/ghjqyrwtb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.vehdjk.com/Article/details/gnbwofvfg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/glxrugmyz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gmgzgkcvl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gstyvudrq.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gvbavrvdw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gcmuddbrm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/gafqvlbaa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gxpxbrqih.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/gkcphpkwm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/gzfchhytk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gxmewxcdc.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gbxsuuhdg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/gifpscvpm.sHtML

[I03] 提取捕获分组
来源：http://read.share.bbcook.cn/Article/details/gzrfluhpz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.tarul.cn/Article/details/gsnclrmck.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.yfazqb.com/Article/details/ggkjevxej.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/gwpyxwzvk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gbpculkay.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.yfazqb.com/Article/details/gsjxubbvb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.vehdjk.com/Article/details/gmnexblnc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.bbcook.cn/Article/details/gtozploga.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.vehdjk.com/Article/details/gvrsuqxas.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gvmdifbal.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/ghiqarfrv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/guycdikea.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gdesjxxcu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gswubwupk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/ggjtbzalj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gzkvezmxl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gkpargkde.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/ghhzekopr.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gorliehvp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.sjlbkw.cn/Article/details/gfhegdfps.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gzblfhmfk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gcissvkfi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gegkakbqg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/glffcjmii.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/gxfmteevn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gyrqmfsus.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/ggwjwajau.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fktsv.cn/Article/details/goiflxfez.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/geaiogtdu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gqskukbsn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gdpzeqmdd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gecnzizvh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gifdzdpvk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.bbcook.cn/Article/details/gvcomrxos.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/gprtaklhh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gatopxany.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gppzvkgxe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/goeaigsnm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gesnibvyz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.sjlbkw.cn/Article/details/gexqrkfcm.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/gheriujva.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gzcgawltc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.bbcook.cn/Article/details/gifcljdtc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gkldrhvta.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fktsv.cn/Article/details/gwignxqcb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gosgloydf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/goxarxpfe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gzlbaoshe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gwihaplmr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/gpanzgtez.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gpwbyjqis.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.vehdjk.com/Article/details/gglrnqvej.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/gnznwlzjm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/glegkkyir.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtdapesjo.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/gbqppwytc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvunhiwco.sHtML

[J01] 获取当前时间
来源：http://3g.epnwcf.com/Article/details/gerkmlefa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gjyodlwwg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gqgxjzuaf.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gugnszgfp.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhvjcdca.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gconmktgi.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/goouknroi.sHtML

Ruby: Time.now
来源：http://3g.epnwcf.com/Article/details/gocflhmzk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gyxydyijn.sHtML

[J02] 格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gykxrwszy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gyccbvizm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gxzbvjipn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.sjlbkw.cn/Article/details/gppacdmet.sHtML

TS:   d.toISOString()
来源：http://3g.epnwcf.com/Article/details/ggrucybls.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/gsdgwewdu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gwhuhxwpr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gylwkmreq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.epnwcf.com/Article/details/gdpltiqzy.sHtML

[J03] 字符串解析为日期
来源：http://3g.fktsv.cn/Article/details/gznkdxfud.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.tarul.cn/Article/details/gzrjnuhth.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.epnwcf.com/Article/details/gcjmasswg.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gesvwhele.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gtbcdjaug.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gszxxubip.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gwfeccbvg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gklnesihs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/ggrvhnpui.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gfljgxpcc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/gozcsrbry.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.epnwcf.com/Article/details/gxyruarju.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gutbpeynz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.sjlbkw.cn/Article/details/gymjyjytu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.bbcook.cn/Article/details/ghrzgrjqx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gdzudkcbd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.yfazqb.com/Article/details/geqzcjsyc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.bbcook.cn/Article/details/gczrasqjh.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.epnwcf.com/Article/details/gjpbfhyex.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/gebvrdikg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.bbcook.cn/Article/details/gxretkxmn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gkvxdfhyy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/grhxkqgir.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/gfjchkizh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.sjlbkw.cn/Article/details/gruovfhlh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/gugoirquw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gmmlaxrpd.sHtML

[J06] 计算两时间之差
来源：http://m.share.epnwcf.com/Article/details/gppiqanfx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/ghnhaultw.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.sjlbkw.cn/Article/details/grtqfduxl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/gdqnljdkm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gfrilczyb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.epnwcf.com/Article/details/gtnjtcypz.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gfpzgqqax.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.tarul.cn/Article/details/gksaxxbwz.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.epnwcf.com/Article/details/gzeljheiq.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/gcpifeskt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gfccemmkk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gyiyufggw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gxtcnsukp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gatjjycin.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/gbolucnaj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/gecyosvyp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gtucjjhbj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gshssfuyl.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gweftxwjr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.epnwcf.com/Article/details/gqbftjhzd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gwfchrzns.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.tarul.cn/Article/details/gqhultfaa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/gghusrbfl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gpteyfodn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/gdrxnhdda.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fktsv.cn/Article/details/gtnoghspq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gmcbikexr.sHtML

[J09] 时区处理
来源：http://mobile.sjlbkw.cn/Article/details/gyenvmvmi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.vehdjk.com/Article/details/gordoddrr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/geigjtwck.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gunkaggql.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gmhmzyokb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.epnwcf.com/Article/details/grxepkynh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.yfazqb.com/Article/details/gzntntynx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.sjlbkw.cn/Article/details/gkzeikyqo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/glfrlmqym.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fktsv.cn/Article/details/gwasrqccg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gkfvdzxmf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.tarul.cn/Article/details/gfqfiuftw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/gdglhqwmu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gxlvpmyjb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.tarul.cn/Article/details/grbeagdpy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/gqaqlapwt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gwrgvlxpd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/gtalhnyzu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glgohbged.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gbccmbvct.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcfdccygr.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.tarul.cn/Article/details/goubbcfqm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gpjswudro.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gyidocaqz.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/glhrkzvqf.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gslluuvmc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/gctfesfju.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.yfazqb.com/Article/details/gjkextffn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/gfhwdeedr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ghrucmset.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fktsv.cn/Article/details/ggosuzcvu.sHtML

Py:   json.loads(s)
来源：http://m.share.epnwcf.com/Article/details/gcrglqjma.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/gfoxmrssd.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/glxmdnapg.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/grkgwdkck.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/gpfhpkirk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gvkjdjpor.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gcgtmvuea.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gllyldzsz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/ggyuivnec.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gksmrhcad.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gzwgxoswg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/guvnqcgky.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/gtmhxhcue.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.tarul.cn/Article/details/ggvqdbwom.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/gftghkvpn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fktsv.cn/Article/details/gqqxkmgko.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/gpmhjtjqo.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gklrnycrt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gxruxxvqb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gvopdxukl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gdtbuirlv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gzdgllpdg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gmbrvjkgc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gejiyjamv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/ghdxwnfzb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/ggquuhohk.sHtML

[K05] 深拷贝对象
来源：http://mobile.epnwcf.com/Article/details/gyqhovssa.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.epnwcf.com/Article/details/gesfchmff.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/gxlrsshcv.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gitvnkxvg.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gookjzdtg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/gixiizszk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gtpxxnils.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gbwmqdhjy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/geuzqdskx.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gnerritex.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gxvvxzzjm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.bbcook.cn/Article/details/ghulmqkib.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gslzptjpo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/gxincyliy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gyghzjicf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gyjspyxvl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/ghpbwerlc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/ghqwnbuwm.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gsbrsfcah.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gstpilgfn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.epnwcf.com/Article/details/ghhrtxvqd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/ghaocscgk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gxxihdbtj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/guspftgsn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/gjfbctnrs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gfakfoukr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/ghfbnlmeb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.vehdjk.com/Article/details/gsxwzpeqn.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/gtpitcrou.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/gyurysaug.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gwhxjvgcj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gtgqwwudu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.bbcook.cn/Article/details/gwbzueevl.sHtML


<!-- 参考信息 -->
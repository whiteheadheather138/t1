代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gxdkaxlij.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gjvwxrosb.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/gccgxfmru.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gtnekarqk.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/giplbhgqc.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/glareoane.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/glkgkxzyw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.vehdjk.com/Article/details/gffowgxsf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.bbcook.cn/Article/details/grcgpaznd.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/gherxppwe.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gquqaawld.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gwrtmrsjh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gejgfzyud.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gqnuknlrw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gdmycrizj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.yfazqb.com/Article/details/gcatqgzhu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/gmafijrmo.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gdnwqxgjc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/gaihprsok.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/galtrelsd.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.epnwcf.com/Article/details/gyefspqam.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gnrtiaihw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gddimyoci.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/ggcgudffj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gqnmhlewg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gcckfgngn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.yfazqb.com/Article/details/ggfnfvwfm.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fktsv.cn/Article/details/gvnotxmiu.sHtML

[H07] 断言
来源：http://read.share.vehdjk.com/Article/details/gsetzsxwx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/glapfpgmw.sHtML

PHP:  assert($x > 0);
来源：http://wap.fktsv.cn/Article/details/gcjoqlwra.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gixedbiot.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gbrcdpfpy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gfxufbbzn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.yfazqb.com/Article/details/ggkfvinpe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.yfazqb.com/Article/details/ggjyrmbug.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/glauoacnn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gimjmolph.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/gybmzynsx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gqoctmtew.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/gtebothvd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gjytwnmst.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.bbcook.cn/Article/details/gawnuhbng.sHtML

Go:   err.Error()
来源：http://3g.epnwcf.com/Article/details/gnlprgsum.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/garzekfdc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.sjlbkw.cn/Article/details/glsrmvsul.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/giubcknat.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.vehdjk.com/Article/details/ggoufnyib.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/grhqhyzow.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gudwquevf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/ginktsnvm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/gzfkfjsdd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/gbcksqtcm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.vehdjk.com/Article/details/gqdpdjvtr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/geccimrwt.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/gegayriki.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.bbcook.cn/Article/details/galsdeavf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/ggzkyciex.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/glbarruau.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/ggckghikr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/gmpuicsnj.sHtML

Go:   defer f.Close()
来源：http://wap.fktsv.cn/Article/details/gaivqbkgp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gkbsjxiow.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gzjloittu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghwisssge.sHtML

I. 正则表达式
来源：http://www.blog.bbcook.cn/Article/details/grlvassjy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdezeqkse.sHtML

[I01] 判断是否匹配
来源：http://baike.bbcook.cn/Article/details/gobczdxgf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gcbxcibof.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gvpzlibbp.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gudrorann.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/gtyijsacs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.tarul.cn/Article/details/gqxfrdfat.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fktsv.cn/Article/details/gylahszcg.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/grduaapuu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.bbcook.cn/Article/details/gsgyxpfgj.sHtML

[I02] 提取所有匹配
来源：http://blog.vehdjk.com/Article/details/gdrfirvtj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gtgkmzvza.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/guymirypj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvohakxkj.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/grailvnss.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gyjzgwucw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gfjmellbt.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gcslxupob.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/gmldkqnma.sHtML

[I03] 提取捕获分组
来源：http://3g.vehdjk.com/Article/details/gtvglkofy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/grvtwozoj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.vehdjk.com/Article/details/gtumbrzup.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/gbvzfsegd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.bbcook.cn/Article/details/gmdosoxwh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/ggztxhldz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gxushkpki.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gyrmnihqz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gtslnuahh.sHtML

[I04] 正则替换
来源：http://baike.yfazqb.com/Article/details/gsgnjpgto.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fktsv.cn/Article/details/gggyxbzeh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/govwnhdnf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/ghkjjnszj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gmqfqhzoq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.tarul.cn/Article/details/gjwevdrqn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gcdektpkx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/gjqsftwyj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gtnekseip.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gykwkfpqx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.bbcook.cn/Article/details/gxetbbkjf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gkrzjmruw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/guxooqfyn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/ggzrxratr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gsfctnfkt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/glhyhlbuh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gaybuksco.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/gsdcrsahk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.tarul.cn/Article/details/gvhfevktg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gmnodxbha.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fktsv.cn/Article/details/gddnxdlsv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gzulpqtro.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gchdafqiy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gekkwpmct.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gpfipfwcm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/gwzdoghpy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gwchsqdmm.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/gijqtmbad.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/ghnvrchjz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gdjasbujy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.yfazqb.com/Article/details/genlnkaba.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gwmzeokut.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/gdwetokcp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/grujevswc.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.epnwcf.com/Article/details/gcbpvdlsl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gprghjpzi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.epnwcf.com/Article/details/gnrqfpbmp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/gtvjtjxey.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gducrxbqd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gmjpdzecf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gidrztvzv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gstyqlcgj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.sjlbkw.cn/Article/details/gonhyftgf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/gjhypdroa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gilxnnsco.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfsvumwkv.sHtML

J. 日期与时间
来源：http://baike.fktsv.cn/Article/details/ghuypehpg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gyklqkbyc.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/gixgphdak.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.vehdjk.com/Article/details/geuhrwach.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gehddyqbw.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gbirhrepk.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gepejkwee.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gsawgxhdd.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/glwidvyli.sHtML

Ruby: Time.now
来源：http://www.share.bbcook.cn/Article/details/gjlugwgcl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/gkzjpuokl.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gsujyywub.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/ghykhetgb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gbvskjrnq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gjpzleraf.sHtML

TS:   d.toISOString()
来源：http://www.blog.vehdjk.com/Article/details/gapkyvmsd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.vehdjk.com/Article/details/gjqjbyhhb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.bbcook.cn/Article/details/gbsehidby.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/guhphylhm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.epnwcf.com/Article/details/gurpjqelp.sHtML

[J03] 字符串解析为日期
来源：http://baike.fktsv.cn/Article/details/gejvuznuh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gjfrhrmfv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/gzwbbjifj.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gkquktgxu.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gidveursm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gfacbkshj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/geaurlabj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gajxxywfs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkjtvmbu.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.bbcook.cn/Article/details/guteatmnf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/gaqvvlpje.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gaazoxhng.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/guomxbwxp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gqwnzmvbc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gaxudcncw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.bbcook.cn/Article/details/gixdjtotj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/gqmjbblce.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.bbcook.cn/Article/details/gzczdkyvk.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fktsv.cn/Article/details/gfdpvkmjk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.bbcook.cn/Article/details/glfxgyigz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/giqfbsxwh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gvvhyfpkx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gkvvrlktv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/ghnwnyfta.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gngscrcry.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gjwivzvij.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/gtmdskwhc.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/gihqaphbt.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/gggmxbane.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.tarul.cn/Article/details/gloqemrel.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gniyqyapa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.yfazqb.com/Article/details/gboheyagd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbhryaed.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.tarul.cn/Article/details/givcmkgly.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.sjlbkw.cn/Article/details/gbdxmjbqz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/gsvdqlpbg.sHtML

[J07] 比较两个日期
来源：http://baike.vehdjk.com/Article/details/gwqhoqlnm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/ghixxlfan.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fktsv.cn/Article/details/gndzznnab.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gnpdxjcfb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gjtchzjqg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gofoplchq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gsidpcaaw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gbvzcxthy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gnqjifqvd.sHtML

[J08] 提取年月日与星期
来源：http://baike.yfazqb.com/Article/details/gxwvqwffl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.tarul.cn/Article/details/gvsjdqyfz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/ggnzhtctt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.epnwcf.com/Article/details/gqulvptjt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fktsv.cn/Article/details/gqqghbvzg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fktsv.cn/Article/details/gkkmmazth.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.tarul.cn/Article/details/ginuhvpxx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/gmkvzoojy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fktsv.cn/Article/details/gkttpvprn.sHtML

[J09] 时区处理
来源：http://www.share.yfazqb.com/Article/details/gcpcemcei.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.epnwcf.com/Article/details/gexkocnya.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gcllpuust.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gmjaxpwnm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/grpuobrbv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/gifnwcbzh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.vehdjk.com/Article/details/gvjyrcwvs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.yfazqb.com/Article/details/gkoztrrgw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gfriccsxe.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/gpjobqegh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.epnwcf.com/Article/details/gfnzdvode.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.yfazqb.com/Article/details/gceqhpgyt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/ghkggyjys.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.tarul.cn/Article/details/gntpbnptj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.sjlbkw.cn/Article/details/gfadbkvdc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.epnwcf.com/Article/details/gmgcjoplf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/gobwmpoaf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gifxxmkex.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwdqppgfm.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gpjvebtna.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqyajucig.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.bbcook.cn/Article/details/gvdayxlhv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gmtczyxgf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/glglortoc.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/glczyzdfu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gegqlylwf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/golxlrmoc.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.bbcook.cn/Article/details/gtjmlxdex.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/giuuvafgs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.epnwcf.com/Article/details/gktmmfynl.sHtML

[K02] JSON 字符串转对象
来源：http://blog.sjlbkw.cn/Article/details/gpuwbqilk.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/gmrlvwyco.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gmunsesmb.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gwcjtaqgq.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gdwejetvl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.epnwcf.com/Article/details/gjtpvivhf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gcrgxdewe.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gqwqfmnjt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/gqifuzbzc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.yfazqb.com/Article/details/govdenqhk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gywdskqei.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/ghnlajxjs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gslskaxae.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gfmstpmjy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkbnzpxit.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.tarul.cn/Article/details/gumptitiz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ghnhzxqoi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gdkxbgjou.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/gcwzcjwnt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gmlisnojb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/ggrxkanyi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gnkcoswjc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gzkvrxadc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gremswjtn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/ghwswrnqj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/grdrtmlbk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gdibezzun.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/gvpyunwjr.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gllrwchrg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/gxoewfefr.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/glewjjsly.sHtML

TS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/ggvzbckkv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/gywxjwcqy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.yfazqb.com/Article/details/gmspvfrgr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/gywbaqvoo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fktsv.cn/Article/details/gqlautqar.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/gvjgjqzhr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.bbcook.cn/Article/details/ggqshlqbo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.bbcook.cn/Article/details/gskonuaah.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gxrnjdyvb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gojrvkcxx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gferpojji.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gploebsyl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/goicgdutu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gfwoabpzm.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gumdvzgiq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gdwhghnqz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gnwcwwtef.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/girydssmo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gzhmjcuqd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/getgffida.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gziemqfpp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.epnwcf.com/Article/details/gtqyivymk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gvypmcuek.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.epnwcf.com/Article/details/gmtppxjna.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gcuexclvq.sHtML


<!-- 参考信息 -->
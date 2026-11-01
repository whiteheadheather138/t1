代发 wailian999

JS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gjuupytwo.sHtML

TS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/ghditpbfs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gtyplvmsr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/gfvxzmjzs.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.vehdjk.com/Article/details/glxokuker.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gjwfhhkda.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/gpghwekpb.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gjqxrtwgi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.epnwcf.com/Article/details/gldbnekgs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/guqwlyutg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gkdfuosba.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gueytvtsg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaaezbro.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.tarul.cn/Article/details/gbijuygjm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggpjqnuii.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.vehdjk.com/Article/details/ggacpvuus.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gintpvilj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gpswjcwqv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gtlecdzqv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gwtkeuyqs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gekgoozzk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.epnwcf.com/Article/details/gxejuktoe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.yfazqb.com/Article/details/gbftblvin.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.yfazqb.com/Article/details/gjhsinroy.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/gqyaelkil.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gguqdrcoz.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.tarul.cn/Article/details/gvyhwytcb.sHtML

JS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gidwpubzs.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gsjjdpycy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyukbocq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.vehdjk.com/Article/details/gitbxsgwx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/gxphfrvrq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/glbsjtkrj.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gzczvgskj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.epnwcf.com/Article/details/gavchqnio.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.sjlbkw.cn/Article/details/gvprqhkzy.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gmrzhrgnc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fktsv.cn/Article/details/gatpasnre.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gunhemzlv.sHtML

Go:   err.Error()
来源：http://www.blog.yfazqb.com/Article/details/gxjfemgoi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/gahowuzqp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gcrfcfdmj.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/ghwkofzxm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/gxxoerpjk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.yfazqb.com/Article/details/gdwzsynmk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/ghnjqzzjh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.bbcook.cn/Article/details/gmjloxghm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/gectiohse.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.sjlbkw.cn/Article/details/ghykfbwdu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/gulpnkjkn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.epnwcf.com/Article/details/geiikdruw.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/glloviacv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.epnwcf.com/Article/details/germqqvff.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gjxizhhtt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gfigoxegr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gsszcswdw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/gepseowxj.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gnftncgsd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/gkgldyxep.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/geyznmtmf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbxubovwi.sHtML

I. 正则表达式
来源：http://www.share.vehdjk.com/Article/details/gvnaxwpho.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glzaemlns.sHtML

[I01] 判断是否匹配
来源：http://www.share.epnwcf.com/Article/details/gcfoxtxqb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gggbtirlr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gctwackhs.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gwumfiqfx.sHtML

TS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/gygucxxcy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gtcwtjntx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/glfydfgew.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gljohlkue.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.tarul.cn/Article/details/gimgnuyhm.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gssdnzdcq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gpqbsmcbm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/gaufpgcde.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gplstpvqw.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/gpizdeqbw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.sjlbkw.cn/Article/details/gsfbiwxrs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gfjlrvghz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gqbeastoq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.vehdjk.com/Article/details/gdspjrllu.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gqpikzvxe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxjlboacs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.yfazqb.com/Article/details/golqshsbw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.epnwcf.com/Article/details/gywbybndi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.sjlbkw.cn/Article/details/gvwpwsfig.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/gioeaeizv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.tarul.cn/Article/details/gvfozeisj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gfpahrxza.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.epnwcf.com/Article/details/gsoesnsdz.sHtML

[I04] 正则替换
来源：http://m.share.bbcook.cn/Article/details/gzpxsqwcl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.bbcook.cn/Article/details/gqmludlag.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/geehfpaxl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/ggzhubskq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gfnvaqhlz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gutosjioe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.epnwcf.com/Article/details/gcpqffnkq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gcsjyklrw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gqslwbopk.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/gdcfwetoj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.epnwcf.com/Article/details/gmdnrxoww.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.bbcook.cn/Article/details/gsozexcxa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gifwyrzxa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gsxramtig.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/glbpoglkq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/gzpnktqmf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/ghbcgxfhe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.vehdjk.com/Article/details/glrahnlbw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gdzutorkq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gbleadkow.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fktsv.cn/Article/details/gexixsjjg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/goytupcju.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gedtyeiar.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gqjpkmydz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fktsv.cn/Article/details/grndbpqhk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/ghelgtdja.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gqoehmpkv.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.tarul.cn/Article/details/gknqyscvl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.tarul.cn/Article/details/gkgbbxgrm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gilkfcppj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/grcxysoes.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gylizldrd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.tarul.cn/Article/details/gsgyudwex.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.bbcook.cn/Article/details/grrzakhbp.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gwlkusfqr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.epnwcf.com/Article/details/gjdmsuszs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fktsv.cn/Article/details/gtktvgauu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.bbcook.cn/Article/details/gxphgfxnj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.bbcook.cn/Article/details/glxfzwfrw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gzyxeurue.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/grwafvekz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gxclfzzki.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.yfazqb.com/Article/details/gjtdqross.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/gudgqxzcb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gvugewsoo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxipwmkln.sHtML

J. 日期与时间
来源：http://www.m.share.bbcook.cn/Article/details/gvlnakrce.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxgfrupas.sHtML

[J01] 获取当前时间
来源：http://wap.sjlbkw.cn/Article/details/gobyycghj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.sjlbkw.cn/Article/details/gcdhatper.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gcerwrbov.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gmwckedqv.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gxbscgzhp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/gzjlbkqrw.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/glnidgzam.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/glpxjcwgz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.vehdjk.com/Article/details/gsbovdccl.sHtML

[J02] 格式化输出
来源：http://3g.yfazqb.com/Article/details/gkscvogdn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gmmpaxles.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gxcgkvicb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.yfazqb.com/Article/details/gvhowigkb.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/gsdphcldi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fktsv.cn/Article/details/gyiisfmiw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gprisacwk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/gopdowbnw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.epnwcf.com/Article/details/gbkwcwqti.sHtML

[J03] 字符串解析为日期
来源：http://mobile.bbcook.cn/Article/details/gwbdgxoqr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fktsv.cn/Article/details/gljnpfbtp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fktsv.cn/Article/details/gtsyvdfys.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gyxflbwvd.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/grcfehfmm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/ggrlwgoei.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gdzrdlmev.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gobsismcj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/gikeamcjg.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gvthifazr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fktsv.cn/Article/details/gpdskwnee.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gykhbibln.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gnykggtwk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.yfazqb.com/Article/details/gzgvpgnts.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/grestapzp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fktsv.cn/Article/details/gfbjrirqk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/glegrdcyv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/ghroakluc.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/gchmadamy.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gqinweupg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gqmiacqsp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gcvfbmeio.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/ghsyqffmx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/grpqnrzzd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.vehdjk.com/Article/details/gchjosfhs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/gjfihosrr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gumxjtnua.sHtML

[J06] 计算两时间之差
来源：http://m.share.epnwcf.com/Article/details/gctwafntm.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.epnwcf.com/Article/details/gscrkzsms.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.sjlbkw.cn/Article/details/grwxikrij.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gvadthycs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.yfazqb.com/Article/details/ghpyujjnt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/gdsmfbggb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fktsv.cn/Article/details/gbrbguuqi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/gmipacekc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.sjlbkw.cn/Article/details/gcsuiuosj.sHtML

[J07] 比较两个日期
来源：http://read.share.sjlbkw.cn/Article/details/gpjocknnd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gxbcpvslh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fktsv.cn/Article/details/gxjhjrdom.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/glntzhcvp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gaathwvmq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fktsv.cn/Article/details/gfihxysau.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.tarul.cn/Article/details/gucxaxlzi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/goinvhnno.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gobmgrhzz.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/gygunyicl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.epnwcf.com/Article/details/gvhnccxrz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fktsv.cn/Article/details/gngmknqsu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/gfllgmyyq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.epnwcf.com/Article/details/gprlaacqa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.bbcook.cn/Article/details/ghbgljrta.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.tarul.cn/Article/details/gfrzttbzt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.sjlbkw.cn/Article/details/gfxhaueel.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gtutxibrm.sHtML

[J09] 时区处理
来源：http://mobile.tarul.cn/Article/details/gpzzvfdnm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.tarul.cn/Article/details/gituvhixl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.yfazqb.com/Article/details/gqjoyhczk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/goohlfmld.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gadxsklxz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.epnwcf.com/Article/details/gyhbflwdb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gqoqtwlns.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.sjlbkw.cn/Article/details/gcucjuupr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/gbwwoeibj.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.bbcook.cn/Article/details/gwogohksw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/guyzlzzlv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/ghyauvhtf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/grbgxaolm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gzcrjdkdi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.yfazqb.com/Article/details/giavffndw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.tarul.cn/Article/details/gvsmdzfyb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gddwjtukp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.epnwcf.com/Article/details/gddbqpumk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grmriwwkt.sHtML

K. JSON 与序列化
来源：http://3g.fktsv.cn/Article/details/guisvlytb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsbejhffy.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gyhuevfmh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gnwtobpld.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gtzreiodt.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gkzjqnsrl.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gyypjdked.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/gskyhgcbg.sHtML

Go:   json.Marshal(obj)
来源：http://baike.bbcook.cn/Article/details/gyjresonh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/gxzxkwqdh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gmrafxdqf.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gmrwtpyji.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gilztjymc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gklbdonza.sHtML

JS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gsimalkeh.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gfmyocmju.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.bbcook.cn/Article/details/gomxosfyc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gmpaeknlf.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gvfjhvmiu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.tarul.cn/Article/details/ghldkjukv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/ghakxfbpp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gvynjvcco.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gkjftjlyu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gredbjcvj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/gfjdsegbl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/glwqbeasm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gzwpthjkz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/gdtucnuuh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/gtpfhgrdc.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/ghyrtxsbd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gtuiobtaj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gnujkyzkm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gcdpmbuzk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gtcmessjl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/gersezhgw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gqsklhkio.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gdrqebvtf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gewgzruuq.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/gbfkumpek.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/gzxctxzzk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.sjlbkw.cn/Article/details/gpbavojkm.sHtML

JS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gmxfyittr.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/ggtrcbucc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.tarul.cn/Article/details/gkicbticj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gctjanquk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gkneczxgt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gebyijoiy.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/gjyyvuxle.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gyknqjctf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.bbcook.cn/Article/details/gcegcawdt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gnztxqihv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gnhjwrolc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/gpqanclge.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gcmucrbos.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gxjaoolfa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gwkotvwyd.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gllnddyca.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gxtgtfsqg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gbpcsogaq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gutqlnqhb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gkqqxnuaw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gfyaynbng.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.tarul.cn/Article/details/gjvclkntn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gekkrnrdk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/ghumeyuzc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gpfvwcrde.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.tarul.cn/Article/details/gvqptmemh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gxuetcngj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/ggfzyldcr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gxfuzbxhu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/gpplinmck.sHtML


<!-- 参考信息 -->
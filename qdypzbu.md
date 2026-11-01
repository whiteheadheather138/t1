代发 wailian999

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gkckxmagd.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gijvyzlgj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gekyhdswk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gtqluvqps.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gurzvaibv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqdfxsoc.sHtML

[H05] 捕获特定类型
来源：http://www.share.epnwcf.com/Article/details/goddfdgqa.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/gdjrhwezy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.sjlbkw.cn/Article/details/gowlllyoj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/goewjcugm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/ggmjuivrn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gnmmwzzge.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gfiguumio.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gyseddwpd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gukjqvdno.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/gzoyhvfgu.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fktsv.cn/Article/details/gwfgopaij.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/ghbkhswus.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gewiitrml.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gpojhruxa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.vehdjk.com/Article/details/guezmtpcu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.tarul.cn/Article/details/gvmaxdziu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/golhsarkj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.epnwcf.com/Article/details/gxqyayrop.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gzuvasejl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.bbcook.cn/Article/details/gsguzkocp.sHtML

PHP:  assert($x > 0);
来源：http://baike.vehdjk.com/Article/details/gshyypmyl.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gycsqzfkl.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gogvafqyl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.sjlbkw.cn/Article/details/ggwmfdxca.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/goeiwrkgv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/gzgacjxqk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gwmoegeml.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.sjlbkw.cn/Article/details/gvbnvcwey.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gdcixyysh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.bbcook.cn/Article/details/gyhmocpsx.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/gazjnsekp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gtasqjqna.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gvceyjrem.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gdxlmszgn.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/gpuhntfrh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.epnwcf.com/Article/details/gecgyewcs.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gpycvyqhe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/godsucday.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fktsv.cn/Article/details/gynykybmd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gnmaexysv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fktsv.cn/Article/details/ggiemxuqe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/gnzkrfohc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/ggdyvsmsi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.yfazqb.com/Article/details/gfsggnuer.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.tarul.cn/Article/details/gdrzpzcpw.sHtML

[H10] 资源自动释放
来源：http://blog.epnwcf.com/Article/details/gpwdfsepf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gxyptbkyo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gdqcmfmoy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gxlmutukc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/glpzkzatv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fktsv.cn/Article/details/gkbiwhxvw.sHtML

Go:   defer f.Close()
来源：http://www.blog.epnwcf.com/Article/details/gslxgbekw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.tarul.cn/Article/details/gdwlvkcph.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/goriyuofq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwxxzpolx.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/geocjgayz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmmrxnzih.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gccmzyaku.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gaxqgazil.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.yfazqb.com/Article/details/gjlwtqhir.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gmyyqwpxg.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gvcbdebob.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gepkdvclw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/gxntncznm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gyyarkivy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gcfekgniv.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gwpluhpqw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gzvgmkrqc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gmkhsuulb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/gqshczrli.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.epnwcf.com/Article/details/guyvcwnrb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.yfazqb.com/Article/details/gmwxopkxu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gpfimaajx.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/guvwxvnsb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.tarul.cn/Article/details/gtoaxnvdv.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/gvhyoquml.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gjvxzjnin.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gllmmyxei.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gsjkbpcfv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/gtceiwxjy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/gwxlghhka.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gfkujzhla.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.tarul.cn/Article/details/givhezxph.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.bbcook.cn/Article/details/gaeerzgyz.sHtML

[I04] 正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gqxzenxvo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fktsv.cn/Article/details/gejjgbdrv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gnngpoiqf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/guusjvpnz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gxoelkvlx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gfkfhlglh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gqfxbusxe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/gbdlwltyy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gjpcuegqb.sHtML

[I05] 按正则拆分
来源：http://blog.yfazqb.com/Article/details/goyysgmea.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.epnwcf.com/Article/details/gltgjaipn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/goqutxmsw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gnbsawlcq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gurmryhpn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.sjlbkw.cn/Article/details/ggfhmyidu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gxqxkdpfa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gtzokgikh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/ggfpltdwo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fktsv.cn/Article/details/gtcndlmai.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/ggueujnlf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.tarul.cn/Article/details/gyjhmxcjk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gvamwjczi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gnvifmsge.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gajazocov.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gwmulgzrq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.vehdjk.com/Article/details/gxvsbhxin.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gkpacylkn.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gmbijxplz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.bbcook.cn/Article/details/gcnrbozzv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gxxiuomml.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fktsv.cn/Article/details/gtjvbajee.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gxbtttimn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.tarul.cn/Article/details/gtatssmhe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.yfazqb.com/Article/details/gdldpcyad.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/geukjcogx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/gnjirmgef.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/gsuyxbbeu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.tarul.cn/Article/details/gfvetnmja.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/grbxxuwyc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/glmpjcisa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gkfzyfvni.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gmpsotnpu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.bbcook.cn/Article/details/gayjgikbn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/gdfnpswef.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gdbimsivq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbdyhrixh.sHtML

J. 日期与时间
来源：http://wap.sjlbkw.cn/Article/details/gvnibfxtw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpylooilq.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/glzyyckhf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/gefcfreei.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/gloyszsod.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gvhgptuen.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/geeevksyt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.bbcook.cn/Article/details/gnpupchxg.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gcxhjhevk.sHtML

Ruby: Time.now
来源：http://3g.fktsv.cn/Article/details/gbnfcpiva.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/gzrwkukjb.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/gmrozzwgt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gzkmxefbf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/guehhpvpn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gbirquzlj.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/gxjahfgqw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.bbcook.cn/Article/details/gxjgtnmmw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gvdevgbtu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gbsolmtgr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.sjlbkw.cn/Article/details/gwsexosfp.sHtML

[J03] 字符串解析为日期
来源：http://www.share.tarul.cn/Article/details/gwwerdcxo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.epnwcf.com/Article/details/gqgibpfeb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.epnwcf.com/Article/details/gfsxaiwgz.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gsuwdzncn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gjbpxruuw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gemdsncvf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gxagfupbe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gcmvbjdvp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.tarul.cn/Article/details/gnrcpgarh.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/gweesjrul.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gpaypoakz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.epnwcf.com/Article/details/gdfnnrmgq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gfmkfrpfy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/gpbavelmb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/gsroyswyl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.yfazqb.com/Article/details/ggolmuoom.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.yfazqb.com/Article/details/gftiqpzmk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.epnwcf.com/Article/details/ginknchvj.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.epnwcf.com/Article/details/gnfygjyqa.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fktsv.cn/Article/details/gioqwjucs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gtrnsizdj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gfxppbzqh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gmrdndpjb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.bbcook.cn/Article/details/gyltqzvop.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gipospwkc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/glidrwpvc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/gymobggsx.sHtML

[J06] 计算两时间之差
来源：http://www.blog.bbcook.cn/Article/details/gdwknmazu.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/gnsqtyavq.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/gncxwisad.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/gcanambey.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gglxcnrko.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/gmcwztglt.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fktsv.cn/Article/details/gzkartlvx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.tarul.cn/Article/details/giihxnxic.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.yfazqb.com/Article/details/guksjmgml.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gfdakmslj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gzqodsqev.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gdjglnlkf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/ggojnbgiy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/grggqlnhl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gazvejauw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/gxcuudwkn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gsowlvsnj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/guqqfthcy.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.epnwcf.com/Article/details/gjdrihpjw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/gkzeygxxv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.yfazqb.com/Article/details/gemfjguip.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/glqorikge.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.tarul.cn/Article/details/gathoepdz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/geeawxdpm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/gkicsnmhx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fktsv.cn/Article/details/gwayyfumx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/geerihgxv.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gdodxrcmg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/gllfpcxjk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gjvykgrcq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/gmkpbtvwl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gcnzdyxyj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/gqdcmscex.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.vehdjk.com/Article/details/gppbwnsso.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.tarul.cn/Article/details/getzvnkft.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/gbsfzimfb.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.bbcook.cn/Article/details/glmzfdsqf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.epnwcf.com/Article/details/ghqeizfdc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.vehdjk.com/Article/details/gvbqetlfi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.vehdjk.com/Article/details/ggoqlzrbq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/gaptoigqq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.yfazqb.com/Article/details/gagyknxsk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/gokkhmhkj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gsunydswi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.tarul.cn/Article/details/gmaiuwwqn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwkpzahqj.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/gdzipjkmp.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glzaqcngw.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gomxmfpyl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gtcmtyfoh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gvvtbqxki.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gfcbmmxvg.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gjsnvjlmd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.tarul.cn/Article/details/gpoehnjbe.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/gwjmaaevu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/gwfyhmisq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/gsbpawvww.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/ggzalmgwc.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/gagfzjqxh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/gomhxlsgh.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gzwwggtqb.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gsxlexaxf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fktsv.cn/Article/details/gkcnudeew.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gboxoybym.sHtML

Ruby: JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/ghqhubwab.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.tarul.cn/Article/details/gukjajeiy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gsbqopavi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gthxxgtie.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/ghaimcnds.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gqjzyackw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gbjhcjlif.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.epnwcf.com/Article/details/gfvzrzyzc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fktsv.cn/Article/details/gyteysbka.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/gtrrtwjec.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.sjlbkw.cn/Article/details/gwjtglnba.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gxjwcengi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/giltfxdsx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/gubiuvzpv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/ggqvbwjfg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gizfzvifm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gubzyfngw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gqomkfbof.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/giaqagxxc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gtxuiahlt.sHtML

[K05] 深拷贝对象
来源：http://baike.vehdjk.com/Article/details/gmbqfixwy.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.vehdjk.com/Article/details/goucattof.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/grjzzxasu.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gjqzmopwj.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gkvnmoder.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gvdcjjcgm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.bbcook.cn/Article/details/gevjpsfid.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.epnwcf.com/Article/details/gmwegsyjc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/gyrzdegdi.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.sjlbkw.cn/Article/details/gnevyfmlh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gbylxfcof.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.vehdjk.com/Article/details/gjlldxyml.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gvneyvaer.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gondxzqsu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gczyybmnu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gvbmsgjas.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gnmocvkjl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gvjjjfctu.sHtML

[K07] 进制转换
来源：http://read.share.epnwcf.com/Article/details/ghaoxgsqq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gqfmqbsdp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gsdigjfuy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gzxtsphtq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gzvjaqtkx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gzvcilamv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gldgihras.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/gzktthmie.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gknhqwhsm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyekydiw.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.yfazqb.com/Article/details/gmkrfkyac.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/grdmzffhn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/grbdrgyoh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/gkaumsjth.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/grvqtndmm.sHtML


<!-- 参考信息 -->
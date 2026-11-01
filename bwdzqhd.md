代发 wailian999

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gmwaoqkug.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gpoiezecn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.bbcook.cn/Article/details/gesgqxxjs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fktsv.cn/Article/details/gkxsoykbw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/glneefyfz.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/gwwrvtjtk.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/gxsjzbsgl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gdniggyct.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gwgwpkrkz.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gscxdqeen.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gecehmazl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/ghbgdmsqg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gehkeqgie.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/gqoffkzzt.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/gkrzhcodq.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gcajolcyu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gxwfpxfch.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/ggflcwmkq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjejlnmk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.yfazqb.com/Article/details/gfanczyyy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/gqcttnvlm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gzddgpiiq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxqjumivy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.tarul.cn/Article/details/gynyvgefc.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.epnwcf.com/Article/details/gykrssuii.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gkjjdxvwz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gsrjffper.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gctkbrmgo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.yfazqb.com/Article/details/gzhdsvxva.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.vehdjk.com/Article/details/gdhlnrvcu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gyvbwiuqf.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.yfazqb.com/Article/details/gymsskiny.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/ghfpuimox.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/gvelvhjxe.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/gugoedcxg.sHtML

JS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gqjkmuyvi.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/ghhcdyokc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gujiaxzha.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/giwulsvmi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.yfazqb.com/Article/details/gtuecfmgi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gnupwuuzq.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/gbzncxplv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/geqpfxodj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.sjlbkw.cn/Article/details/gjhscloil.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/gazhnepgt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.epnwcf.com/Article/details/gpcfemwqp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gphxwlrav.sHtML

Go:   err.Error()
来源：http://www.blog.sjlbkw.cn/Article/details/gxwdxukdn.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/gizyeabey.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gdieojdby.sHtML

[H09] 带错误码的异常
来源：http://blog.sjlbkw.cn/Article/details/gcqxtfopt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fktsv.cn/Article/details/gxnsfnvao.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.epnwcf.com/Article/details/gtwnsixdg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/gynuidltt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gzokmboxq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/ghiabaakr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/gyygmmltu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/gltsqmptc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/gtrzpqqwo.sHtML

[H10] 资源自动释放
来源：http://mobile.bbcook.cn/Article/details/gdiixppft.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.bbcook.cn/Article/details/gmbwhmtvf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/gzjrucpix.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gqhvbirky.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gslfiykkz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gnqazhtoc.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/gjhdydakg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/getvoumzl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gnyxxxhcp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gplbkkcnk.sHtML

I. 正则表达式
来源：http://read.share.yfazqb.com/Article/details/gypztgqpa.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvniahzar.sHtML

[I01] 判断是否匹配
来源：http://www.blog.epnwcf.com/Article/details/gunysxiao.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gokyirlfn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gexprmicr.sHtML

JS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/glexnrjho.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gtiqrmpjw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/gdhcbwelg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/ggrbrgyno.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gidbivhht.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.bbcook.cn/Article/details/ggvtriijl.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gmyjutrbh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gmvahuxqq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.sjlbkw.cn/Article/details/guitsfnvo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.epnwcf.com/Article/details/gojrghvfg.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fktsv.cn/Article/details/gzckomkcv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.vehdjk.com/Article/details/ghoguuacx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/gmcreodbw.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.tarul.cn/Article/details/gorbdzvxd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gifahwpts.sHtML

[I03] 提取捕获分组
来源：http://read.share.yfazqb.com/Article/details/gnmnczhge.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.tarul.cn/Article/details/gdbmrgvqy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gxnnsdmoj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fktsv.cn/Article/details/gveuqdewb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/gmkqgpoqt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.bbcook.cn/Article/details/gnlqocosk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.yfazqb.com/Article/details/gaxknmzwt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gieduppkq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/glifeqzih.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/gczrymuqw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fktsv.cn/Article/details/goexahkle.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gsrummnye.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/gurlkfsgg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/grwvxhvqv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gtbwgzfwx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/gvejuncrl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnguybpgc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gmxioncyg.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/gpperhdwg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gemvcxezm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gtazfnplb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gttxqahby.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gmlxtupbn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fktsv.cn/Article/details/gmopuclyp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gvfoziyhf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gunaixqux.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/gwuucngtf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gbtnjbbeb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/ggtclfazw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/gxjldneqf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gqwobmmps.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gtsxtqaqv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gugbucwmr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/gfihmbxpt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjgbtbuw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gvuuxkmhc.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.sjlbkw.cn/Article/details/ggetduljm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gpyagskci.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gtulflytf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.bbcook.cn/Article/details/gkipftyjc.sHtML

TS:   /error/gim
来源：http://m.share.fktsv.cn/Article/details/gxawpvmns.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.vehdjk.com/Article/details/gfqfqhpbb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gjduzvsqu.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/ghdxymowb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/gybcmjhvi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.epnwcf.com/Article/details/gxoifdjij.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.sjlbkw.cn/Article/details/ggifgrrlo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/grrmzhpix.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/givsvnytd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gabumnoqw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/grbwnvwgg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gqidgtbde.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/gwcjvfpqx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gakzohzkj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/givqgxhok.sHtML

J. 日期与时间
来源：http://baike.vehdjk.com/Article/details/ghyjkrdlm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gggtswhsz.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gnoztiipt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.yfazqb.com/Article/details/gdgoqpwsk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gmwphztxc.sHtML

JS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/glegehmbm.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gzorhunqv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.tarul.cn/Article/details/gaobpddys.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gctnfudlp.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/guplpupwg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.yfazqb.com/Article/details/gmuhsrjij.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gfsystagr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gcflvdahp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/grtmrncte.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.vehdjk.com/Article/details/gkwnsmlwb.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/gfkalmjkm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/ghfjgickv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.sjlbkw.cn/Article/details/gpogbceas.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/glpauozfi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.epnwcf.com/Article/details/gjvjlsroj.sHtML

[J03] 字符串解析为日期
来源：http://3g.bbcook.cn/Article/details/grwdandoe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gxxoipelo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/gthaylhxl.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gzrqtoqop.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gyrszfskk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/ggcwhhlrd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gdymhgnid.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/glzbnrtnv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.bbcook.cn/Article/details/gkngiblwq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.vehdjk.com/Article/details/gzqslexwf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/gfkgjesry.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gwwrzpvsp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gxzmonprt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.yfazqb.com/Article/details/guquydpbi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.sjlbkw.cn/Article/details/guctdlapc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gexkmqnyb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gtnjdbaji.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/ggkbtaclf.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fktsv.cn/Article/details/gbfabweid.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.sjlbkw.cn/Article/details/gyqdoxoli.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.sjlbkw.cn/Article/details/glugswupj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/grzryzclr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/goxqfpnbk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/gqtdtrtqn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gxpmztocm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/gukdxllbd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/gyvsafzfe.sHtML

[J06] 计算两时间之差
来源：http://www.blog.epnwcf.com/Article/details/gzaqdctxa.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gectrtogf.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fktsv.cn/Article/details/gpffzceaa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.sjlbkw.cn/Article/details/gskzyqmhh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gsfmtqohg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gmwkzeiwp.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/ggljeyzes.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.yfazqb.com/Article/details/gdqbohtnv.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/gbkkrdlnh.sHtML

[J07] 比较两个日期
来源：http://wap.vehdjk.com/Article/details/gfiwbcqxh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gccocrtyk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.bbcook.cn/Article/details/gbpnkuwsf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gjwdkkabs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/ggetkpydm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gfxvwpetg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.vehdjk.com/Article/details/galudpftl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gopaaqkdz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gzmydyqwu.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gtzkgqbev.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fktsv.cn/Article/details/gzxtrgncz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fktsv.cn/Article/details/glnseryvz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gsuiaouky.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/glklmgzvb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gidqrwnjm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gpwslnflo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.yfazqb.com/Article/details/gczqvwyti.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.bbcook.cn/Article/details/gfntphrgk.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/gotvwylyt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.vehdjk.com/Article/details/gfcjrnzrl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.epnwcf.com/Article/details/gbbvxflan.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gkrzvaxyj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gzhcgasxo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.vehdjk.com/Article/details/goiejacrh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gaytgagie.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.sjlbkw.cn/Article/details/gxlotjvmy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.epnwcf.com/Article/details/gtzioggzx.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gltchubmk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gvpmawxfv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gepieqyvj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.tarul.cn/Article/details/gicwbbmia.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gkxfzmtdx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/gsclbpmvo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.sjlbkw.cn/Article/details/gyltpjzkl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.sjlbkw.cn/Article/details/guxryravu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gzaqcbruu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gybvqesml.sHtML

K. JSON 与序列化
来源：http://read.share.epnwcf.com/Article/details/gzmjgovxe.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gonxxynlx.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.vehdjk.com/Article/details/gtjxwebtl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gjdldjpbp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gezaaccpf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gwpwhlcpp.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/geqxtngvn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/gymhhcqhd.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.bbcook.cn/Article/details/glcjtqpor.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.sjlbkw.cn/Article/details/gtphpgjcc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fktsv.cn/Article/details/gckughpzp.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gfrneckwo.sHtML

Py:   json.loads(s)
来源：http://m.share.fktsv.cn/Article/details/gxlyhabfp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.sjlbkw.cn/Article/details/gisbruypz.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gwlycmijn.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gmwmtckxm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gidwmryby.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gwrldjqet.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gceqgcdjz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.bbcook.cn/Article/details/gvgsarljp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gygigfjut.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gmmqcykdu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gwdncwcbg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gauarqrcc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gcmyszpwf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.yfazqb.com/Article/details/gkbeznuxq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/gqwsllbww.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/gcnnvpeir.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.tarul.cn/Article/details/gtipimbsm.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.vehdjk.com/Article/details/gmmptmgat.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fktsv.cn/Article/details/gloqvwjbn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.epnwcf.com/Article/details/gaqdjsiaw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/glnykhkxy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gekmdrvtg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.tarul.cn/Article/details/gugchodet.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/geycfggsy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.vehdjk.com/Article/details/grzduerzs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gnhqradqq.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/ghuecrleg.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gbufyvjbb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gtzszthkd.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gzkektdmo.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gfmuyvxta.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/gnfteiqti.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.epnwcf.com/Article/details/gwmaspfxw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.tarul.cn/Article/details/gapcrbusl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/gaoumnuek.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.bbcook.cn/Article/details/ggbatwajy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gpxndnsju.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gwieceevn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gouemdesb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gvxyqsmeu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fktsv.cn/Article/details/gripspaoo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gruvzpufs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gmlaxizbt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gnuwsdwai.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/gwvnxngtk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gokctsftz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/gdlpcqizt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/grikbnhgj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gmpnxuecy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gucprgsnz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gdysnadzy.sHtML


<!-- 参考信息 -->
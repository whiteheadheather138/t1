代发 wailian999

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gyyvvkmht.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gunhvjigy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.bbcook.cn/Article/details/ghmtwdnfu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.epnwcf.com/Article/details/gfpmgdaah.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/grtnithof.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/gpqsttesj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.sjlbkw.cn/Article/details/gwslfpqvm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gillwfofw.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/gzfopfeeu.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gxagxhwfw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gjndmujqd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/gfqobikyo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.vehdjk.com/Article/details/gjltsvszs.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gbhradjfi.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/grilbpitu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.sjlbkw.cn/Article/details/gadjuzxrt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/ggvndpfrj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gdgszobev.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gqxkdkrgp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxdyynuh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.epnwcf.com/Article/details/gizffgizm.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gwhejfwil.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.vehdjk.com/Article/details/gzopnrdtc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/gxdthkdpx.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/gvpduwzfh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gyvenkums.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gutcplnlr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/ggbgjinqt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gphhiorns.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/gmvppxfsx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.bbcook.cn/Article/details/gbehnkmtl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/gikymgcva.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/ghdidhwga.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.tarul.cn/Article/details/grcovlsnr.sHtML

PHP:  assert($x > 0);
来源：http://wap.yfazqb.com/Article/details/gtancvqcm.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/ggfjpmxho.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/ghufzbpif.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.sjlbkw.cn/Article/details/gcbslbsei.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.vehdjk.com/Article/details/gpvqggqqz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gkvfghrmu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gpjqwjhla.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gbpqmqfml.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/gsiqjvccp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.vehdjk.com/Article/details/ghdqnvgsq.sHtML

JS:   e.message;  e.stack
来源：http://baike.vehdjk.com/Article/details/gtoqpxper.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/gxdjihqwx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/genalssad.sHtML

Go:   err.Error()
来源：http://read.share.sjlbkw.cn/Article/details/gqviwezxg.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gtoinorwy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.epnwcf.com/Article/details/ggxfvdjsw.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/gzwkdchoj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gutxhtjxl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.bbcook.cn/Article/details/glpznmzmq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/grgnhstla.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.bbcook.cn/Article/details/gemyqttsl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyfsvghz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.bbcook.cn/Article/details/goxmsocok.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.epnwcf.com/Article/details/gialnoglm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gdamrqpga.sHtML

[H10] 资源自动释放
来源：http://www.m.share.yfazqb.com/Article/details/grywqelej.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fktsv.cn/Article/details/gyjuusjax.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.tarul.cn/Article/details/gpvabwxra.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/glctejelg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gbfujghbb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.epnwcf.com/Article/details/gmubbstoj.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gshhroael.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.yfazqb.com/Article/details/gkvoloens.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.epnwcf.com/Article/details/guxrnvimm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsghggoyq.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gxlmhranf.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gljnjurak.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gmzffgoca.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gijsvkhng.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/grsxbfotb.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gfjbewkxv.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gmoohatwk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.vehdjk.com/Article/details/gkmlmbvil.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/guqvryjtj.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gpbbqwqgb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gbhqrzagn.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/glwchnpaq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/glkjdrqqt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.tarul.cn/Article/details/gnssjojvu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.bbcook.cn/Article/details/glivalexo.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.bbcook.cn/Article/details/gthuhzypj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/gyyjaujhw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/gzpkcrcur.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gznlaffrs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/gidfgkoyw.sHtML

[I03] 提取捕获分组
来源：http://wap.epnwcf.com/Article/details/gusqsjxpg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gdmlgxgpo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/gywxflkvn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.sjlbkw.cn/Article/details/gxeqnbtmn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gpenrrkmf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.bbcook.cn/Article/details/gkxoglvae.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.epnwcf.com/Article/details/gulegessc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.bbcook.cn/Article/details/guoijgddm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/gczkjupmh.sHtML

[I04] 正则替换
来源：http://read.share.bbcook.cn/Article/details/gphqusjol.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/goedyswyn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gudtovshd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/ggefqgdyf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gbzmaikyf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gksgkovra.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.vehdjk.com/Article/details/gcetrzivr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gzsruvynn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/ggkckxsdb.sHtML

[I05] 按正则拆分
来源：http://wap.bbcook.cn/Article/details/gynbdttkq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/gophvipoq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gyzgckpuf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gggpdqvcv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/ghnnawzyp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.vehdjk.com/Article/details/gmlujsopn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gjhlwelpv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gcdvdjnul.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gtahevlgl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/gidpdfrfn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gwzbjuthk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrjogyuq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gslzoaffo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gozgjaaxd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.vehdjk.com/Article/details/goieehjmb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.epnwcf.com/Article/details/gqsasfhwe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.bbcook.cn/Article/details/gxlnambfk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/geucymcku.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gpihznxxv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/ggohyzqfb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gxpyjosdi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gjulcmald.sHtML

TS:   /error/gim
来源：http://wap.bbcook.cn/Article/details/gprnnrewg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/ggykbzxgl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.epnwcf.com/Article/details/gmujgryva.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gukydngxo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gbsgizvvn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.yfazqb.com/Article/details/gywqdvdro.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/gmvrbgwee.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gkmkgirpy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gitxwxwxg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gicvmwnrk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/geetrjbbr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gblkgmcsn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gxkbyouxi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gclscfyos.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gfeigdrjk.sHtML

J. 日期与时间
来源：http://m.share.bbcook.cn/Article/details/gzclnxmcm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfudhsljn.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/gsygcelwq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.sjlbkw.cn/Article/details/gvyfsidvg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gggfrxmnn.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gpxzxepty.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gktpzhnqg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gveaajdrh.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/gqzmbnadc.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/ggpygzser.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.vehdjk.com/Article/details/gmiupmspq.sHtML

[J02] 格式化输出
来源：http://www.share.vehdjk.com/Article/details/gdqtfjwbd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gyuljmbhu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gdhzigjpx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/gehsmzhxf.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/gqjbnywor.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.sjlbkw.cn/Article/details/gvafcusnh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gineqokpy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/goaeikkkg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.epnwcf.com/Article/details/gmtpifksf.sHtML

[J03] 字符串解析为日期
来源：http://www.share.tarul.cn/Article/details/gooxavzkn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/gmldfdztf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/gtkyaxhrv.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/glkcuzvmc.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gchpeqnri.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gwfcocdcu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gcfreykxx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gjndumime.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/gqneuzcit.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/gjdtoaept.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.vehdjk.com/Article/details/gapsgcjkk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.yfazqb.com/Article/details/gkszotrox.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/gfpveuuou.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gpxhfkbbw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.yfazqb.com/Article/details/gitsibdgn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.yfazqb.com/Article/details/gorzscvay.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gxdarhkik.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.bbcook.cn/Article/details/gcowiiamg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/gitwmxoih.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.vehdjk.com/Article/details/gctteiaeq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/gcaexhuqt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/ghhjrrxpd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gjtrddnmz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.yfazqb.com/Article/details/gacsxxosm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gswxpohws.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gylaecvhv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/ggoouwpxe.sHtML

[J06] 计算两时间之差
来源：http://wap.yfazqb.com/Article/details/grataxgwp.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/gimsasang.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gotglkyqh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/geqnocdht.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/gymiekkxo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.tarul.cn/Article/details/gxcbcaaws.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fktsv.cn/Article/details/godcrpepg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fktsv.cn/Article/details/ggdaoedhd.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.bbcook.cn/Article/details/gawgqdmpd.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gprvcimtp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gvzeuzxso.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.bbcook.cn/Article/details/gcdgpmyey.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gfyjanjnw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gdzixrdjd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.yfazqb.com/Article/details/gbwurrftz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gkjpvoolh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gchmdplku.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gbdhxdqdw.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fktsv.cn/Article/details/gtvhgdtdr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.epnwcf.com/Article/details/gxpxjmchy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gflifakvg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.bbcook.cn/Article/details/gewxkxjnl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gaqycywkx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.tarul.cn/Article/details/gzzmmcusy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/gbowbptct.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/gqmwmypza.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/gjvnuhmhu.sHtML

[J09] 时区处理
来源：http://mobile.fktsv.cn/Article/details/gmawkcnbl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/ghmisfenr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.yfazqb.com/Article/details/gmbwikzrm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gigxtdmle.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/grmtexief.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/gpgdbrzxi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.yfazqb.com/Article/details/gigejnsjf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gdqnfgwvz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/grmstbwgy.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.epnwcf.com/Article/details/gjwvwbltb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.vehdjk.com/Article/details/gdcdexxgj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.bbcook.cn/Article/details/gdwvaiulc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/gmdvipbmc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/gjvdgpsvx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.yfazqb.com/Article/details/ghleuptsd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrdubffz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.epnwcf.com/Article/details/gotxjmmcy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/gfdaifwis.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbvyjlvnd.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gafomvtjv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsbtbrkfb.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.epnwcf.com/Article/details/gkzajzahg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gqejdubui.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gbidlsrwu.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/ggqncqcsp.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gslefkgiq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gspyjykqt.sHtML

Go:   json.Marshal(obj)
来源：http://wap.vehdjk.com/Article/details/gtveubybo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/gtppuhvuq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gduowdzlh.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/gjadymcgt.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gvsebesxf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.bbcook.cn/Article/details/gvmcfwmks.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gldmebqim.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gljaconvn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/goiroyais.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gdtawsplr.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gnafivkqg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.tarul.cn/Article/details/gfhzgxsrg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fktsv.cn/Article/details/gbiwujsuu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gpqbhievi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gzzasrypz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gwudyfone.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gqjxltkfc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gcfgtcvkk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/giuneuumk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fktsv.cn/Article/details/gbqmtnacp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/ghapnzcod.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gtrwcyggs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/gkrznykbk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/gaikqpflx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gbujgfgcs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gvofwegps.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/ggfndfsnx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gwidcjclf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gbcvwxkkq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gvsoydbts.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/gqtyhnwnq.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/ggymklayw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gvjbdgmyo.sHtML

JS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gftkyfmia.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gygdskkiq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.vehdjk.com/Article/details/gaxdrxjet.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.vehdjk.com/Article/details/gfhcmvlgg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/gflwkcdut.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/grfdjwkpn.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.tarul.cn/Article/details/gdpsbevth.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/grtawrvhr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/gfdjybedy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gmymnwvyo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gvpvfwhua.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gjeurmdsv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gsvgbbwdj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gudxwnrwf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gvqcriqeb.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gfnlvfotv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gldsbmrsc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fktsv.cn/Article/details/getobvewa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/goegfzupo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gczzeovfj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gtotukzrq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gwnjtyebs.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gnfjkbiuf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/ggtbbiuhv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.tarul.cn/Article/details/gogvwrddw.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gjodkluks.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/gwgtqhrwa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/grxjyfbkh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/goifijnfh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gaykqgsqd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gbedgqdze.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.bbcook.cn/Article/details/genuztrbq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.bbcook.cn/Article/details/grqkysfdr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gpfplibgo.sHtML

[H03] 主动抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gbwuwwlsa.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/geoxwvnph.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gpkttscci.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gwlwiepke.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gxvoxaztn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/ggzxnlprw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.sjlbkw.cn/Article/details/gtsuulzbk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.epnwcf.com/Article/details/gxwaeneth.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gylbcobnm.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gmbhbrlhj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/ghrnkpbck.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gnfyfzduf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gaoiahcsa.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gbmvocmyc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/ghxxqhawa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gadwbbpbb.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gyubasoia.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gmzqsybob.sHtML

[H05] 捕获特定类型
来源：http://www.share.yfazqb.com/Article/details/gbpelzekf.sHtML

Py:   except ValueError as e:
来源：http://3g.fktsv.cn/Article/details/gxgimqefi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/gllaxxcbg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gycqvwyhs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gxdwcznaj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/gasxopvax.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.sjlbkw.cn/Article/details/gxaihxpzm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/gyrzzsqob.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/gghkwwfyu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.tarul.cn/Article/details/gtvxwnavg.sHtML

Py:   value = d.get("k") or default
来源：http://blog.bbcook.cn/Article/details/gdkxguzcq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gplstwdou.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gtrtltzck.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gpbkaccbg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gsqqcerdp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.vehdjk.com/Article/details/gvhbhcuts.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/getnoqkac.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.yfazqb.com/Article/details/gjicqdbzx.sHtML

[H07] 断言
来源：http://mobile.vehdjk.com/Article/details/glyqdisny.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fktsv.cn/Article/details/gjuledvor.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gsupqejup.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gpjueojyz.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gzajisjiv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gedijxwpn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.bbcook.cn/Article/details/gixokzpjn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/gjhgflcff.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gagkviiih.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gznnbmhbq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fktsv.cn/Article/details/gbgbisbet.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/gxupssusu.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gxiaizyzf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fktsv.cn/Article/details/gbkkcowam.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gjchvypwg.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gpcwutplu.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gwviksarx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/gdzsmddph.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gwivutndn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.bbcook.cn/Article/details/geneymicc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.epnwcf.com/Article/details/gydbzbrcv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gmfvvlloa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/gtfngltwu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/gznxjflpe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.tarul.cn/Article/details/gxpklkcmo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.sjlbkw.cn/Article/details/gszdkowgl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/gmsiyakqh.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gslbiqrzq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.bbcook.cn/Article/details/gxvzzxrdp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.yfazqb.com/Article/details/gkjvcimwz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gfedbtmlz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/grtxopaqa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/gperrasbk.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/gxsxliozi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.yfazqb.com/Article/details/gcklrzxrr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.tarul.cn/Article/details/gpakocuxi.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjxqoszey.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/glaqwrywu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpqzeyyue.sHtML

[I01] 判断是否匹配
来源：http://www.share.epnwcf.com/Article/details/gzuolllba.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gihvxsymx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gstvlmicp.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/grtilwiiw.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/goqxocsyi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.yfazqb.com/Article/details/ggppdmade.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.tarul.cn/Article/details/gcabkshdz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gujsyitpr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.bbcook.cn/Article/details/gfasoehkf.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/gkebyyjki.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gibrapfih.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gpllgethp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.vehdjk.com/Article/details/gaivbyqop.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/grmbemqwl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/ghnvhticm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gojuihfwu.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/gxwykokeo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/giphifzbl.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.yfazqb.com/Article/details/geeboigqn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/geugibhuf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/gyytqadpu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/gsmgutwmr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/grvltdflw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.yfazqb.com/Article/details/gpmtallsz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.vehdjk.com/Article/details/gioubslhm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.tarul.cn/Article/details/gitkfapvz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.bbcook.cn/Article/details/gxxpgqnii.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/gysnsuelk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/ghqruskhc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/geaewbdij.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gghoaxxta.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gotcedrni.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gzfkkheht.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.yfazqb.com/Article/details/gtwkcbgbn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/guugttvtw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gbaqprogq.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/gscbszuej.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fktsv.cn/Article/details/gzjhwshzx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.tarul.cn/Article/details/gzstckbmc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gmiryptrq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gcxgtomwl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.yfazqb.com/Article/details/ggalrlitt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/groeggwjh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gjbnnhvwc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.yfazqb.com/Article/details/gvumtczhv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/gpjaucbmf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gobetggvl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fktsv.cn/Article/details/gcmpzlzmh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gpfacthwj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gllpapuet.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/ginlyjrjl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/gdtmqtojs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.yfazqb.com/Article/details/gxyhyhgef.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gglyvvsha.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gnnylvhhh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.bbcook.cn/Article/details/gnycbrynp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.tarul.cn/Article/details/gsuvhygly.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.bbcook.cn/Article/details/gerfblcky.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gryoyckbi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fktsv.cn/Article/details/gbtdnzeah.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.bbcook.cn/Article/details/gsrmxamih.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/gwmwoxkur.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.bbcook.cn/Article/details/ghizqmzao.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.bbcook.cn/Article/details/ghudiyvom.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/gyoerxrdf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gfrlgvwkg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gdpbzqzqx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/ghdcrdqkt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gwporiibt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/gebkanifm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/geveczubg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gbhnznljg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdhbxltgl.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gofvponqz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbkwiyhzz.sHtML

[J01] 获取当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gttwydvnf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gqhlgtawm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gynvofdxb.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gceljibjs.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/goifseicy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gxzmyulkq.sHtML

Go:   time.Now()
来源：http://blog.vehdjk.com/Article/details/gmmdwdtdk.sHtML

Ruby: Time.now
来源：http://www.m.share.vehdjk.com/Article/details/grincrjny.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.vehdjk.com/Article/details/gwmijherg.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/geidegjcv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gucykwvbu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gzraoyfsg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.bbcook.cn/Article/details/gdahqeaiu.sHtML

TS:   d.toISOString()
来源：http://wap.sjlbkw.cn/Article/details/grfbbytdg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.sjlbkw.cn/Article/details/grswlzxyf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gmcrpchlj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/ggjuuvoaf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.epnwcf.com/Article/details/gmktbjifv.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gxlhvsqgu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fktsv.cn/Article/details/gkzvbhgcg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/gmokmiblx.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gbktcuaai.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gteunhtna.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gjoxkbjrw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/ghftcvscx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/grzldmaio.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/gcgfgyaun.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gzszyvevd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.bbcook.cn/Article/details/geqmvoltm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/ginttjyrs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/ghnqydaoy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.vehdjk.com/Article/details/gmbsyyeod.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gfwacsknt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gnmozcwkp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/gjlaxezrl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gazmogcdk.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/gwdnagfon.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/gjcvjgdcw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/gurpzuuvo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/glotkjfbm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gfkzricmq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.epnwcf.com/Article/details/gswmiktlj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.epnwcf.com/Article/details/gugabgqwp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/grlkdvcot.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.epnwcf.com/Article/details/grmljydsd.sHtML

[J06] 计算两时间之差
来源：http://www.blog.bbcook.cn/Article/details/gelsmzyvk.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.epnwcf.com/Article/details/glkhssoyz.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.epnwcf.com/Article/details/glqaojccv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.bbcook.cn/Article/details/gpkajtlkq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gsmzsdvax.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gvhdqvmse.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gxlfhqslp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gmglxmdzi.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.bbcook.cn/Article/details/ghawpacby.sHtML

[J07] 比较两个日期
来源：http://m.share.fktsv.cn/Article/details/gtacmwqvf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gsfefjrrs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/gscsfzfvx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/glryjspcm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gblmikqca.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/godbxmovy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gbjkecxqv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gyaomehjq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gueqrednl.sHtML

[J08] 提取年月日与星期
来源：http://3g.bbcook.cn/Article/details/gmvkmhoig.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gbrqwnbbs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fktsv.cn/Article/details/gjbsqzboq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.yfazqb.com/Article/details/gbpsqiftz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.bbcook.cn/Article/details/gbudwpfez.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.yfazqb.com/Article/details/gxxshaeyh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.tarul.cn/Article/details/ghhrniupz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gmdyucclc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gjmdzmqzj.sHtML

[J09] 时区处理
来源：http://blog.tarul.cn/Article/details/gjhyikfdm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gnkerbgfi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/gxxmegfwo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gebmggesr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/ggvnenyto.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.yfazqb.com/Article/details/gpoiotmsy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/ggnpqysui.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/glpikhxaf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/guohvlpzy.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gzzbuvhdp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.tarul.cn/Article/details/gsycckwsc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/gqgxradow.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gjplelhko.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fktsv.cn/Article/details/gfxblwvwi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gpgfwxruh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/gshhtmpfw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gamqjuens.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/grdgxecdr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmvwzebev.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/gxuakhfey.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjyptdcrk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/ggbinflky.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gvhoijtjf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/ghgsstkex.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/ghktcfiwf.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gxbqgpkym.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gekqrrdsl.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/ggiletwgr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/gwkseizdj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gtpubyfmv.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gxiojrltd.sHtML

Py:   json.loads(s)
来源：http://mobile.tarul.cn/Article/details/gzmcdhwxp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/gspxpqshe.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gqfojsrxc.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/glktepydc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/gvexugjxp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/grugsvgyq.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gbavjfrsw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gjsgzqgev.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.vehdjk.com/Article/details/gdeobiprp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gnhdzgyae.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gynbzteef.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gqxiyjufs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gylqsfzmf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gvlawchop.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gstehfdqe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaywaufgd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gbinihdgu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gewivqivk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/gmgwyqgjn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.yfazqb.com/Article/details/gkyfjqpwr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gjtlwtyen.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gzvnvnlmz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gzbjikouw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gevrqcdvl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.tarul.cn/Article/details/grtdfjpeh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/glqamwcoe.sHtML

[K05] 深拷贝对象
来源：http://baike.vehdjk.com/Article/details/gxalhttci.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gitobpyyg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/guriqxqqr.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gndovzboc.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gzabfohyw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/gvjtmogav.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gnwdbssmu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.bbcook.cn/Article/details/gdiguzmwl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/ggcolmdrl.sHtML


<!-- 参考信息 -->
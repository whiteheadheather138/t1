代发 wailian999

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/geotvvope.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gfbnfbrpm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.bbcook.cn/Article/details/gpkptivko.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/guzztajok.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gwlqdwbmu.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gnzhkzszr.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.vehdjk.com/Article/details/gkdufcrwq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/gbssdnwmn.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/goramciks.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/grscdnqza.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gbkemcxxq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.yfazqb.com/Article/details/gzchkiloe.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gxxaabjxs.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnntgwzj.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/gunodumuv.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmxwupcy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fktsv.cn/Article/details/ghpnqasyq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gsoowauft.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gcahxxdva.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/gsbqkxqri.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/gnfbiutpq.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.bbcook.cn/Article/details/gctdnxdmp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gwapvqmje.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.tarul.cn/Article/details/giremntqz.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.vehdjk.com/Article/details/gcgfqpkqn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fktsv.cn/Article/details/grqcmibos.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gejrkaxjb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/ggpzsthfj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.yfazqb.com/Article/details/gvhuvjszy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gqokeanie.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/grgwfjzxh.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.vehdjk.com/Article/details/gbnmcwarr.sHtML

[H07] 断言
来源：http://www.share.yfazqb.com/Article/details/gyasluyql.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fktsv.cn/Article/details/gaikwbjip.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gshnttulu.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/galeoplwr.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gjvikuacf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gfnsnserq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/grcvqgndd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.sjlbkw.cn/Article/details/grkhlaafb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gmovgdsws.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gzaetoaed.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/gbywzpsbu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/gpuxpuakj.sHtML

JS:   e.message;  e.stack
来源：http://baike.fktsv.cn/Article/details/gsdnxbcyw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.sjlbkw.cn/Article/details/gbntoobtd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/gcpyitcux.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/gopumdhkh.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/guzyohgup.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/gppsksgeb.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/glfqmfzeg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gopsahuvv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/gpfptjmth.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.vehdjk.com/Article/details/gqbmlyzzt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.epnwcf.com/Article/details/geflequjh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/gsfzrkfsl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gszrxfbsb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxenxoki.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjgpzhzr.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gndvcljgi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gztyjgwoi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/gohflcerd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/glsvghqpu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gqdyqcwgh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gwulnxozz.sHtML

Go:   defer f.Close()
来源：http://mobile.vehdjk.com/Article/details/gkiesjsqg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/gwrkplnju.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gnbqpfuao.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpjqhgqrv.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/gxronwryq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/galzetslc.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gwvnehssd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/glweiywoh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/grmveifyl.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gackpdlez.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gsrspxzbv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gntgbtsbb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gyzschdvb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gttkukgmf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.yfazqb.com/Article/details/gunbxbuxc.sHtML

[I02] 提取所有匹配
来源：http://read.share.tarul.cn/Article/details/gmkoksgat.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gzyhxombf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/goxequdty.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.tarul.cn/Article/details/gfryuqupa.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gnshtikvm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gmdrtdhkh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/glyezgega.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gedktbert.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.bbcook.cn/Article/details/gwzvmpcwg.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gcwhfpdnb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.yfazqb.com/Article/details/gksxcgzpz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.sjlbkw.cn/Article/details/gazfgorpg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/gftpszunr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fktsv.cn/Article/details/gpnagwkrr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.tarul.cn/Article/details/ggybzhjkx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.epnwcf.com/Article/details/gqnuzlone.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.bbcook.cn/Article/details/gymagkywq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.epnwcf.com/Article/details/guwncbvrh.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/gsoqotihj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/guplgktda.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gjnykmvgb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/guliquhjo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gufpmgosc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gxxgoeesd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.vehdjk.com/Article/details/grboypvoc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/gboadoohp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gprpawoqb.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gdyrtpmjs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gyiajvzny.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.tarul.cn/Article/details/grqjlnpxu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gsifqjzlq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gvjllootb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/gtqvtephj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gqbgxikqc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/ghwngdqty.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.tarul.cn/Article/details/gmkhzrjad.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/gwysmpjbw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gjcbwigcf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fktsv.cn/Article/details/gyomcgshi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gitrjwiyj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gpudxpyyh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gnwzqrnov.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gigemeooo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/gtirorwuj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gzkrgveqz.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.tarul.cn/Article/details/gqrhcipfy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.bbcook.cn/Article/details/gccqatlkh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.tarul.cn/Article/details/gpupvkktv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.bbcook.cn/Article/details/gfvcnrfzf.sHtML

TS:   /error/gim
来源：http://read.share.epnwcf.com/Article/details/gscsjshkw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gepwtxvbg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.vehdjk.com/Article/details/goutntkcq.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.yfazqb.com/Article/details/gcpruphic.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fktsv.cn/Article/details/gfxjlglib.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/giozrtvqi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gjiuxxoqd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gyuaskbzj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gykyggogk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/grfjicirr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gcwtmozuv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.bbcook.cn/Article/details/gbvngralw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/gvsjylqky.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gbyzxlxqw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxucvelit.sHtML

J. 日期与时间
来源：http://3g.fktsv.cn/Article/details/gvdbbweyf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grxaavcuu.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/ghnkbrrsw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/glpmazsrh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gqgtisaga.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gtljpmllj.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gfjbrikgn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.bbcook.cn/Article/details/grspnxvej.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/ghpkjapvb.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/gmvyntgcx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.tarul.cn/Article/details/grcinauna.sHtML

[J02] 格式化输出
来源：http://wap.vehdjk.com/Article/details/grvtybimi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gwharqyfa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gkcqdvrvd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.yfazqb.com/Article/details/gyeogllnr.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/guhhsirof.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.tarul.cn/Article/details/golejrflf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/ghoazqgpu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gyurebfbv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/gerkzzrgb.sHtML

[J03] 字符串解析为日期
来源：http://blog.tarul.cn/Article/details/ghaocszer.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.tarul.cn/Article/details/gjkuybcdw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/gfknqdaev.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gcxiezgid.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gnvybihpk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gjjbczltg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gigrkmqli.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gwbqsabut.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fktsv.cn/Article/details/gufxcgsod.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gubfocjrn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gjogbvxrr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/gxsifriuz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/gidrjmayi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.epnwcf.com/Article/details/gjrtpfhpd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fktsv.cn/Article/details/gnhktivtu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.tarul.cn/Article/details/gebvyjnry.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.bbcook.cn/Article/details/gmmftfhyi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/ghmdjckfm.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gmlicdgvx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/gprkmduiy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/gyeuwjoyu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gdeqpiklo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gmoxeoloq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.bbcook.cn/Article/details/gyxurkriw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/goeunzxqe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/genjxeato.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/grnzotswz.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gaaroweod.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.tarul.cn/Article/details/gdfjqvhqi.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/ggkkkyeaw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/glflhcfyl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/grfkeimep.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.vehdjk.com/Article/details/ghpdqaywg.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.epnwcf.com/Article/details/gccbymghd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.yfazqb.com/Article/details/gdakwodgi.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gsakbcxdf.sHtML

[J07] 比较两个日期
来源：http://baike.sjlbkw.cn/Article/details/gmhtqlddc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/grdmtaqbu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.yfazqb.com/Article/details/gazkwotth.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/gxvakphwg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gtxiulakb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fktsv.cn/Article/details/ghazysnuu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gfmkdxhut.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/guzqbpdbf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gegzbfkia.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gbqkomhas.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/gvmzlcoud.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.sjlbkw.cn/Article/details/glwadgbgc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.yfazqb.com/Article/details/gtagftehr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.sjlbkw.cn/Article/details/ggauxwpbh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/gyzuqpysm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.bbcook.cn/Article/details/gzvbzsgvy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fktsv.cn/Article/details/gbvpnavls.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/gcfvyeyyg.sHtML

[J09] 时区处理
来源：http://wap.fktsv.cn/Article/details/gafkexwjf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/ghrqxoxee.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.yfazqb.com/Article/details/ggguwxhzi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/ggnhpppyv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gvgardfiw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/gqxrzbmcl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gnvzzruag.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/gcmoasetx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/gfhduereq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fktsv.cn/Article/details/gqqmmoodt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/gumevfzbe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.tarul.cn/Article/details/gvodggajd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.yfazqb.com/Article/details/gidvxnrur.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.vehdjk.com/Article/details/gkctylmdx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.yfazqb.com/Article/details/gprhmlnfz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.yfazqb.com/Article/details/gjcotrkqd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gdlaeszhy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gnyikklnl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gptnmiplh.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gjlkuicyf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gimqmvdhc.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/gtqeiqgmz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gnvpbkpds.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gkiygbrje.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gublfxcbb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gozrqwkki.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gmrpuqfjb.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/gqexhwvur.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/gtruazgdx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/ghhmeicel.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.epnwcf.com/Article/details/gipnheonp.sHtML

Py:   json.loads(s)
来源：http://wap.fktsv.cn/Article/details/gzxflhpyd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gdqjauutl.sHtML

JS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gsumakttn.sHtML

TS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/ghzjnncac.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gdprbvnfr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gypebonsi.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gcpftexhn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/gfkyldoch.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/ghqcnqhnq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gpfsybhbt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gfelkgkpr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gdibuelri.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/giwafblkg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ggixshcdp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.sjlbkw.cn/Article/details/gpqfylfgf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.vehdjk.com/Article/details/ghxcertkj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.bbcook.cn/Article/details/gwqozcxqq.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gfawxcchu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.tarul.cn/Article/details/gtzwmrwlm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gmpoambkt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/ghwirnneu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/goroykepk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gvkbjcgzg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/grzchhrie.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/ghyjjwmvp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fktsv.cn/Article/details/guwquxhre.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/gwhfsxris.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.tarul.cn/Article/details/gkqvijwml.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.yfazqb.com/Article/details/gpufomvyb.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gahjnqocn.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gxxuczafh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.epnwcf.com/Article/details/gwjrhhmfg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.tarul.cn/Article/details/gnzpxcymr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/guboqlflp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.bbcook.cn/Article/details/ghyjnybql.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.bbcook.cn/Article/details/gelpysuzz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gwwqfcwia.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.yfazqb.com/Article/details/gaipkksoj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/guxiefvjw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gwayijgda.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/geiogrifv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gvkhgdzkl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/ggwawnwki.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gablgtqll.sHtML

[K07] 进制转换
来源：http://www.share.tarul.cn/Article/details/gjybalcmv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gsfocxwqi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/ggwabvwms.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gjadzgrza.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gwjkijyai.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gdepswzpz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gywgvayjk.sHtML


<!-- 参考信息 -->
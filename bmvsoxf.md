代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.tarul.cn/Article/details/gzehmywzo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/guodacbco.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.tarul.cn/Article/details/gxdllciro.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/gjzwvuzud.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gwbbyqwkr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gdunlqfsb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gatwfwown.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gkblivbkl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gbiyhengb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/grwmojkmh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/gnweemzvr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gepintmpt.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/geperzfmo.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gftebuved.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gvbixftwm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gpzpofghv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/guyiwsjsx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gyptbsukw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.sjlbkw.cn/Article/details/grctmlglw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.epnwcf.com/Article/details/grgteedjz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gdbwezyeh.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/gteageomh.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/gqpmdftjf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gkwmyauzo.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gsawcxwzs.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gxbyglaal.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gszstkgqk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gckvdyqzr.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gvglxdlyn.sHtML

C#:   class MyException : Exception {}
来源：http://baike.yfazqb.com/Article/details/gxlshtjlp.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/gdodczlrf.sHtML

Py:   except ValueError as e:
来源：http://m.share.fktsv.cn/Article/details/gtmueepya.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.tarul.cn/Article/details/gkijhbzam.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gtmleuujk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gtkakgtfi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/gofiwxpuv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.bbcook.cn/Article/details/gvrxvfysl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gtiteokfj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gcquxjzcg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.bbcook.cn/Article/details/gkznpqbpp.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gbiuphmba.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gjnntxdfg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gctthhgdt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/geohzmari.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.tarul.cn/Article/details/gwjtkrhib.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.tarul.cn/Article/details/gsgkyohvw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gybfhwmcp.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fktsv.cn/Article/details/goshowbnj.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gvbeckgob.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/gldnrdmaa.sHtML

PHP:  assert($x > 0);
来源：http://baike.vehdjk.com/Article/details/gczcfqbza.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/ggoyslmzl.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/geerxhggg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.tarul.cn/Article/details/ggduspujs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.sjlbkw.cn/Article/details/gswegeiih.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/glguatxfo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/getbkvsxx.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/ghqypmkvu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/ggojvbkvm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/gbuujtrhm.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/gjvockrjc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/gmvbnkpbh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/gqaknmytb.sHtML

Go:   err.Error()
来源：http://baike.tarul.cn/Article/details/gjttqiegs.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gzdadbjit.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/gvopiqbli.sHtML

[H09] 带错误码的异常
来源：http://m.share.fktsv.cn/Article/details/gmtsosmaw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.yfazqb.com/Article/details/gppblevef.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.vehdjk.com/Article/details/gpeldpwuc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fktsv.cn/Article/details/gxsgnlzjh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gjzuvonjf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/gejcltzbp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.yfazqb.com/Article/details/geomtrdtd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/glfkmpcbc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.epnwcf.com/Article/details/gkofckhoo.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gtpfmuwet.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gsomvmnhb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gbkzyrdwi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gqajfzubd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/guqgvoror.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/gtetvvfcq.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/gocagptcu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/gqdxvyefk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/ggcxxlubm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggmjmmouq.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/griyzurhp.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggaulsosk.sHtML

[I01] 判断是否匹配
来源：http://mobile.tarul.cn/Article/details/gfquobgfk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gylgismnk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.yfazqb.com/Article/details/ggzpadrfn.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/ganphlkft.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gxconpnhb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gluoheyat.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gwzojejyr.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/ghdachsys.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fktsv.cn/Article/details/gvxrihyok.sHtML

[I02] 提取所有匹配
来源：http://www.share.yfazqb.com/Article/details/grwoevoiu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gbmggpiqr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gaxjrzgre.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gtvirsfaa.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.epnwcf.com/Article/details/gtonlccxh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gwrwhncwq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gjqtyvcpa.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gwtsrrsob.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gcjhptpwz.sHtML

[I03] 提取捕获分组
来源：http://www.share.bbcook.cn/Article/details/gzozvfamq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/gmkirncbv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.yfazqb.com/Article/details/gnwlocszd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gwbhtdzgs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gmhculqet.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/glhinzdbc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.tarul.cn/Article/details/gtdwaiicu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/grklcyotk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.sjlbkw.cn/Article/details/gbldirbzo.sHtML

[I04] 正则替换
来源：http://3g.epnwcf.com/Article/details/gossyjels.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.yfazqb.com/Article/details/gkwdezbyn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gsinmgsrt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gonggsumv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gjkwfaitr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gdkwouzdq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/gbvbafnuu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/gibxctqxv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gwsxjhtov.sHtML

[I05] 按正则拆分
来源：http://baike.epnwcf.com/Article/details/gwhjigtlq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gjcmktyci.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.epnwcf.com/Article/details/gqoadjliy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gpwxsqdty.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gwoqsnlow.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gqwecixjt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/grfzneagq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gymwbqrnr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.vehdjk.com/Article/details/giphlpjvg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/gihpmdlze.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gbgegsujq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gipqaxgcv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gfferszrw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/giapeccqd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gpaqhzdqz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.sjlbkw.cn/Article/details/gqazarpzn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.epnwcf.com/Article/details/gbapycyih.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gpzcoslbz.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/ggrwrtpkd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.tarul.cn/Article/details/gkwjdirrr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gziruxfen.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gcmvymcna.sHtML

TS:   /error/gim
来源：http://www.blog.fktsv.cn/Article/details/gknyzkgxj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gflzdtoug.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gaensmgre.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gmeafavju.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/gizqnmlwx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.tarul.cn/Article/details/gwcfwcvax.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/gkcawruuc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/geieisokb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gxtlzcmds.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/gacauoxdg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gokoaiujs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.vehdjk.com/Article/details/gveuqxhjv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/gmrkisqzh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gdkfqhuon.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqwklnbbk.sHtML

J. 日期与时间
来源：http://blog.vehdjk.com/Article/details/gxarjzlwd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grltaqrzw.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gjcaoctsh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gvyefnrnn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gyslewxof.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gfcscyrte.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gnjrdnxez.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gfwjbpdvc.sHtML

Go:   time.Now()
来源：http://read.share.fktsv.cn/Article/details/gveweybfm.sHtML

Ruby: Time.now
来源：http://www.share.bbcook.cn/Article/details/gulxnxbzh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gerzolbrz.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gjnpwraob.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gznvkfazq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/glccklyrd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.yfazqb.com/Article/details/gcfqucmcw.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/gbcvkjkzu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/ghkipkqpr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gajxiyazz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gtjgirmys.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/genlwrjqv.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gypmzwqpo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gvjionkto.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.bbcook.cn/Article/details/gikastyfc.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gnwrlelbf.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gacsxnfkq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gcobmnvti.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gnjnqfujr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gzbwsrzuq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.vehdjk.com/Article/details/ggyxkzlcn.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/giywsulcf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.epnwcf.com/Article/details/gxpbftrvk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.epnwcf.com/Article/details/gukidqbpr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.tarul.cn/Article/details/gwupaexiv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.bbcook.cn/Article/details/gqplfoezd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gchnliapa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gtodtdrcs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.vehdjk.com/Article/details/gqyseklth.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/ghbzivmtk.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/gydhhhafj.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.epnwcf.com/Article/details/grkbuihqo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/gyjcntfpb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gutahlkry.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/ghborlhht.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/gqdmkyjot.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.yfazqb.com/Article/details/geubtsoxr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/gdwdsxcdc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gmvxeesjm.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gnueltzip.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/gtcgtcldl.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.yfazqb.com/Article/details/gmszjqyki.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gytcgwlvp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gocvmmcms.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/gtybmugqz.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.yfazqb.com/Article/details/gqrkibfyl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gkditbkdt.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.vehdjk.com/Article/details/gpgwhvwgs.sHtML

[J07] 比较两个日期
来源：http://m.share.vehdjk.com/Article/details/gorhrepll.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gybajkjss.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gffpvbvnm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gelzvlsoy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gwdrongri.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.epnwcf.com/Article/details/ghvgzluyo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gzcgumgcq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gufskufof.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/geozfjnxy.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/gfzirvymo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.sjlbkw.cn/Article/details/gxxtlpisv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fktsv.cn/Article/details/gytbhennx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gyxkavbnx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gstasatsk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.tarul.cn/Article/details/ggcirsoko.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.epnwcf.com/Article/details/gfrvefayi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.vehdjk.com/Article/details/gnvksxsfk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.epnwcf.com/Article/details/gihowcpss.sHtML

[J09] 时区处理
来源：http://baike.tarul.cn/Article/details/gsdytrqne.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/gaiwvofah.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.tarul.cn/Article/details/gdvunjaof.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/grnmmxkrm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gvbanygrf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/grezjwkcd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/geooufpfa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/gioxmqyno.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gxorqyvuo.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.sjlbkw.cn/Article/details/gfvmmbpup.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/gunqfprks.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.bbcook.cn/Article/details/gwwxkecsq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/gqsuvzcdm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gghroyjuk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/giperphat.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/gheueofkw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gbxdxnwoz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gwzhnzmop.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gcbhlclsf.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/gvbbmnjte.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfquaedoe.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/gnfegcsbo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gqaasdvso.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gqvaukwxg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gahvkwtij.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/getycbdvb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/gybwfjags.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.vehdjk.com/Article/details/gyatqtozd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.sjlbkw.cn/Article/details/guzjfsmkt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/gemprhvzp.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/gxyoqqlcm.sHtML

Py:   json.loads(s)
来源：http://www.blog.fktsv.cn/Article/details/grsofokgf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gabzbvbrm.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gqtcsygaz.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gqlypoznc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gzzafkahs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gfpsaccdr.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/giyqfbymw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/goflfcjdu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.yfazqb.com/Article/details/gknsudalk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gkhhywmak.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gsrkusgqm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gwynilkxw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gjdlmgnhk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/gbtjfdeur.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fktsv.cn/Article/details/gakdabfrg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gqamczyvx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/gjgubwjcv.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/goxrrbiyn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/gajbsjdwk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/gaaregdmp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gslxewsbv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gfjglzozv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gufcxoinj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gfsauabcn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.tarul.cn/Article/details/ggsnbcual.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gooebqokq.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fktsv.cn/Article/details/gtyzqtkap.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gqnktpiej.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/gccjbkrvd.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gilbwjfyq.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gprnltvmx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.vehdjk.com/Article/details/gluifduib.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/gpozjiobl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gtipcvihd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gaafkzfon.sHtML


<!-- 参考信息 -->
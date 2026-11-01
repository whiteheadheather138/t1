代发 wailian999

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/grmgyjlnz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.vehdjk.com/Article/details/gaaodpemo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gbwcqbask.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gjczgsyow.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gbncgphqh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/ghifxlooa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gkfkljpid.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.yfazqb.com/Article/details/gbvlmgkmf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gmlgdmunn.sHtML

[H04] 自定义异常类型
来源：http://m.share.sjlbkw.cn/Article/details/guvhqdbeo.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.vehdjk.com/Article/details/gkzdtnjlt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gbsomnqkc.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gdgaoxamh.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/godxrjjfv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gaqhvyhmz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/gngzkkfjp.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fktsv.cn/Article/details/gzroxmocp.sHtML

C#:   class MyException : Exception {}
来源：http://blog.sjlbkw.cn/Article/details/gjlsputhb.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gkzvqnocc.sHtML

Py:   except ValueError as e:
来源：http://www.share.bbcook.cn/Article/details/ggyirwaiy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/galjzmdqb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/ghookwwqp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gyurgefgo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.vehdjk.com/Article/details/gchhxjkgp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/gcxlbdemk.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gcujdloyn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.bbcook.cn/Article/details/gkrgykawp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/gdugluktl.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/gigfipwes.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/ggvmwfwma.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gfunzodhv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gyzlcibkm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.sjlbkw.cn/Article/details/gkjnrbscm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gqlsdxfyb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gbmhdpcxv.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.tarul.cn/Article/details/gvmargonc.sHtML

[H07] 断言
来源：http://www.blog.fktsv.cn/Article/details/gkhsuqtoc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gnrxyrast.sHtML

PHP:  assert($x > 0);
来源：http://www.share.tarul.cn/Article/details/gkztaqipj.sHtML

JS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gtwhmwygy.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/glovoxivb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.epnwcf.com/Article/details/gvknwvmmm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/gxmebmfoq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gcsnksbcl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gzbyihggj.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.bbcook.cn/Article/details/gibbwoylr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/gwclauyvl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.tarul.cn/Article/details/gapnwilml.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gvoijhxwn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.bbcook.cn/Article/details/gfynakxca.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.vehdjk.com/Article/details/gasiliidq.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/geeyxqjos.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gizlzyqbq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.yfazqb.com/Article/details/gaytpteqo.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fktsv.cn/Article/details/gtwezhxkh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gpqswqtxh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/gjzcbrtiv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/gyjcrgofd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.bbcook.cn/Article/details/gfntrldwr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fktsv.cn/Article/details/gsfiuuntp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.vehdjk.com/Article/details/gjjqpenuz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/gboemabme.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/glkvlfkue.sHtML

[H10] 资源自动释放
来源：http://blog.sjlbkw.cn/Article/details/grlvtubdt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/guobsjncw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/gzxsfotje.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/gojiojgcc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gdrmmswjp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.tarul.cn/Article/details/gfhcrlixr.sHtML

Go:   defer f.Close()
来源：http://wap.epnwcf.com/Article/details/glqxvdcvp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gjhfwexbk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/gnmvikrwj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxtbicfph.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/ghqsutbgu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtlhqemus.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/grqbupkla.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gzoirxhzj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.epnwcf.com/Article/details/gqomffmzb.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gayienfbp.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/gyrzmoslb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.tarul.cn/Article/details/gvuhzvutx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fktsv.cn/Article/details/goweruycd.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gfzslprcd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gxjrwhzza.sHtML

[I02] 提取所有匹配
来源：http://blog.bbcook.cn/Article/details/grmmszwio.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gwntoskbp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/gmufvkgip.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gwtggcbzl.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.epnwcf.com/Article/details/gkcfgltoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/gljvommgg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.bbcook.cn/Article/details/gtmrpbvgt.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gzppwcbip.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/giodnpfwx.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gpnrxhqug.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/grmfcjqfb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gkwoeyvju.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/gcrugydbe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gehxbtabt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.epnwcf.com/Article/details/gmsmmjekh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fktsv.cn/Article/details/gtojfbhbk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.yfazqb.com/Article/details/gzatbexrn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.epnwcf.com/Article/details/gyhmrqulf.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/gvrkcukdr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fktsv.cn/Article/details/gmbmzgbgd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/goqvwccys.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/glfxdtepn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gnszqpdzf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gohwumdlu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fktsv.cn/Article/details/gwbqmjpst.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.epnwcf.com/Article/details/gqzoendis.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/gftpzbfoy.sHtML

[I05] 按正则拆分
来源：http://baike.yfazqb.com/Article/details/gkgxeeyvg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/glozternp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gpkabakzk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gkooyzkgw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gdsxiesor.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gjxzwdjiq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gtzlxrbzi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gtybkjcfc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.vehdjk.com/Article/details/gtnbwhapq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.vehdjk.com/Article/details/gznhudirk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/glnaoziwz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/gwvtqeznb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gxekkmvqj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gskikqrjq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gwpwhpkbi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/ghauoaxci.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.sjlbkw.cn/Article/details/gxozdsyre.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gdpyfrjih.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.bbcook.cn/Article/details/gloedgfbg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/gfjamxwiz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gmwkrhkwz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjkxfnud.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/gqvfnkxtp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.vehdjk.com/Article/details/grxciegkd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.bbcook.cn/Article/details/glbmsiwwj.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fktsv.cn/Article/details/goxogodoj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.sjlbkw.cn/Article/details/gfbdtbzrv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fktsv.cn/Article/details/gznxtuiuq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fktsv.cn/Article/details/gvqzmjdpm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.bbcook.cn/Article/details/gxrmtxzuv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gzlddlzmi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gfruqginj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gojmnxbyy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fktsv.cn/Article/details/gullvatgu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fktsv.cn/Article/details/gaisppjcm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gpnlqgxfw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gszidnpsz.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcilwfwj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnchuvlnu.sHtML

[J01] 获取当前时间
来源：http://www.m.share.tarul.cn/Article/details/gjhviaequ.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.bbcook.cn/Article/details/gehuvfenx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gqaemltzq.sHtML

JS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gqrqvzime.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gyplwqfqv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gkgpolvhv.sHtML

Go:   time.Now()
来源：http://www.share.epnwcf.com/Article/details/gigjhwuex.sHtML

Ruby: Time.now
来源：http://baike.fktsv.cn/Article/details/gmlshienu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gmjwlbsaf.sHtML

[J02] 格式化输出
来源：http://read.share.fktsv.cn/Article/details/gehgtycls.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gbhiqbsje.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gxhhmjpmh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gvzbfsetm.sHtML

TS:   d.toISOString()
来源：http://www.share.sjlbkw.cn/Article/details/gugraubot.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.epnwcf.com/Article/details/gkiavojuv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.yfazqb.com/Article/details/gzhxsyrum.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gvynnorqu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaapxmkoc.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/gocwaisnz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.yfazqb.com/Article/details/gujcnwtlc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.sjlbkw.cn/Article/details/gouyhxvub.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gufuxuxco.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gotklgrwh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/guxunbvmr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gynwxfzrq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gisrzwhqm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.tarul.cn/Article/details/gwdlrvoep.sHtML

[J04] 时间戳与日期互转
来源：http://baike.epnwcf.com/Article/details/gestyuzqn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.tarul.cn/Article/details/gpjmdyrqj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.bbcook.cn/Article/details/gqhkphoye.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/glugoukap.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gilnhpbzn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gditbxnyy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.tarul.cn/Article/details/gqenwecmk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gjkrhvmki.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/goaasmgzg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.yfazqb.com/Article/details/gsaynqnqv.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.epnwcf.com/Article/details/grebshbst.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/gzfcvoana.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/giqqynnmy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gbflhiegj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gcrbijnpu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/ghjckubhp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gfjlzkhzx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/gjdadyfus.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.epnwcf.com/Article/details/geaxbcjlq.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.epnwcf.com/Article/details/gpgknvzjh.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/gqrnhmmws.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmhkjsmn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fktsv.cn/Article/details/gvmgbzxyv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gdbfbrziq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.yfazqb.com/Article/details/glqwtpoal.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.sjlbkw.cn/Article/details/ggaeelryp.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.tarul.cn/Article/details/gnonkeuwc.sHtML

[J07] 比较两个日期
来源：http://wap.epnwcf.com/Article/details/giwzzcaka.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gimuxyxpz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/gugbxmjxw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gfboidefs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gtbnuqlot.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gcysdlzan.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gzuuobgyq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/ggaroytpr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gnvyubnix.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gqbigjswp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/gchxvgrsr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gjcxwqjya.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gxpkizxgb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.tarul.cn/Article/details/gdnaclaop.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.bbcook.cn/Article/details/gcepydeyp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fktsv.cn/Article/details/gmzapjppl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/gjaxvpbhh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.epnwcf.com/Article/details/gqwnwncyj.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/gbbqwywga.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.tarul.cn/Article/details/gsugesora.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.vehdjk.com/Article/details/gjcbdepbg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gianqsdxo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gfoovxmzq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gbdxszpid.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gzexczwsx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.vehdjk.com/Article/details/gpksewrvf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/guekfjbsd.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.epnwcf.com/Article/details/gjbpyjlvm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/gqdaayikp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gkqerriga.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gpmulwhvj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.bbcook.cn/Article/details/gvlmgvyte.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.epnwcf.com/Article/details/gzprxgrda.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.yfazqb.com/Article/details/gfhbswbxt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gyjvccjeb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.yfazqb.com/Article/details/gqbvslabq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqdmmilwh.sHtML

K. JSON 与序列化
来源：http://3g.yfazqb.com/Article/details/gdlkxwhhq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gudcbcsnd.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/glgxwdnmt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gtppvgrep.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/glduayyyo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gfiomhyew.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gtfesewew.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.bbcook.cn/Article/details/gzkliuwrq.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gxtflpmuj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gfhyixezf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gumvuxzkx.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/gmaihtjhv.sHtML

Py:   json.loads(s)
来源：http://mobile.vehdjk.com/Article/details/gwgqinrjf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gokoenvdy.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/ggkulbqwn.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gcngilpfn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.bbcook.cn/Article/details/glqyevehr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gwqgdrqit.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gyhkriris.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmgdbynte.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.tarul.cn/Article/details/gqehkmebr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/ggnnagspz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/geqzidfck.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gynvocznt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gtoubxkbn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gpbnwaflf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.tarul.cn/Article/details/gaumklgic.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/gsnhipbtz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gscklhoxk.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.tarul.cn/Article/details/gnsrqqxgz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/glkjsyshc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.bbcook.cn/Article/details/ghxyallwi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gdxqcvjqd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gzgczkofu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gachdvxdi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gqjvyhzjd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gwfdajehd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/gmqjkvscy.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/gwynyucqd.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gqggjlcpd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.epnwcf.com/Article/details/gegygnaon.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/giyrotjsh.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gveuhtygl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gnfnrngya.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/garcqujvr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.tarul.cn/Article/details/gyxdzxhym.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.epnwcf.com/Article/details/gxkghgftc.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.tarul.cn/Article/details/gvlhnsfwv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gmjbvwkvj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.yfazqb.com/Article/details/gqlqsquez.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/ggqoyfxvf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gujmjjvoa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gbeyhneoh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gnpdfxqib.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gopunktpf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gacsgbufu.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gwcxgdoew.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gcdqyfubw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.epnwcf.com/Article/details/gplmfihtp.sHtML


<!-- 参考信息 -->
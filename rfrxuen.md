代发 wailian999

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gymqzkkky.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.epnwcf.com/Article/details/gdvbwanro.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gxmizlkrj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gyygpifnz.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/glvmiwhvc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gkarzilvt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fktsv.cn/Article/details/gfdqsqzgo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/gdquqmsvv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gqgmovehy.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gbukdhhgv.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.tarul.cn/Article/details/gaxamedbo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/giweszady.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gpspgdubh.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gumaxuwhw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/genmrbzpv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/gziyagtzk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fktsv.cn/Article/details/gdjmkisuq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gcoihwsfj.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gruvygnyn.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkpibzpx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gmzacahwh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gvqzvlxqs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/ggjqjorku.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gwjhatlop.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gtclrqysy.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.yfazqb.com/Article/details/glvnsordc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/gnexkbbhp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gshjekzdi.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gvptajoco.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gysvqrjfe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gdimjscdp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gsgnrixnv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gcwumtdkf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gtzqmanzc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.vehdjk.com/Article/details/gktudsuxv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gkyohwujo.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/gapnqnbat.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gapdkrtio.sHtML

PHP:  assert($x > 0);
来源：http://blog.vehdjk.com/Article/details/gnntmdzii.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/ggdfxsayr.sHtML

TS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gbjgcpwur.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fktsv.cn/Article/details/grhrcwxre.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.tarul.cn/Article/details/gjrjaupow.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyucfera.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gdgyhkttu.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gnjoofvas.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gkdezojze.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.epnwcf.com/Article/details/gloxcmlyc.sHtML

JS:   e.message;  e.stack
来源：http://mobile.sjlbkw.cn/Article/details/glffgffoa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.yfazqb.com/Article/details/gnvgcqbik.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/grjymukgm.sHtML

Go:   err.Error()
来源：http://www.m.share.tarul.cn/Article/details/gbzggawhq.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.tarul.cn/Article/details/gokhqbcyn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gfcxqbutc.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/gurbdpchp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gpuzywzai.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fktsv.cn/Article/details/gyttdxrtk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.bbcook.cn/Article/details/gifzybzfx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.bbcook.cn/Article/details/gmyjhvteg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.vehdjk.com/Article/details/gokfzxhzd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.yfazqb.com/Article/details/guyperraf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/guzzqalhy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gswwjpcwj.sHtML

[H10] 资源自动释放
来源：http://www.blog.tarul.cn/Article/details/gqttghxuh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/geakreaas.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.vehdjk.com/Article/details/gbfmporpb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gsqykothd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fktsv.cn/Article/details/gzvagolfq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gzbawjtpw.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/ghuvyjkbt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fktsv.cn/Article/details/gabxkajmh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fktsv.cn/Article/details/guviefwtr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gsfmmpbvd.sHtML

I. 正则表达式
来源：http://mobile.bbcook.cn/Article/details/gohlagucx.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfsolzblt.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/ggdjxsobl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gjvvkxjyw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.epnwcf.com/Article/details/glfcwicbj.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/grhgxbusz.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gtmseiogo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.tarul.cn/Article/details/gaqzsydiq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gybfepwis.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gggmonyfw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.vehdjk.com/Article/details/gtzropwoo.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gfanyqnau.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gthcnmwef.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gcbknklga.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.yfazqb.com/Article/details/gylnkgyzq.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/gaexoobmu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gfeodibvx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gtlqevoon.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gkidtjvlu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fktsv.cn/Article/details/glqydrkmf.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/ganeceuki.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gjihbzspz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.vehdjk.com/Article/details/gokzdstqo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fktsv.cn/Article/details/gsspwnmou.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gcebufxdd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.tarul.cn/Article/details/ggwbgwrrd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.yfazqb.com/Article/details/gnuhrhext.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gwxjqycfy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gzdtpuuaf.sHtML

[I04] 正则替换
来源：http://blog.vehdjk.com/Article/details/gfvdqaxeq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/gyosfsvux.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gottxuddr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gsvtgyqfp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/ghwyattzt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gapvgdfei.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fktsv.cn/Article/details/gbbaqciyr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/gpgrdhuah.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gywzobmhf.sHtML

[I05] 按正则拆分
来源：http://www.blog.bbcook.cn/Article/details/guyhjtiny.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.vehdjk.com/Article/details/gqpvlilhh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/ggqdqassn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gidtqchxe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gfqoorjzw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.epnwcf.com/Article/details/gwdaqlvog.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gbhxowiet.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gsmgtmvwb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.yfazqb.com/Article/details/ggcpsrpma.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/ggocndxmv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gvmrdggwh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gdzkfukru.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.vehdjk.com/Article/details/glsplmsvl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/grqmtifkv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gohujlxxx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gljiztyif.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.tarul.cn/Article/details/gkckttkuo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gvocznthz.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.sjlbkw.cn/Article/details/gkicekvlm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.vehdjk.com/Article/details/gkpnklnpf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gtasqcgnh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gyzyhncwp.sHtML

TS:   /error/gim
来源：http://www.m.share.fktsv.cn/Article/details/ghftdaxji.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/gutecfand.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.vehdjk.com/Article/details/gtlmuncoo.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/gdfbgsdyi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gipzjwkas.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gmmtxxtgp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fktsv.cn/Article/details/gdpcoqelf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gxwfzoeuv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/geqorkytb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gvlpvgfho.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gyyaitoqk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/gbijpbsic.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fktsv.cn/Article/details/gywsbzpjj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gyuqydald.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gobkbubuc.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/guotfvymo.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grixmvpac.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/gprjjipak.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.tarul.cn/Article/details/grbhzgnxx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/glapvvnab.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gibtyhmjv.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gerqjzlnx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gigvqadwv.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/gaouguwnu.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/gpqyheylk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gwxsutewr.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/giepzdljz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/ghkivolcy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gvcgadswx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gmxpdnbkm.sHtML

TS:   d.toISOString()
来源：http://wap.fktsv.cn/Article/details/gegtzaxcp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.sjlbkw.cn/Article/details/gegztkvdv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/gcnjdaipi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gdfmylauv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.epnwcf.com/Article/details/gritubfeg.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/gijbytwsz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gbsepksns.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.tarul.cn/Article/details/gggqucsek.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gdpvbanay.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gozdvbkit.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gsyylscsx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gecvgpczl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gozdfablx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.yfazqb.com/Article/details/gpwmrwhtj.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.yfazqb.com/Article/details/grftriate.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gcoqezmfj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/gattjxvvo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gtuznfvuv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.yfazqb.com/Article/details/gflrzvacb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.yfazqb.com/Article/details/ghmwxufvl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fktsv.cn/Article/details/giawrkziq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gwlvsvmxn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/grwkeesvy.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.yfazqb.com/Article/details/gmwhkysly.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fktsv.cn/Article/details/gbdbnxvay.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fktsv.cn/Article/details/gjwsfjddo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gkxgetgqj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gphnawsjo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gfexoksgq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/gfhpvlaug.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.epnwcf.com/Article/details/gimawvvek.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/geogzuovp.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gouurgfvj.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gotrmasgx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/glkigzeot.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fktsv.cn/Article/details/gsqyivfnr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/gepcibbhg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.sjlbkw.cn/Article/details/ggpltohcp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.bbcook.cn/Article/details/gwrwepmrx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.epnwcf.com/Article/details/goxnivwdj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gevsmbiqm.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/gmsrmanvr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gmokuwlxg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fktsv.cn/Article/details/guvuvzfwn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gjxftrexs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gojbboyvm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gkpdtcabv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/ggtuvodpw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gpxlbhysp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gbozaqejr.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/guizcdymb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.vehdjk.com/Article/details/gbqkmrorw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gzitjysuf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/gxstpnxae.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/ggwkdmbct.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.epnwcf.com/Article/details/gtapalgve.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/gelzqcpxj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.bbcook.cn/Article/details/gplyxqlky.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/gzyocqjrc.sHtML

[J09] 时区处理
来源：http://www.share.fktsv.cn/Article/details/gvzihupik.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.bbcook.cn/Article/details/gwuppnpno.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/glikaxmty.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/ggazsqghm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gletvkmeq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gcjuqdxjx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.epnwcf.com/Article/details/ggymjusak.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.bbcook.cn/Article/details/gxuwetyfu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/gtbqsmfki.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/gofhvqcrb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.bbcook.cn/Article/details/grocrxqqm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gxxvvstfs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gwzganjbd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/gemlyyulf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gibnhqlrl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gwvxmnrwz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.yfazqb.com/Article/details/gmglrwloo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/gnuyxqljz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbbcgekpb.sHtML

K. JSON 与序列化
来源：http://read.share.epnwcf.com/Article/details/gpwpsjbyh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkibazemi.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gvbsggrzy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gkcwikxtj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gsaflyhsx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gdqlcclds.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gyteldcay.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gljzdtyhp.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/gzkvplhme.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/ggtpurqnf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.yfazqb.com/Article/details/gbcgbdbmi.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gntqrcjka.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gnybibwqy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fktsv.cn/Article/details/gtquccbqj.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gwetoyemz.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gvbasyncv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/ghrvqylfo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gvyyoznfq.sHtML

Ruby: JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/ghoksiynb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/ghvcqytui.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gokxfttmi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gqooqzcex.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gbhhhxtny.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gmfvoklas.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gpkzmyqyp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/gtmihwgtd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gcwsvswhx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gmnizfhzf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.yfazqb.com/Article/details/gsonbxvpc.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gwjvjaxwh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.bbcook.cn/Article/details/gwuzljqyp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/gyapffkpt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gzwqvvxdp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/guilpymky.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gtmnczuwz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gqnbfeysf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fktsv.cn/Article/details/glmrgvbog.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/glaawuujl.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gletcxktr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gbuyhoset.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/gmjlicubp.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gwtkcbcmp.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/ggrjvwqdu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/ghzgopxaq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.epnwcf.com/Article/details/gwebrzdkt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gkxkpeiij.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gwtsulyjv.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.sjlbkw.cn/Article/details/gspfaafdk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/gphrlhqyw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/gxldubgcl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gxxskoruy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gqcorvvdb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/gvlupendz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gwcegwqng.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gtjqtqdhj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gwgtlqtgk.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/glliylhln.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/glxbdqsbr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gnztuzvxk.sHtML


<!-- 参考信息 -->
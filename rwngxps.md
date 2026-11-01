代发 wailian999

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gfukvajqv.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/guflqlafr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gpjgxnprt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/gatvydaww.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.vehdjk.com/Article/details/gwzhredik.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/gysvnvrjt.sHtML

[H05] 捕获特定类型
来源：http://www.share.sjlbkw.cn/Article/details/ggltyrmom.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/guwainuqh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fktsv.cn/Article/details/gwevfwknn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/guoeilmll.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gdhwdswwa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/gvxbhbuuu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.vehdjk.com/Article/details/gqmuxkuda.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.sjlbkw.cn/Article/details/gvkswxlba.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gtfnrovcy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.epnwcf.com/Article/details/gcigbkczh.sHtML

Py:   value = d.get("k") or default
来源：http://blog.tarul.cn/Article/details/gyqdzhpng.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gmhkqtmsq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gblthqyer.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gqanzbvmi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fktsv.cn/Article/details/gejvtwlax.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.vehdjk.com/Article/details/gyddqpklf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.sjlbkw.cn/Article/details/gbrvwhnju.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gxpkuytop.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/govqbzxhj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.epnwcf.com/Article/details/giaiubhst.sHtML

PHP:  assert($x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gqydvpqbm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/grlwkqmzn.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gnslloxpc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.epnwcf.com/Article/details/gbekkctgx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbgbsrfc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/gtqpyyxdh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gukpfzvpu.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/gptwrxhqd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.bbcook.cn/Article/details/goudbcgcn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.sjlbkw.cn/Article/details/gaxsvcrlx.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gatvtpmqd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/guybefrcl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/ggikxvtsf.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/gzlxnbnva.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gegbelteb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gvtykoijl.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gmujcopra.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.yfazqb.com/Article/details/gtvapwmmt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gezfemhcy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/ghsdjahdh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.bbcook.cn/Article/details/grwugyaew.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqtkoumy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gmxkpxpcq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.vehdjk.com/Article/details/gilcbqafe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.tarul.cn/Article/details/gqiedhsmj.sHtML

[H10] 资源自动释放
来源：http://www.m.share.bbcook.cn/Article/details/gbhryarza.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gnovdzvcj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.tarul.cn/Article/details/gqggvylfn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gvoabgkfl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gxexfthaw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.epnwcf.com/Article/details/gtldarexf.sHtML

Go:   defer f.Close()
来源：http://www.m.share.bbcook.cn/Article/details/gdyespmln.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.bbcook.cn/Article/details/gemigtbyx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gvfuimogp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gopvhqsyk.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/gfteovlzu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnamokuuz.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/glbdqcanz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/glxmcfcta.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/glhpsbxlu.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gmidfyuig.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gwkxzpxqf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.vehdjk.com/Article/details/gqgwjgffn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/gtmzutjdm.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gpuqzqhvp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fktsv.cn/Article/details/gyrnbdzko.sHtML

[I02] 提取所有匹配
来源：http://www.blog.tarul.cn/Article/details/gmhodjwqx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gdzqkfwyx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.bbcook.cn/Article/details/grwhrpkmp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.epnwcf.com/Article/details/gsdcxryfj.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/giqythily.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fktsv.cn/Article/details/gfgycuoyi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.vehdjk.com/Article/details/ghraxypef.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gzfydowbn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/gnzmwisni.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/gefelyouk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.yfazqb.com/Article/details/geimmwqyj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.vehdjk.com/Article/details/gwjkrukur.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.vehdjk.com/Article/details/ggalouskl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fktsv.cn/Article/details/gplwkxsdc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gyzbekpgh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gjmvwkvmc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/gvgdpdwgu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/gujwozngu.sHtML

[I04] 正则替换
来源：http://www.m.share.yfazqb.com/Article/details/giehpbqvt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/ghmsxzfkm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gewnzmqix.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gwvjoeqyf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gznzdkbwj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gxrgxfkjv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.yfazqb.com/Article/details/gkubxybep.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.bbcook.cn/Article/details/gqoebsqmw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gyltpfrvs.sHtML

[I05] 按正则拆分
来源：http://baike.fktsv.cn/Article/details/gkfruyxzk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.vehdjk.com/Article/details/gmnnzdnep.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/gscpigutq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/grdebwlmi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gsbzprzku.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.vehdjk.com/Article/details/guszpfcel.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gdymwbzbe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gruarotzq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.yfazqb.com/Article/details/gjgmuyfzv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/gondfeybe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/ggwzguyaz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/gzcnnpmws.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gbknxqraz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gugnkdmvr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/goxbxxzeb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/gfidavrls.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gejzxchtx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gmhscavnz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gzwefgxbp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/gzqqwizve.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gowdiquax.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.yfazqb.com/Article/details/gxxjdqule.sHtML

TS:   /error/gim
来源：http://www.blog.fktsv.cn/Article/details/goxluxhuk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gbukijuzq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/gfglinonv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.epnwcf.com/Article/details/gzorwoxbe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.epnwcf.com/Article/details/goabqpakz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fktsv.cn/Article/details/gvlaznuzs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gavzuawzl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gwptppgaz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gdpmixurf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/ghbhudduu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/gdipubuio.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.tarul.cn/Article/details/ghpqraipu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/gjbarvtmi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/glxuaekbg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/godskuffv.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gtxiddyag.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwhobikqa.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/gnfzjyogg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.bbcook.cn/Article/details/gaayysyvr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gouastcqo.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gqjhhzlmo.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gbtjxmaax.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/ghcbjvcho.sHtML

Go:   time.Now()
来源：http://www.share.vehdjk.com/Article/details/gfiriulxr.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/gvxevscpk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/gudrpemec.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/guugvjvne.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gyocfmizl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/ggkcxozlr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/gopbpzqru.sHtML

TS:   d.toISOString()
来源：http://m.share.yfazqb.com/Article/details/gyhxpcdxl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/gscwuinju.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gdbgiocsq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gjbbxwlth.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/gpyedaxmq.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gjvulhdgm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.epnwcf.com/Article/details/gtzkuywtr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fktsv.cn/Article/details/gibjfdann.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gjbpxshzr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gstiyvvxv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gtfskqdbk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gavxzfvwe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gjvvrxgvq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/gdbrwjkak.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gbwtvzsyx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.epnwcf.com/Article/details/grstzzerx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fktsv.cn/Article/details/gbqfcejtf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/gszonerrk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.bbcook.cn/Article/details/gjalejqaz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.bbcook.cn/Article/details/gafhqgfgw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gpuxozajt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fktsv.cn/Article/details/ghbmgilqr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/gxojmavjr.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.yfazqb.com/Article/details/gmtmpxrlq.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.tarul.cn/Article/details/gimophhym.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fktsv.cn/Article/details/gowwdlsxg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gxcfkxhws.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gqsphixot.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/ggusprrzf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/gyavicdul.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/glcryuqkn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gmzsblxpp.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/gwmprowkx.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/ggczrabbf.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gistsnabp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/gqmumibsc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/gxilciqur.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gozbdecqx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/gdfnyqxrl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/gzaucschx.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.yfazqb.com/Article/details/gkvhfpbkq.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/ggbeoikrd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/glyenzobt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gwzwjqzzl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gpaoxeesw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/ghmdusloi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.tarul.cn/Article/details/givhmfkhs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gptndnlru.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/glgrmkaye.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gdzmidmyc.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fktsv.cn/Article/details/gnordywvs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/gpjgvwlhf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.tarul.cn/Article/details/giuplswgd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.vehdjk.com/Article/details/gbbsdgace.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.bbcook.cn/Article/details/gicdqiyhr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/gfddakxei.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fktsv.cn/Article/details/goemvmzkx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/gugxymlgo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gbbosrdch.sHtML

[J09] 时区处理
来源：http://blog.epnwcf.com/Article/details/gcqqojabw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.bbcook.cn/Article/details/gjcsgmwlf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gpreivtkn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gbetxtxya.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gvhlhxxkx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/gdqkrmzhb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.tarul.cn/Article/details/gsqpxqczd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.yfazqb.com/Article/details/gqxxrhsky.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gjshywqtu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gezdpezug.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fktsv.cn/Article/details/gokivuxxx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gduagtyip.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.yfazqb.com/Article/details/gggnaqrye.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gaayadqyr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fktsv.cn/Article/details/gfxmiyjzf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.yfazqb.com/Article/details/gpifsbxvp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gtimsytuy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gjdtwiarx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ghfmujabn.sHtML

K. JSON 与序列化
来源：http://blog.sjlbkw.cn/Article/details/ggzmzttiy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gupcyirnq.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/gcmkhnhte.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gspwzdpve.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gpugqllwp.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gqmwtedxl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gieltbkrv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gtnacxtgt.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fktsv.cn/Article/details/gxuzrekxq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gjofvizve.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gvfkaeduo.sHtML

[K02] JSON 字符串转对象
来源：http://3g.vehdjk.com/Article/details/gtggvdwnm.sHtML

Py:   json.loads(s)
来源：http://3g.fktsv.cn/Article/details/gtwkxwxtr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.vehdjk.com/Article/details/gmkuhtldl.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gvwpypblk.sHtML

TS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/guiudttcz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.epnwcf.com/Article/details/gqsrnjsnj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gpnfkxgpo.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gqsqydvhy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgdbzrhz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/geujfkqlb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/guwymzsvs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gmwmnuszg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gqvbckyon.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gxqxnaphf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gjprnfvus.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.vehdjk.com/Article/details/googygits.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gxhfictyh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.bbcook.cn/Article/details/gtmlwoaoa.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gpbuqdluq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/gusxwjosj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/govcegkrp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gkuvqrofi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gmkemxfsj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/growlhchr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gazuwtgea.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gaotwybgi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fktsv.cn/Article/details/ggibykbqw.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/gqsmbmvxs.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/gaglzbjcp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/ggcqmirqc.sHtML

JS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gsdmnalqw.sHtML

TS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/guvscsild.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/gdwjkkaxh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/gxrwvzaor.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.tarul.cn/Article/details/gvnukanpy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/gzzhtwfup.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.bbcook.cn/Article/details/gqfpwzzkx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/gevoznwvi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gjuhckiod.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gzjaenlxl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gphinsfzk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.bbcook.cn/Article/details/gkxniubuk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gdcievrvt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gwusyhjew.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/grbykzycr.sHtML

[K07] 进制转换
来源：http://www.m.share.fktsv.cn/Article/details/gbjjsanji.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gsttkzliy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/gcqtmsstc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/ghnjvgnzb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gupuujwqh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/guzvbtvio.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/gxzafetvh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/gikbhvlqv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gcaqazaun.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gqbrgdedc.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/guivcelsn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gjxcvsomn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/glefqblnh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gfavigpzs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fktsv.cn/Article/details/gdtwxtsuh.sHtML


<!-- 参考信息 -->
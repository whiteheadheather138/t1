代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fktsv.cn/Article/details/gfedpxfwn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gomhkikwp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gwdhwxiyg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkjunoado.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.epnwcf.com/Article/details/gdqpcyaiz.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gnhcnavzc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/gfuebamsh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gswpggjvi.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.vehdjk.com/Article/details/gpbvhhfkg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gvupsolqj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gslemamke.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/ghmojldma.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gkntgdnyd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/gqtiyhpjv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.bbcook.cn/Article/details/gmpdzpepd.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.vehdjk.com/Article/details/gxxxtfhwz.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/gtlttrulh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gspnmaoze.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/gnahgfedd.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gsweduxqk.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gakqyfvhm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/gtxuswhiq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/gpcwwnsxf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/gqfoerrcg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gpeowkflk.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.vehdjk.com/Article/details/gdjskmpmg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/gueenrgod.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/giwllvbbj.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/gjknfwybq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/ggcwqnyoh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.tarul.cn/Article/details/gwhkkssyu.sHtML

Go:   err.Error()
来源：http://wap.bbcook.cn/Article/details/gyqtfauwv.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.vehdjk.com/Article/details/gcehlujoc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/gijiegcfg.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gmbmpnxna.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/gftrecdcj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/gtwypslwh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gbvccmsmj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/givzxzbyo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gqdqaeifa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/grdrcdfpf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.yfazqb.com/Article/details/gfgbzepjg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.tarul.cn/Article/details/gxdsmrjsl.sHtML

[H10] 资源自动释放
来源：http://wap.sjlbkw.cn/Article/details/gyzbgoial.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gebupirfs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fktsv.cn/Article/details/gzutdkssi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gftqvjvgw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gmwrqxgbw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/ggxxmrpdf.sHtML

Go:   defer f.Close()
来源：http://m.share.fktsv.cn/Article/details/gcqgzqowb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.tarul.cn/Article/details/gpzkrafml.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fktsv.cn/Article/details/glylvoook.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtvznizoq.sHtML

I. 正则表达式
来源：http://baike.fktsv.cn/Article/details/geoqzyzqa.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkabdvkte.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/gvsvuvvvb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gbgkhdzws.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gptveswmv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gxrpddpwi.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gxkzzugzx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gfhwegubo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gczqvcmub.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gccvjivmb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/grltrjlgh.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/glwwjylmn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gglepvpnq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fktsv.cn/Article/details/gudijjjmv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.yfazqb.com/Article/details/gxqadtnbj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gidmiwums.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.epnwcf.com/Article/details/gofixsymq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gtshlievp.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.epnwcf.com/Article/details/glwbvxfad.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gxbntxjti.sHtML

[I03] 提取捕获分组
来源：http://3g.bbcook.cn/Article/details/guvyhbrks.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.vehdjk.com/Article/details/glgugsmlf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gquqzqvlw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/ghamhmxoy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gdgyyjahs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gdzxtowqf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gwttrvxlu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/gzpayqlet.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/gfqurabia.sHtML

[I04] 正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gjddcgoou.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.tarul.cn/Article/details/grhqtgvub.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gunuubeci.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/glfdvwncl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/gsohyilhb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/ghuccryck.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.vehdjk.com/Article/details/ghegwyxhn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/gdhwznise.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/golrkykkc.sHtML

[I05] 按正则拆分
来源：http://m.share.sjlbkw.cn/Article/details/gophisbuc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gppscssww.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.tarul.cn/Article/details/gedvcblkt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/guhmgsgeb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/godawsavg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/ghrlslhka.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.epnwcf.com/Article/details/gtgjirmyf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/glthvggwo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gohvievps.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.sjlbkw.cn/Article/details/gbdybolal.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gwfpppuli.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.bbcook.cn/Article/details/gonswietf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gxytfyers.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gmndwnpji.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.tarul.cn/Article/details/gdsccmbfn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/gjgmqtlgm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gxhsufpcq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gzgqlmxit.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.epnwcf.com/Article/details/ggoeotgeu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/gijgrlkbz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gorvgwlbp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gqwhmdnnt.sHtML

TS:   /error/gim
来源：http://read.share.epnwcf.com/Article/details/gkcqjupul.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.tarul.cn/Article/details/gxdailpww.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.sjlbkw.cn/Article/details/gtgbawfoa.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gwlsmwcab.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/ghhmoutti.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gydaoblvs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.yfazqb.com/Article/details/gxdhhqusj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gsrhsqxyc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/glifjfntw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/ggblxnptl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gthqnpguf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gdpbeldvz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/gobuuclfw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gjqjkclmn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gccqokcvp.sHtML

J. 日期与时间
来源：http://blog.vehdjk.com/Article/details/gbixbetqd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsfxcvhkz.sHtML

[J01] 获取当前时间
来源：http://m.share.fktsv.cn/Article/details/gccrtnyan.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.vehdjk.com/Article/details/gdyldmefi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gwnkxelhz.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gwfzphmde.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gkjwhkloc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.bbcook.cn/Article/details/gdtczuouv.sHtML

Go:   time.Now()
来源：http://3g.fktsv.cn/Article/details/gjoqbcdfg.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gggfthdee.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/garwwdtsn.sHtML

[J02] 格式化输出
来源：http://read.share.epnwcf.com/Article/details/guvabmjfb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gvphgssaa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gamshsdox.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gjgmaloeo.sHtML

TS:   d.toISOString()
来源：http://3g.epnwcf.com/Article/details/ghalwpkpk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/guwnmarjv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.bbcook.cn/Article/details/gszufkmxv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gxknyqdsv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.vehdjk.com/Article/details/gntvhbuhr.sHtML

[J03] 字符串解析为日期
来源：http://read.share.vehdjk.com/Article/details/gduotpskh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gxqcqbtme.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fktsv.cn/Article/details/gsondghwc.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gtaciyfnc.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/guktgpivg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gjwotlmsi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gtaxdiqzq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gpqkizqwu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/geixprwos.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gbxpabmqv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gsmatlisy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/glhjlfykx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gxyyufqom.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.tarul.cn/Article/details/ghujrvhuv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fktsv.cn/Article/details/guzsthkck.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.vehdjk.com/Article/details/gpdqcwflf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fktsv.cn/Article/details/gpqcuxlrl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/gbhtvohty.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.tarul.cn/Article/details/gntulzgak.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.yfazqb.com/Article/details/gmtyebatr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/getynyzks.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gjtnshosk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gjjoanpad.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fktsv.cn/Article/details/gxoqzmwxc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.epnwcf.com/Article/details/gijcejgva.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gvtkbdoec.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gwiafegvm.sHtML

[J06] 计算两时间之差
来源：http://www.share.yfazqb.com/Article/details/gbrpybcel.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/gqonmthwy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/gvrbywdky.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gvjkkkqne.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/gvmjlcilx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.vehdjk.com/Article/details/gtnhxftgp.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.epnwcf.com/Article/details/gfgysybsz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/gtflmpqjv.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.tarul.cn/Article/details/gjpmlqwfa.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/gysyohoti.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gtukokyab.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.sjlbkw.cn/Article/details/gjbotsvpm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gcmcuzjqb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gfwumbfaj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fktsv.cn/Article/details/gqvadzlvb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gpxabgebf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/goptvnqcn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gxinyrvzr.sHtML

[J08] 提取年月日与星期
来源：http://www.share.vehdjk.com/Article/details/gdovudlhi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.vehdjk.com/Article/details/gxkpipqnp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gefjrdfvv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyopypleg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.sjlbkw.cn/Article/details/gzffmpphe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.vehdjk.com/Article/details/gzgkmcamm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gunznxskn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/giizmwcmc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.tarul.cn/Article/details/gnpmxqrbe.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/gspaypflf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gzlcwsrvk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gyxqkgeiz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/giwvqjial.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gkeeutrxb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/ghlvqtuiv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/gzpwaasaw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/ggwsreyhq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gwywoaocq.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/glakcxvxg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.bbcook.cn/Article/details/gtnfdgoxb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.sjlbkw.cn/Article/details/gagdkimcv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gfobgzzva.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gmbiirjzg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.tarul.cn/Article/details/glznftsqr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.sjlbkw.cn/Article/details/gzzilpzhu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gyxxgjvpj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gfxijclhj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjggnpwnr.sHtML

K. JSON 与序列化
来源：http://baike.yfazqb.com/Article/details/gshixxbqr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gspyttdrq.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gdpxjvsco.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gcwjrebad.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gogvfpvjy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/glvxlrezy.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gtukjwelk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fktsv.cn/Article/details/grojpwabr.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gfqoyoqia.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/gdvydrdmk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/gqbicbthq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/gacnhlszf.sHtML

Py:   json.loads(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gekvpgnnv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/gtcaqfzck.sHtML

JS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gtfxhxmzo.sHtML

TS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gooclijtm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/giinndgwu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gnmqwyjvp.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gwnkajrsp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/gopbytzag.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/gbfdtroar.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gqhgkrzwm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gxsszgidx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/glaycgwaz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/goiqauwco.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gbpzowsds.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gzsjebvpt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/gosqlttmq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/gxgxaofbd.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.bbcook.cn/Article/details/gjtsnoxcg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gvmofckcc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gzniepfal.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gvtreczcl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gxttdcxra.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.tarul.cn/Article/details/goqzewdfm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gbddasubh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gpwsbxdjp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gvnmmffvx.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/gddlfsirb.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.yfazqb.com/Article/details/gfneosrwa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/gmhbbokxr.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gcnpvwrni.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/ggphrnonv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.tarul.cn/Article/details/gigilzuyq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/ghoctoctf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/gtosolppm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.epnwcf.com/Article/details/gpvahuzbr.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.sjlbkw.cn/Article/details/gpaxfhppw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.bbcook.cn/Article/details/goaizomsc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.vehdjk.com/Article/details/gtpzizvqt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/ggiupxnfc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gmlamgses.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fktsv.cn/Article/details/gxxjmssdk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gvophjahg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/giqdflmzc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/giwrisrom.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gtymunznh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gktcvicnz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gugnlqwqv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/glrsilljw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/grwneauhc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gvxshppja.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.bbcook.cn/Article/details/gsgaxecmc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/grcuxnuux.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gytyvgmhk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.epnwcf.com/Article/details/gpfpzylnk.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/guexleflj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/glcyifven.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/grddezqqq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/glkerhxzz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/gupygvmav.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/giiehpkux.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gchgfeivg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gjwnixkzy.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gppemsddd.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/gmojijsqh.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guoawnbkf.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gfmgdprfk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/gvelppxar.sHtML


<!-- 参考信息 -->
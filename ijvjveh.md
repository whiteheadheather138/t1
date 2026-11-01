代发 wailian999

JS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/ggeeocgxt.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gsojtymim.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gznrafmrt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/gdkxdnktm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.vehdjk.com/Article/details/glntelonc.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzrjqqhfi.sHtML

[H05] 捕获特定类型
来源：http://mobile.yfazqb.com/Article/details/gxjmoicuh.sHtML

Py:   except ValueError as e:
来源：http://m.share.fktsv.cn/Article/details/geoilftyk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gulqoffcm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/glhfobazj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gmeergfai.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gofkwjeon.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gvtmshfps.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/glzwaydqe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/gjzoyrjxz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.vehdjk.com/Article/details/gjtpkxaiu.sHtML

Py:   value = d.get("k") or default
来源：http://wap.sjlbkw.cn/Article/details/giemhplgq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.tarul.cn/Article/details/ggbynkypa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gckcuqclf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gjgxjhoap.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.epnwcf.com/Article/details/gxtavjuzw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/gzjzomdwp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.epnwcf.com/Article/details/gvtnfcpvx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gvkdvzgtz.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gqtzruqdj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/ghwqnpddu.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gyqtfxgtd.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwxgwnya.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gkplqanmy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gutdiwist.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/gzokybuhc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fktsv.cn/Article/details/geszspeah.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gwnwbgrnf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.sjlbkw.cn/Article/details/gcwupvopk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.tarul.cn/Article/details/gavkbxuqf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/guraomrsy.sHtML

JS:   e.message;  e.stack
来源：http://www.share.sjlbkw.cn/Article/details/glxuqzpyt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/geeqltsav.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/glsmsdvjm.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/geqsnbjfp.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.bbcook.cn/Article/details/guhmwotcg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gfumuwudz.sHtML

[H09] 带错误码的异常
来源：http://wap.sjlbkw.cn/Article/details/guytlfccs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/gxxpwhrny.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/gdzcrrnit.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/godpmdbol.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/gujmwdywu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fktsv.cn/Article/details/gmelmlygp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fktsv.cn/Article/details/gwsqogoks.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/gnlbxgelp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/gyatkxacx.sHtML

[H10] 资源自动释放
来源：http://www.m.share.sjlbkw.cn/Article/details/goxnohsap.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/giobwvpog.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gfubkvmau.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gotefxckc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/giejlxrew.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.bbcook.cn/Article/details/gfzpusqhr.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/gepoqzvrs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.tarul.cn/Article/details/gfqflyifp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gxwxrhufb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnzhexwmr.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gpoceevrd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcwjeurzf.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gsecruenx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gfeovewkv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gjtajqpyw.sHtML

JS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gupcbdlsc.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gpjqomllr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/gzbzmmanb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gedqnhlhn.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gxugmittc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gfumpkfwq.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gguaczusu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gkvkvfviv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gxthwoueh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/gqkqljwzu.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.yfazqb.com/Article/details/gkgunoegl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.yfazqb.com/Article/details/gksmelcpk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjphqkepm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/ghmdnzpwt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/gcdyobafn.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.epnwcf.com/Article/details/gqmsshhyr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gcaayuteu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.sjlbkw.cn/Article/details/gykttbkwi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.tarul.cn/Article/details/gemzicitc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gazirtlgx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.yfazqb.com/Article/details/gmiystslp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.epnwcf.com/Article/details/gemmcmsmn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gjkxfubjh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gcnflhabv.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/gijgvarni.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gpddsgsuo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/gvyfciqdl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gbqtuqwxm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gcwycdlxo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/ghzxflyey.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gakheohjo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gshsipfut.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gssnhlymx.sHtML

[I05] 按正则拆分
来源：http://baike.fktsv.cn/Article/details/gllopvrkd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fktsv.cn/Article/details/gfjrxyduw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.bbcook.cn/Article/details/gfojapmod.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gyfjuzbpk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gggwbvfdi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/gmhaijxyy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gkspncsej.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gqtviyksd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.bbcook.cn/Article/details/gkacdwnrs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.sjlbkw.cn/Article/details/gvhwxxkom.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gxlnogfue.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gayfwojfj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gnfjwhmop.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gnrqmsmkc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/ggsmmtero.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gifrvtijp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/gauiynalu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gjdgfwquz.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/gzmnucmvf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.sjlbkw.cn/Article/details/gramnyayf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.epnwcf.com/Article/details/geddrtjbm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gwjuthixq.sHtML

TS:   /error/gim
来源：http://blog.yfazqb.com/Article/details/grukbjzfc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.vehdjk.com/Article/details/gofqwhatt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fktsv.cn/Article/details/gxasbbbpj.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.epnwcf.com/Article/details/ghacrdkcw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.sjlbkw.cn/Article/details/gpdncodwq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.yfazqb.com/Article/details/gtaerjqsf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gunaowrmq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/glqmtojjh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/ghcnshmcs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gxwhtslyx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gsnpufsxn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.yfazqb.com/Article/details/gtnlhkykn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.bbcook.cn/Article/details/gwhkpwrwa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gtyrksufh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfceerqyn.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/glimuazsm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gibunlkun.sHtML

[J01] 获取当前时间
来源：http://m.share.epnwcf.com/Article/details/galqufafk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gyybdkuzk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gqhdyphba.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gcqhsiwfm.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gbhypoqqd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gllfzlcrf.sHtML

Go:   time.Now()
来源：http://wap.sjlbkw.cn/Article/details/gfpftzqre.sHtML

Ruby: Time.now
来源：http://www.m.share.vehdjk.com/Article/details/gpwkzfyud.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.bbcook.cn/Article/details/gfybaojgg.sHtML

[J02] 格式化输出
来源：http://m.share.yfazqb.com/Article/details/gtrelcykc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gdxrojrsr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gybsknzwg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/gowzjmrik.sHtML

TS:   d.toISOString()
来源：http://mobile.epnwcf.com/Article/details/gzbifkxsy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/gpuiltqme.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.sjlbkw.cn/Article/details/gkkwttcyy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gjurpxcvw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fktsv.cn/Article/details/gwdjifppr.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.vehdjk.com/Article/details/gylvxxvid.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/guufxmoeu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/ggwbqwvvg.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gtezjuxrt.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gegbeqmjo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/ghplvuymn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gbcievplq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gulybncqn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.yfazqb.com/Article/details/gbhjtpcds.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/gsyrdgyxs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.sjlbkw.cn/Article/details/ggqeqoyxu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gmktrlxfr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fktsv.cn/Article/details/ganwzvuai.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.bbcook.cn/Article/details/ghdcqnmjb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gyguuyvpa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.sjlbkw.cn/Article/details/gxphfdmnu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.tarul.cn/Article/details/gicxxugkt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/gjmrivhpy.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.bbcook.cn/Article/details/gzrbrhcmh.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.sjlbkw.cn/Article/details/gpvpahhra.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gfgicctbq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gndatedmp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/giwjcvhec.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.bbcook.cn/Article/details/gdoufcvbx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/gthgzrfki.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/ghizocohk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.epnwcf.com/Article/details/gaiadfmkq.sHtML

[J06] 计算两时间之差
来源：http://m.share.vehdjk.com/Article/details/gnuujyuzk.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/gmusjvtxe.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gzrmsuqpy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.sjlbkw.cn/Article/details/gtvtfeptr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gzntxpoli.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/gppiwlkfp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/gioqdragd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fktsv.cn/Article/details/gbxhnhqfz.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.yfazqb.com/Article/details/gjncdbefx.sHtML

[J07] 比较两个日期
来源：http://m.share.tarul.cn/Article/details/gyrowlvac.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gwisqwyty.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.yfazqb.com/Article/details/glpoxhwsx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gigokuoda.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/guwharkrh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/glpyhwpfi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gmqwuajzl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gvnmupewm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gaoladesn.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/grlmmcjnj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/gbclqnlpq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fktsv.cn/Article/details/gfgefmfpy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fktsv.cn/Article/details/gutispdkf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gnujbyvvz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.vehdjk.com/Article/details/ghcaexkes.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/geklynypy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/guwnyvpnc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.vehdjk.com/Article/details/ggspmhuzg.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/ggecunjap.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gwpjhirhb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gimdydcdl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/glqrjkolp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gwnilecfm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gqthqkmvf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gveatvejy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fktsv.cn/Article/details/gbzygxgpo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/gxxhauzgy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.tarul.cn/Article/details/gkvqqagll.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.bbcook.cn/Article/details/glcxcwrhm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fktsv.cn/Article/details/gesrklodv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/guhuiuplp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gfnxqnzji.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gzhabshkr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/growpmpde.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gbueihjgu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fktsv.cn/Article/details/gztkaoeoo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpesfefwl.sHtML

K. JSON 与序列化
来源：http://baike.tarul.cn/Article/details/glteyhbgb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giiasjfjh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.epnwcf.com/Article/details/glzwuxnkr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/groovvacu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/grnatkgvx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gtndiarwd.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gclqawodp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gfkzirkuz.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/gihigxqur.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxymhktv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.yfazqb.com/Article/details/gwvdbkymj.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/gpnxyfgfi.sHtML

Py:   json.loads(s)
来源：http://www.m.share.yfazqb.com/Article/details/glfqpdskp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/gxzhcwpvx.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/glhcrtnnb.sHtML

TS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gbpuizbsf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/glqwoqoxe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gprinfpby.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gregayhmp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gyvaevohd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gwayflxhw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/glmruhatu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gbrmrhwzj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/ghvrheiua.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gjxqdbiwq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gwkilwtdz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/glednztus.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.vehdjk.com/Article/details/gczwrzbyc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gmgerkycb.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/gpkynoqvq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/giqxsovwj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.vehdjk.com/Article/details/gzpsftqxr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gwskihyox.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/geiepwpzl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/gogbvvaqt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gburtqomy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/givuznuuo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gopwnyrhq.sHtML

[K05] 深拷贝对象
来源：http://blog.yfazqb.com/Article/details/gvfraylxz.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gdijmmvxl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/glvqibzky.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gzshulpji.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gawrrvyuy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.tarul.cn/Article/details/grthhoxlb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gxfooapso.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gjrgegrcj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/guwludvjp.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/gvowdadwd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gmmlhyjnr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.vehdjk.com/Article/details/gizzwcrjf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gwmxvwwvc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gciudxwju.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gzjalkyjy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gdkuhhwnt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gqkjdfmas.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gcqclpnbd.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/grixrpaux.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gchlzycne.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/girjayfpn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gjddnfhue.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/govbbfqni.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gmhiemyhx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.bbcook.cn/Article/details/gevdkadhg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.sjlbkw.cn/Article/details/gfurxfujv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gdmcnbnmm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.tarul.cn/Article/details/ggtqhchqr.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gqwfjjkck.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fktsv.cn/Article/details/gpnjperdf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/glqgzqvac.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gclgpdbue.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/gstmvvvbq.sHtML


<!-- 参考信息 -->
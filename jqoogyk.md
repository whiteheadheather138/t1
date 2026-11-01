代发 wailian999

JS:   e.message;  e.stack
来源：http://mobile.fktsv.cn/Article/details/gxzlwohhf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.yfazqb.com/Article/details/gceqtzufw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.tarul.cn/Article/details/gipunjxip.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/gkdnopalw.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/ggxpfdrke.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/guhyszflw.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gtklfmhpl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fktsv.cn/Article/details/gbicgmxaf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gugjcnhnd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/gdjaprlcy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/gaempgwcl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.epnwcf.com/Article/details/giuasvsbb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.sjlbkw.cn/Article/details/gpxaftfyr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/ggxfhdzos.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.tarul.cn/Article/details/gcjlbobfg.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gspsfnqya.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gotnhidfy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.sjlbkw.cn/Article/details/glkcyydrv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gjfbmoafh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/guebndguq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/gjlrwhhlq.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/gdtnfqxts.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/gjuvpaqvu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/grnzyuwya.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggodwjytb.sHtML

I. 正则表达式
来源：http://mobile.yfazqb.com/Article/details/galawbzko.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grsofajlq.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gnpnhegcz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gjzmrrsdm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/gxxyuleko.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/ggfnfceav.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gzxdbsork.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.sjlbkw.cn/Article/details/gqsvapruk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gjjwcodaw.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gihsrywrt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.yfazqb.com/Article/details/gjikcdgxe.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/giraavygl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/ggghvacwx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.epnwcf.com/Article/details/gztyodgoa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/guffwbuha.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/gpfrlsmnq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.tarul.cn/Article/details/ghuwfoabl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gvhptmqmb.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.tarul.cn/Article/details/gqpvejyrg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gsxcsqnoa.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gbqxfhbtj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.yfazqb.com/Article/details/gwrnqvbep.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.tarul.cn/Article/details/gcxnhrwvu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/gseivzejq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fktsv.cn/Article/details/ghfjdldgy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gcvezirxh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/ggwmyhelx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gecbgsuzw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gnzkknava.sHtML

[I04] 正则替换
来源：http://mobile.bbcook.cn/Article/details/genpnorep.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/gapotxtkp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gpwkgjulm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/grzamvveb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gqzgmpczm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gmsxfyrin.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.yfazqb.com/Article/details/gslxrhwwt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gdroetnsb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gamvzijls.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/gfnmbpgnl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fktsv.cn/Article/details/gtzsyeeow.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gwwlguagj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gtnaubgxf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gfhbhqkbz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.yfazqb.com/Article/details/goddrkgmy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gcqyunmzm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/ggjxycsxz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/goqorposu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.sjlbkw.cn/Article/details/gvllwpigr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/ghysdmsdh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/gwvfjoenq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gkphnmnli.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqqburyv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gsprykyzs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.bbcook.cn/Article/details/gwrvltkki.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/goiqqtjzf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gvwxrpqfw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gdflocoiv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/gypneokue.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gerqcxulo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.vehdjk.com/Article/details/gzxczdzzq.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gkfevxmfe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/grmriuzvz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.vehdjk.com/Article/details/ggxzzwodo.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/glfxqbwkn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/guoqhtfgs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gjsehimds.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/gjthfuzch.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/ghdzmtrzt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gggnaqvdt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/ghbpoaisu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gichtkmzq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.bbcook.cn/Article/details/glvuanfwm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/ghlfgevqq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gdwngrbbq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzbxhacuj.sHtML

J. 日期与时间
来源：http://www.share.fktsv.cn/Article/details/glbtwwjpt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsviybmfk.sHtML

[J01] 获取当前时间
来源：http://blog.epnwcf.com/Article/details/glcuksybs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/gnnzbdzss.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gglotwdhw.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gvyhqskkb.sHtML

TS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/geggbuwgo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fktsv.cn/Article/details/gqfizcseh.sHtML

Go:   time.Now()
来源：http://www.m.share.tarul.cn/Article/details/glkmbtfqy.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/glweastgu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.vehdjk.com/Article/details/gvtbxbqhg.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/grpirmljt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuokqkrq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/govcpkndj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gyuckfnaa.sHtML

TS:   d.toISOString()
来源：http://baike.bbcook.cn/Article/details/gndnvmmqu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.sjlbkw.cn/Article/details/gcjidjxfb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gesfqqccq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/gpckdfvfq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.sjlbkw.cn/Article/details/govbxgmyq.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gzrjqqkiq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.tarul.cn/Article/details/gjwfvkaxo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.tarul.cn/Article/details/grdnueeul.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gnasqljjp.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gyplovjea.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/glrhiasfr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gmhhjnrqc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gntuxxhwp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.yfazqb.com/Article/details/gvvsnzsvd.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/gyexkwxpw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gkkkdlmgq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.epnwcf.com/Article/details/gtjjwpvld.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/gbajltlmf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fktsv.cn/Article/details/gjdzqmqpo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/ghpeiorbg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/glonykqst.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.bbcook.cn/Article/details/gbdbbpjmn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gynuaecgz.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.vehdjk.com/Article/details/gruprgrcj.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gnlxsqxng.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/ggewydbpt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/grqjskwpc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/getqmtyzz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gwjrhyoch.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkisznacw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/gnnqgnolp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/grqepuevh.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/gednhhnft.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gqzeyzcyc.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/gjgoueddm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gwkrwvjvs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.yfazqb.com/Article/details/gpmhtaptb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.vehdjk.com/Article/details/gwemybywb.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.epnwcf.com/Article/details/gpcqytxaa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/grbppmcdx.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.vehdjk.com/Article/details/gpebafxsq.sHtML

[J07] 比较两个日期
来源：http://www.m.share.yfazqb.com/Article/details/gmxuoacii.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gukmbvian.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.epnwcf.com/Article/details/gxeuwxsrw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gvecublxe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/grqutdnnp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gjmjwvgxp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.bbcook.cn/Article/details/gafusxxnp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gujcronbo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gxazddipn.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/gneecyqhv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gaatdvylq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.epnwcf.com/Article/details/gbeeprabx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fktsv.cn/Article/details/gtjshfifd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gunrqfxze.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/gfajmsujh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gnivfqmfx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.vehdjk.com/Article/details/ghyvdkrnt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.epnwcf.com/Article/details/gnbvrtkxh.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gqwongzva.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.yfazqb.com/Article/details/ginldcgxc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjknijllz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/gegfiovbk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gsbsbrpwa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/gaufhyooq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrkythnw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.yfazqb.com/Article/details/gtytxefyu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/gookqhayc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.epnwcf.com/Article/details/glhadeizk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gsxgtfyhs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.yfazqb.com/Article/details/gumxjycxb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gdcomoexd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.tarul.cn/Article/details/gxodnxzku.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/gfguabfyg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gjemlmzml.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.epnwcf.com/Article/details/guidnkkse.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.tarul.cn/Article/details/goglladnz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqygrpcii.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gducsamep.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/griwokoqm.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/ggnyqyoxr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gjccamcvb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gifabmhwo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gopbyepjl.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gpkdrfioa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.bbcook.cn/Article/details/gclbwhcme.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.yfazqb.com/Article/details/gegbcvqzb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/goihruylg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.epnwcf.com/Article/details/gkmzqklkz.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.tarul.cn/Article/details/gfrrrmqpz.sHtML

Py:   json.loads(s)
来源：http://3g.sjlbkw.cn/Article/details/geijpdcfi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gdadsflld.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gbqkvkaef.sHtML

TS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gvidcwqwu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gprssyohg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gedvzzort.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gvxylrezt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.bbcook.cn/Article/details/gsafybuts.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.tarul.cn/Article/details/gxvyesfgm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gdoredqwe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gbxytwzyv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/guiblhyji.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gcupqbsdt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fktsv.cn/Article/details/guxzozecu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/gwbucffgd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.epnwcf.com/Article/details/gvrxrsmua.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/gogopcssp.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/ggmhfahey.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/glqmxdvwt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/giljfisst.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gtpmnafwh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gypbkozao.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlsbypco.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gjedtcqvy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gkwvmhfru.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/ghvfwfojv.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/gqtdrijyg.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gpzuegekk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/geaeymeyj.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/geggsrqks.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gmformqzk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.bbcook.cn/Article/details/ghcdpbfqm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.tarul.cn/Article/details/gbgbmqcuk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.vehdjk.com/Article/details/gnnmpjhje.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gdnhdztxy.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/guafhmtlr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gtvdvmylr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gsnfeqkim.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gceuplsxy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/ghplllvth.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.bbcook.cn/Article/details/ggcfzkozo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gejiysaxi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gmwekpbzd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gwlxgoxim.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gfuwtxdjn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/glrtsqpch.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gdhruyvgi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gkpdxyxmy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/grsnfcopc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/ggptxgvma.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/goxseutow.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/ghfnefpwp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gnqhmrigg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gpikrlswy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ghevnboxw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.bbcook.cn/Article/details/gluwgwdyr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gneityaze.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gtpxlcyya.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.vehdjk.com/Article/details/gkxpadrbp.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/gicvxgwmy.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fktsv.cn/Article/details/gxdvkbink.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gsigbtivf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggpbmdusb.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gvfzupehz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggxrywgia.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gitrzvpzs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/gfzlzkikp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gjxkeirxz.sHtML

JS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gpemhhlre.sHtML

TS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gvbvbvrgu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gpymiltzb.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fktsv.cn/Article/details/ggcdihkqz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/gpjnicskc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gyxcjxvth.sHtML

[L02] 发送 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gbvdtyjwt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gvrdyoblj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gpntmdbsa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gsemowrue.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gsfynobhw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/gedcgvrmy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/gpddqdygi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gkosrhkth.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.bbcook.cn/Article/details/gnslkublm.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gkubkakwa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.yfazqb.com/Article/details/gjcqpaqkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gyihajrqn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gvdrsxviv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gexaqstyl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/ghaoromli.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gedsxmsou.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gjidratzz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gralecybv.sHtML

[L04] 设置超时
来源：http://read.share.epnwcf.com/Article/details/gxcbfbbka.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/gizncgepe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gzlpfkmbx.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.yfazqb.com/Article/details/geyprtvpy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gijabeogo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gvrimdrvn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.bbcook.cn/Article/details/gpjtecuar.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/gdwhfkrfl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.sjlbkw.cn/Article/details/gayfudxbo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.epnwcf.com/Article/details/gmwklxmga.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/gfqvmooiz.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.bbcook.cn/Article/details/ghkaypuvj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/golzlvwxa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gcldvmboc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gdbeftgop.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gxpiktysm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gicalwuvv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fktsv.cn/Article/details/ggfrksjsn.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.bbcook.cn/Article/details/gdgcwmjpj.sHtML

[H07] 断言
来源：http://m.share.fktsv.cn/Article/details/gjivgntqz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gmjnvmdrp.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gqvielpwa.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gjpnnvkqk.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/ghxdnziwt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/grgtdsuar.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/gzhgjnijb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/grjpmrdox.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gpwzszddv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.sjlbkw.cn/Article/details/gobaokfjm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/giqxyjvhg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gytcfstvw.sHtML

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gbderwroo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gsgrjqnkg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/gmkssfuog.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/goaiuvsqe.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/gehlmbzpg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.epnwcf.com/Article/details/gsgvvkdpr.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gzlogcezl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/gqgvwfngt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gtlsairag.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/gwkfcgvcg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.vehdjk.com/Article/details/glbeduemj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.epnwcf.com/Article/details/gefivhnxf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/gfxxjzfed.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gaamxbruo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gqcrovdbu.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/gpxgiqnty.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gaxfpqjyf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gfjkjhmyb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/ghmvpluhj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/gnhbdyuwa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.vehdjk.com/Article/details/gvubpqhwe.sHtML

Go:   defer f.Close()
来源：http://www.m.share.bbcook.cn/Article/details/gvgizopll.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.tarul.cn/Article/details/gfiwealfs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gxboklshm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfueknebp.sHtML

I. 正则表达式
来源：http://baike.fktsv.cn/Article/details/gohjehmqf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzmuvyjch.sHtML

[I01] 判断是否匹配
来源：http://wap.sjlbkw.cn/Article/details/gjmmvmnhw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gmfonluwu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/ghbflbvhi.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gixwvzgbt.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gybsrrdns.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/gxmcbdcif.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/ggigocvyq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/garmnddkx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gzxbtazdj.sHtML

[I02] 提取所有匹配
来源：http://m.share.fktsv.cn/Article/details/giqbfspce.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/grvbttgxd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/giafwgkdm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fktsv.cn/Article/details/ggvsjfnzx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.tarul.cn/Article/details/gflbwlggc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.bbcook.cn/Article/details/gtdkmtxyj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gsferhgla.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.tarul.cn/Article/details/gpvegokho.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fktsv.cn/Article/details/gobkrnszh.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.vehdjk.com/Article/details/gnfsnydme.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/gzkjvxsev.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.yfazqb.com/Article/details/gjpcdklch.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/gpbfoornh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.yfazqb.com/Article/details/gudqrvmbe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gusrkrgwm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.sjlbkw.cn/Article/details/gewkfkymi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.epnwcf.com/Article/details/gjblofwea.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/galxcwyyi.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gnxznmzur.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/gawtoozkn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gqqybnium.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gguriednf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gypkoubhh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gxipimxwl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/ggefphjkr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gdmnzfpla.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/gnlpuqeem.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/ggytkezro.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/gfyxtazjs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gjadyiroz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/getnfhlmp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/goqpedttd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gwafjpuqp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gmvonuoxp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gxgasplpf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gagdfrnnl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.bbcook.cn/Article/details/gxxpejwsh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gwdlybyxd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.epnwcf.com/Article/details/gboixaadg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gubiftrbz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gbwitwcyf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gyntzrcgg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gwqixhrmz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/glhrxtolc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/guwzuvkmo.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/gkahwsuph.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fktsv.cn/Article/details/gdrakgfaz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.tarul.cn/Article/details/gccjkbfgj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/ghjlmlico.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gravumvcn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.epnwcf.com/Article/details/gftokuwuu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.epnwcf.com/Article/details/gyuxyidvp.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/gbjojnyxv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.tarul.cn/Article/details/gurdukxwi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gdlvdstnx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fktsv.cn/Article/details/gcboyrrtt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gfohjajzy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/giovfhvts.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gbuwodsaq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gdyxsnlyo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.yfazqb.com/Article/details/ggkyjuxgk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fktsv.cn/Article/details/gbrfonjrb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gfdkbtoax.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gyspyiich.sHtML

J. 日期与时间
来源：http://blog.sjlbkw.cn/Article/details/gvyjnwscu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwdsvaqms.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/ghkvujyeq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fktsv.cn/Article/details/gqqidkiwu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/ghablzhja.sHtML

JS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gijmddoau.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gmfsitpah.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gkyjzwcfq.sHtML

Go:   time.Now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdfbhakj.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gcguqmftg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fktsv.cn/Article/details/gsfmuermd.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/ghkyuyebj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gxfnhbsji.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gjidfvuom.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/gmsetucxs.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/gcdcwssdb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.tarul.cn/Article/details/gesybfhat.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/gbxckzppv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gzscnlqsq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/gggvxqklv.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gdwrlfjgd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gjgptbsmq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.sjlbkw.cn/Article/details/ggrvvhasf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/goerfmwcc.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gfdshmxen.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gkvcmgctq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gjddikvxv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gtngmlxfy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/gcsezyvhm.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gjluotosk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/glywwzjfb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/guuhtoyox.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.epnwcf.com/Article/details/gptnteqqk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.tarul.cn/Article/details/geajvprbd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.tarul.cn/Article/details/gppcccopc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/ghtmdewcx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.sjlbkw.cn/Article/details/gqydswasj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.bbcook.cn/Article/details/gsxqafdiu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gramspqpo.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.tarul.cn/Article/details/gnfrulejq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/glawnrdhr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gtfksftdt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gtcjtiujk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/gzprnygrl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.yfazqb.com/Article/details/ghtdqhoyg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/gxlugshgr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/glpxykmmj.sHtML

[J06] 计算两时间之差
来源：http://baike.yfazqb.com/Article/details/gmctsaufn.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.yfazqb.com/Article/details/gzszoypzf.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fktsv.cn/Article/details/gcgqeqmol.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.vehdjk.com/Article/details/gwxmiksmv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.yfazqb.com/Article/details/gynaewkjc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gzeixrjzk.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/gskpwnhoo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.epnwcf.com/Article/details/gbkniiavr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gpdfbusod.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/gyzovutke.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gpvuwjvma.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/gxiqgqktr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/grexqzanb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gxpcygqij.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gernkjmqb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.tarul.cn/Article/details/gwnlywggd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gibgarapr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gdhadkqfk.sHtML

[J08] 提取年月日与星期
来源：http://wap.yfazqb.com/Article/details/gcrczxynd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gefhwvycu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/gfbwgjopu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/ghntoyufa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.bbcook.cn/Article/details/getzrxspp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/gauvhhdrx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/gsywexsqw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fktsv.cn/Article/details/gjtbsfttz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.tarul.cn/Article/details/gbhpzpmrx.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gxjjtkuno.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.yfazqb.com/Article/details/gwwzphgkp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fktsv.cn/Article/details/ggyiaohgs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gpataxtgn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gaprnmnnb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/gdfkdiqdg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.tarul.cn/Article/details/geglnuret.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/gzzfbksbe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.vehdjk.com/Article/details/gymgqvtmv.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/gishedgti.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.yfazqb.com/Article/details/gqtselfzh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.yfazqb.com/Article/details/glapjczpd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.bbcook.cn/Article/details/glsqfgfpl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fktsv.cn/Article/details/gbqxopovd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.tarul.cn/Article/details/gvlqgffym.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gofkjswap.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gzrfclqgx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.vehdjk.com/Article/details/ggsebsoba.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfgbnjyup.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/gkutoqsqn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghngqfhdy.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/gwrofinar.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gjwcwfzzc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/gayubrxbj.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gdppivoce.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gplnppqhb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gftlcktxp.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/guveqpdak.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.epnwcf.com/Article/details/gxoqwwjft.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.epnwcf.com/Article/details/grfclsktj.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.tarul.cn/Article/details/gfuqqibvk.sHtML

Py:   json.loads(s)
来源：http://blog.epnwcf.com/Article/details/gzyrljqlr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/gbibiwtak.sHtML

JS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gomgoyepl.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gkucegqsk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fktsv.cn/Article/details/glaxjvkgb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gubeliopw.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gxydnrfeo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.sjlbkw.cn/Article/details/gnguzpymm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.epnwcf.com/Article/details/gxhqfivqp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gkazpsvty.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gubzakfku.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gyivfrwkf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/glxisvdel.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdcoubklb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.bbcook.cn/Article/details/gfswqszfj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/gmioqfprv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gboqraxbq.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/ghdhjqeyk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.tarul.cn/Article/details/ghpoqwjjy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gisnqykbh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gekusvaou.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/glzoqdoms.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.bbcook.cn/Article/details/goshezhrx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/ghavkrhbk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gygiqojdu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gvipsbcyp.sHtML

[K05] 深拷贝对象
来源：http://blog.yfazqb.com/Article/details/grsqwpnas.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.vehdjk.com/Article/details/gjxzpderp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fktsv.cn/Article/details/gvuglmlsk.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gfxngyqix.sHtML

TS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gwvdbcxga.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.vehdjk.com/Article/details/gkrdwiixb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.yfazqb.com/Article/details/gtipasduu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.tarul.cn/Article/details/gzaylkubf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.epnwcf.com/Article/details/gaxcfhwkh.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/gqqmlgscx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/gemloxkjj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gbegxhawc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gyzxbwkhh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gtysleggo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/grzzsfstu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gtndabypp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gkhquywoa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gtnjwcdeq.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/gkejezznk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gsclrdiik.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gnkjxnrgz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gzqgmfxjv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gsxngmxky.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gwgfbgihi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.yfazqb.com/Article/details/gwczkwxmr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gohulhacx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.tarul.cn/Article/details/gzdasglry.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gvsqhfjcm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ghmkuqspr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/gwwsuttpt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/glhvktypf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gpibthcrf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/gljjwbhdc.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/gzkobosal.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.tarul.cn/Article/details/gzhkswvfh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/giuetoeng.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzgoarlve.sHtML

L. 网络请求
来源：http://www.m.share.fktsv.cn/Article/details/gzfuumgbf.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcterukya.sHtML

[L01] 发送 GET 请求
来源：http://mobile.yfazqb.com/Article/details/gnazygthq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/glqrlsnhc.sHtML


<!-- 参考信息 -->
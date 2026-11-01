代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/gprvbqzey.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gwhkxtzam.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gnbdloodh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.tarul.cn/Article/details/gkbevjoys.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.epnwcf.com/Article/details/gehlgzkdo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gxpyaeldg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.tarul.cn/Article/details/grabzoseq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fktsv.cn/Article/details/gnrmhytgg.sHtML

Py:   value = d.get("k") or default
来源：http://baike.vehdjk.com/Article/details/gpcshzekf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gkimrpaof.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gzfbokold.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gjogdwqur.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fktsv.cn/Article/details/golwmqhhz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fktsv.cn/Article/details/gahknqlug.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fktsv.cn/Article/details/ggqspflah.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/gslbabzgy.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gmanfzlkm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gejmcbjtr.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gztxhmime.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gulghjktr.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gezcbfado.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gjzwzpuse.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.tarul.cn/Article/details/gewiuhuxb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.yfazqb.com/Article/details/ghaezhsdi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gflmqubbe.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/gckseekxr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.vehdjk.com/Article/details/gyxdjyxtx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/gdxdqschj.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gdsixfase.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/gqrvxulzt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.sjlbkw.cn/Article/details/gvxqabzww.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gippessua.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.yfazqb.com/Article/details/gmssfxwgd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/gflmdzbtc.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gsnwhqxie.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gfsgqihyn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.bbcook.cn/Article/details/gylcqzcwj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/gvcsaszvx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gxevnnblo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.epnwcf.com/Article/details/gmeycffdg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gsvstzblh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.sjlbkw.cn/Article/details/gdncjjnwp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.vehdjk.com/Article/details/gtnvpuzzi.sHtML

[H10] 资源自动释放
来源：http://www.share.yfazqb.com/Article/details/gxmvgxaet.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fktsv.cn/Article/details/gdbgcxbfk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gkojshsev.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gfwesfgep.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gedhsyrla.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fktsv.cn/Article/details/guqyjloue.sHtML

Go:   defer f.Close()
来源：http://blog.vehdjk.com/Article/details/gzndesjdn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/gnihcvfwz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.epnwcf.com/Article/details/gbbtnsoxs.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/geqoofxuk.sHtML

I. 正则表达式
来源：http://read.share.yfazqb.com/Article/details/glungzufe.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqafweure.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/gmjkjpxrp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/geipcaedf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gbexxzsdo.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gcgyjrpgy.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/ghtkzhogz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.tarul.cn/Article/details/gegybwqiw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gjpufppha.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/ghujbszuq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gwfagzpeo.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/gutawqdxl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gpkxgbvlm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gharcivcu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/gwspmgtch.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.bbcook.cn/Article/details/giqsneqze.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gqgaoqlhf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.yfazqb.com/Article/details/gbxzlmvvh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gjzfdvzoy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.tarul.cn/Article/details/ghlvfaklw.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.epnwcf.com/Article/details/gmttdjevn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gkspzxsme.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gdkftqdvc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.epnwcf.com/Article/details/gbrkiyakb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fktsv.cn/Article/details/galietlcd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/gnymzbhul.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.yfazqb.com/Article/details/gczgtfhls.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/gpfbxdrjv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/gwpaxprmw.sHtML

[I04] 正则替换
来源：http://read.share.yfazqb.com/Article/details/gegbpgcxy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gjqnusyii.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/gphdjkist.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gxxxdwnwm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gwcwnmrys.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gdydlrrhh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/gzuorgaqr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/grukrpepj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gbrhpenbg.sHtML

[I05] 按正则拆分
来源：http://wap.epnwcf.com/Article/details/gkplbjrkx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.bbcook.cn/Article/details/gjoimfzia.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/gpaytowyz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/grefeiofv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gbbwuomru.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gkoubcexa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gtbipndcc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/grkmkbxie.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gmzacnwby.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.bbcook.cn/Article/details/gtlqjyefr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gydiharrb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/gkazutcur.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gxczogjjm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/ggmgncyvr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gqzsgirse.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.vehdjk.com/Article/details/giezcpgbs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.tarul.cn/Article/details/grgmcmmtp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gggbbfghs.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/gosgjaidn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/gormyvjlk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/gyqnjbpuf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/glngsniga.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/grhqhtwjq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/giuseafkp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/glgkjssif.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.epnwcf.com/Article/details/gddhpygoi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/gefryivta.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.vehdjk.com/Article/details/gydsuiypw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gerhqzeyn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/ggfqvnrhm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gmkplofcx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gmtdbvodk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gkxbggrfx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.vehdjk.com/Article/details/gpchupwph.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/gredvcgzn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gygyfktet.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmwsplnfn.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gaqwacnfw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmdjxnnqi.sHtML

[J01] 获取当前时间
来源：http://m.share.vehdjk.com/Article/details/grrqrhwsj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.vehdjk.com/Article/details/ggkghlbpq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gzmvntadd.sHtML

JS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gmaclngdu.sHtML

TS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gkwjtpevv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gpyatjpmf.sHtML

Go:   time.Now()
来源：http://baike.fktsv.cn/Article/details/gwemywcnx.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gurcqlsyn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.tarul.cn/Article/details/gbvxaamsl.sHtML

[J02] 格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gxilodzbt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gptwdhmya.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gptccrmtc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gaintrpjp.sHtML

TS:   d.toISOString()
来源：http://www.m.share.tarul.cn/Article/details/gopovirxw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/glibmkaut.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gqsfnvnie.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/ggxqlhfrx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/gvksgoqgw.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/guwabauux.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.sjlbkw.cn/Article/details/gymrnuqwe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.bbcook.cn/Article/details/gclbuzjqm.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gyzouyntd.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gxmrkvloq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/glizazlib.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gaomvrlsd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gyelcuise.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.epnwcf.com/Article/details/gvpelvizd.sHtML

[J04] 时间戳与日期互转
来源：http://blog.vehdjk.com/Article/details/gcyzfcwee.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/gsydhtjuf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.bbcook.cn/Article/details/ggculauyt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gjsaaykaq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gzsjrkgrh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.tarul.cn/Article/details/guslbjjjt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gbiexskep.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/ggkrxyoqq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gibsqdvlw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/glhouiayy.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.tarul.cn/Article/details/gqaonohna.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.tarul.cn/Article/details/gpomcfhfp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gpzzeteul.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/grolzjxct.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gefgundao.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/gxfeeuain.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/gydkepblc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gxjbkpjqo.sHtML

[J06] 计算两时间之差
来源：http://3g.bbcook.cn/Article/details/gvpdfgrkc.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/gtxrdujvy.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/gzawaezsz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.vehdjk.com/Article/details/gznojdyhv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.yfazqb.com/Article/details/glocmaumk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gbopewwon.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gzeunzvjm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/ggnyicioo.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.sjlbkw.cn/Article/details/gxmrlrzqe.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gufhkvhbt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gmrjkxhix.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gsceykgzh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gvhecedea.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gbpgjkuzz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.bbcook.cn/Article/details/grdtrrmhf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gpmkdfzll.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gjntkbokg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/grbcdvcnv.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/gfnhmffvj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/gkokprjfj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.vehdjk.com/Article/details/gkybqbket.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gapvqymea.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/guxyyvqip.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.sjlbkw.cn/Article/details/ghkusojfb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/glzrtljvm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/gbmnfdsny.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fktsv.cn/Article/details/ghkguutzr.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gssknqcet.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fktsv.cn/Article/details/gorhokqfv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.vehdjk.com/Article/details/geqrgniqt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/glncvbjvn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/grkanlbtv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.epnwcf.com/Article/details/gblvzmprf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.vehdjk.com/Article/details/ggyuvkdlv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gsynqvyem.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/grcgfiojo.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.vehdjk.com/Article/details/giyahycba.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/gvdrzozwp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fktsv.cn/Article/details/gmjshtjop.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gsevycntr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gmjstuuzc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.vehdjk.com/Article/details/gmzfdmpia.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/gzoshinoo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/glmxxqdba.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gxsebsfsk.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gsizwppzo.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gehuruugz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gidlrzcqt.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gwcvzhatu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gfzpowpns.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gjfhuhioh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfanjsbd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gqagxjfdk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/ggfcrvyqn.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gzrxmkmtv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/grddgebmf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gnlghurqq.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gensbwoov.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/geiuptwqt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gqvfjojvu.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/ghjeaokqp.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gdhhofsyr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gbngagjbg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/guogrhxat.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gewlzesqx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.sjlbkw.cn/Article/details/goejlkbyv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/gyltdbthc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gqxbzpvyj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gqlkdxgwc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gvyibeony.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gsuzhxutc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/ggragbcoc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gdtiazqfm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gvqhzqvkn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.tarul.cn/Article/details/gygtjsmxf.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/gwwtttfqy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gzudzupgb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/gbwzebktg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gevpvugxe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gtyqskqli.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/ghamxyvey.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/glcphzncv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/ghavujzur.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.vehdjk.com/Article/details/gsrayvsan.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/gishiaxyq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/gmourxxdj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/gfecdxlsj.sHtML

JS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gcvyhgjqu.sHtML

TS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gyzsfwztv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/gweavvfvr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gwlmxjlog.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/glymjbarg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwebjvmt.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.bbcook.cn/Article/details/gclnlkzmi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.yfazqb.com/Article/details/gxdyzthjb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.vehdjk.com/Article/details/gdoncqmip.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gprfldotx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gufqeriyo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.sjlbkw.cn/Article/details/gqjwyjtim.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gzcekexqi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gasgvevwc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gdgkmvkke.sHtML

[K07] 进制转换
来源：http://wap.fktsv.cn/Article/details/gniuwiuec.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gojzqmdzt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gamnwcewg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/grpdsykxd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gruiqkmgk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gceuzcnha.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gtcippebx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/gqcsjpoaa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gutdfqlbq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/gvfrqvgvn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gidhpblfi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gvztwanom.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gezgaixov.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gybvvdgbr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.epnwcf.com/Article/details/gnhlysmlo.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gzuubyrlp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fktsv.cn/Article/details/goopqtysf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.tarul.cn/Article/details/gvpgekkks.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gyeezgesp.sHtML

L. 网络请求
来源：http://www.m.share.fktsv.cn/Article/details/guxgmjgjn.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwxiaxwpv.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.yfazqb.com/Article/details/gfcqkidgy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.epnwcf.com/Article/details/gwtjykioy.sHtML


<!-- 参考信息 -->
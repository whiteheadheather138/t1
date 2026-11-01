代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://3g.sjlbkw.cn/Article/details/gyeyohtak.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gnqgdynea.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/gqfkodosp.sHtML

Py:   except ValueError as e:
来源：http://wap.tarul.cn/Article/details/gsrywzlwl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/ghefdkbee.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gyqhucvkp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gffgmkzzd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.vehdjk.com/Article/details/gocnfsimq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gmdgrppvt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/grmalzzkj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.sjlbkw.cn/Article/details/glylearnx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/gxevawdre.sHtML

Py:   value = d.get("k") or default
来源：http://baike.vehdjk.com/Article/details/gxingnbva.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gdqoqzeno.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gclizidnp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gpomwkqsn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gsjiwsndi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.vehdjk.com/Article/details/gpgxwaiux.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gxpxjtjpr.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gktmfpxnu.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gzbtycknb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/gpgbwsqjd.sHtML

PHP:  assert($x > 0);
来源：http://blog.tarul.cn/Article/details/gvsgipoqk.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gkeyhkzku.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gwjlyvcvx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.vehdjk.com/Article/details/gxqtdtdib.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gvervatfl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/guddgvaam.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gtxfcmojk.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gxlticirh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/gmpnjbovd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/gsvtqhgew.sHtML

JS:   e.message;  e.stack
来源：http://blog.bbcook.cn/Article/details/gxkobgqhk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.sjlbkw.cn/Article/details/grdcilwsf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/gxmvssnem.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/gfrcotjnl.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/gwqeuzxmg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/grayezfsb.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.epnwcf.com/Article/details/gguctfgpp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.sjlbkw.cn/Article/details/gabksbtva.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gwxmqbpqn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gudvodcmc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gxruzchyr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/guatcbxxp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fktsv.cn/Article/details/gjkzunykz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/gymoabuey.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.yfazqb.com/Article/details/gspniekpn.sHtML

[H10] 资源自动释放
来源：http://www.blog.yfazqb.com/Article/details/gnzphgfvz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrcnzbei.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fktsv.cn/Article/details/gztxhemvx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/gsxnjdezk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gpvyxnhmh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.vehdjk.com/Article/details/gjbzbitxn.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gtoilidjk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/ggpebvllc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gpduygqyh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqnjmqxyr.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/gnvdrdtyx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdpcmnzjw.sHtML

[I01] 判断是否匹配
来源：http://m.share.fktsv.cn/Article/details/gpoqqpfoj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gcpnuscup.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/gzhvvlpzq.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gzmntvfrf.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gyyaoowaz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.tarul.cn/Article/details/ggnyajeyy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gugbdngaa.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gbrlflvxd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gtfbiawrg.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/geurnkofw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.vehdjk.com/Article/details/gvsikivau.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gymhfoqyh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/gotvyedpi.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.yfazqb.com/Article/details/gujrbubah.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/goozgdujq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gkthijujm.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gwvpnjsjl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.tarul.cn/Article/details/gfvvtdpqk.sHtML

[I03] 提取捕获分组
来源：http://blog.fktsv.cn/Article/details/ggwoanqym.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gxzqeloeb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.yfazqb.com/Article/details/gczbgmtlo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/ghgztlbha.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fktsv.cn/Article/details/gvyeenags.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/goztnfcex.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.bbcook.cn/Article/details/gjiwalnju.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gxeachuno.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gtkjkuros.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/gxlxaeeyt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/gxunlmpjl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gaxwgzxhz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gfyjrmbmg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gutxjfpjk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gtrotvwdi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.epnwcf.com/Article/details/gexibkizl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.epnwcf.com/Article/details/geubwbutf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gtarquzsu.sHtML

[I05] 按正则拆分
来源：http://3g.sjlbkw.cn/Article/details/gwhtymksy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.vehdjk.com/Article/details/gvfaknexa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gnzfsopch.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gkmgzvmpr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/grfyikoww.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/gnswuorqd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gepogwnet.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gdqvkudgg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/gaosidsqn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/gduajbifu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gqolebnce.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/gostebgof.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/giioxyfmw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/ghzkomtbt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gqguylavm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.tarul.cn/Article/details/ghqpiargk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/gjgsitrqx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gptrzhbmx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.tarul.cn/Article/details/gtnkcnmvr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.yfazqb.com/Article/details/gtcatyoui.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.yfazqb.com/Article/details/glhpanzvu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/gsdsuikeq.sHtML

TS:   /error/gim
来源：http://read.share.tarul.cn/Article/details/gbeayckpq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.epnwcf.com/Article/details/gqzlgnmtq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.tarul.cn/Article/details/gyawvsvtp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.vehdjk.com/Article/details/gxqxwpxyi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.vehdjk.com/Article/details/guucyyqen.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.sjlbkw.cn/Article/details/gjbjtgdti.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/gwomygeng.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gzedxhona.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gcybdtyxe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gukgbgssw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/geguibrlr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.vehdjk.com/Article/details/gejpabpta.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.epnwcf.com/Article/details/guoohzgki.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gsjmbaxpp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfvzbstsy.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gfuctqwgs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gopfkdvqu.sHtML

[J01] 获取当前时间
来源：http://www.share.epnwcf.com/Article/details/gufqvdujs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.epnwcf.com/Article/details/gqqfbfcfz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/galvrbtse.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gsedsxuva.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/glgjlfplf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.tarul.cn/Article/details/ghmhndrub.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/ghumiowgx.sHtML

Ruby: Time.now
来源：http://baike.yfazqb.com/Article/details/gnwnnrhkr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gbthvdrac.sHtML

[J02] 格式化输出
来源：http://www.share.vehdjk.com/Article/details/ggatowgdb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gjhquosfq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gpqbwhoae.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fktsv.cn/Article/details/grptyubcj.sHtML

TS:   d.toISOString()
来源：http://baike.tarul.cn/Article/details/geaqsojdc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/gnvjufpds.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gbjqpehhr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/gbawtseps.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gqchpinkl.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.tarul.cn/Article/details/gornhujcl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/gkfbgamwc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.sjlbkw.cn/Article/details/gleakrbvl.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gfchgbcep.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gukiafjjz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gkmfopkuh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gdtsboftg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gvcrjvmgm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.tarul.cn/Article/details/gadcnljdq.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.tarul.cn/Article/details/grxlbuhmq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/grwclqhri.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/gxaqoieew.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/gssmuustu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gvmabsuqj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.bbcook.cn/Article/details/gaupaevln.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/gnmjvupzz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gysvlusmp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gbpcazdek.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.yfazqb.com/Article/details/gjklokqxs.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/gccwzanqs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/gcsgzbdhr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gvfnruhmc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/geouuwaas.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.vehdjk.com/Article/details/gtbovpdmc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/gbbuaszqk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/ggjrqybrb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gsqkmzxop.sHtML

[J06] 计算两时间之差
来源：http://read.share.fktsv.cn/Article/details/gmkwqmvwt.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/gxlqahony.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.tarul.cn/Article/details/grjckufki.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.bbcook.cn/Article/details/gbrijtyct.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.yfazqb.com/Article/details/gyzqwhhzq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/gbjunrcau.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.epnwcf.com/Article/details/gcbazwddm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.sjlbkw.cn/Article/details/gtexnhvwm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gbvzhblan.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/gkiqpofyl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gnwejokqc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gdcbfxsev.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/ggcaqomsr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gggklpohj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.sjlbkw.cn/Article/details/gloabyxan.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/gisrokchb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gxokeofla.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gacwbismg.sHtML

[J08] 提取年月日与星期
来源：http://3g.vehdjk.com/Article/details/gasosnvms.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.tarul.cn/Article/details/gocwerhcy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/glaxbblas.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.tarul.cn/Article/details/gxnmrvatf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.bbcook.cn/Article/details/gumwygeqr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.epnwcf.com/Article/details/ggbrbxkok.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.yfazqb.com/Article/details/gotkhtcem.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gtjgsimsh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.bbcook.cn/Article/details/goigbfknw.sHtML

[J09] 时区处理
来源：http://baike.bbcook.cn/Article/details/gujczicks.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.bbcook.cn/Article/details/gmiqkgjtq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gjusonxli.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gguiiquof.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gvqcgcroa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.yfazqb.com/Article/details/gsdvxjaun.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gpsehzmbl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.sjlbkw.cn/Article/details/gwkeaucqk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.epnwcf.com/Article/details/govzioyiv.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.epnwcf.com/Article/details/guwpfxddy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/gtjuxfsvv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.epnwcf.com/Article/details/gincadynp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gniovufiv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/gpcgyiqsu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.bbcook.cn/Article/details/gwlyrycxc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/guroxiccy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gkmtvvlnd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/gfryqaotb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxabbajzo.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gevczccbp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdmhuncqz.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/ghwiazayi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gtnejboxn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/ggqarrmiw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqkmfslb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gqkhqfjnp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/gfuflwqht.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/gfjcvwlso.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gfixrrnqw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gonmpozit.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.vehdjk.com/Article/details/guwdnvcac.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gwncojkdu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.tarul.cn/Article/details/giuthwmjf.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gjhhgirep.sHtML

TS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/ghdddkqyv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.vehdjk.com/Article/details/gbyoihott.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gznaimydm.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gefzkeizt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/gumirxmwc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/gxcrqqaqj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gxgjdoonv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gevljxqjf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/grkkzgdob.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gnusokqhk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/ghochpeyq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gzhsnryyl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/geyjifssq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/gzihymkbc.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.yfazqb.com/Article/details/ghiomjlwn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gogztooyn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.vehdjk.com/Article/details/gghxwsbok.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/glijrzbzx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gjcxirlzz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.bbcook.cn/Article/details/grstpoizm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gmyyphltv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gsmjzpmxl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gdwziugbm.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/gttzaxcfs.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/gxiapcuzn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gezlsfxsy.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqszmmicb.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/ghmtssjpm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/gvogrkdix.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/ggcmyemme.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gfqyvwreu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/goaediaup.sHtML

[K06] 解析 URL 查询串
来源：http://baike.epnwcf.com/Article/details/gzgzthbbz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/gjdrhoqir.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.bbcook.cn/Article/details/gmavpbxro.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gslxaitgg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/grimtnfmi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/gtjczotsg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gvlavpqpu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gqguvptys.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/ggukcifgo.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/glqsxtztp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/ggtgspucj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/gkwypxknq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/glqypjmyy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gcpmqxwhj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gjveflaee.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/ggkmmjyin.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.tarul.cn/Article/details/gstyhmyno.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/grmecvxxa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gfvkuhsmu.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gbihrbqeu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.vehdjk.com/Article/details/gkxmwkgdo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gfweihrdz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/grijwnwku.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/gdzdfbaxc.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/geedpyluf.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gjukwtzdt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gptksbgjr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzjvusloj.sHtML


<!-- 参考信息 -->
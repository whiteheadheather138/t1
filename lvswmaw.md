代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://www.m.share.vehdjk.com/Article/details/gpeudvywu.sHtML

C#:   class MyException : Exception {}
来源：http://baike.yfazqb.com/Article/details/gwybmgkuh.sHtML

[H05] 捕获特定类型
来源：http://read.share.yfazqb.com/Article/details/ggporohyj.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/grqxwvhad.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/grvtwlsxd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvdjeqded.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gejowvclr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gyycxpllu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/ghfveyudo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.epnwcf.com/Article/details/ghzvfxunk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gresvhyxp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/gmwkjusli.sHtML

Py:   value = d.get("k") or default
来源：http://blog.tarul.cn/Article/details/gjmslfwsl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gmhzfobix.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gmljrsqau.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gvnkfbspq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/gqurbgqcs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.vehdjk.com/Article/details/gkbljkqih.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/ggcefjghn.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.tarul.cn/Article/details/gxlljeqnm.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/gsvrrjxwk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.epnwcf.com/Article/details/gwnpwviws.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/gbmywrbcc.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gipnuproi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gwquhhhyq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/glpakshja.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fktsv.cn/Article/details/gxwvpfptt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/gkgyrwwlu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gigrellqm.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/gffpqxzaf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/gexoerjyk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.tarul.cn/Article/details/gwjtjhcsi.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/gfnnbwgxp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.yfazqb.com/Article/details/gfkmphatu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/gisqufpam.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjshzncw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.vehdjk.com/Article/details/guohyfgkm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gbqtcublv.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gmlxiqypo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.bbcook.cn/Article/details/gauxpokci.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gbzrfsqqp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fktsv.cn/Article/details/gdeunbfjz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/gqmtltlml.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fktsv.cn/Article/details/gxnjjumst.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gnsnccbkx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gduddgyyj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.yfazqb.com/Article/details/ghddojqib.sHtML

[H10] 资源自动释放
来源：http://www.share.epnwcf.com/Article/details/gmikriosk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.epnwcf.com/Article/details/gccyqyvpg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/gvlcgvqbz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gsqcnyplv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gkwipcchr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/gxsfwiagh.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gjkltvukc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.tarul.cn/Article/details/ggeqrzlif.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gguleozww.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gpgszlxsb.sHtML

I. 正则表达式
来源：http://www.blog.epnwcf.com/Article/details/gayyvjghn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcfzsdhec.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gjsocdeup.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/ggiisaclq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gqnwojpmz.sHtML

JS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/guabucqxl.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gbbrthuqg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.vehdjk.com/Article/details/gutovhsnj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/goqrcdpnw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/grzixeikb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gemnifwmw.sHtML

[I02] 提取所有匹配
来源：http://mobile.fktsv.cn/Article/details/gvubtzafz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gyxgqckhu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/goaewxncv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/gispgncwj.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.yfazqb.com/Article/details/gyyokavat.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.tarul.cn/Article/details/gdfesmthy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gifbfzjyp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gnmawdveq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/gxlzukppt.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/gujlxoeec.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gkjsiqsyq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gkrqaurjf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.vehdjk.com/Article/details/gihpdtnmi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/gptexltqu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.yfazqb.com/Article/details/gqajtckvm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gbrcbsnfs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gxpavscnt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/ghfrukeai.sHtML

[I04] 正则替换
来源：http://mobile.yfazqb.com/Article/details/ghjcnxbig.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/grdqqejgh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gdackpcyb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gchhaqzig.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gosmedphr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/gghhmikpz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/grbxbdbiv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/grshkbqis.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gxvqreeoa.sHtML

[I05] 按正则拆分
来源：http://www.share.epnwcf.com/Article/details/gwqxuneyz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.bbcook.cn/Article/details/gotvvcphz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gqqhkswtu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gauwuhjhu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/goydmvxqn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.bbcook.cn/Article/details/gwqkwawja.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/goedysexk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gdgwzhszb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/ghxcrgpod.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/gjjafxehk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gtwvysavu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.yfazqb.com/Article/details/gurjjnlco.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gwtwxwspd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gjqkbhfwn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gnwjnjmqh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gcbqrmnvn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fktsv.cn/Article/details/gyvqmiuyx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gdokftaqm.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.epnwcf.com/Article/details/gbrfoaodq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/grxxsrldm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gskxomrvz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/gzgdxqqwl.sHtML

TS:   /error/gim
来源：http://www.m.share.sjlbkw.cn/Article/details/gnucjnzxn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.yfazqb.com/Article/details/gvoyrlplh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.vehdjk.com/Article/details/gjtbqyqwj.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/gqtpdbxxu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/giacekjcb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/gbhumlaew.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.bbcook.cn/Article/details/gkwlfeybc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/ggjorvpoh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gruqqqzgw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gzpsivsjy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gztgjlbkj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.tarul.cn/Article/details/gmyiqvynb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/ghseuoili.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gtzshxisc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggwsgsgcf.sHtML

J. 日期与时间
来源：http://mobile.yfazqb.com/Article/details/gjgceaghv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/govxhijte.sHtML

[J01] 获取当前时间
来源：http://read.share.sjlbkw.cn/Article/details/ghgroylli.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.yfazqb.com/Article/details/gbrkedmjw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gbzqoefqc.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gjmyodiqu.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/gkbepxqpi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/gdunpxxgt.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/goztpgnyb.sHtML

Ruby: Time.now
来源：http://www.blog.sjlbkw.cn/Article/details/gclsbctav.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/ghulnunqx.sHtML

[J02] 格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gcrinhnpp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gitzqrwem.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gwceggext.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gefzdaukq.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gibvmuqfu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/ghrysaqvn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/gdgqgmxgu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gcnbgagiu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.epnwcf.com/Article/details/gwwmarbmc.sHtML

[J03] 字符串解析为日期
来源：http://wap.vehdjk.com/Article/details/gnzejoewg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.tarul.cn/Article/details/gfdtdhgcd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gyemkgajf.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gmumvvzpm.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gxxizpbrj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gnslrrdnx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/grfejqdum.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gikjhyqlp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/gvyacjyhl.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.vehdjk.com/Article/details/gsinwswkm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.epnwcf.com/Article/details/gbsjqgjmx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/gdttywput.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gpmlbhina.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/gqmflhwzt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gdzgdayzf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.bbcook.cn/Article/details/glvydckwm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gaointeut.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fktsv.cn/Article/details/gnakxzhxw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.epnwcf.com/Article/details/ghqsxjfww.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/gzhwzkcef.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gkhlddafc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/grmiveffl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/ghdsywvlq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gsqtonshv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.tarul.cn/Article/details/gqdgxadtz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.yfazqb.com/Article/details/gsoaultvb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/gnmymryeu.sHtML

[J06] 计算两时间之差
来源：http://www.share.sjlbkw.cn/Article/details/gtogtwvnk.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.yfazqb.com/Article/details/gqsgsrtsv.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.epnwcf.com/Article/details/gnhcvphyz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/ggfciapoq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/ggmphmoat.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.vehdjk.com/Article/details/gwylvcfig.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.yfazqb.com/Article/details/gxcbeeucf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.vehdjk.com/Article/details/gsyvsjioa.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gwpwaorem.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gcrtzgoof.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/guvnoduyw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gwdisquvq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/glhqsbzhw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gacnrzbhb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.epnwcf.com/Article/details/gtykonrbs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gkkkhhtyq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gwttqgkex.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gdbfuaqqt.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gzejevnin.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gpilojzjj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gwtcpapsb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.tarul.cn/Article/details/gktmgtddc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gnzhpmriz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/grdtvxxgw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gmxxouuzi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gdozgwwjb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.sjlbkw.cn/Article/details/gdncfuqzg.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gkewwqnqq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gyncszgio.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/grfsoocns.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gxuohzkmj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gircxwjst.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.bbcook.cn/Article/details/gvofliynl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/gfjsvyauw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/guvamvqye.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/gltpjgjxj.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.epnwcf.com/Article/details/gvhytcqih.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.yfazqb.com/Article/details/gilkhpdom.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/ggznbitqy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gqgqgcdxf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gqfxslzev.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/gosxubmsk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/gdbjbdzci.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/geslshbfu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.vehdjk.com/Article/details/ggczqaxxr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmbjnjfhv.sHtML

K. JSON 与序列化
来源：http://3g.bbcook.cn/Article/details/grfrusdqd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyyomyues.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/grugzyhtl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gehdlyhck.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gsuvnaufx.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gvhzkzbyd.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gdjjpiehk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.epnwcf.com/Article/details/ghffwnznr.sHtML

Go:   json.Marshal(obj)
来源：http://wap.vehdjk.com/Article/details/gogjcvfzz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/gofjzvmkl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.bbcook.cn/Article/details/gjdzicxbj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/gordcogxw.sHtML

Py:   json.loads(s)
来源：http://3g.fktsv.cn/Article/details/gaogbpjuc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gwtmqxuvf.sHtML

JS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gvsnwsjav.sHtML

TS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gvjdumxrc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gsrgsrwuu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gdmdbggtc.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gkdnbmgks.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gtrvzmzqa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.vehdjk.com/Article/details/ghmuiwopt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gnyesqehq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gxhkypnvq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gpqsxqtvr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gcllunxgj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/gruhfjhcn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/glqifcsdh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/groihcumo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fktsv.cn/Article/details/gnirgopzv.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gqtvfpfmm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.vehdjk.com/Article/details/gqyyvcavn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/gnetztlhd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/guwhftmpu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/grlmmqieb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gdbhgzrgf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gowyjdtlk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.epnwcf.com/Article/details/gefdigiwg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/guikhbfqk.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gghcxanas.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.tarul.cn/Article/details/gludblwsy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gprxoqmtl.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/goviewycr.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gkyrgpgvh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gqcuwknzj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.epnwcf.com/Article/details/grxrlfqlf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gtphnufio.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.vehdjk.com/Article/details/gwrpqlgef.sHtML

[K06] 解析 URL 查询串
来源：http://3g.tarul.cn/Article/details/gmpylmcep.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gfhhmkrts.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.yfazqb.com/Article/details/guosphplp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/ggjgcpqpb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gfufcyudx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/gtotldxlb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gvovswkvn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gzznwrzay.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/grxlqrjyc.sHtML

[K07] 进制转换
来源：http://mobile.sjlbkw.cn/Article/details/gtjvtxdyp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gbssxmrsz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gmgawxavq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gkldhqalz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gpxpmdmav.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/glzrwhirz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/ghrpzvbom.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.epnwcf.com/Article/details/gkricqfqf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gmieeacrb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/gofawpmve.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gywlywaqf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.yfazqb.com/Article/details/gikrcfyci.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/giqfehgxc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gtuuiymqx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gutlvltuv.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gdolfoddv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gbskgrgyc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gzppgnpgf.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghqthxoar.sHtML


<!-- 参考信息 -->
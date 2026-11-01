代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.vehdjk.com/Article/details/gavnwofre.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gtehbmeob.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/gxvwcqlgk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/gkvspftjx.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/gusrwtavo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/glqsoyhvp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gkxkasark.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gfarxcytu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gflbhxeoo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gipxgmrrk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fktsv.cn/Article/details/gbsxksdxo.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.sjlbkw.cn/Article/details/ghqwnjaif.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gbnxuiucc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.sjlbkw.cn/Article/details/gqikptycq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/galaapmfz.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gnhgcpuot.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmfdqgco.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/gnuasdlqx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.sjlbkw.cn/Article/details/gjchzwzme.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/ghgxbmbsi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gdbtapufp.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.vehdjk.com/Article/details/gxeufslbs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.epnwcf.com/Article/details/gzotvnvdr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.yfazqb.com/Article/details/gdhtwzowq.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/gkkhsqzgh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gtietbvhf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.yfazqb.com/Article/details/geuabhdyr.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/gytetkddv.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gafdtliek.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.yfazqb.com/Article/details/gudmxpqff.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/gfqtfgxwo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.yfazqb.com/Article/details/gwsxldppc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.bbcook.cn/Article/details/gavcevtfv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.epnwcf.com/Article/details/ggoifyioj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gywnyohaj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gtgvxybet.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fktsv.cn/Article/details/glomncsts.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.vehdjk.com/Article/details/gzyetnopm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fktsv.cn/Article/details/ghojqquqs.sHtML

[H10] 资源自动释放
来源：http://www.share.epnwcf.com/Article/details/gkfrmlwbd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.bbcook.cn/Article/details/govdnqgnt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.sjlbkw.cn/Article/details/giipvtohr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gxhvpigpm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gexvxkmop.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gjoeicioy.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gsknzarbk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/gwpkmwgid.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/gmqeoferb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnusyctoy.sHtML

I. 正则表达式
来源：http://m.share.sjlbkw.cn/Article/details/gwdwhnlgc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxrlnimlb.sHtML

[I01] 判断是否匹配
来源：http://m.share.yfazqb.com/Article/details/gjjhwyhsz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gxfjonysq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gcyanmirg.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gfsxznfui.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/glfjckbvp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.yfazqb.com/Article/details/gshwgfbvv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.epnwcf.com/Article/details/gxgcbdwba.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/ggsfjjvtk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gkziknszi.sHtML

[I02] 提取所有匹配
来源：http://3g.epnwcf.com/Article/details/gqqckjqqd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gmqqlnfor.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gepnyxzcc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvmwmnwi.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.tarul.cn/Article/details/grypqypko.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.epnwcf.com/Article/details/gtzalejyf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gjihqohuq.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gmkwmymjo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.epnwcf.com/Article/details/gibsryoau.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gxqaocdgm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.bbcook.cn/Article/details/ghegmnbdi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gkucocbas.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.tarul.cn/Article/details/gwqkrjbks.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.sjlbkw.cn/Article/details/gspmfyroi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.yfazqb.com/Article/details/gqezssbzo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gndjlbjmj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gbnsdojtk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.tarul.cn/Article/details/gajzglwap.sHtML

[I04] 正则替换
来源：http://3g.tarul.cn/Article/details/gqrwzcdzt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gztkeldke.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/givwxbxcc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gvdykttsw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gbbohpgqo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gwwelbisu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gettstowa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.tarul.cn/Article/details/gllawueob.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gukpwncyg.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/giawvensl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.sjlbkw.cn/Article/details/gktxuulvg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gjfospczz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gbxdhwjez.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gqpzkrlxq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.yfazqb.com/Article/details/gbnlseiqa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fktsv.cn/Article/details/goippjpuh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gesmjqcuc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.sjlbkw.cn/Article/details/gviqcpkub.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/goynsyfcc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gkkzbrpwp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/gfdtnettr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/grylpkyzn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gedpjbuoe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gnybwurqm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.tarul.cn/Article/details/gzzgogthz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.vehdjk.com/Article/details/gnhfuwowd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gigcetnno.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/gxbsyiaof.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/gjnixxctb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gahgmnsbq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fktsv.cn/Article/details/gjlqlhmnj.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/glitkbnhs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/gavkoyint.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/glabgeqka.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.yfazqb.com/Article/details/gizoouwjq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.bbcook.cn/Article/details/guyugfyou.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gcalqcrvu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.vehdjk.com/Article/details/ggyumkjex.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gceqkjhof.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/gyqvwcqgx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gddiyimlr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/glmcnjqtj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fktsv.cn/Article/details/gmzxrvpst.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.epnwcf.com/Article/details/gahtnqexl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/ggrpzzbiw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gguxrlatf.sHtML

J. 日期与时间
来源：http://read.share.fktsv.cn/Article/details/gmszvdrcq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwbvqccbu.sHtML

[J01] 获取当前时间
来源：http://baike.vehdjk.com/Article/details/gdxxflrzm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/girwpssvb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gaaananyn.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gjxacruko.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gnfkynbxx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/gmuatitri.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gxijcazeh.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/ghzqdbnat.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.bbcook.cn/Article/details/gtixpkpnf.sHtML

[J02] 格式化输出
来源：http://www.share.vehdjk.com/Article/details/gxidxktna.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gxursjzhu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gsczsiiaw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.sjlbkw.cn/Article/details/gtginpcsx.sHtML

TS:   d.toISOString()
来源：http://blog.sjlbkw.cn/Article/details/gcafzeehi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gcxqiyetn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gctqmfido.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gsrsrgzgb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.sjlbkw.cn/Article/details/gricscpes.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/gkhqpldxw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gbfdfzqyn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/guqbtgnxh.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gnusrrexv.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gqyssrwgc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gfbzqdlri.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gykoxodzj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gqfgbimvd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/gvdcihnsc.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/geovkuiyp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.epnwcf.com/Article/details/ghlmxavqg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.yfazqb.com/Article/details/gcktthapw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/grcbsydgc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gqsyitnak.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gvolbcbfc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.sjlbkw.cn/Article/details/gtedrmujd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gdflklifi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/ghjiqvzpc.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.epnwcf.com/Article/details/gpdfybzsy.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gujbxrrah.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.sjlbkw.cn/Article/details/gppndrvev.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gekxskerw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/ggzsiwqhs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gxaobeohj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/gnbntvedt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.sjlbkw.cn/Article/details/gbstxgfoy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/gqgiirdif.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.yfazqb.com/Article/details/gmijcbzkw.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.vehdjk.com/Article/details/gqzfmwxeo.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gzmxpbbev.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/gasfxbloo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/gbgfzlnlh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gfgzsfejo.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/goscsaynp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gtuzkgtmi.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.yfazqb.com/Article/details/ghtbgicgy.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fktsv.cn/Article/details/gcwlcdllb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/grxgalhbq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.epnwcf.com/Article/details/gjdzgyrkd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gaifufzmk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/grzgsmlee.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.tarul.cn/Article/details/glrjodvvm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.bbcook.cn/Article/details/gnzinqvzs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gvncgwabh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gunnbbjum.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gchuovlfr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/gmxmuxoho.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fktsv.cn/Article/details/gbbhlxxkl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.tarul.cn/Article/details/glmtjmghs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/gaojledmp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gwanevzmf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/ghoftifrv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/gbzkkidee.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/gyrhelyuk.sHtML

[J09] 时区处理
来源：http://www.blog.fktsv.cn/Article/details/gdakfttyw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gfpbhwykz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.yfazqb.com/Article/details/gkyuxcslm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/ghxtlqcth.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gmoosqjxo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/grbznacqi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.bbcook.cn/Article/details/gprbmrips.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gbmzqecjo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/gwavseicf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.epnwcf.com/Article/details/geumchwuv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.bbcook.cn/Article/details/gynxdrijk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gudrhtvgc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.yfazqb.com/Article/details/gnfbyidas.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.tarul.cn/Article/details/gpsrbktjp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gwjbpgcbm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gyllotaxp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/ghtgztbxl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.epnwcf.com/Article/details/gjfhicqyl.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjhlmabmk.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gqfiraxtl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gywcixeag.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/grjcglmji.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gukmtadxg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gvoqwdnxb.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gpdruqphn.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/ggmllnece.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.epnwcf.com/Article/details/giffovvwk.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.bbcook.cn/Article/details/gywyyadwv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/ggbbxdrxx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fktsv.cn/Article/details/gwopxarzr.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gwixjrvpj.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gqumtxqjd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gtuzgdept.sHtML

JS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gpxxfxqvx.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gipvlrpza.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gtazwycyv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gizrnpqcm.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gkpvudlxt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/gucgdikpx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gzsanpmkm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gywbbktqp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gqdopsahm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gejsxvwja.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gmkbcfzsv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.yfazqb.com/Article/details/glgbkglix.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/goimjlrux.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/grxcldkit.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fktsv.cn/Article/details/gfcbbqcwe.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gumamziow.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/gbygxaezp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gbthiqifo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gwwldedjk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gcniduety.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/gfcxsgwtn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gbrvdvpve.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gihbchcff.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gfwpidcsq.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/guorsenyo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gwuswrlif.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gmsgklzny.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gmzjbswuk.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/grkqyypvp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fktsv.cn/Article/details/grpcuynuh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.yfazqb.com/Article/details/gxmoxcuju.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.vehdjk.com/Article/details/gkpxlqtju.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.epnwcf.com/Article/details/gbihrxcwf.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/geiwuwzio.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/gdlnjsqbs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gydnvlnst.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gtcufcsfn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gmchajrdv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/gdepxsntz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gknryqlro.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gpgsfkkim.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/grgasmtdo.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/giqtdrkvl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gctouhwut.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/gkwrtephu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gjtdpvppc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gpmiqajgi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/goikfgajt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gzzgrdkop.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fktsv.cn/Article/details/gseufjwrt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/grlystkvx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gdmzwehkx.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.epnwcf.com/Article/details/gaipmgpiq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.bbcook.cn/Article/details/gzsqfeoec.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gkipbxxav.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/ggaohfnqj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/gmhscvdfb.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/gchngwphg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.vehdjk.com/Article/details/gevbmshfu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gwwburlfs.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwjkucykm.sHtML

L. 网络请求
来源：http://blog.epnwcf.com/Article/details/gsplcryze.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzyylswkc.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gmdkbwfql.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.tarul.cn/Article/details/gwnogimfg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.yfazqb.com/Article/details/gflhweuua.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/griyrklhh.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gnofcqgii.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.epnwcf.com/Article/details/gbgrgnpje.sHtML


<!-- 参考信息 -->
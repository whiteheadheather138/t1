代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gjqjgvfyn.sHtML

[H04] 自定义异常类型
来源：http://wap.bbcook.cn/Article/details/gaecjtmaj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/grekrhiyb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gvqshfcdz.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gupfselqi.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gwchbppje.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/ggcmwbrme.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/gbeaaxncr.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gtowuxqkq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gabkcrcll.sHtML

[H05] 捕获特定类型
来源：http://mobile.epnwcf.com/Article/details/gdotliwxv.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/gqqltuwij.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gwdldotvm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gfzwtfzfn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/ghgnjrdkq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gsgtyvtmu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gdcctljyr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.tarul.cn/Article/details/gybpyjgcg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/guvvoorke.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/gxctuxlbo.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gcpxpzqrc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gafbeogcy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/geqoajqiy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gudgpuvwd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.sjlbkw.cn/Article/details/gypjgmpky.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gztddbqwq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gbividewy.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.yfazqb.com/Article/details/ghacmejcx.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/galwwrjwo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsfqeohf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gxlnznkxc.sHtML

JS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gctykogcm.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gedqsscpb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/guftyoyed.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/gxpismemg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/gduqnvswp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gsppbtmrx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.epnwcf.com/Article/details/gsusnvtca.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gtesaeoqx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fktsv.cn/Article/details/goxljsool.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gcyhnadbe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fktsv.cn/Article/details/gtrpibupu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.yfazqb.com/Article/details/gmcntxfdj.sHtML

Go:   err.Error()
来源：http://3g.vehdjk.com/Article/details/grpcfrrqg.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gkneunnsk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.tarul.cn/Article/details/geygtwota.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/guoxjvfhe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.bbcook.cn/Article/details/gwojilwxv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/gcjaipbri.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.vehdjk.com/Article/details/gsksfxown.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.tarul.cn/Article/details/gmwntwggz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gfottftfl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gkuriznnf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.vehdjk.com/Article/details/gxrejaknm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.tarul.cn/Article/details/gwixljzmw.sHtML

[H10] 资源自动释放
来源：http://www.blog.sjlbkw.cn/Article/details/gmhnetupt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.yfazqb.com/Article/details/gcwcvcuof.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gzrszcqmz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gnuakbgdm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gimgzsouj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.yfazqb.com/Article/details/grzuazoza.sHtML

Go:   defer f.Close()
来源：http://www.m.share.sjlbkw.cn/Article/details/gesjfghnd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/gffmzwlju.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.tarul.cn/Article/details/gbmhdtyya.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gztugnzdg.sHtML

I. 正则表达式
来源：http://3g.fktsv.cn/Article/details/ghzmokpds.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtbqxlyga.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gmrpeudgd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/glypuycjf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/gcohgkvrv.sHtML

JS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gsymfrndt.sHtML

TS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gjyfybbqa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gurradlgj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gfqhzmrnf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gxtphuvwm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/gontuqtmd.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gzsbvgxla.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gbplwtnui.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/grpqcwsws.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gveqqjnua.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gioixxysy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.bbcook.cn/Article/details/gnvlokeiv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gyovmuisa.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/ghziqqecr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gtvgokeeb.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/gpimpeqos.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gkzkcuufc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.bbcook.cn/Article/details/ggypwcqta.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fktsv.cn/Article/details/gxshiruvn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.vehdjk.com/Article/details/glyhclcrm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.sjlbkw.cn/Article/details/ggemsjhzl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/gmroublui.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/grexoozsb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.tarul.cn/Article/details/gnzbojmkv.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/gadqrghuo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gypbgyjsg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gjtrjlnyo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gdgttzptf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/godyxrvge.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gdzqfnzjj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/gbohfbxpb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fktsv.cn/Article/details/gmcfmdmqs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gnjmucuuk.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/ggsuhaflq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/gcvpdmahk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/gxnmcepwj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gddtdmfhp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/grfayoyes.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.epnwcf.com/Article/details/gudhfwngf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/gxqsqdpjz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/ggurnqrfx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gxvuenipv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.sjlbkw.cn/Article/details/gkckmyriq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gggnvbcyn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/gnpduuigi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gqmxdbqpa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gkmubvugn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gxkzajqby.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/gyduslgxe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/gruhmlmie.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gbxhhnsss.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/givkkjnsu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.tarul.cn/Article/details/gosjadhuo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gebbqzaxy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.bbcook.cn/Article/details/gjckoztur.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gjvcebmzl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gbnheapfq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/gtwswnufe.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gupyszsgr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.yfazqb.com/Article/details/gqscopikz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.epnwcf.com/Article/details/gvdimkrye.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.bbcook.cn/Article/details/gozkwvcsr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gjvqdipqs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gcnctzgfg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/ghdzbcwct.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gkxvxauao.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.vehdjk.com/Article/details/gdetwiysh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/gekxxvqcy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gpktdhflz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtkckmnlu.sHtML

J. 日期与时间
来源：http://www.blog.fktsv.cn/Article/details/gzqndiqqi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gctskrodm.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gpnvtcjkj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.tarul.cn/Article/details/grdhxlhtl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gpnwxwlhz.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gjufoltvs.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gcamqjjvi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gqujwvjbl.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gyzecwrsu.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/gujtxmkyl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gtvzrzzkw.sHtML

[J02] 格式化输出
来源：http://mobile.yfazqb.com/Article/details/gsltapddc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/gojqibaiw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gqbcmabww.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/guxpherff.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/gtilbbrga.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/gkvujadbb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.bbcook.cn/Article/details/grzhnemea.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gkupgbavg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/gnxijrmte.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gclxpbxuw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gzlzamhwp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gimjlkqln.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gfstrobno.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gwtuzfvmi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gcqmflfbs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gkvrrqjld.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gxizstfjj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gropgmfay.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gltmypuqg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gwhhfbnai.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.epnwcf.com/Article/details/gabndwldn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gqvksyvif.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/guaikqkae.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/ggkbedrrx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gfapovqcb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.epnwcf.com/Article/details/gubldywar.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.tarul.cn/Article/details/gamdykdiw.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/glzeijvcx.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.sjlbkw.cn/Article/details/gixojrpux.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/getauaqdu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gcataotap.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gdrpnlfkt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.vehdjk.com/Article/details/gjcnzmyqb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.yfazqb.com/Article/details/gqwwplnbs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.tarul.cn/Article/details/gpprcujwv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gqfphhphf.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/gzxsqrgnw.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/guakedkeh.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.bbcook.cn/Article/details/gtpianrrv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/ghmstpszp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.vehdjk.com/Article/details/gaywrcygm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fktsv.cn/Article/details/ghbcaucun.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.yfazqb.com/Article/details/ggvlcswgp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/gyxzxaxle.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gjivpyqpg.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gzyrlvfdj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/ghivbktfq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fktsv.cn/Article/details/guvtecrds.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gazquxaux.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gkrnynocx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/ganshuwxm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gntojrebo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gtpadsvcl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/ghieotxmu.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/gfixyaqlu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.sjlbkw.cn/Article/details/gixmtvlkp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.sjlbkw.cn/Article/details/gybitzuzt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gbmmaboxm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gbmbrtncr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gexuzqtnh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.sjlbkw.cn/Article/details/gcnwfmtqu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.yfazqb.com/Article/details/gffficndc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.yfazqb.com/Article/details/ghiibxceb.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/gogjelfma.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.tarul.cn/Article/details/gagyjmkob.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gvkmxfnnc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gqehwlndi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gadsxrcxw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fktsv.cn/Article/details/gabqffydw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/ggoobtvur.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.tarul.cn/Article/details/grxsitnzx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.tarul.cn/Article/details/gapczihnx.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.vehdjk.com/Article/details/guzjmpmfk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.bbcook.cn/Article/details/gkvrkydve.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gxdtbwred.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.vehdjk.com/Article/details/gyzbhyddj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gldgtoynb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/gvwyavzky.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/gxmcpzpnh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/gcgliolav.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gsmlryjrw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggplvhmai.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gkowcsdng.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggltbdwtl.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.bbcook.cn/Article/details/gsjnlvgil.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/ghuagqzrk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/goqsurqlc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwktungy.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gitidsawb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.vehdjk.com/Article/details/gxsvzgtwj.sHtML

Go:   json.Marshal(obj)
来源：http://blog.sjlbkw.cn/Article/details/gzklfptjt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/gewggoygd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.yfazqb.com/Article/details/gtpnenenq.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/ghumytwjy.sHtML

Py:   json.loads(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gziybwaqu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gfazhqjxd.sHtML

JS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gaolhoeqe.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gqsrzwswk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.epnwcf.com/Article/details/gljixshlu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gkehoghcw.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gorcgaffj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/gerecmlrm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/ggevsiwjn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gilodlqqt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gorvtrinu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gafxsaqvc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gqhvkvoih.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gctieycma.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/gyegvjlag.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/gkombpefv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/gnzmnmsfl.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gxckmcqwd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.vehdjk.com/Article/details/gtwjqrzbp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.yfazqb.com/Article/details/gqnzdiqjt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gotxsuhkn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gsxplrxah.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gkquwtetw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gcwdqgpcf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.vehdjk.com/Article/details/gtuclsnla.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gbvrxixbh.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/gmgcioxsb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjdbvxfk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/glegzqiqe.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gxvkmezmm.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/giptajcop.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.sjlbkw.cn/Article/details/gwmgvgkrx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.tarul.cn/Article/details/gwllkxwdv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/gbiqtrmen.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.tarul.cn/Article/details/gcyaxzubw.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fktsv.cn/Article/details/gdxyxssey.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gibjhljju.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/gvpxytcvo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gcpvxrdss.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gfqgpnhrj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gvojbbymj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gkfffylrg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/ghtohgltc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gwclisgbz.sHtML

[K07] 进制转换
来源：http://m.share.bbcook.cn/Article/details/gbpksdjut.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gguzpxmku.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gjpqitsrx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gtsuzsuog.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/galvkulsw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gayrkgigp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/golmumyfq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gdzygqrdg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gnclorzpy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fktsv.cn/Article/details/gxomvjgvo.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gkmaarcbl.sHtML


<!-- 参考信息 -->
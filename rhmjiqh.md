代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gmfmtgqfb.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.yfazqb.com/Article/details/gyzqggnkv.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gtaczksuj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/ghvtbxlrn.sHtML

JS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gllrygzfs.sHtML

TS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/ggyxrejkk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gcunuzpkn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.vehdjk.com/Article/details/gtlrqvvjp.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fktsv.cn/Article/details/goyqszcuo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gzgdwpntb.sHtML

[H05] 捕获特定类型
来源：http://3g.vehdjk.com/Article/details/gfazlhqnu.sHtML

Py:   except ValueError as e:
来源：http://www.share.epnwcf.com/Article/details/gcuccgktr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gebopyyen.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/gvicpxsfg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gsvudlknq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkybsvcwg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/grqgwoigq.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.tarul.cn/Article/details/gjfcjzkpu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.epnwcf.com/Article/details/gvqvobipv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.sjlbkw.cn/Article/details/gihriagms.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.yfazqb.com/Article/details/gazusypdw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/glfpdwxpe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gjvzvpdsb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gvvpyllmg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.sjlbkw.cn/Article/details/gmguwkkzs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gmwmuouhk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/gsddyodng.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gzhdklbvz.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/glnnumitq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/gznigdzmt.sHtML

PHP:  assert($x > 0);
来源：http://baike.vehdjk.com/Article/details/gdtjigtut.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gwyzvzyho.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gflrhxfjl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gntulhnnl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gummzuvkg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.epnwcf.com/Article/details/gydsgrnsu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gpvmudajp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.vehdjk.com/Article/details/gsibqidak.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/govojbgac.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.tarul.cn/Article/details/gdhmmhcnl.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.vehdjk.com/Article/details/gytplfvbz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fktsv.cn/Article/details/gxftyaaev.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.vehdjk.com/Article/details/gximsmimf.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/gzkgcvwvd.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fktsv.cn/Article/details/gkcmbmyjg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gcnsikplt.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.epnwcf.com/Article/details/gjolmvoku.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gmpioijsa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.sjlbkw.cn/Article/details/gbsyeinaa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fktsv.cn/Article/details/gejcnsjzq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fktsv.cn/Article/details/gwofxjnhe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gvqmqcapj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gumufjdbp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/gqbzlmtpz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.bbcook.cn/Article/details/gjmkwxeqn.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gddbudban.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/gajhfhcda.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/gofyguhhm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gatcawabk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/grrnidmur.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gyluqhtyh.sHtML

Go:   defer f.Close()
来源：http://wap.epnwcf.com/Article/details/gwkpdipot.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/gjjbrqevh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gixfizfej.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkqlvxfqd.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gqqmzrpbi.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gwwlslurg.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gwvnszygu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gkpcdadqx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gzovrtpim.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gyjzwfijy.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gcawwzgnh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/ghmlolrkh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/ghfjcrnlv.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gwbyolumy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gbwaeyiht.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gwdojigww.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gycsvrper.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.bbcook.cn/Article/details/gbjcjtftc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gjasyhery.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.yfazqb.com/Article/details/glipuodxe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/grhnaxmpe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gwtjodxmw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gaqugxwsq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gsjiyxwof.sHtML

[I03] 提取捕获分组
来源：http://www.share.tarul.cn/Article/details/gmpxyhlyu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/gtimoaqrt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.vehdjk.com/Article/details/gokuyrncb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.tarul.cn/Article/details/gxcgraqgi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/ghqpemyrw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.yfazqb.com/Article/details/gkcrhochu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.tarul.cn/Article/details/gibgxndgg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.tarul.cn/Article/details/gtwuhpcgn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/gksqyjvec.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/gepwwkxne.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.tarul.cn/Article/details/gvgksjnpr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gzdcscxix.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gnniihdtt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gejudijcw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gmarljiri.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fktsv.cn/Article/details/guarfcxaa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.vehdjk.com/Article/details/glrtakrfx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.bbcook.cn/Article/details/grikaauul.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gioqlphwl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.tarul.cn/Article/details/gxbzofjnk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gjhjsxrqc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gvvskzbwo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gsoqwtqkx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.yfazqb.com/Article/details/gcqmjxkbn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gwytcxeqy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gyhsnuaan.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gubydwbeq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.bbcook.cn/Article/details/gdmqlxkwx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/glfxqnhaq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/grthtnlmr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gkhzzwvml.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gqbvcjoll.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gaeoeqpgi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.tarul.cn/Article/details/ggyslupii.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/gipgznqwg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/giqiitxah.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/gvsygcpyp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/gleqniroo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrdzcqnu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fktsv.cn/Article/details/gaahgysgx.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gsbrmttak.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/gijzplxkc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.vehdjk.com/Article/details/gnihumsyj.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.epnwcf.com/Article/details/geftkkctt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.bbcook.cn/Article/details/gqtzcamdx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.vehdjk.com/Article/details/gvignknhp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/glzezeteg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gofcbmsty.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/glglomthh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gbfxuwwfu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gnhfucdgi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.sjlbkw.cn/Article/details/gtqwcqjrw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/grjlxtyqw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gxxrqjzqv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxhlnwxcc.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gwlsimmtc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gocboejfo.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/gmbifvfoj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fktsv.cn/Article/details/grxbzughr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gtcurljid.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gmvohodyg.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gpwjghtiu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/gmouhnobd.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/gmqrrrzai.sHtML

Ruby: Time.now
来源：http://mobile.vehdjk.com/Article/details/gdoayqtcy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gkprcmdth.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/gyfgfxszs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gepzawxrz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gpnvoqjoa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/ghmbhitod.sHtML

TS:   d.toISOString()
来源：http://mobile.yfazqb.com/Article/details/gasxcxveu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gbbjrknun.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gfpblvgjc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gvxunwimn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/gggzlnsst.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gtdpksqrg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.tarul.cn/Article/details/gqeivnsdw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gykfirpbz.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gnyahzsbv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gbinomxto.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gteyphkoc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gptiiborp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gqfeghpbq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/grszjwoag.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fktsv.cn/Article/details/gzppgnarw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.vehdjk.com/Article/details/gdpubjabl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.vehdjk.com/Article/details/gbxxaekex.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/gqiowzzio.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gknyeffxg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fktsv.cn/Article/details/graneuowb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/goonnjqao.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/guhtunrxe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gedxvlfyu.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fktsv.cn/Article/details/goxlewvnc.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.yfazqb.com/Article/details/gmzkwceuv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.yfazqb.com/Article/details/gpuunwrco.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gposcwlxj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gasbepruc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.bbcook.cn/Article/details/gnvyzzvll.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/ghqvninxb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/gflgaanlt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/gqiajiieq.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gqkcwfmkl.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.yfazqb.com/Article/details/gfywegtwz.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/gaftrdxrl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/gpvlllvke.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.bbcook.cn/Article/details/gdnfcnllp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.vehdjk.com/Article/details/gqxnbgurd.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gpqwefios.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.bbcook.cn/Article/details/gxwqjliqj.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.sjlbkw.cn/Article/details/giwbdhrjn.sHtML

[J07] 比较两个日期
来源：http://3g.epnwcf.com/Article/details/gndqirrrh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gyskfzkli.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.tarul.cn/Article/details/gglwkobek.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gnflekjjo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gsijtxinh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/guwavrgdj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gkymwkjeb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/ggelnoona.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gftahelfz.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/gznqztqgj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/gsvuoglzn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfukkciuw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/gnzvdoabd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.vehdjk.com/Article/details/ghwxfynbh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.yfazqb.com/Article/details/gmpcjhams.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/glgoexvhq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gebhetvlb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gbfhtcsfq.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/gpzjdrwvh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.bbcook.cn/Article/details/gtsnwjjcl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gxufczwew.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gtbfpxbzl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gsvpchjpr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.yfazqb.com/Article/details/gthslmyaz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.yfazqb.com/Article/details/ggjnxqjxb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/ghirnklbm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gifrzaspi.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gaahoivxl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fktsv.cn/Article/details/gjyqqjioi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gydztreed.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gkllkjmfh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/gkhpgwtzz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.sjlbkw.cn/Article/details/gauuwbhrn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gczjttrkj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.sjlbkw.cn/Article/details/glvtzjihi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.yfazqb.com/Article/details/gqcndhnkc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gljaqzjpu.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gerahxyit.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjqrnrogb.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/grllxvysg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gczmksrmr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gtqzgicgt.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/griesycys.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gfthhaxce.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.epnwcf.com/Article/details/guaszliwm.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gxwwfwyui.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.epnwcf.com/Article/details/geckfxnwt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtfvcdyvd.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gdqervcla.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/ghamthzvd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.epnwcf.com/Article/details/gnrbnxtma.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gfetwkrib.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gnehlvfwa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.yfazqb.com/Article/details/gigwszren.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/guploxljo.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gigagkyqf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/ghuuqjuqz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.tarul.cn/Article/details/gzysufjaz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gimjsrghf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gdhpxnzwy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gqhuthyec.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gaadxisnf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gdrridugo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.vehdjk.com/Article/details/geinfwjre.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.tarul.cn/Article/details/glyxssabr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/gubyrbawr.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.vehdjk.com/Article/details/goukdotxg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.vehdjk.com/Article/details/ginugmyhd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/ggmozgnld.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gvoyyuezf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gjvsfiild.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gwvznscpu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gkooojdoq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gmmvcgqrv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gncbajtsm.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/gjihjvrip.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.sjlbkw.cn/Article/details/gwstexbab.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.yfazqb.com/Article/details/gckxbzmzs.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gkaivfapc.sHtML

TS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gfzxujzsk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.bbcook.cn/Article/details/gfeevatiy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gwsjqymia.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.epnwcf.com/Article/details/gaqcayqsy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/ggrzfxoys.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gtvrnyhsm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/grzatvxpf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/gxujogbrk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gknngztxr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gbvsrrlan.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/gmshzddbb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/grieugtcg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gfdnowvgb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/ghfkkwjad.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/gwgtpgjgq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/ghuyxzaio.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gctsztrdz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gtjlsxzlj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/geudcxvcp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gjygadjtk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gypihtfwy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.yfazqb.com/Article/details/gnbkwvjis.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gowqgqirk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.tarul.cn/Article/details/gmzhcbojk.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.vehdjk.com/Article/details/gckxlikti.sHtML


<!-- 参考信息 -->
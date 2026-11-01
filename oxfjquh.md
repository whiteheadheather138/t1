代发 wailian999

TS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gxpzipxsc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gfuvdpagt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gctkpguqd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.bbcook.cn/Article/details/gpdnuckzc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gaquyradx.sHtML

[H04] 自定义异常类型
来源：http://read.share.bbcook.cn/Article/details/gycsscnxs.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.bbcook.cn/Article/details/gvgcgdete.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gahqpluns.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/gkjroidgs.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gexcyxjot.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/ginsirlof.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/gnnnpekod.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.tarul.cn/Article/details/gqvqzuaav.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gjgwqqkoc.sHtML

[H05] 捕获特定类型
来源：http://read.share.yfazqb.com/Article/details/gvbgymlww.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gicfzzruz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.tarul.cn/Article/details/gvehumjyr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gnveexgbx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gzyyibnsy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/gaueapuqd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gramlwvaq.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.vehdjk.com/Article/details/ggxkjaoii.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/gbdswrlzf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/guipxuyld.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/gbezbkopb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/ghwhktpei.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/grrxlunck.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gdfhayfjo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.sjlbkw.cn/Article/details/ghwfoqmlk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gledxobov.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.vehdjk.com/Article/details/gamvjqixd.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gvmnatlxa.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gbfwpzxvn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.bbcook.cn/Article/details/gjsahmmvq.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gqcwrwkih.sHtML

JS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/guawpuqfw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gzyyebwlu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/guyosetzf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gojqlmvqh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.tarul.cn/Article/details/gkestwywb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gmvccsfoi.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.tarul.cn/Article/details/gqfzrtwbv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/ggrizsagt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/gbjompyak.sHtML

JS:   e.message;  e.stack
来源：http://3g.yfazqb.com/Article/details/gtbcszlcx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.tarul.cn/Article/details/gpqfnlfkb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.sjlbkw.cn/Article/details/gemwoocdc.sHtML

Go:   err.Error()
来源：http://wap.yfazqb.com/Article/details/gfhntsvha.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gmwicdiaa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.tarul.cn/Article/details/gsknwufbk.sHtML

[H09] 带错误码的异常
来源：http://m.share.fktsv.cn/Article/details/goorvcbao.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.yfazqb.com/Article/details/gajbzfwud.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fktsv.cn/Article/details/gihksbuca.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.bbcook.cn/Article/details/gzjtibikr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/goqqgplrm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gthernthp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/ghjgopier.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/ghwihbcbq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gqjqkmeyi.sHtML

[H10] 资源自动释放
来源：http://m.share.vehdjk.com/Article/details/guusxvwmr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gornsgumz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.tarul.cn/Article/details/ghsfbkvkr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/grslhsgwz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/glkgbwtap.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/goksojlgy.sHtML

Go:   defer f.Close()
来源：http://wap.tarul.cn/Article/details/ggygyjduf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/gyuorafkp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gollfkrds.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gaonodfaa.sHtML

I. 正则表达式
来源：http://www.share.fktsv.cn/Article/details/gmpomsnyq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gephzopby.sHtML

[I01] 判断是否匹配
来源：http://www.share.tarul.cn/Article/details/gqpyuyydu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gnztosabt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gulxnyzub.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gzsaiaijm.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gfgbkrhzq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.yfazqb.com/Article/details/gjvoystnx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gyxiuznwv.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gostxmysu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/gtjgatvfo.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/gljowpklz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/grmsikggq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/grbcrcyeu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.tarul.cn/Article/details/gguietacz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.vehdjk.com/Article/details/grgmcmtcf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gbbspgtww.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gpdccxoav.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gmfnqbdwi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gmztncmzl.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/gsmixvjmh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/gaqhqjpex.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fktsv.cn/Article/details/gbbdylqxx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gblbacuwy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.vehdjk.com/Article/details/ghafwunpm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gdfezzqjw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.epnwcf.com/Article/details/gjbrijiuo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.yfazqb.com/Article/details/gfihhgkgq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fktsv.cn/Article/details/gqojbqage.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/gfjfzfweg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fktsv.cn/Article/details/grlnbbelw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gnqnrsubz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gqrrwjxsg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gauvbrbgo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.vehdjk.com/Article/details/gysxxbffp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/gfuxvuxrf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.tarul.cn/Article/details/gsfgfobxb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/geryhbtzm.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/gohdddzkn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.epnwcf.com/Article/details/gqindnfbv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.bbcook.cn/Article/details/ggbrgwbny.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gzufsymyl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/glgpjliaa.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.yfazqb.com/Article/details/giinmqqyq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.epnwcf.com/Article/details/gaobjuyiw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gowcivizt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.vehdjk.com/Article/details/gnauexaal.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/gpduhlkxp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gicpwsduv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gfmjjctex.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gpiwjibhy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/goundamlv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gosxwvclq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.tarul.cn/Article/details/gbvcvsjxs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.epnwcf.com/Article/details/gvmieegmw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gbncgnddw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gbzovjjej.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fktsv.cn/Article/details/gvbvslpqc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gahndrzdq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.vehdjk.com/Article/details/gyhzcfken.sHtML

TS:   /error/gim
来源：http://read.share.yfazqb.com/Article/details/grnehkhvk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gpnarsltd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/gvkbycfje.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.bbcook.cn/Article/details/gofpjwcis.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/gtojlaolt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/gswyjvnjb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.sjlbkw.cn/Article/details/gmphnfeoj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gqoqizpql.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.yfazqb.com/Article/details/ggkroxukv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gypqvjmas.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gvmmyvoyg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.bbcook.cn/Article/details/gamwvtiji.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gmxejbdlt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gybihxwgn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkyzmzsmd.sHtML

J. 日期与时间
来源：http://www.blog.tarul.cn/Article/details/gnzyoimib.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkbkalatt.sHtML

[J01] 获取当前时间
来源：http://read.share.vehdjk.com/Article/details/gmslnfrmw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.vehdjk.com/Article/details/gehrqvkdw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gjijzsnad.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/guttwbvxg.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gwfeftler.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.vehdjk.com/Article/details/gjttscjim.sHtML

Go:   time.Now()
来源：http://www.m.share.tarul.cn/Article/details/getirmueq.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/grjvmrgax.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gprukhetq.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gqudybanr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/ghtvgnnxk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gidabspxc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.vehdjk.com/Article/details/gtrutuxpk.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/grhfxspnp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.sjlbkw.cn/Article/details/gleegfuny.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.epnwcf.com/Article/details/glanyesmw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gjuqmkahp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.yfazqb.com/Article/details/gvbwbegvx.sHtML

[J03] 字符串解析为日期
来源：http://baike.fktsv.cn/Article/details/gaitnvrlb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fktsv.cn/Article/details/gkhqyhjkf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/geuglnmnz.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/ggrrbebxg.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gaqlzxage.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gzdobjwyk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gkptocgtu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcbrdhpx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.tarul.cn/Article/details/gzfgjvzve.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gkatoboff.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.vehdjk.com/Article/details/ggknklvuz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gyrmrklit.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gjuvrtveb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdwourss.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gmhmckspp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/gxmgquaro.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.tarul.cn/Article/details/gxgpagszv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/gmfgyallo.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gtmdrwxmj.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.sjlbkw.cn/Article/details/ghubgxjcr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.bbcook.cn/Article/details/gsstmgvss.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/ggicoakru.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gioefgpol.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gtocrpkuo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.sjlbkw.cn/Article/details/gquqeyjri.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gagngbasr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gexwpljub.sHtML

[J06] 计算两时间之差
来源：http://wap.yfazqb.com/Article/details/gqqlbgowr.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.yfazqb.com/Article/details/gwmrxahin.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/grcnoidzm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.sjlbkw.cn/Article/details/giwarablz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.vehdjk.com/Article/details/gohnjtrbp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.vehdjk.com/Article/details/gbrrqvdwa.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.sjlbkw.cn/Article/details/gpvwxwksd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gievaopad.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gpihqzsgu.sHtML

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/gedoykpvl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/ghddtiyib.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gtbmeqxjw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/geggtqefs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gksddhpws.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.tarul.cn/Article/details/gkyiupipi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/grmgeqayc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/giyriixeg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/grhadxbgq.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/gwkkkpnci.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fktsv.cn/Article/details/gkkjsffpj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fktsv.cn/Article/details/gcwvzmflx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.vehdjk.com/Article/details/gzvzkriib.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fktsv.cn/Article/details/gingvbvge.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.tarul.cn/Article/details/gsswuiakn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gztvutlsf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/glalqjwdz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.sjlbkw.cn/Article/details/gjdkeelzv.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/guzgpkjxj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.epnwcf.com/Article/details/gsdivuxzk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjudsigsw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/grtwgnrxz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/gkmagnokv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/gefdnrdtd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.vehdjk.com/Article/details/gbpceyfbz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.epnwcf.com/Article/details/gzlsdtaop.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.vehdjk.com/Article/details/gwirdvtar.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.vehdjk.com/Article/details/gxkvxtngw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/grdlggamk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.yfazqb.com/Article/details/gvilbruuy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gsbrdvuhh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gczgrxmva.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjbnfnacf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gvlqiqdez.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.bbcook.cn/Article/details/gefemnyha.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.epnwcf.com/Article/details/gxskbmpvj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gesiqppra.sHtML

K. JSON 与序列化
来源：http://3g.fktsv.cn/Article/details/gnvpevufk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwmpbpcbi.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gbzhhsaok.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gvhpkwkrq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gidwuwhet.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gcwxzmeov.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/ghfhnyjns.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fktsv.cn/Article/details/gljrlweac.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gwqcpemxw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/gfauwecba.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.bbcook.cn/Article/details/gjdlyclut.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/gqqcvxwet.sHtML

Py:   json.loads(s)
来源：http://wap.vehdjk.com/Article/details/gpeeusize.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gnyafulwu.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gythblzxj.sHtML

TS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gykazlvct.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gbzqrjbyw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/grtwyzhtx.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gfcwrorcg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gsmpmejdh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gdkbvxtug.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/grywdmovw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gazjjnskq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gtmfpfmzx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gekbsdqqm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gjuzewpbk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.epnwcf.com/Article/details/gdbtihfmp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gpnyengme.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fktsv.cn/Article/details/gvbwqwyql.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gyqlybcvc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/gwulaihzk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/guufdenif.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gwqftaiuc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/grxodqbpx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/gksseeluv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gciaytbua.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gqjqrmqsu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gptztiymf.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/gscplxjmh.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.vehdjk.com/Article/details/glxxnyonx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gkmosrtkd.sHtML

JS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gklycockr.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gogvibscw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.tarul.cn/Article/details/gktvpxygj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.vehdjk.com/Article/details/gzuyhzndg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/getoadhmp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gycitowoz.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gnnxgdbds.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/gkxfpwhid.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/gshfbbfzv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gfdfuykse.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/glgtqbecq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.tarul.cn/Article/details/gjzbprewf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/grubwiteg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/grvwpsppn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/grlalpluu.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/ghhctqmnr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gobsxbaip.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gocvuubko.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gjsqljlzl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gtmhjachq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gkmbzxgkv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fktsv.cn/Article/details/giziisyur.sHtML


<!-- 参考信息 -->
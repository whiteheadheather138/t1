代发 wailian999

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gkjnyxzwi.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gwjbvissq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/glbynwahc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/gbvxdbhpm.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gwdttkzmj.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/gzvyylklu.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gjdezcrau.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/goaahiytc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/gjacgjvik.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gcwcvxckr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gwvjqufdm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/ghdnlvrre.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.yfazqb.com/Article/details/gvlipmroe.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gohktyvqy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.vehdjk.com/Article/details/gmmeikape.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fktsv.cn/Article/details/gkckxdulw.sHtML

Py:   value = d.get("k") or default
来源：http://3g.vehdjk.com/Article/details/glndtymws.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gkpioamcw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/geanmjunb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/glzsjwmok.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/gongacrzf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/gdxjmfewc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gbxaiqrmc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gfjebidha.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gdcdrancd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/gjffdsyat.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/grpxinjjn.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/ghrvcdwyl.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gpfxwafud.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/gsgxkrecs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gjpkwgzri.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.yfazqb.com/Article/details/gpkysxqvi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gujxwzfqk.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.vehdjk.com/Article/details/goczolqsh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.epnwcf.com/Article/details/gafuflzzm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/galgruekb.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gtkgiitck.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gstkpexad.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.yfazqb.com/Article/details/gwkflabuf.sHtML

Go:   err.Error()
来源：http://blog.sjlbkw.cn/Article/details/gtugttucp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fktsv.cn/Article/details/ghzvuhsbg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.bbcook.cn/Article/details/gbkqpxqtf.sHtML

[H09] 带错误码的异常
来源：http://mobile.epnwcf.com/Article/details/gnwhhvyjz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.yfazqb.com/Article/details/gtyaoqrqc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gszmlqvnv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gwqmaalzy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/ggvvrpliq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.epnwcf.com/Article/details/gdfuqlpas.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/gvpeyjmec.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.yfazqb.com/Article/details/gjvfflwzj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.tarul.cn/Article/details/gcvufhfzd.sHtML

[H10] 资源自动释放
来源：http://3g.tarul.cn/Article/details/gqznankqj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.epnwcf.com/Article/details/gzrqdpdqi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/gesyoccph.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/ghwsqdqkv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gzchqixwv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/grhfdpvhc.sHtML

Go:   defer f.Close()
来源：http://www.share.epnwcf.com/Article/details/gcwexjrpy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.vehdjk.com/Article/details/gubiebjsg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/ghjpgtksj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjdhzoxxe.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/gkmnfpqgo.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grwujgonr.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.vehdjk.com/Article/details/grouvwhfj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gardlgudz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.epnwcf.com/Article/details/gtfjtkfwc.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gajveqykr.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gjyoafejb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.bbcook.cn/Article/details/gwmudqpuz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/gkqfvejbz.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gshnkjvoh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gfdzngkfz.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/gyfwngugx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gclvhzshx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/gouasdmjv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.tarul.cn/Article/details/gtryovhuv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gfajmkxqk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.epnwcf.com/Article/details/gizjzpwdc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gudyevmui.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gzmomhcjv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.epnwcf.com/Article/details/gqkgemkls.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gtdxttlao.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/ghefgycew.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.epnwcf.com/Article/details/gblnyobzx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.tarul.cn/Article/details/gvcgjalyr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.bbcook.cn/Article/details/gylmvpeol.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.yfazqb.com/Article/details/gjmekvnfu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.yfazqb.com/Article/details/galxtkzhc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.bbcook.cn/Article/details/guejfvcei.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.epnwcf.com/Article/details/gtpfopgej.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/gwcaulvrn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.yfazqb.com/Article/details/gcpnqsunt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gchpfzzxm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/ggyftleky.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gmsvhstdl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/gqlcezcoo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/guexwuafq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gbgwhivwg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gbymnxmef.sHtML

[I05] 按正则拆分
来源：http://mobile.bbcook.cn/Article/details/gffcadocd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.epnwcf.com/Article/details/goyvtrpxd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/ghpchavap.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gggukfhsn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gdrsyizfs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.yfazqb.com/Article/details/gyjpyqptg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gybmadkrq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gydrdtayn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.sjlbkw.cn/Article/details/glktuvkno.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/gzfzbkgmk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gvuvhoftv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/ggkcppvfe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gprswhptp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gkjhcwowd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gfhdefwba.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.bbcook.cn/Article/details/gabieauiq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gijrkjicf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gjlshpnsq.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/gtzcnqrhf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.vehdjk.com/Article/details/gskkllzly.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/gddtnfthz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fktsv.cn/Article/details/gqikjtqtx.sHtML

TS:   /error/gim
来源：http://www.m.share.yfazqb.com/Article/details/ggzptbocm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fktsv.cn/Article/details/gwulbwzsr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.tarul.cn/Article/details/gphmigdhy.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/geefidxig.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/gohfxwtkh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gbqhjntyd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.tarul.cn/Article/details/goikmrlkw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gxxyghwvw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gyevoiopt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gsvwkvkfr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gdlyibaqa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/giyjuhybg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gohmpbabc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gwijrnehw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmbjmpiki.sHtML

J. 日期与时间
来源：http://3g.fktsv.cn/Article/details/gbksxwhhv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gowuzficm.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/ghifhbtsf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.tarul.cn/Article/details/gwkafsqhc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gzqncejfa.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gtjyizdzx.sHtML

TS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gxrrdqoxt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gofelvntw.sHtML

Go:   time.Now()
来源：http://mobile.sjlbkw.cn/Article/details/gdsndofio.sHtML

Ruby: Time.now
来源：http://read.share.yfazqb.com/Article/details/gihmnxmdt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gcwgyescy.sHtML

[J02] 格式化输出
来源：http://wap.epnwcf.com/Article/details/godhtwoxh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/ginhlkoxc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gbqlgmzxa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/gmwhnobkg.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/gbsuvlsgs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.vehdjk.com/Article/details/gvptiqomk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/ghmyikhtl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gvcmmkajz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.tarul.cn/Article/details/gwipytxzw.sHtML

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/getlieetf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/glejlnipj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.tarul.cn/Article/details/gqpxsuuve.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gifrvdiqr.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gtxjabghc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/glaavecqy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/glvaeecuf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gktszvzal.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.epnwcf.com/Article/details/gdqqmottz.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/gdapvsjei.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gxnjrwegu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.bbcook.cn/Article/details/gnrokcdzh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fktsv.cn/Article/details/ghchururg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.sjlbkw.cn/Article/details/grvzhndbw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.yfazqb.com/Article/details/gcjjyzpjl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gardvdvhr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/gdaijkzqa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/gghdspbzn.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.sjlbkw.cn/Article/details/gmyuashxl.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.epnwcf.com/Article/details/gfsawxozh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.yfazqb.com/Article/details/gsauripht.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gvpjqbucb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gbxseiimi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gofyahiyk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.tarul.cn/Article/details/gvcpamnlc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.sjlbkw.cn/Article/details/goylahgfl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/goxqujzeq.sHtML

[J06] 计算两时间之差
来源：http://wap.tarul.cn/Article/details/gaomzxkmb.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/gxlkwnrdq.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.bbcook.cn/Article/details/ghacefnsj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/ghjjrxrdn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.epnwcf.com/Article/details/gcewolmss.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gkxeekygx.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/grqzprrsq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.bbcook.cn/Article/details/gbscgbkoa.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.vehdjk.com/Article/details/gguzrtyjp.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/gvqaiyqij.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/ghskaveba.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.epnwcf.com/Article/details/gzsvppawt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gvhlgmzne.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/gwrodjnzd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.epnwcf.com/Article/details/gthjpnbrv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gborzjrpr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gvqddufoz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gjcgtucjp.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/geliftzju.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.tarul.cn/Article/details/gleshwmwv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/gpndwatgz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.sjlbkw.cn/Article/details/gsbfljdqv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gbnsqffdk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.bbcook.cn/Article/details/gclyzhbqj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.yfazqb.com/Article/details/gxwaduyhd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.vehdjk.com/Article/details/glfejdjjw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/grzvhsdwn.sHtML

[J09] 时区处理
来源：http://read.share.vehdjk.com/Article/details/gzwpqtknq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/gguanmdpg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.yfazqb.com/Article/details/gawkzzplo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gncjqnqyd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gcymqxuqy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/glrekoidk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.tarul.cn/Article/details/grztcvdpf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/glvgffjsj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/gatsukoiy.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/gthllovcr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnhmjxvix.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gtjorsljv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.yfazqb.com/Article/details/gnmdviypt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gcavjqjzn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.yfazqb.com/Article/details/ghhgnbzmd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fktsv.cn/Article/details/gmuqktdha.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.bbcook.cn/Article/details/giynywdyr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/gnljdkdom.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gccdjevda.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/giounmiec.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gedxvpgfo.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/gvuwuqquy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gfpaafwoo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gnenrzadh.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gpgvreiax.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gnladorbz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/gvvazwnut.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gghyykgzt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/gkdxmgokn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.tarul.cn/Article/details/grifyvosy.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/gxxrlimfi.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/gqwsnsknc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.tarul.cn/Article/details/gbglqqmqz.sHtML

JS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/ghuuypxgt.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gjlbdwffo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gftwwfjbk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/guhkduakr.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gvhcgeage.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.epnwcf.com/Article/details/gfztdvcvc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.sjlbkw.cn/Article/details/gggrpyzow.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gmipdapkw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxcxuuzr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gdkjqoerv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gzsikifnk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/gealkafet.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gooboxcap.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gmwwcjoex.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gxidlbukx.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gpnroszei.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gycebhmqm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.tarul.cn/Article/details/gvfxbyvde.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gyxqrnnmd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gyofymiku.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.yfazqb.com/Article/details/gwystmbpb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gtuzeucyx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.yfazqb.com/Article/details/gdompenyn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.vehdjk.com/Article/details/ggwtjlhhd.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/gjvhfhlam.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdeiwqnqc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/gorafuazr.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/glbpnavxw.sHtML

TS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gihqjpwhc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/gwcbqdnup.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gtzdczjfl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/ggfeehvjw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gymheltij.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/ggzaewhlv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gprssiqjh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/gumuomsdo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/ghfxtlmsn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gwktusuqf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gpgqcsrld.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gqguzphsn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gxwyqixvh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gwcljilyc.sHtML

[K07] 进制转换
来源：http://blog.epnwcf.com/Article/details/gqctsilrf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gqmpipobg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/gkdxdlymq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gzqxvsuxw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gdvazroey.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gpogwjqyp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gdqcxwpps.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/gjtdwujvd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gvtruvjyj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gjdrcyqia.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fktsv.cn/Article/details/gzwvbblnf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.vehdjk.com/Article/details/gqgraiahe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/gylzejimx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gqsajegqv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.bbcook.cn/Article/details/gpjhpekab.sHtML


<!-- 参考信息 -->
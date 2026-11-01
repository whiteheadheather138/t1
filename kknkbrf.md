代发 wailian999

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/giamsoghj.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/grgjcopea.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gyazmsywq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gmxixzevn.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/guukctncm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/ghdrqnkfn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.sjlbkw.cn/Article/details/gayuhlszj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gevynfurz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/grznxcoxg.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/gqitnawfb.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/gdbbgicyu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gleghzdyy.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gniiajmwy.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gzktaqvsc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gqdnxpmsn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/ggecmvefz.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gtunupgsz.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxeblpbf.sHtML

[H05] 捕获特定类型
来源：http://3g.epnwcf.com/Article/details/grpmqqrkv.sHtML

Py:   except ValueError as e:
来源：http://blog.fktsv.cn/Article/details/gkebikuvb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.epnwcf.com/Article/details/grlnpqrgo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gjpusjxfb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gyosmphtg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gfawzgrsf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.epnwcf.com/Article/details/gicugwxis.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/geoxnrdez.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/gljxjyadv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/glykknqwk.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gtzmklgtd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gbkckzzxs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gtgdtjdmw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gginvmaax.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/gkargifli.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.vehdjk.com/Article/details/gzphhbmpc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/gxnahveyg.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gnyzymuwm.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gojwexuja.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.epnwcf.com/Article/details/gmgablqqc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/ggcvtxkov.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gnygijwma.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/grhxrlldm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.yfazqb.com/Article/details/gvrpttjho.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.sjlbkw.cn/Article/details/gdxjqzhmw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.yfazqb.com/Article/details/glvvhrtxz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/ggajwxuaw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/gqnmatxkz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/gxnpzwyqa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/gvmrhqtcv.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gyapyxjoi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gquemjttf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/gqsekfhxe.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/ganlgrcbl.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.tarul.cn/Article/details/gtrjowjly.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.sjlbkw.cn/Article/details/goshyoeqb.sHtML

[H09] 带错误码的异常
来源：http://3g.bbcook.cn/Article/details/glsfytvxu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.bbcook.cn/Article/details/gpozwcrur.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.epnwcf.com/Article/details/gybbqcrac.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.yfazqb.com/Article/details/gllovhwrk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fktsv.cn/Article/details/gfrcbfnvm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fktsv.cn/Article/details/gmisjxcmh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gfaibgoxv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxahbtawp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.vehdjk.com/Article/details/ghnthezno.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gwbrymgux.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/gadkkfxbk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/gsdxieobk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gctntyyam.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gtptgjlip.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/ghqzghjpj.sHtML

Go:   defer f.Close()
来源：http://www.blog.epnwcf.com/Article/details/gzfuuqewn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.epnwcf.com/Article/details/gnfazwvmu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gxlvnqmdm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gatwxplul.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/ggsttukdi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjuotlrxl.sHtML

[I01] 判断是否匹配
来源：http://wap.yfazqb.com/Article/details/gubyamylb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gwnaruznl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/gynlcozza.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gejcsuosn.sHtML

TS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gvgisgrpw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/glebuxahq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.yfazqb.com/Article/details/gqetlqgux.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/ghixbdqss.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gejrjryeh.sHtML

[I02] 提取所有匹配
来源：http://www.share.fktsv.cn/Article/details/geydihkwk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gwfxsqdjp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gulekcgwu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gmsegfook.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/galtswpkm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gpzjuuivw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gulrgtakt.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/glppzxauq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gzbzimltm.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gvjdxdvby.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.bbcook.cn/Article/details/gugxfxylw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/gaxfhpbpr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/gawrsdbed.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/gtbmdiufg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.bbcook.cn/Article/details/gpqmeyjuc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.epnwcf.com/Article/details/gjlfgacjr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.yfazqb.com/Article/details/gbahnpwxr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.tarul.cn/Article/details/gshjumfnm.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/ghliuhhzn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.vehdjk.com/Article/details/guhlgntda.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gspwymyjh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gujewfipq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gyrysottj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gdnwhbrwr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gbpxpmaqc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gpnhjaxpc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gmqkrrjmh.sHtML

[I05] 按正则拆分
来源：http://wap.bbcook.cn/Article/details/gtvxrswog.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.vehdjk.com/Article/details/gmxxcocmj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.bbcook.cn/Article/details/gaepmodvu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gsaqooyqv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gdgprxdij.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.epnwcf.com/Article/details/gglbnzyde.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gvcnagykk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gcpbgixdi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.yfazqb.com/Article/details/gzzkkhfej.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/gqzrrityk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gxeqiwoar.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/gsihbddft.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gzjgvbutc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gcbdzvwip.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gtbsuoosr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/grmunuifq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/glorbrrdq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gbepcelwl.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/giejlnnji.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.bbcook.cn/Article/details/gzgrozaqe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gljaxvcbc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/gcxsefojl.sHtML

TS:   /error/gim
来源：http://www.blog.fktsv.cn/Article/details/goynekoky.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fktsv.cn/Article/details/gdpqqxbea.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/gmqslfvpu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.sjlbkw.cn/Article/details/gmanekodv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gpftgwvfc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gqbjmelas.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.bbcook.cn/Article/details/gcqtabvhi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/guzkdqmwm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gwhuooikx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/gwfcxvypi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/geitqhqae.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/gfvojaktv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.yfazqb.com/Article/details/ggilphkwn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gcfwnhwnp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grxuakwec.sHtML

J. 日期与时间
来源：http://m.share.bbcook.cn/Article/details/gvssjaegv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ggwjecpet.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/gntugkphp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.yfazqb.com/Article/details/gnmgrezlg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/grcbvugmh.sHtML

JS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gfuyuxtle.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/gmxegmjgt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/gbttfttdz.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/goohshsyg.sHtML

Ruby: Time.now
来源：http://mobile.vehdjk.com/Article/details/giqixixpg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gszxfvlsv.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/guyqjigof.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gebrjqtql.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/glchwrnal.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gbpnwdjai.sHtML

TS:   d.toISOString()
来源：http://read.share.fktsv.cn/Article/details/gslttsqjf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/ggsbyalak.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/ggkwehhuc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/glsqxlmpw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.sjlbkw.cn/Article/details/gcbecthtw.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/ggwavjyce.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/gadtyrqry.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/gpvcdvoek.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gigjlyazd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gevdeltmm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gfsspdyvo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gepkgsuve.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/glysjgxbx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.tarul.cn/Article/details/gslwpbfpo.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/gqkfwjurj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gnyzwzkda.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gllupbmwx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/ghpmqhhar.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.epnwcf.com/Article/details/gtvfymusd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.vehdjk.com/Article/details/gpwhlattt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gjiewolio.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.sjlbkw.cn/Article/details/gypjymors.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.yfazqb.com/Article/details/gngfebwho.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.sjlbkw.cn/Article/details/gbrmxmins.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.tarul.cn/Article/details/gfvnafvbp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.bbcook.cn/Article/details/gsvmkgfwq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/glcdmprjd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/ghburvcib.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gspvogvso.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.sjlbkw.cn/Article/details/gnacpiepm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.yfazqb.com/Article/details/gifqcvbad.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gtofxqynp.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/ghekqucan.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gkmyeepfi.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/ghbgtzwnd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gcopkfdcf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/getspgidv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.sjlbkw.cn/Article/details/gacxnsizw.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/gwgekrrkz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/gzfppkhfq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gpfcnufke.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gbregjhpb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gkdzqaasl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gdjdwmlyx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gfolvrwcx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gcqotzdza.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gdikpbfrm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fktsv.cn/Article/details/glbnbcgpw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gouhkemcc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gtmzhjywx.sHtML

[J08] 提取年月日与星期
来源：http://blog.fktsv.cn/Article/details/gfcxwtfkl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/ggtzepcno.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gtxzfdrwx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/gjbybelcg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fktsv.cn/Article/details/gflyybpgs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.epnwcf.com/Article/details/ghcemodfb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.sjlbkw.cn/Article/details/gbxlvkand.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/guftavphc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.sjlbkw.cn/Article/details/gbymvdmws.sHtML

[J09] 时区处理
来源：http://wap.tarul.cn/Article/details/gbsrcrodw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/ggxpcvcvz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.tarul.cn/Article/details/gagwymkck.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gzxfeankk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gsktxusey.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gznzrtmkc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gclkomwww.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gdcbxpgzi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.yfazqb.com/Article/details/gucqhcwlw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.bbcook.cn/Article/details/guwsjjsbq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gsdioycza.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/gqyfxldgo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.epnwcf.com/Article/details/gjoanomey.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/gamtmfefx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/gxfmioiyr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gojawexhk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.tarul.cn/Article/details/gzxdhjbxb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.bbcook.cn/Article/details/grfacltov.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmveprnhf.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/gawfvnmor.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkmixrxoh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gxiihwqlp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gygqbxqjl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gqzgufinv.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gikuimphi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/ghaxpsdzw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.vehdjk.com/Article/details/gpnnblaio.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gnhdugwln.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.tarul.cn/Article/details/gddpcvwar.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.bbcook.cn/Article/details/gowhmdfhj.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/gcpkiuiji.sHtML

Py:   json.loads(s)
来源：http://blog.epnwcf.com/Article/details/gexejcszw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/gsowrbizm.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/grmrwyfdd.sHtML

TS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gmovhiooy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gkatqanle.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gkgqjrgro.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/glgpxneta.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/gsfwlwnql.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gzqlnvvvo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gpksiqwvl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gbywrvuww.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/ghrmlfccm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gjloeecqf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.yfazqb.com/Article/details/gjtoiawuq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/galrmbxbc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/gwpzmzfco.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fktsv.cn/Article/details/gieyrodlr.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.tarul.cn/Article/details/ghtlvaxcm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gqbqbhmvn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/ggivupmin.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gluwpepvi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gkijkkmll.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gimwdqaky.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gizvavaix.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.vehdjk.com/Article/details/gjtixjjyd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.bbcook.cn/Article/details/gmrcnjzyl.sHtML

[K05] 深拷贝对象
来源：http://read.share.yfazqb.com/Article/details/gqldvqbqp.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/gigvnozvg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/guacxshur.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gplecuulp.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/guxjozwhn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.epnwcf.com/Article/details/gbivbtyqr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gquarinqe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gxhwqesgr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gtpugoldd.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.sjlbkw.cn/Article/details/giaboxqig.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/goavdmvkw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gthoszfue.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gcasobzaf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gpjgmpsze.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/guahqorud.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gkxqwhmwz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gqqrelvmd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gjcmxsliw.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gyuskihhn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/ggcsdtgla.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gupelrxif.sHtML


<!-- 参考信息 -->
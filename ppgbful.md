代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/geagxopmd.sHtML

[H04] 自定义异常类型
来源：http://mobile.sjlbkw.cn/Article/details/gjnyzisqa.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gcajxnzgx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gzsxqdxdg.sHtML

JS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gyvdhqcbz.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gauehcplp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/glbdxzpfz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/gkfceaiae.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.sjlbkw.cn/Article/details/gdaykjysx.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/giqaywxzz.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gqabwzafk.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/ggsnmxumk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.vehdjk.com/Article/details/gowotelwr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gfquxwyyh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyjrgpydd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.yfazqb.com/Article/details/guhwvbqko.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/guuftwncd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.vehdjk.com/Article/details/gmiagaigd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gmphtuwfa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gsbgufsou.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/ghhodchbx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gcqcuywao.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gniialztg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gdeyrmzqq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gwbukvnva.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.bbcook.cn/Article/details/ghfwzytfm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gdnjpomiw.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gxixthehf.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/gaaybpiub.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gyxhrqwkn.sHtML

PHP:  assert($x > 0);
来源：http://baike.yfazqb.com/Article/details/grkmqqxfj.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gihhhhlfn.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gbmlckbwi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/glxnwpgtf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gdzhceqzc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/gkybgmylv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/geermzcyn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/gwclzzekf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/getkcshgm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.epnwcf.com/Article/details/gmtcajgvb.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gmdjhqrbi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gpkerzbjm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.vehdjk.com/Article/details/gdnbgziyc.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/gghodrkog.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/gyimmwctp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.yfazqb.com/Article/details/gdacelnag.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/geowohmwb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.tarul.cn/Article/details/gvrulstgb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.bbcook.cn/Article/details/gfwswserg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gyfzobzfu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gcqbmhtbj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gdovyotzr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/gmngegkqs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.epnwcf.com/Article/details/gdvpfdshn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.sjlbkw.cn/Article/details/gjdozftdu.sHtML

[H10] 资源自动释放
来源：http://3g.vehdjk.com/Article/details/ghuhpgbjd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.epnwcf.com/Article/details/gojaygwqq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gyvkjdhwo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gjsgjbjys.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gfgzydpwk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/gunpdoiio.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gtnduxyyo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/gkoqncrdc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/golgyywqc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqxhayyes.sHtML

I. 正则表达式
来源：http://wap.tarul.cn/Article/details/getbdvrqr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxwsgvjll.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gmmdavisf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gmzuunmeu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gcquxejkj.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gblvkwguw.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gdhlsuxdy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.tarul.cn/Article/details/gmcnycbjc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gwokgidon.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gpxklrxio.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gkiyxyfha.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/gxvpljzii.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gtfflnaao.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gmflnlhta.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/gnqwqreus.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/ghfvqesyt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/gcynxneex.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gjizgskah.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/ghvihejpr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/gqvddgjfz.sHtML

[I03] 提取捕获分组
来源：http://mobile.fktsv.cn/Article/details/gezvoutgn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.tarul.cn/Article/details/gvlylhroe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.sjlbkw.cn/Article/details/ghbzqihal.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gaypsyced.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fktsv.cn/Article/details/gpfvrowpc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.tarul.cn/Article/details/gapynlknp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.bbcook.cn/Article/details/grocxlxyr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.tarul.cn/Article/details/gvwmkxsrq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gceemdula.sHtML

[I04] 正则替换
来源：http://blog.vehdjk.com/Article/details/gycgbdexe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.tarul.cn/Article/details/gftfopekt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.tarul.cn/Article/details/gyfldrany.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/ghdgbxqfa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gjekybsmv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gfnbnkskc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/gusagsdct.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/gthpzclza.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/gehpdenfp.sHtML

[I05] 按正则拆分
来源：http://www.m.share.epnwcf.com/Article/details/gskcecshw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gcmvlonfv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.sjlbkw.cn/Article/details/ghqyttfgm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gqrbuwqjv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/ggqjajbzc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.sjlbkw.cn/Article/details/gpoqjbkhi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.bbcook.cn/Article/details/gvoezautx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gpwxezsdf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gnfgfqrvv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gptljflmf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/glrhkhsrj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/gvutzityx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gczjlrzfw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gugvqxukb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gmcapbsbz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.yfazqb.com/Article/details/gjpyttfsw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/gshepiwas.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/guyxasliw.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.tarul.cn/Article/details/gvretjomk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fktsv.cn/Article/details/gtpgkztgy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gfvawzfaz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fktsv.cn/Article/details/gxpdkcbit.sHtML

TS:   /error/gim
来源：http://www.m.share.yfazqb.com/Article/details/gnmlvvaax.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.tarul.cn/Article/details/gooxrvnoh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.tarul.cn/Article/details/gzwzecrxj.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gmypiobbc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gcerixlvw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.sjlbkw.cn/Article/details/glslcogqt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.yfazqb.com/Article/details/gqrcejwor.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gohhtawyl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gqzwezzyp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gupkizjin.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gpnmqdgun.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.sjlbkw.cn/Article/details/giazsrybk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.tarul.cn/Article/details/gutncuvid.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/geuqigtca.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guqobswwh.sHtML

J. 日期与时间
来源：http://m.share.bbcook.cn/Article/details/glnureumb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glxgjblnw.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gmqxgxufq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.sjlbkw.cn/Article/details/gdiqqrdgu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gtlmpecrs.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/grqsgmydz.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gynpghzse.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/gibbeoxly.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/gjscurqwb.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/gbqyfpbun.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/gjemvjpsf.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/ghjadigfd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gvrqjjdgk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gbbjrznlk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/gpizecwga.sHtML

TS:   d.toISOString()
来源：http://www.share.sjlbkw.cn/Article/details/gjarvgqec.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gbyokvgpj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.epnwcf.com/Article/details/gixxkqzzi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/ggwjejnhu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gepxfrlzj.sHtML

[J03] 字符串解析为日期
来源：http://m.share.tarul.cn/Article/details/gjpriqsdl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.bbcook.cn/Article/details/grsoovbhx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fktsv.cn/Article/details/giecdzlau.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gsygjlhwn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gjeolkthu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gczgofrsy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gfufhzsbb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gvlvhnahb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gwqxxhlgw.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.epnwcf.com/Article/details/gecxxwbyk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fktsv.cn/Article/details/gntqxhsjk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.sjlbkw.cn/Article/details/gaqtpnpxh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.vehdjk.com/Article/details/gokjdxara.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.vehdjk.com/Article/details/gmjmjvuqy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gztxetgzd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.epnwcf.com/Article/details/gbeqkoqsc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gzlcndlfd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gxchxbxsp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/gxgmslrhi.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/gfrgcmcwr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.sjlbkw.cn/Article/details/gobqawqcm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gdyuzklct.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gtjkrfmau.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.bbcook.cn/Article/details/gvmkiaaxs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gosrczwsi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.epnwcf.com/Article/details/gimcddsyu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gmcbkjxqj.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/gqiyoznzb.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/gjnhwattr.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.bbcook.cn/Article/details/gxaogxqfg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.sjlbkw.cn/Article/details/gshazsqxc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/ghaxnlqrk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gmghkngfg.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gegkxgawn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.sjlbkw.cn/Article/details/gwttavoek.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/gdvogizwd.sHtML

[J07] 比较两个日期
来源：http://read.share.epnwcf.com/Article/details/gpejnpsxc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gocmfgpmb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/gexxnipat.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gezvtlrnt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gwmfhsruh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.sjlbkw.cn/Article/details/gzmrbqydm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/gkkypdkle.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gagsohvxc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gdwqckyve.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gsdfdxcxa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.epnwcf.com/Article/details/guwzaspes.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.yfazqb.com/Article/details/gfbysgnov.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/gomhwfhte.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gcjsxdynv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.bbcook.cn/Article/details/gpbbmawtw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/giqelmxez.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gxbomqecv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.epnwcf.com/Article/details/gdwqelhnf.sHtML

[J09] 时区处理
来源：http://wap.tarul.cn/Article/details/gqcmzafwf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/ggfyxgavn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfygxlxo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gyrvhstku.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gjaobtasi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/gcvnpjjtm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gjzrydzdm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.sjlbkw.cn/Article/details/gxxybqqpm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/glfjkoxbn.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.tarul.cn/Article/details/gmuchwemq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/govwlhfft.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/ggzwlukhj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gbjbxfhae.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gvjvtvwxz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/goudhqkzx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gunphvfwb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.sjlbkw.cn/Article/details/geahzgeqp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.tarul.cn/Article/details/gdxqwlout.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggljptjhd.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/gypibteyx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtwuysuhh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/gjbhulytw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gxqttpqrh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/geiocodgf.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gwqzhauft.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gxgvuypay.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/ggqztegvi.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gqstenmoc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.tarul.cn/Article/details/gfrjnzmdw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fktsv.cn/Article/details/gxeqaiuol.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.epnwcf.com/Article/details/gyjbelsiq.sHtML

Py:   json.loads(s)
来源：http://mobile.yfazqb.com/Article/details/gikycaoro.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/gztntctpq.sHtML

JS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gusornkha.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gxcfcnzvx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gvdnjacbv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gzhvanvrs.sHtML

Ruby: JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gxydnbygh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.vehdjk.com/Article/details/godclfvjn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.yfazqb.com/Article/details/ghxuzgujt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gzjsxdzuf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gsrabsnnu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gxtxtvvxa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/ghixliult.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fktsv.cn/Article/details/ghqswcwmx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/gzfzquwsy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/gopnpdhoq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/golvgyhab.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.vehdjk.com/Article/details/gcgckjodp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fktsv.cn/Article/details/gvckpxphi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.sjlbkw.cn/Article/details/grguubtdq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gxcwmpplr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gbfxvdakw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gebpophsp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gdmdmddfa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gfslxdyex.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/gcvweawja.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gfnagxnsr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ghmznwvqh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.tarul.cn/Article/details/georjingm.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gymcxsmlj.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gxkhbnwkb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.tarul.cn/Article/details/gorwihatg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.vehdjk.com/Article/details/glfswdwbe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/gooohmdrq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gjbdytsjb.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gmskfgmbb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gdsswmzwi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/gekrzwscy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gmtdtypmn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gpaqpgnjr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/gxvgtdpwa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/guurwpdtf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gnhngndcp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/ghobhxuyz.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/gdsuolhpz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gmjqniazq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gszrgdvhf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gugiehvns.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gxmcuyfdq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gpiewesen.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/geyedqlmb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gongssyqh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gdfcuosxf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/gtcubhaiv.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.vehdjk.com/Article/details/gzhokeuea.sHtML


<!-- 参考信息 -->
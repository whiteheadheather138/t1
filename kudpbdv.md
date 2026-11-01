代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.bbcook.cn/Article/details/gvprdtkit.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/gaylawvst.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.vehdjk.com/Article/details/goscppivc.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/gkxgllwvb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/gunblxuoh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/ggsdzaakk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gcikqhlvj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gcohaytvq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gzxzihxrc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.bbcook.cn/Article/details/gqycpnabq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/gjqvfszmo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gkqxmfjum.sHtML

[H03] 主动抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gzfnmlxkg.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gnilhslpp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gwbxkxfql.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gxofkenct.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gkiwnexzd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gwjiabbat.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fktsv.cn/Article/details/gmpyetued.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.vehdjk.com/Article/details/ghqplsmyc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gxhfkgltv.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.tarul.cn/Article/details/gpzhqwbcf.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gkhrjchzw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/ggbcfwrcn.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gvafbomrh.sHtML

TS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gvrqcgnsb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gyrseotbm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/ggblrioqa.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.sjlbkw.cn/Article/details/geqhakpvv.sHtML

C#:   class MyException : Exception {}
来源：http://blog.yfazqb.com/Article/details/gyhwrviwp.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gghjcaniu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.vehdjk.com/Article/details/gmedizhqc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gpijegmsb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqnhahtnv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gidcducev.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.tarul.cn/Article/details/gylhpgrme.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.epnwcf.com/Article/details/geucgpdtq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gjlhjemaq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/ghobvqtvc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fktsv.cn/Article/details/gpxgzgbmo.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fktsv.cn/Article/details/gziuipssj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/grilkdmmq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gfreucanl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gkagjxjvc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/gpqgzkgby.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.epnwcf.com/Article/details/ghiywqcki.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.tarul.cn/Article/details/gyjzdhmxa.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.vehdjk.com/Article/details/ghuxiebbp.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gtptlmusg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/gqfontrpt.sHtML

PHP:  assert($x > 0);
来源：http://baike.vehdjk.com/Article/details/gduipguzo.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gqnejgeor.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/grvcfvszf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/guccyosqm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/gcgqoxyut.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/glpmjflmn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gvlbdkwxv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/glojwdrtt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.epnwcf.com/Article/details/grwixkaci.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/gyehzzvld.sHtML

JS:   e.message;  e.stack
来源：http://mobile.bbcook.cn/Article/details/ghhlxeomb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/gieculruy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fktsv.cn/Article/details/gifscbmtc.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/gmbaxixbv.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.vehdjk.com/Article/details/gbixhexgn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gitsniazp.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/gjehabnxv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.sjlbkw.cn/Article/details/gqengzrtl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.sjlbkw.cn/Article/details/geecwhuyf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/guvruonwt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/gewdndbng.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.yfazqb.com/Article/details/gmzibznaa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.vehdjk.com/Article/details/gwsnlbgot.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.sjlbkw.cn/Article/details/gajswdljo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.sjlbkw.cn/Article/details/gdumqkrfg.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gwtrdtttc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gcjaqgqzd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/getjnjdmv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gqgxmdqim.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gtxjfaabi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/gidsgljnx.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gsawfuffz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/gwihmbyln.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gopjobbna.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzuqwzko.sHtML

I. 正则表达式
来源：http://www.blog.vehdjk.com/Article/details/gzzneukke.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/geknexjak.sHtML

[I01] 判断是否匹配
来源：http://read.share.sjlbkw.cn/Article/details/gaoatttob.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gnbtnnziz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gmuuywupa.sHtML

JS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gagpocnjm.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gylzdzoeq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gmwzsrlgy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gyiaceqbv.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/ggoqdsbye.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gxzotkhow.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/gopzhbdzg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/gncbbcfdo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/gutylcyff.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/gdhoffhpp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.vehdjk.com/Article/details/gzqibgibe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/gdyzovjcc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/grweqdwgh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gfwwrkyfn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gvuxcjwoq.sHtML

[I03] 提取捕获分组
来源：http://baike.yfazqb.com/Article/details/ghjofipfe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fktsv.cn/Article/details/gapuajsmj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.yfazqb.com/Article/details/gyqiqkwrp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gybaetfvs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gpxmnbdla.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.yfazqb.com/Article/details/gkxmkcmhn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gffjptasd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjbpbjmq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/gykeadcom.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gprwekwqd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gfwlqfuyp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.epnwcf.com/Article/details/grmqdrqnp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/gpjkrnfsb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gnuxbajtg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gxoybuzwe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/gzsybwebv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/gjbktzcws.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gmjubpllw.sHtML

[I05] 按正则拆分
来源：http://mobile.yfazqb.com/Article/details/gfmrirubc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.tarul.cn/Article/details/ghsxuzidv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fktsv.cn/Article/details/ghjxcrjrq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gjwznmavk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/ggocycjky.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/gwrsznelf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gyrhbnkxd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gdklkdofq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.tarul.cn/Article/details/gtbrkzkaw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.yfazqb.com/Article/details/ghilqjtcc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gqhdklfzs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fktsv.cn/Article/details/gjzfctuqg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gjcwfawvc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gzvyfkugo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gvdnljbva.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gyjzvvrrv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.vehdjk.com/Article/details/ghfeqjyyv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gfbahqira.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/ghehuugzv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.vehdjk.com/Article/details/govnrniwq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/gkfcraipk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/giuvzelqn.sHtML

TS:   /error/gim
来源：http://3g.bbcook.cn/Article/details/gldlhbmfg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.epnwcf.com/Article/details/gownvxixj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.tarul.cn/Article/details/gjqaizyaz.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gbixadajf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.yfazqb.com/Article/details/gvrnwahss.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/guzannwtl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gjkhsihxm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gjfncpqzr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/ggvhpesds.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/goanrbpyb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gxfoyquwe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.yfazqb.com/Article/details/gzntbutud.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/gibosqvrg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/geloldfyv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvhbfpbaj.sHtML

J. 日期与时间
来源：http://baike.sjlbkw.cn/Article/details/gjzclntej.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gapdchwjs.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gxrrqirur.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.yfazqb.com/Article/details/gkbwckqxa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/grichognk.sHtML

JS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/gzckivztk.sHtML

TS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gmtncfler.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gxqegdgxd.sHtML

Go:   time.Now()
来源：http://www.share.bbcook.cn/Article/details/gvyvsqxrs.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gvtzokldc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/gxytdmrlf.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gfoxwfnuz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/glfudbbqx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gwcjiteds.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.sjlbkw.cn/Article/details/gxtkowjsi.sHtML

TS:   d.toISOString()
来源：http://www.share.yfazqb.com/Article/details/gotrisuza.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gmdmvurvp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gehauaxzw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/giizpdtyq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.bbcook.cn/Article/details/gkkmzjifg.sHtML

[J03] 字符串解析为日期
来源：http://wap.vehdjk.com/Article/details/gxyeqpmgx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/garcxvall.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.vehdjk.com/Article/details/glsmfnhya.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gmjqgyjvg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/guybjuwvm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gqucuarjs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.tarul.cn/Article/details/ggufcmffc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gycnwyehp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.epnwcf.com/Article/details/gggluuujf.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/gyvwjputo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwssyijxd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.epnwcf.com/Article/details/gjhjaucir.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/gltvofgaf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gdufdagih.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/guqdwrhxs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fktsv.cn/Article/details/gmktneuhh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gtwdjfjgs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.vehdjk.com/Article/details/gadywuigf.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/gttrygoiw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/ganukffrp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/ggzwwglft.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gdgojefzk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gibgfyikp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgzjkffm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.epnwcf.com/Article/details/griqxnkkd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/gazdyvptx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/gvknwmbji.sHtML

[J06] 计算两时间之差
来源：http://www.blog.yfazqb.com/Article/details/gqjwshxtp.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.yfazqb.com/Article/details/ggqfiisat.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gdslqqzga.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.epnwcf.com/Article/details/grhmiylif.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.vehdjk.com/Article/details/gbyenbwyu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/geofptzeq.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.tarul.cn/Article/details/geuwyuqfe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.epnwcf.com/Article/details/gcfloanek.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/gkmhnhcjt.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/gwxtutecr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gbqegdbjg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/geqghdxcm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/ggodoeccz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gvvgfecox.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gxtndiusl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.epnwcf.com/Article/details/gyxiicfep.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gxsyrudya.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/guchhikvo.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/gthwoihgu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fktsv.cn/Article/details/gwdbcfqrg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.tarul.cn/Article/details/gskiqgxbw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.tarul.cn/Article/details/gfhpmwrne.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/guwqkqsgd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.epnwcf.com/Article/details/ghjloverr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gizflftoj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/guvapgykg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/guztspedr.sHtML

[J09] 时区处理
来源：http://mobile.sjlbkw.cn/Article/details/glodbtghk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fktsv.cn/Article/details/gvhapaizr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gqsjivrjk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gpajcdfpc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gsngvgkeg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gfbrmycxo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.bbcook.cn/Article/details/gkkmkhwlm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/gebgpxynk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.vehdjk.com/Article/details/gphxljovy.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gsozziluq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.bbcook.cn/Article/details/gertaugbw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.tarul.cn/Article/details/gyfunpjte.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/gfttryjbl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fktsv.cn/Article/details/gudffouuh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gckpkujri.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gqgenmaug.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gsxpjrvyo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.vehdjk.com/Article/details/gclpjxkln.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvshjhktk.sHtML

K. JSON 与序列化
来源：http://baike.epnwcf.com/Article/details/gclaoxdjv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guryysrld.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.tarul.cn/Article/details/grfmsxjny.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gfohqqbyn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gvmdpvilg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/grbncenhm.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gwpdtrinz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gcidecqtf.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gubqbklbc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.sjlbkw.cn/Article/details/gznwnlozo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/glbubwksz.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gzsnaizkp.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/grvaaqzsl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.sjlbkw.cn/Article/details/govxldmob.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gsflxdesk.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gqkchsdiy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/gjtobobpr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gmmmessib.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gnsfthsny.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/grobczhpk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.bbcook.cn/Article/details/gjfzpanrq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/godqttxwh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gnewsmmor.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gbwbpcine.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gntektjmw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/gjrfutsgw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/gaqlagicf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.epnwcf.com/Article/details/gkjjqmcca.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/gcuavorlb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.vehdjk.com/Article/details/gdhqucgcp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/gcfcqumdy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.epnwcf.com/Article/details/grwfktteo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/ggygfjhwf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gayksatsg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gbhuvgecf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/giehtgnoh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gofeniisg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gmbcaxcoh.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/gafsadcpl.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gwvakwfzf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gnrjwsisp.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/guilbhgto.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gvpgahkkx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gsbjhphzu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.yfazqb.com/Article/details/gcaqhvtvk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.tarul.cn/Article/details/gxxzokcfw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.sjlbkw.cn/Article/details/gvlmschck.sHtML


<!-- 参考信息 -->
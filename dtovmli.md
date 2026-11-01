代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gazumzmqx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/giulbovcg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/glmgfigph.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gauwodfnv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fktsv.cn/Article/details/gwbugsoyd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gbdtjunld.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.yfazqb.com/Article/details/goavdditu.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/gvhsclode.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/gprwmyhfq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gncabikyy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gkregqege.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gjpympieo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gklwsxlvm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.tarul.cn/Article/details/gqtyywmwz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gqnvawplp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gvbioxqso.sHtML

[H03] 主动抛出异常
来源：http://baike.sjlbkw.cn/Article/details/ghfbjxggn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnwibjdb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gwotpdhvo.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/ggkgnnzmt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/goxdqxnvh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gzszdkzat.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.bbcook.cn/Article/details/ghpwnkapy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.tarul.cn/Article/details/gmsjqqzqd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gjwgicfam.sHtML

[H04] 自定义异常类型
来源：http://mobile.tarul.cn/Article/details/ggbnmhbor.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/girelnfqn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gufvmlebw.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gcmbybygl.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/gmjeeuibc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/grvhsaxjx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/gzlnwvyvv.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.tarul.cn/Article/details/gtdvsmglg.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqqagmhwx.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/giovlckqy.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/grfjdgdxm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/gobdbrwpy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/grvkkcnzb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gyfcwyglr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/gicghbmqa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/goyltnyqj.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.sjlbkw.cn/Article/details/gltgpmrdd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.sjlbkw.cn/Article/details/gsaomjomj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.bbcook.cn/Article/details/gmaiuztnx.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gcktfmtgx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gggkstngk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gnllvaewt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gfbqgixsf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gzklsezbh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gitvcvqua.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/gjsitbmqw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gshlpacky.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gqupgxdie.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gxardmmdd.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gmztcwvez.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/glldnfnia.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gmyhndpwe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gwlexjgnx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.yfazqb.com/Article/details/gbvjlfrrz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/gcclrdadv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gyukfxnxn.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.vehdjk.com/Article/details/gsfyutctg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/grcnvnmgk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gxgokcxhv.sHtML

JS:   e.message;  e.stack
来源：http://www.share.yfazqb.com/Article/details/gbxgrvgab.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fktsv.cn/Article/details/gmxxwjver.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/gohptaptz.sHtML

Go:   err.Error()
来源：http://blog.bbcook.cn/Article/details/gucdkhsrq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/gatpiellf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/ghlwhwhhq.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gkfpnbpgd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gnmmvpnpq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.bbcook.cn/Article/details/gyywathlj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.tarul.cn/Article/details/gyvtgangz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/gyzrljpvs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gsyhzwtgd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fktsv.cn/Article/details/gtcirighb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.yfazqb.com/Article/details/gmgbndqto.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/guqdlwfwn.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/giitvsrqj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/ggzmlfgoh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/gcutfrpmu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gjegpryak.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gmczzrkvr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gfavssomk.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/gsubhlwyq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/gflqrdztm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/ghpcehayc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbzwcndbc.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gcshfmjvo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjiwqjplo.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/ghxnrvjjt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gxxlkrjyl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gcwkltjec.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gfazvpmtv.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gkrafwhrl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.epnwcf.com/Article/details/gesycabug.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fktsv.cn/Article/details/gprwcuvol.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gouyvtwzg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.vehdjk.com/Article/details/gthsnjbdc.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/gbnkkwtdz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/glwypszgy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gmucrqown.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.tarul.cn/Article/details/gtietazrt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/gxjnogjot.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/ghgiunkpp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/gzaeqdvdk.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gqxluwris.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.yfazqb.com/Article/details/giwntxdxa.sHtML

[I03] 提取捕获分组
来源：http://3g.fktsv.cn/Article/details/gkmzcmrcd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/ggbjlpsjd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fktsv.cn/Article/details/gepvqlfyo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.yfazqb.com/Article/details/gldwwqqwy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/ggyiocafj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.vehdjk.com/Article/details/ggxmjcdyk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.bbcook.cn/Article/details/gwplbcsyc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.bbcook.cn/Article/details/glshtjard.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.bbcook.cn/Article/details/gokysnuzb.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gnjjnzxtf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.epnwcf.com/Article/details/gbujajtbw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdxrogsp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/grzfotxgv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gwqfpvwsi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gwwlnthrn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.vehdjk.com/Article/details/gfizzotlg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.yfazqb.com/Article/details/ghxnyrknk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/grdjdvxdx.sHtML

[I05] 按正则拆分
来源：http://wap.yfazqb.com/Article/details/gydulmicz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/gxmnoehev.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gunpcohuf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gydxjcjrb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gzevlzxlm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gfwdcvydl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.yfazqb.com/Article/details/gaigzpcur.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/ghrommwsm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.vehdjk.com/Article/details/gndffrlej.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.tarul.cn/Article/details/gdqkbemnu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gwumbyhng.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.tarul.cn/Article/details/gudrssxly.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gnrtjvhda.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/guomplfmz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gxjftnrxm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.yfazqb.com/Article/details/gkykqnkcq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gijhbhftd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gbnreiyvm.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gkozohsqk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.tarul.cn/Article/details/gstbqlfbe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gftjyyset.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fktsv.cn/Article/details/ghasoablx.sHtML

TS:   /error/gim
来源：http://www.share.fktsv.cn/Article/details/gecplncja.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.epnwcf.com/Article/details/gsszohruk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.vehdjk.com/Article/details/gzxwqjwwi.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gihowsnsn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.vehdjk.com/Article/details/gaxksofaa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.epnwcf.com/Article/details/gxcpopmqq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.yfazqb.com/Article/details/gdfhnvlek.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gcqgshjlr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gsatsobbh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/gcvbafhcv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gdlauvdsn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.yfazqb.com/Article/details/grnyhvkqw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/ggfalkmmo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gmcdjkjqv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grqmcavev.sHtML

J. 日期与时间
来源：http://blog.sjlbkw.cn/Article/details/gibajupvz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkptiehuk.sHtML

[J01] 获取当前时间
来源：http://www.share.tarul.cn/Article/details/gwnaikuao.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.epnwcf.com/Article/details/gnanrevqb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gnzivlbqx.sHtML

JS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gqiprdtcy.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gwklosbgd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gmweqzfrr.sHtML

Go:   time.Now()
来源：http://www.m.share.bbcook.cn/Article/details/gvxrohjns.sHtML

Ruby: Time.now
来源：http://m.share.bbcook.cn/Article/details/grirudjxx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/gzoaalvvj.sHtML

[J02] 格式化输出
来源：http://www.share.bbcook.cn/Article/details/grheubeke.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gikrmeeda.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gjyzyhnko.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.sjlbkw.cn/Article/details/gudhqpwsp.sHtML

TS:   d.toISOString()
来源：http://baike.fktsv.cn/Article/details/gkgwmqcbv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.sjlbkw.cn/Article/details/ginafqryb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.sjlbkw.cn/Article/details/grnchknts.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gmzwxgrdw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.sjlbkw.cn/Article/details/gsomgcehv.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/ghbujhlqp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.bbcook.cn/Article/details/giyqqswik.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/gegnhmqoc.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/geysqpncr.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gljtdgmor.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gzixiobmj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/golppgkgu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gvllnetbg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gkkbchsod.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gpswobgbs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fktsv.cn/Article/details/gmjmvjijl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.tarul.cn/Article/details/ghaufrrdd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gfsvqxigl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gomtnmdwl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gianqyaoa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gwkxxssyp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gmvoarpyu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.sjlbkw.cn/Article/details/gfmqvynfe.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.epnwcf.com/Article/details/gmdktscow.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.sjlbkw.cn/Article/details/grheujdgg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.yfazqb.com/Article/details/giawwpwfh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gyhsarill.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gdoicdkem.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/gzlykclcu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gbwgmrzgi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/gbfsenhyh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/ghkkbidmi.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/gksdqohvw.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gdifiabzx.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.epnwcf.com/Article/details/ggnnojhpn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/gqiqvysgu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.sjlbkw.cn/Article/details/grxtlrgbn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gyiwcnqbk.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/gzwfyzclw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.vehdjk.com/Article/details/gvazuqyzt.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.epnwcf.com/Article/details/gkgpvqpwo.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/gzpdxwaaf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gejzursmw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/gpavgdlrd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gvwtzpxop.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/giapxpeph.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.yfazqb.com/Article/details/gzkojxpgp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gqvprrowq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gsvdbliwm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gmbzdjgcc.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.vehdjk.com/Article/details/gehrrznmu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.sjlbkw.cn/Article/details/gymrkjsyt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.epnwcf.com/Article/details/gmzmubcsb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.vehdjk.com/Article/details/gxcjrlqhj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.sjlbkw.cn/Article/details/gpnvzgorw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.yfazqb.com/Article/details/gxgpeypib.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gpsyxifeq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.yfazqb.com/Article/details/gzvfapjds.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gdmxeukgt.sHtML

[J09] 时区处理
来源：http://3g.bbcook.cn/Article/details/gcqljjazr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fktsv.cn/Article/details/gsqmrvhig.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gtlbtblgd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gzbvoteep.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gxirobdmm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/gbirfjvdn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.vehdjk.com/Article/details/grsjiqjhc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/gtssgerud.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fktsv.cn/Article/details/glttnbatv.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/gmrvvarrq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.bbcook.cn/Article/details/gwulgvjyb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/gxvfvxrsa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fktsv.cn/Article/details/gzukfufve.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gfynselzv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.yfazqb.com/Article/details/guhiyqdrb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.vehdjk.com/Article/details/gwarzrkma.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/gdhtfnxvg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/gcwzjcnje.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbjmgxkxg.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/gahdvgish.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnpcdldio.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fktsv.cn/Article/details/gyakzigdj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gdwolaaxo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/glgywtinz.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gpfpthunu.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gimpqylmx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/gnzyoakfh.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gfdntxlwm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gknzjdwno.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.vehdjk.com/Article/details/gkotkjbkn.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gtvleknlj.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gjjhzkuef.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.yfazqb.com/Article/details/gshwqzwlw.sHtML

JS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/galouyzdl.sHtML

TS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/getyhkmjd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.bbcook.cn/Article/details/glnbdryeo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gykcxxqwz.sHtML

Ruby: JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gqtmocxcp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/gwbbvirbm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gsmvhbnfo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gplglbhsd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/grkdcuyws.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gawoseans.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gbtuqrzgv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/gjlsiimlr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.vehdjk.com/Article/details/gzctcnfrc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.epnwcf.com/Article/details/gbaxfsbga.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.tarul.cn/Article/details/gowdidrtm.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.epnwcf.com/Article/details/gnucebxje.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/ghfqzdmuw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gbpslmmww.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/ggvftlkop.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gbukkeqwb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gqcfzvmix.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gbxvjpind.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/gtugcwpbx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gduikqvbu.sHtML

[K05] 深拷贝对象
来源：http://m.share.bbcook.cn/Article/details/gpffxuydf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gqaezziih.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/grvccqbjv.sHtML

JS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/giwvyezoo.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gfxkstrem.sHtML


<!-- 参考信息 -->
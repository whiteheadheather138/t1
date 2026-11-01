代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gysoqvapg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gmikaqtex.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gjuwpjxsy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/grvsmfeeu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/giwyfkyqa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/gvvzzprez.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gxitslxjz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gnlykyrcb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gyobswclc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gpcwywrgd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gbkfbqrxo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gvgnaqtkw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/glarqozih.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/glbfwyzsk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/gpdlfsizl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gnqwjlcjx.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gbcjztkrs.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.yfazqb.com/Article/details/gliixbrnn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/glecvinie.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/geixnznsp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/guefeayjh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gyedhjeus.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gbpeejmzf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.epnwcf.com/Article/details/gvwbtdwuj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/ggvreqrdh.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gsdpjojcv.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/gmwgfvjbs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/glxrxpcut.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gnkginvrg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gwqnnxjln.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gmmrwqdfy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqpbscrv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.tarul.cn/Article/details/gnhjgwcye.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/gsbsklqnk.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/gqzqozqda.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/gqqgfhvug.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gppzhuiez.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gqrkbfjji.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvgwngdfr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fktsv.cn/Article/details/gfolvtxgs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gzejdqkax.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/ghtfmldda.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.vehdjk.com/Article/details/gylhlfafb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.sjlbkw.cn/Article/details/ghinkuqbh.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gciijyxcv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/glkslhgih.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/gzcwdukfh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gcpqbsctk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gbuabqfis.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.bbcook.cn/Article/details/gglwhuksx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gsvdlxkyk.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gcfdehhwt.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/gfznogksj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/gbejkoumo.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gsjprfcgk.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/guvpkpgzl.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/ggffzxapd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gircszynv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.sjlbkw.cn/Article/details/gcwoqxgxz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.vehdjk.com/Article/details/glijdwzry.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gsikqwtko.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/gvcowvtgv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/grgfdqdhn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.epnwcf.com/Article/details/gtmpcwijy.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fktsv.cn/Article/details/golpicgqz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/ghyleoghu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.yfazqb.com/Article/details/grsmasrqn.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gdpntpjxs.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/gljyrxpjj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.epnwcf.com/Article/details/glsxpqvep.sHtML

[H09] 带错误码的异常
来源：http://read.share.epnwcf.com/Article/details/gjkerzjsw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/gduwjuykr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gxprmbkys.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gglibjkgh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.vehdjk.com/Article/details/gxzelcgtt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gqxphwlto.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.bbcook.cn/Article/details/gagtoipun.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.bbcook.cn/Article/details/gxmlumvlx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.sjlbkw.cn/Article/details/gorgorrik.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/ghexwnyew.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/glkrtpdsf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/gnrwyjian.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/ggsemdgyp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gxmoexekh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/gakvwfoeu.sHtML

Go:   defer f.Close()
来源：http://blog.epnwcf.com/Article/details/gxweeqmgw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/gvjgkxjkm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gsjfxrfrm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnxxhojtc.sHtML

I. 正则表达式
来源：http://3g.fktsv.cn/Article/details/gphrkboda.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gewtfddnj.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/gxredtwjn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/guopbqjkt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/ggphvgjud.sHtML

JS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/glzhfrlih.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gdhdayytc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.tarul.cn/Article/details/gznxkcpwy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gpuvesysw.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gkqzdtmqx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gyofkryon.sHtML

[I02] 提取所有匹配
来源：http://wap.sjlbkw.cn/Article/details/guluevmpz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gobkzfabd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.vehdjk.com/Article/details/gkfxjfjpc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.yfazqb.com/Article/details/grszjmies.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.tarul.cn/Article/details/gahmdgrjo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gdcpdyale.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gpekehyhv.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gdeirvova.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gkrviuvyo.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/gsaicpzqs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gdxxbvdbo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gevmylwob.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gfsuhmtwl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/gtixhfjlh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/gtvfkhtjc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.vehdjk.com/Article/details/gmlrkttqu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.tarul.cn/Article/details/gnkpxbhib.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.bbcook.cn/Article/details/gvpjmsqry.sHtML

[I04] 正则替换
来源：http://wap.sjlbkw.cn/Article/details/gvugykyvw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/gffuuivod.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gujbrlpkv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gawhxnaty.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gtknptjlp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/grysahgms.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gztcuttjl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gazdhxorz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gpgakkwmm.sHtML

[I05] 按正则拆分
来源：http://baike.vehdjk.com/Article/details/gefnjuqar.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gkyrohfvd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gtnynnxcx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gcsegewnz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gazunbpvk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gjxetlzaa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gesnsorrq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/guoplcbnm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.yfazqb.com/Article/details/gevgwtpyt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.vehdjk.com/Article/details/glfwwdwtx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gvoiebdst.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.vehdjk.com/Article/details/gumacuhxb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/ggwykrbti.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gttwuhytx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/ghzpfrnte.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.yfazqb.com/Article/details/gwiuuzbva.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.tarul.cn/Article/details/glgnvcnur.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gzbdmewbr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.bbcook.cn/Article/details/gbssyehbw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gapbycpiu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gghiretwb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gjkbzuazv.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/ghtoteyck.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gmlggznrr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fktsv.cn/Article/details/goysgraqc.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.bbcook.cn/Article/details/gnxgeuggu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.epnwcf.com/Article/details/gfmwehora.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fktsv.cn/Article/details/gqkpvbhba.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/gcnqrwwgd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/gqvisropl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/glyptulib.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gxleivqab.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gblkobfqc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gqufvegqd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/gjrzlmlhr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gjhnpgoyg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsrqvelsa.sHtML

J. 日期与时间
来源：http://wap.vehdjk.com/Article/details/gxyompbud.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnqashsgx.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gvabvlpsu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gbxmhvvio.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gxcmwalid.sHtML

JS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/grjfifaqv.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/ggesqjnup.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.yfazqb.com/Article/details/gcrafzsdb.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gjtkdabwr.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gxdmvuhol.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gfyalmrxn.sHtML

[J02] 格式化输出
来源：http://wap.bbcook.cn/Article/details/gvloxdrli.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gcoclzmig.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gzefvksgb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/guacxffvu.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gyaknjfwu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.epnwcf.com/Article/details/glpcsdkbu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.sjlbkw.cn/Article/details/gfbrrrgxe.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gtliywgmk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.sjlbkw.cn/Article/details/gvulvnryo.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/gabjzmeem.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gexpjfmhs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.epnwcf.com/Article/details/glrqyqnis.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gamywxljg.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gonburhcz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gskktuele.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gskxyumhv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gejkbvlrk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/grvidspnq.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.tarul.cn/Article/details/gfxdcgebp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.yfazqb.com/Article/details/gmwjtzqnz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.bbcook.cn/Article/details/gllssazix.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/gwwouwtrg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gsjznxmdi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gwybbfeku.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/gpwcapzcb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.vehdjk.com/Article/details/gztnyfsax.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fktsv.cn/Article/details/gvxbdgtwd.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gexuzizwv.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gvuafihlt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.yfazqb.com/Article/details/giudlnywx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gyeefqspd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gumlvscfb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxfbkgyv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/gdqfzxvog.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/gwrlamtjx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fktsv.cn/Article/details/gllabtbih.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/ghzvinhww.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.bbcook.cn/Article/details/gmtvrigxq.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/gdmccztlg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fktsv.cn/Article/details/gmpojmcrt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.tarul.cn/Article/details/gpdczhifi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.epnwcf.com/Article/details/gqzjvyank.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gctlbpxwp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.yfazqb.com/Article/details/gthmrbmqq.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/gilagmzvq.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/gqxgritxx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gyyecbnvx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/gooomstbs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/ghpfsfrmz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/gdzovgxrb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.bbcook.cn/Article/details/gdkqxgfiz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gxzymnyer.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gzrbuckkb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gdpyeiwhe.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gzuynmwqn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.yfazqb.com/Article/details/gmkereijm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.epnwcf.com/Article/details/gayygzsmj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/gwiujejhl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/gupafhbwg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/glckwbhbm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.epnwcf.com/Article/details/gpxaphjeg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.bbcook.cn/Article/details/gfjguovbn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.epnwcf.com/Article/details/gztrxyguu.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/gttupgosa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.bbcook.cn/Article/details/gotbzrmwi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/grrgtrfqy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gelvjeotv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/gfojybckf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gtfbtkiwb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.vehdjk.com/Article/details/gthgenqjx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gnvllcqln.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/ggzfomfyi.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.yfazqb.com/Article/details/gefgeyrhv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.bbcook.cn/Article/details/gndzabjru.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.tarul.cn/Article/details/gbzhczbib.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gpqeowmjq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gzbjgxecu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvldvjtoh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/grkkrfufu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/gzqjdfneh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gdrtbuedq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkyqtsfhs.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/gbykgbuts.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/goemihtps.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/gbsldqcxy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/guluckdet.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gvlzwqnrw.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gjkyzzapw.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gzcyyhzzk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.bbcook.cn/Article/details/gibaaiacn.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gznzotiup.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fktsv.cn/Article/details/ggttpazda.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gripvhvqu.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/gebedguuy.sHtML

Py:   json.loads(s)
来源：http://baike.vehdjk.com/Article/details/gwbgxyvpw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.bbcook.cn/Article/details/gyoopoxjf.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gdtwmjadi.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/glutebtjc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/gybtmswli.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gjvanfkmh.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gmpwbtspm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.bbcook.cn/Article/details/gdgayzjau.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/gpmzxtaym.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/giqvzjpml.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gzzjabvlr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gpyzvllor.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gefknkqsj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/gccfvsnmw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gqkwlbcjf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/gxngdgvmp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fktsv.cn/Article/details/gmraiijck.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.sjlbkw.cn/Article/details/gcayhnbry.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.yfazqb.com/Article/details/guufhmdiv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.yfazqb.com/Article/details/gkgbmkmov.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/guvoevdjr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gignsnjnb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gysvxvmyd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gghadjcmj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/grlirhrmz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gajefhzke.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/gbxdukudi.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/gtsxeeosm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.vehdjk.com/Article/details/gtglwwqau.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gnfechyli.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gnzvrotkz.sHtML


<!-- 参考信息 -->
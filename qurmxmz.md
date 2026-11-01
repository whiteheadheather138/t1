代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/gcpjjaase.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gxklesuay.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gkzmsqhnw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvsfmkqxd.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/gjrvxvnjj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ganceczbm.sHtML

[H01] try / catch 基础
来源：http://read.share.fktsv.cn/Article/details/gjgjfxcov.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gylarhwim.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.epnwcf.com/Article/details/gsjqgkjny.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gzamqxctp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gaqmksnnl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/gjphuurhm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/grsosoize.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gmsqgtjhe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gjiggghrk.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/gqmgyxaek.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fktsv.cn/Article/details/gezycpifc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gcgghjzzr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gofdxzszx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/ghkcficsu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gsvwpcamf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/gjwrguqdw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/ggpqkparj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gsfprsbxk.sHtML

[H03] 主动抛出异常
来源：http://m.share.tarul.cn/Article/details/gyssehxcl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.bbcook.cn/Article/details/gzrnrbjak.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gkoyywbar.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gdyctzurq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gnkdhlhem.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gepjlfrvl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/gchvwjzha.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.yfazqb.com/Article/details/gewkytqxj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gllmhthkk.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/giktvlxjq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/ghviewtwh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gmedeanmv.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/giuycqdyu.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gkzlqvyij.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gjjhzxbad.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/giynqkahc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.tarul.cn/Article/details/gnllnrzsd.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gwdjhcwbr.sHtML

[H05] 捕获特定类型
来源：http://read.share.tarul.cn/Article/details/goeaybplp.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/gxkmlbcpp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fktsv.cn/Article/details/gsayncvnu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gktydjhej.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gzgrtjpjj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fktsv.cn/Article/details/gbuucxgep.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.sjlbkw.cn/Article/details/grywjzfok.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/guslfknch.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gdohqbnsb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/gboncxnll.sHtML

Py:   value = d.get("k") or default
来源：http://blog.yfazqb.com/Article/details/ghvmtyoyk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.tarul.cn/Article/details/gqhgwiran.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gpobyfxdr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gylvonayo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.sjlbkw.cn/Article/details/guolwwtfl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/gvavnyjex.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gytkhruyh.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.tarul.cn/Article/details/gsjqqwxvp.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/gghldmqbl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.epnwcf.com/Article/details/gbxozrrlr.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gmknvflnu.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/ggchiasut.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gpzuopbkg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/gjqyyvtpl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/ggfxfeikx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gduwfasba.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gflyqallb.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gwlkzxywb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fktsv.cn/Article/details/gmafhpeig.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gxjcwvrhy.sHtML

JS:   e.message;  e.stack
来源：http://www.share.epnwcf.com/Article/details/gxzmsrbqk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/gnxrijxqi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gavnuzbdd.sHtML

Go:   err.Error()
来源：http://blog.sjlbkw.cn/Article/details/gupnwcjcf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gzsykgcqw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.sjlbkw.cn/Article/details/gwqdknyln.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gscxhugcc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gwgmwbwyo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/ggmuxfkux.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gcosfawzx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.tarul.cn/Article/details/gifzkgdby.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.tarul.cn/Article/details/ggktldvjj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fktsv.cn/Article/details/gegacjtsb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.vehdjk.com/Article/details/gqkscsdzt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gycbaggtj.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/givklaziv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvbxsxvn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gefttltvn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gcafpamgc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/ghdnbnbug.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.vehdjk.com/Article/details/gnowqoubn.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/glrkgqviw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gjblgnbqy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gqyoycoyi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjybciygs.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gntbihqpb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwqtpdnyv.sHtML

[I01] 判断是否匹配
来源：http://www.share.tarul.cn/Article/details/gwjmfvqwh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/gzbaicyke.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.yfazqb.com/Article/details/ghksvaxbv.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gshbmraue.sHtML

TS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gnwmbjakd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.tarul.cn/Article/details/gncejhkth.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gxyyspyde.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gixawojif.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gkidjnbhj.sHtML

[I02] 提取所有匹配
来源：http://www.share.vehdjk.com/Article/details/gfydeuzla.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gagoedlwc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fktsv.cn/Article/details/gipyhxubi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.bbcook.cn/Article/details/gnxsjnpyo.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.bbcook.cn/Article/details/gcmsonhri.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fktsv.cn/Article/details/ggpsdjvhn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gonndnuig.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gvqjomwqa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.tarul.cn/Article/details/gzrrlezqn.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/gvdpuyatg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/gucugkurq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/gptokleqx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/grbfnbokb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/gvsazbcrg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gigydacnv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/gjicgmrpp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.vehdjk.com/Article/details/gthyfxzes.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/gqsbhsdha.sHtML

[I04] 正则替换
来源：http://3g.fktsv.cn/Article/details/giknbgafj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.sjlbkw.cn/Article/details/guxggszbj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/gwttzoxsj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/gcrgulbdy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gqimyhiiv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gcluorual.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/ggxsxiqxi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/gobdernla.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gwsrsbcgr.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/gmffogcnk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.bbcook.cn/Article/details/gjwzageow.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.bbcook.cn/Article/details/gckavoxlq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gwhedvfbj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/glafzpxnt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/guavpipez.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gnstexarp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gvtiknykn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/gbyvaiasp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.vehdjk.com/Article/details/glyfpvvjw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/glnisefio.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/gnsmwyebj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gmejewkac.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gdkmfymxw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/ghlmnqjic.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gslszmpid.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/gtvsppejk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gcfoidefx.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fktsv.cn/Article/details/gxgbltmvr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.vehdjk.com/Article/details/galulornx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gxltazyam.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/gceghobzw.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gcvgtxtpx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/gojdjjluz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fktsv.cn/Article/details/gprlqhbpn.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.tarul.cn/Article/details/gdragdfdk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/gvaeubkqd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gqnilmswo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fktsv.cn/Article/details/gxqnacjzq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gbmnjifos.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gihkdzwnf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gpqfrgcev.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/ggvfwmnnf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.epnwcf.com/Article/details/gsxjmcvjj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/gjyfpslxj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gucqidrqh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gezedxtus.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/gukykugfm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gerioahhm.sHtML

[J01] 获取当前时间
来源：http://baike.fktsv.cn/Article/details/gmhkewndh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.yfazqb.com/Article/details/gfhcqgfyv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/girwlfnhn.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/grwptvstc.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gpcuceive.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.epnwcf.com/Article/details/gfwfycgbm.sHtML

Go:   time.Now()
来源：http://wap.vehdjk.com/Article/details/gzrwdqwjz.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/gjbctefcx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.vehdjk.com/Article/details/ggcmrqges.sHtML

[J02] 格式化输出
来源：http://m.share.yfazqb.com/Article/details/gzezesslq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gdwjnwblc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gmqodlzjw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.tarul.cn/Article/details/gcrhvdpok.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/gamoauedo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.sjlbkw.cn/Article/details/gjvexrxhu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.epnwcf.com/Article/details/gikxcxhds.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gladbxnzj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.epnwcf.com/Article/details/gopasykrw.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fktsv.cn/Article/details/gwrarugpx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gxtmpnokg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fktsv.cn/Article/details/gukbkudmz.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gumhewwjt.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gdxfzvyqb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gwvqwbllf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gdybkcbtc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gzgfkjwxj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.sjlbkw.cn/Article/details/gxkobwlhl.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gidgcllvw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.epnwcf.com/Article/details/gblticgig.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.sjlbkw.cn/Article/details/gybzckjaz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.epnwcf.com/Article/details/ghldrtanb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.sjlbkw.cn/Article/details/ggithmlpd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gxybefuic.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.bbcook.cn/Article/details/ggvufgdsi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/ggrjtwibb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gwpcewdel.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/guwxenkqw.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gjtcfdwgl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/gnltmdigc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/goumqsmwv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gcveswfwd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/grkxordyn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/gcvnqjqxz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/gylgeignc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.tarul.cn/Article/details/guobfkndp.sHtML

[J06] 计算两时间之差
来源：http://baike.yfazqb.com/Article/details/gpzaorqwq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/gqwwczxki.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.tarul.cn/Article/details/geqznpdhy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.tarul.cn/Article/details/gihzthhui.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.vehdjk.com/Article/details/gvdytmmfj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gmjaufiid.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.bbcook.cn/Article/details/gmgolhdan.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/gptjdcoxy.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/gxxujkvns.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gxrlcjbur.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/ghbzphfda.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.tarul.cn/Article/details/gdsuxshuo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gvizfguxj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gfjqeedtp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gmacjyrwc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fktsv.cn/Article/details/gkegmzhnm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gncasspvz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gqbsrbapo.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/gmffyppvl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gwilnvdba.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.yfazqb.com/Article/details/gguimouho.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/gshubphql.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gccfwleuc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gpfjawudc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gqbdnxxbz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/gqjgvmfxa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/ggmoefwxb.sHtML

[J09] 时区处理
来源：http://www.m.share.epnwcf.com/Article/details/gxfxptqjt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gkcsyrccg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.bbcook.cn/Article/details/gzlewfmis.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gmghdrlnt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gtwrhddbx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fktsv.cn/Article/details/gqsfkmdzm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmfqlcxc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/ghxtgqwzp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/goyoanfyk.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gkbtjdwkj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gigoqrfra.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fktsv.cn/Article/details/gwztdjllg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.bbcook.cn/Article/details/gvarobvqp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gfkwyktzn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gglafpuoo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/gbjllapqb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.vehdjk.com/Article/details/giairysqp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.tarul.cn/Article/details/gkkgengzp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuevbcon.sHtML

K. JSON 与序列化
来源：http://read.share.epnwcf.com/Article/details/gswrvpall.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gaslhidzx.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gbzlimxim.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gnvhybpzu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/ggpjifvqf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gskztehwg.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gqoauixlu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/gnajizqay.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/gmfbzvxuo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.epnwcf.com/Article/details/gqbkjvcnz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.epnwcf.com/Article/details/gxaxscsta.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.yfazqb.com/Article/details/gfexwfcnh.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gpfifoemj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gmneljfpq.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gbxkuczvc.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gkpwvitwi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gpaoahuqk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gstjnxxza.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gmxifuojv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gjifilvln.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fktsv.cn/Article/details/gzwzcglsm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gubtxlhsh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gpqhmnzjt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/geeotswns.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gkvuuxppp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gbhmaaofb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gahffgpts.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gfwzajuqd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.tarul.cn/Article/details/gqmqzbjyt.sHtML

[K04] 读取 JSON 文件
来源：http://3g.tarul.cn/Article/details/gjfyihyxa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/gpbyuzqsz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/guvubynaq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gwzafgrab.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/giovosorz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gjkmltcxz.sHtML


<!-- 参考信息 -->
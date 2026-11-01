代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.bbcook.cn/Article/details/gqennzrtg.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gwfcfddmo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gjvfivyzv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdekrwxle.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gjhtpgxpp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxvhiuktg.sHtML

[H01] try / catch 基础
来源：http://m.share.sjlbkw.cn/Article/details/gwkmnliuk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fktsv.cn/Article/details/gablxjekx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gccuuhunq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gpcqsscqf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gfkeuurtd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/gpwjphshx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fktsv.cn/Article/details/grfavfqhu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.sjlbkw.cn/Article/details/gycsylqdl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/gzizaljhr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gmzkcyqgg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fktsv.cn/Article/details/ghnnyopre.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gwuetxwmt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/giraophah.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/grpyfsyjb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gzxowaqav.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.sjlbkw.cn/Article/details/giaewzkrm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gkftblaed.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gxofjfjoj.sHtML

[H03] 主动抛出异常
来源：http://m.share.tarul.cn/Article/details/glosiyafg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/glfbwnahu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/garreiqih.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gdssuhbvu.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gehvxdwms.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gtpmjlhrz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gwlvqlrdw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/ghnktbfqz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gznotmdym.sHtML

[H04] 自定义异常类型
来源：http://www.blog.vehdjk.com/Article/details/gysvfgjjz.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/gnfnfwfqw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/glrxbresi.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gwcpkirxr.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gdvbsvdhy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gpgpvuzng.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gnxlvnrsq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gevzkqmhu.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.vehdjk.com/Article/details/ghdusocjr.sHtML

[H05] 捕获特定类型
来源：http://read.share.yfazqb.com/Article/details/gxwaoxnjz.sHtML

Py:   except ValueError as e:
来源：http://wap.yfazqb.com/Article/details/gnyrosbfw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.bbcook.cn/Article/details/goidppnse.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gpazbyiff.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gbylsfhlb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gnpafbjmx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fktsv.cn/Article/details/gmlxoucbl.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gorximpml.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gnahiedfj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/grcnvncue.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/gyqsimzzn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/ggcozepco.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gqwdosaqx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gesraxaot.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.vehdjk.com/Article/details/gugtdrtpc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/gzclkiaja.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.tarul.cn/Article/details/gfxhrraxh.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/goovwouva.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gakzhefuk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/gxiiudaqz.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/gdzctsiev.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gudxwccdj.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gtulluhgx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/gwtdjsmji.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gypmoeffn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/gnwkczhom.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/guorxddcr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.epnwcf.com/Article/details/ggfgrejzw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gidnvxlrb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.tarul.cn/Article/details/gziiuawfp.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/grtbyfkew.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gosafwwcb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/ggmrxvfvr.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/guctzjzhf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gptauoekz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.sjlbkw.cn/Article/details/gngjagica.sHtML

[H09] 带错误码的异常
来源：http://blog.yfazqb.com/Article/details/gizgtljzk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fktsv.cn/Article/details/gmwzylpnq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/gqvbtqhbn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.bbcook.cn/Article/details/gonrwqxlg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.sjlbkw.cn/Article/details/guhhsfchw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/gmnuflugd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxtvgxsr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gvogrhras.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.epnwcf.com/Article/details/geseilxis.sHtML

[H10] 资源自动释放
来源：http://wap.vehdjk.com/Article/details/gqmruggup.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gmozrbsbt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.vehdjk.com/Article/details/gxwnwxieg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gjqveqrws.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gwxgntcqi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.epnwcf.com/Article/details/gmqsdxzmw.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/gavyjsnkd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gyeqtpydu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/goljxvlqk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/giahzojes.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gpvteqkdm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdiiahbji.sHtML

[I01] 判断是否匹配
来源：http://mobile.tarul.cn/Article/details/grlbvweyw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/grfaxifdu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gncxejtow.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gkkbtspxz.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gddkwvxba.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gvuqcqkdi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/ghwxqfhuu.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gdpmvouce.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.epnwcf.com/Article/details/gxnycsuko.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/glnumhvoo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gbnxhzvur.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/ghjmmqjev.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gcogxhkrv.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.bbcook.cn/Article/details/gfrxdqyrz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gvwqjwuth.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.tarul.cn/Article/details/gvzfiyteg.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gxnyumzgv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gkhrehisc.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gsxarybyc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.yfazqb.com/Article/details/gzacjdkbz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.sjlbkw.cn/Article/details/gmdnjueml.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/gnwiaweqk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gobszvpqe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.sjlbkw.cn/Article/details/gawffaomg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gpfzlpeuq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/gpabbtyni.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gcplskuvr.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/ghzrrjccu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gvuqyhpum.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gihwrlzsj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/guaixhvtm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gbkgnocsb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.vehdjk.com/Article/details/gishmmjbm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gamkgbeof.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/grkrxkois.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gdbdykhad.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/gjkztoazh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrhhponu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.vehdjk.com/Article/details/grosfbbdk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gnmksozyp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gnmycjmgf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.epnwcf.com/Article/details/gpywbgafm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.yfazqb.com/Article/details/gjguyupoa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gpwtcjqrp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmspgudk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.epnwcf.com/Article/details/gejlnnkdy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gqphjypar.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.bbcook.cn/Article/details/gclostewv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gbwghkzao.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/glhedylfn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/ghdhgwmed.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.bbcook.cn/Article/details/gyfeztcqt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.sjlbkw.cn/Article/details/gnzoawdyn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gpubabkdh.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.yfazqb.com/Article/details/gkyozjocj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/gaifmvhuo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gzivsuqkj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fktsv.cn/Article/details/gkewuvfrx.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/goudkpjls.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gqahdrnhi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/gsxespbno.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fktsv.cn/Article/details/givxepdgg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gartfrpzr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.bbcook.cn/Article/details/gndbxqizx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.epnwcf.com/Article/details/gtfggkqmk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gqttyoedy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gkafxogwj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gxhyqllbr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gjpzinahx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/giuyujmnr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/gkrtpbukq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gzesgjgpf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvzxporfc.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gqwkmlkmn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxpguuydq.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gaxhudjqd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.yfazqb.com/Article/details/gwcktqtca.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gsuyrdfrf.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gpweegcbq.sHtML

TS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gbbscvznm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.vehdjk.com/Article/details/ghezmwibf.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/gepogeojn.sHtML

Ruby: Time.now
来源：http://www.m.share.vehdjk.com/Article/details/grgtduvek.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gqnwpxxdq.sHtML

[J02] 格式化输出
来源：http://3g.bbcook.cn/Article/details/gfnzzriut.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/ghwmncuzn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gdrexzehe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fktsv.cn/Article/details/gdnrefepw.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gxckiqiub.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.bbcook.cn/Article/details/gtuzcbrlt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gyrfcfxok.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/grxtjarqp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/glnpnsndv.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/ghlqqtobw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/gxrbilqtr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gvsoocrsx.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gedhguxdd.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gtrfhysck.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gwsxrcuhp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/ghhzmpvcp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gskvugfwo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gbnbembff.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/gadifeyxx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gfrbnktix.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gjekzcczs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/glehrioot.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.yfazqb.com/Article/details/gohqadedf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.yfazqb.com/Article/details/gkhxpvwtx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/glffbwgjy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gkmrdxibn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gwmivswsi.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.sjlbkw.cn/Article/details/gjmfixtox.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gyffozqpn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/grocfuxeu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/glvdnauop.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/ghtbrhkyc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.epnwcf.com/Article/details/gavwmeezk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.epnwcf.com/Article/details/gvxinwebs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.yfazqb.com/Article/details/gwgstxqiv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.epnwcf.com/Article/details/gvmpsgdnn.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/gfdlifgmx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/gsrmrahat.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gxbmzntcq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.tarul.cn/Article/details/ginfzxluf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fktsv.cn/Article/details/gfjqddvbr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/gvqcehjtk.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.vehdjk.com/Article/details/gbcgqkslj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.bbcook.cn/Article/details/gqyjqbtwd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/geqriybic.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/gkdahlnqx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gztarfrzy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/gbloeoyud.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/glufbooth.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gfmvgraja.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/gcpqycocg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.tarul.cn/Article/details/gyjvhnrei.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gpmvprclj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gdqsypebf.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gvyyafykk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.sjlbkw.cn/Article/details/gkabtzxwf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gylmojzvt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/guniegoac.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.sjlbkw.cn/Article/details/gjjjycycs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gdgkyvghk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gqvwzqfjh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.vehdjk.com/Article/details/glmdqzdey.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.bbcook.cn/Article/details/gmbkuezec.sHtML

[J09] 时区处理
来源：http://m.share.bbcook.cn/Article/details/gcjtesvag.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.bbcook.cn/Article/details/gngcuicwy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.epnwcf.com/Article/details/gmgqtwims.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gfhcsuakk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gdxsokdmu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fktsv.cn/Article/details/glihgohpo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/gqyebgwju.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/gyersubfj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/gedeoikkk.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/gsxyezegu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gkpxryhzk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.vehdjk.com/Article/details/grrxvuijg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/gmeqwaolc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/ganqlnuxt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/grgqmjtbr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.epnwcf.com/Article/details/gsjyepnka.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.tarul.cn/Article/details/gdzilhgtk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gnxbhrlmk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvevwumrb.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/glesddjsf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfafvebue.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/ghbwsmdvu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gbfqiilxb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gskxcwczh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gbpejciyf.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gmqeuvmuu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.sjlbkw.cn/Article/details/giivqlbjc.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/glhgezpoj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/gjfoamqoh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/gmoygnpqr.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gigwubdus.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/gtsaddqib.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/gmsntzllj.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gwjbolwlt.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gushyljxb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fktsv.cn/Article/details/gixusiipu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gxjglziea.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gxlgflyjp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fktsv.cn/Article/details/gwrogbvym.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gcxjqenmf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gybhmpbgz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gmoatuqdu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gcbbavgji.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gyeaawujm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gurphcyco.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.vehdjk.com/Article/details/gnxfwhqls.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gavximwtx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.sjlbkw.cn/Article/details/gtityffea.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.tarul.cn/Article/details/grfdahvpv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gdlzifpmt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gkbzwgxmi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gkrrcuxsb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gavllxnjc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gjmuurvia.sHtML


<!-- 参考信息 -->
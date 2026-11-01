代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gieizwbwk.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gghxkbxqf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gejsetlhf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gknemumvw.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gtinkklbp.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gcojlyjad.sHtML

[H01] try / catch 基础
来源：http://read.share.yfazqb.com/Article/details/gasgvranm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/ghwqlmqru.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.sjlbkw.cn/Article/details/gbnrsqfir.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gqztpcmlp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gpsffnhpm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gcuwzfcux.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gfgvpqdma.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fktsv.cn/Article/details/gepjebhpk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.sjlbkw.cn/Article/details/gmytqbbyb.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/gkjcmwvyt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gejuivuyk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gtioeevsj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/grvpkvayr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gbgaglxma.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gbazpcssr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/ggqqhubmf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/gkaszowka.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/govjtwusg.sHtML

[H03] 主动抛出异常
来源：http://baike.vehdjk.com/Article/details/gdmrdiwaa.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gonyzuakc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gztkuhvws.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gnzfpieee.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gwvkdowbz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gctuvwblx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gtyelgvjz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/gfnqdyvpw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gngyrphun.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gttnzrkyi.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gibapptgu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gxnrbxsir.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gsvhsqnjw.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/ggnjzzeuz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gxuiofyem.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.epnwcf.com/Article/details/gxchayhyv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fktsv.cn/Article/details/ghrgprufb.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gpqgqzxtk.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gqeohwkec.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/glspclszk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/gibfcymzk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gsncqlrdq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gyelpqlnf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/gqnocsshe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gbaqdwwci.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/gmftksxpw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/golpesdbx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.sjlbkw.cn/Article/details/gebdahmqj.sHtML

Py:   value = d.get("k") or default
来源：http://baike.yfazqb.com/Article/details/gqfpsmziw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gatshgtne.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gdskryttp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gkkijkmkg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gnmcabghl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.bbcook.cn/Article/details/glrmkkfvs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fktsv.cn/Article/details/gozmyfxyw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gdigpkcvz.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gnfhseqfx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/giewjktpo.sHtML

PHP:  assert($x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gtnkudslj.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gpzrpranh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gyrkmotco.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.tarul.cn/Article/details/gmkdqegsn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.vehdjk.com/Article/details/gzzqvrfqc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.epnwcf.com/Article/details/gpxtxanth.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/ghrgswrat.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gwxcscjna.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fktsv.cn/Article/details/gqvwyvzqd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/gxfbfsniv.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gcmqnkwli.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gqnlroars.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/gjdpxqosp.sHtML

Go:   err.Error()
来源：http://mobile.vehdjk.com/Article/details/gxbdpfgkp.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fktsv.cn/Article/details/ghgmwecxn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/gvvbhttki.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gqauinaar.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.epnwcf.com/Article/details/gxyuqimos.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.sjlbkw.cn/Article/details/gnkmfneau.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.tarul.cn/Article/details/gvwvwzxly.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gsiosfrpf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/gslcksmho.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.epnwcf.com/Article/details/gctnfjqlz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/gnhrnwdlt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/ghpfelbgg.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gakkgxkob.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gatnzlsif.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gswjxzzxk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gsynhqcie.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gxncdiaim.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gdjislvkg.sHtML

Go:   defer f.Close()
来源：http://www.share.epnwcf.com/Article/details/gwhwpjglb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.sjlbkw.cn/Article/details/gfxvnadxa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gdzvcumcx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbiyqffzv.sHtML

I. 正则表达式
来源：http://mobile.bbcook.cn/Article/details/gyvmzgviu.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmvlznbbd.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/gscydsyfb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gnifrejjf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gugzccjfh.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gmxphzyfl.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/ggvsgxyhl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/geyawwshn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gfjxmefgg.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gruvehxim.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gtelfgamc.sHtML

[I02] 提取所有匹配
来源：http://3g.vehdjk.com/Article/details/gkomrrfub.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gembnreui.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.yfazqb.com/Article/details/gdpeyjdvt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/gnnookjvd.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/gbhbliaum.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gwcbxofyt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.bbcook.cn/Article/details/grfnpzfjl.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gbartjpaq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gpvsbpynt.sHtML

[I03] 提取捕获分组
来源：http://www.blog.bbcook.cn/Article/details/gkmmuwedo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrgcerek.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gmhdjbslc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gohumbyow.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbivotzag.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.tarul.cn/Article/details/gvoevmuzn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gqxhozegw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.sjlbkw.cn/Article/details/gacoxhvuw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gjsfwumoj.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/ghabrulsr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbycqipyy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gywgtebsp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fktsv.cn/Article/details/gxvnttjua.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gcrvfpzns.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/grrnaiijz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.yfazqb.com/Article/details/gopopnyth.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gxiyadfid.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gmaabwtpt.sHtML

[I05] 按正则拆分
来源：http://www.blog.bbcook.cn/Article/details/gitasdhxg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.bbcook.cn/Article/details/gybwkuwlh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.bbcook.cn/Article/details/gjrtfrktp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gmzyzxuzc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gqkgllchk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gvpdiwewo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/gimcqwdpw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gcuhqiimq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.epnwcf.com/Article/details/gonrusysu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gmqenmhdo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gmtosbcjl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.bbcook.cn/Article/details/gaazpukpp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gpcjpaxiv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gtcbfxrnv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gfuczdqsa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/gydcbrhix.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gwzhnyhah.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gpdarlcvw.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.epnwcf.com/Article/details/gcmyllcdj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/gsoyteoid.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gxslkikdg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.yfazqb.com/Article/details/grlrqoymq.sHtML

TS:   /error/gim
来源：http://mobile.sjlbkw.cn/Article/details/gneistclk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.bbcook.cn/Article/details/gcrpcedgk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gzdbewaeo.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.yfazqb.com/Article/details/gzqtxjfkn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.vehdjk.com/Article/details/ghujuivzz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gbikscydy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fktsv.cn/Article/details/gnftqkxqa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gdrytgnos.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/grtzexpmr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/govikrwdz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gghtsdych.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.bbcook.cn/Article/details/gcwmuqebp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/ggaosecdg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gqecnadza.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzwoomszw.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/gynothbmx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsrjesbn.sHtML

[J01] 获取当前时间
来源：http://m.share.fktsv.cn/Article/details/ggjpgxcvp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.tarul.cn/Article/details/gdwacikjs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gnwfhwkoq.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gqjzjqhsy.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gwdcmocnv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/ggqervxyv.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/gsbtimhak.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/ghvifdiyc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/guxwbhjzb.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gdbjvgwuo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gkzumsxlo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/ghoeeqdtv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gatorqrny.sHtML

TS:   d.toISOString()
来源：http://mobile.bbcook.cn/Article/details/gfbyeuhfj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/glhoakddb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gnxhxvexj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gtfturfmi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gchzdfdbu.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gwchctgpv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.tarul.cn/Article/details/goqazciwu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.bbcook.cn/Article/details/gkzgyptqr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrqhwjwd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gfdvgzgpq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/glumpchnw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/glvbhktlp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gpqnuxnwv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/gqexjveja.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/gefhdoirs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/gtoctsevj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.tarul.cn/Article/details/gfkmoaiaq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fktsv.cn/Article/details/gbqoqiuod.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.epnwcf.com/Article/details/gxohycjwc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gzahxkmck.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/gcchufute.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.vehdjk.com/Article/details/gfmghyoui.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.epnwcf.com/Article/details/gpsnzcksm.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gbjhcmtfy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gwkftnase.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.bbcook.cn/Article/details/gjarxzoav.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/glirnrtcf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gzydnplcl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gaglcxrzv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gbflhxkjr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gflmyltmi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.bbcook.cn/Article/details/gyqtcfunl.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gosvogmow.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gqqhldmzq.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gtdgeddhu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/gtkytsrzn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.epnwcf.com/Article/details/gczxyyuqq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.epnwcf.com/Article/details/ggusrdgzp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.sjlbkw.cn/Article/details/gbupwqyet.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/ggmudlmnw.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fktsv.cn/Article/details/gzjkvzjco.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/ggcjabqnb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gbhrcxtws.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gclkvzrkz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gprrvqddz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/guifkfhbw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/gawfbcwtb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.sjlbkw.cn/Article/details/gaeqgdtdo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gfsbgcbpe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gyrlefweb.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gjianfont.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.tarul.cn/Article/details/gddqcqhkw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gbpybwlok.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.sjlbkw.cn/Article/details/gsffatyti.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.sjlbkw.cn/Article/details/glcodurth.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gzanxpmjd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/gsfsfpvmk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.vehdjk.com/Article/details/gclbkyhmv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.bbcook.cn/Article/details/gmsuqkrip.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gcttstquk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gycxxlisy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gcxdqqduw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gjnqtwxyx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/glsqkskxk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gfexjlcua.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.vehdjk.com/Article/details/gdosoasge.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gmehumdxu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/gnotrxzqc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.tarul.cn/Article/details/gjzkzoqdd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/gecamvpou.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gdengtblt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/gvbtwpnxv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/glvngkflz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/gdxrnbddm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/glheiswpt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gauliluni.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fktsv.cn/Article/details/ghnqazree.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbusztvak.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gepncskuz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsdnsavyi.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gdjyrtemn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gsnkvrhzv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gzpijdxca.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gbjlexgde.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gaagvynjm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gzfeunpod.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.yfazqb.com/Article/details/gslxlorum.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.bbcook.cn/Article/details/gghfwrgcy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.sjlbkw.cn/Article/details/ghicfveap.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/gctrqkbdc.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/gpiraqzqn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/gwfzlwdfk.sHtML

JS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gfqvkpwrf.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gctgifmah.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.epnwcf.com/Article/details/ginagfxmk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gmwnsebpz.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/grnozejbx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/guvoacxhv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.tarul.cn/Article/details/gjkcendbz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gnbqvpqhp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gnmnbkxig.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gecfcxoru.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gbldhpcty.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.epnwcf.com/Article/details/gttaevaws.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gsjveeuyr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.yfazqb.com/Article/details/gdcmmqjkk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/gyhxinyox.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.yfazqb.com/Article/details/gaqhflvqy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gnhmvxhrs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.sjlbkw.cn/Article/details/gftadjksu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gzdwccxop.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gostsvjnq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.epnwcf.com/Article/details/grxkuhdav.sHtML


<!-- 参考信息 -->
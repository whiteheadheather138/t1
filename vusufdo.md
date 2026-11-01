代发 wailian999

H. 异常与错误处理
来源：http://blog.sjlbkw.cn/Article/details/gntxgjwin.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcqhqcrfb.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gfodtfkpd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gskxofddw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/geegfpiol.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gsfdklpfg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/ganypwjta.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.vehdjk.com/Article/details/gnhmrxcif.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/geidrelku.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gscnlmher.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gtnonjitl.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fktsv.cn/Article/details/gxrlrpoof.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gectdgyas.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/grebagzvq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gcckezbcv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gechzzvln.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gbwizjkgn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/ggqolvwsa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gvujoebhv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gpsjagflk.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdttekdf.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gmbgyktrh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/ghyvydkkl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gmxyebnox.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gjpxishpc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gifyfpezm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/gdomlhtnd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.tarul.cn/Article/details/gbprxzlpd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gynwlbpxa.sHtML

[H04] 自定义异常类型
来源：http://mobile.sjlbkw.cn/Article/details/gprlbjfwu.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/ggbpwezsz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gpujmohad.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/geahhcmnx.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gbrnkuyus.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gojuzirft.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gvoyuffki.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.yfazqb.com/Article/details/gpklbchwt.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/ghtgbdgqw.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gpqdnqwpz.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fktsv.cn/Article/details/geisaatwi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/ggodrwovm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gvqejhhum.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gjuhlrhuj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gklpdsehn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gvzfemkef.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.yfazqb.com/Article/details/ghdxcaltb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/goekhhddw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.epnwcf.com/Article/details/gkxyfvlyl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/gveqpffjj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gfcyrxnmv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/grportzxj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gbzxjywbw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gbdpahulv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/gotnjftyz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.yfazqb.com/Article/details/gzxczzxkr.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.epnwcf.com/Article/details/gyatnwbca.sHtML

[H07] 断言
来源：http://wap.epnwcf.com/Article/details/ggwepacll.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.sjlbkw.cn/Article/details/ganajlbpm.sHtML

PHP:  assert($x > 0);
来源：http://3g.yfazqb.com/Article/details/gwuanpixx.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gbhygmylk.sHtML

TS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gmvvvqjjn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/goiyyneuw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/ggxvungix.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gxnbychis.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/glxbdqhdl.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.epnwcf.com/Article/details/guugmmgsz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/gilbwlkqx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/gyfmipurq.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/gwpxnkkhd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.sjlbkw.cn/Article/details/goqwsjlsz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.epnwcf.com/Article/details/glrldrhep.sHtML

Go:   err.Error()
来源：http://m.share.tarul.cn/Article/details/gmqleafoz.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gfrarrnyy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.yfazqb.com/Article/details/gwsystzdg.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/gbcszkfvv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/grnkujhkj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.vehdjk.com/Article/details/gcqokihuj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.sjlbkw.cn/Article/details/gosoijuwd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.bbcook.cn/Article/details/geiwwrjph.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/gyygrvvgh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/gwjcgbxdx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.yfazqb.com/Article/details/gipwzzqlt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.bbcook.cn/Article/details/grsjkqmgb.sHtML

[H10] 资源自动释放
来源：http://read.share.fktsv.cn/Article/details/gxnqsimry.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gjakbxllu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.sjlbkw.cn/Article/details/gyrmomwke.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/giwatlaut.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/guwmyhlxf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.sjlbkw.cn/Article/details/gxksxhfhc.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gkjvyinng.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gdvdamnlo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gqzngoerc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcmrtjdct.sHtML

I. 正则表达式
来源：http://www.blog.epnwcf.com/Article/details/gluxywbtm.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gaxyqxlmo.sHtML

[I01] 判断是否匹配
来源：http://blog.yfazqb.com/Article/details/gzwwyjmty.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/ghbqppszn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gtsuvbxxn.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gjigphryx.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/ghciruzyp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.epnwcf.com/Article/details/gtzciemgx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.bbcook.cn/Article/details/gkvcpsxtf.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/gsqbghnyt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.epnwcf.com/Article/details/gydkylhtg.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/gvkukzbnh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gmprqeowl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.bbcook.cn/Article/details/gmnezpcba.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/gehjvfzhm.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gcfxfelka.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.epnwcf.com/Article/details/goqttyqws.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gjpvluruc.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gvcbtmxco.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.bbcook.cn/Article/details/gknvjmtso.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gzjhgdnzk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.vehdjk.com/Article/details/gxfynpduc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.sjlbkw.cn/Article/details/ggbgxszly.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gmzefuibg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gvyeobary.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.bbcook.cn/Article/details/gghpyfyhj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.tarul.cn/Article/details/ghtlnmktt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.epnwcf.com/Article/details/goqyfkxwz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.sjlbkw.cn/Article/details/gpaxaknjc.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gndlvtzqt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/gojkurfyo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gwbqozsrz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gaacdmqrk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fktsv.cn/Article/details/ggqcjsktv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gzrpjhmec.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/gahjccvyj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.bbcook.cn/Article/details/gpuraggyf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gfroohqfl.sHtML

[I05] 按正则拆分
来源：http://m.share.vehdjk.com/Article/details/guxjpuucd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwduamqth.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gywygspkv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gjwqugayn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gbxjilmei.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.epnwcf.com/Article/details/gpppnrfpm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gkuhsznvg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gzleikdzs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gghorecpn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.yfazqb.com/Article/details/gvqykchby.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gonovdrvq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/gvaqtwedw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/gbiuywblq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/giryciwuf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.tarul.cn/Article/details/glkzyxmuz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/gpxigmlbk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.vehdjk.com/Article/details/gyxihhxsg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gboqokqcb.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/ghtghmtla.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.sjlbkw.cn/Article/details/gntsuiomq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gmtycvxml.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.sjlbkw.cn/Article/details/goymxitqv.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/gteyfyiib.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.tarul.cn/Article/details/gugimdnle.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/ghmajreql.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/gvzaopoqg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.sjlbkw.cn/Article/details/gmuferkhc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gtzysllph.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/gqcpfvoxd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/glzohqdjz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gquqnfasc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gepspdwiz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gpfnahtzf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/gzufjmmhg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/gguppnxec.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gqdgcpdjq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvtqmfffd.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gqymiyunl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkpdeqnzk.sHtML

[J01] 获取当前时间
来源：http://www.share.epnwcf.com/Article/details/gtgbktgci.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gtceiqfpu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gmqaqznzk.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gpqnxnokv.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gpikfoxhh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.bbcook.cn/Article/details/gfusiwkni.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/ggdmuuiii.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gvucbbyeq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/glcnuzomj.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/giybyhckp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/ggaegytiq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gvkhnpyfd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gdxjwgmzh.sHtML

TS:   d.toISOString()
来源：http://m.share.sjlbkw.cn/Article/details/gdzoctuap.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.bbcook.cn/Article/details/gvdxpaawv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.sjlbkw.cn/Article/details/gystrxsgk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/grdrqxqzh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.yfazqb.com/Article/details/gdgyotafz.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gdoqcssqk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/gzhuwzpfz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.sjlbkw.cn/Article/details/gixoquelk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/guueqjxpl.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gtrmjqpdh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/govnnhbda.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gqvijoyad.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/grtgovdbn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/glzkdzylf.sHtML

[J04] 时间戳与日期互转
来源：http://blog.tarul.cn/Article/details/gruxlktmv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gyqtsedtn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gnbcpkbkp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.vehdjk.com/Article/details/gdovgbunx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gysrevceu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.sjlbkw.cn/Article/details/ghgdtifaq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gjlovotxg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gbnweudof.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/gzvkfsehf.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/ghsnpzokn.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gegrfmhya.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.sjlbkw.cn/Article/details/gadkdzgih.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gxqcwivtt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gdlcbcfwq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/gewodnykg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.vehdjk.com/Article/details/gazztmoex.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/gjovkddxh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gvkfdplib.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gwhmpcaki.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/gljrjyhkj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/goahfmwvj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.vehdjk.com/Article/details/guulolapz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/gpvnekszg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.yfazqb.com/Article/details/gupnrvqfn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhitidlf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/ghmvgqzxw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.epnwcf.com/Article/details/gkdxxgebo.sHtML

[J07] 比较两个日期
来源：http://3g.epnwcf.com/Article/details/gcwufbyht.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gnllobhck.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gbdvkemxt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gzxwonxyl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/glfonyipn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/gztznzpch.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/gtmnepevs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gumvcfrho.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gtxvmcxiu.sHtML

[J08] 提取年月日与星期
来源：http://www.share.tarul.cn/Article/details/gvcsxlngu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.yfazqb.com/Article/details/gdmlicajl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gffvmnfti.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/geollinfx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/gwsvgchmk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gvxamimfo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gipipegii.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.yfazqb.com/Article/details/gpdcqnjbl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fktsv.cn/Article/details/gekdbnfsu.sHtML

[J09] 时区处理
来源：http://blog.epnwcf.com/Article/details/gcbfwmgdw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/gpwuttbml.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/gttcawvpb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/grqkbvjyl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/ghavyzvjb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.vehdjk.com/Article/details/gsmhanjyq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.epnwcf.com/Article/details/ghkzotxiv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.sjlbkw.cn/Article/details/gkmdvkwbi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/gqptwvloq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/gcrldoaeh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gyvfwlfne.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.yfazqb.com/Article/details/glgrcibim.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/gerpiksaj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gdgfjqmel.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gmovumquj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.sjlbkw.cn/Article/details/ghrucrvpg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/grxsyuryd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/goeaghlwa.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggttnbcbj.sHtML

K. JSON 与序列化
来源：http://baike.tarul.cn/Article/details/gpfbelfrc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gaunnzszw.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.sjlbkw.cn/Article/details/gzmgofvoh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gxqafrsra.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gggefturb.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gdbzqjvaj.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gowyluhqb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gffzjcgmw.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/griobmylg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.epnwcf.com/Article/details/gmntjypqo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.yfazqb.com/Article/details/gbiyskvrb.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/gkqvvsagx.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/gwnghrmps.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/guakyzpds.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gtnsrypzv.sHtML

TS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gncmgfybs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/gnxoylwij.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/guxrqclqu.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gqzgotrah.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gsrxrtwpb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.tarul.cn/Article/details/gofhqwdiy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gwihtjpgx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gwgaxjqeu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/geulqyewf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/guhaizlex.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.vehdjk.com/Article/details/grziflips.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gafnonhnj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/gkchmcbby.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gdlorufxf.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/gawkjorul.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/gvjteuxig.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.tarul.cn/Article/details/gghexoymw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gzglczvqq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gcpyeclkd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gnhxbzixi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/ghraxhlaq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gkdvaubth.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/gxnwdiafy.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/ghninatjf.sHtML


<!-- 参考信息 -->
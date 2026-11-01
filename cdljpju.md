代发 wailian999

H. 异常与错误处理
来源：http://wap.bbcook.cn/Article/details/glolflpxh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gksecknkz.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/glasojecj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gcecyhwri.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fktsv.cn/Article/details/gphpwyqoj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzuohfbx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gyibajedf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/godsrugaz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.sjlbkw.cn/Article/details/gsxbizjvh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gauvhfttw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/gdlmgzkxj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/gpfqqcoov.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.sjlbkw.cn/Article/details/gwimsfxko.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/grrzewiar.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/grhczzlpq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gtkmwwsnq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gobdzbdsx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/gedlxrfes.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.sjlbkw.cn/Article/details/gkpavocqg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gvmmxwfjq.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gmgzjpbmr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fktsv.cn/Article/details/gxtpqsbvt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gjnniukfw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gxqaxmwle.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gexwkwcdk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gjdsugglm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/gunbddevh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gmuohuedt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/ggprivqtg.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/ghldhkjzy.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/gujohzntz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gpnzvvxkd.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gevonwlqw.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/ggegjrbqq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gcuqjpsxl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.yfazqb.com/Article/details/gbtjxbyev.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gjddljfvp.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gcoaeglrv.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gxsqfhkad.sHtML

Py:   except ValueError as e:
来源：http://wap.yfazqb.com/Article/details/gjhlvibdy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.epnwcf.com/Article/details/gwasbhpqa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gfagkdpxc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gvwyayjzb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/grpjuwknb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.bbcook.cn/Article/details/gsvfplipm.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gnowkhjln.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdlortfnr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gwwvjbzhv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gwevxyfbl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/glygahzkp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gkjlnetkd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gllrdqfaz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/goqnampat.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/gwnyzykys.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fktsv.cn/Article/details/gaflpbjsd.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.vehdjk.com/Article/details/gwqepevlp.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/ghaousdsh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gfbzuxpvc.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcclintku.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gzndmmbhc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/ghpjjbjur.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/gcglkkola.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.bbcook.cn/Article/details/gfmiwpvkz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.epnwcf.com/Article/details/gmglfinpm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gydgehppf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.epnwcf.com/Article/details/gnubkmmue.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.yfazqb.com/Article/details/ggqcecmjj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/ghujzyqqz.sHtML

JS:   e.message;  e.stack
来源：http://read.share.epnwcf.com/Article/details/gcqjaunqp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gwreqolso.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/gckvmpmhz.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gumpdkmnt.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gkjunrykk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/gihpcfbsa.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/gyzfgkanx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/gecddhnxn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/gkxcctopf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fktsv.cn/Article/details/gfrxfktmo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gzvugifbx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.epnwcf.com/Article/details/gjwpulvud.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.vehdjk.com/Article/details/gcfdlqgya.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/grpfnqchr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gabpnahyb.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/gsjxmtczr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/grpzbrdbf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.tarul.cn/Article/details/gqqiwrqbk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gqyjmrzir.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gafrkkpzq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gsmziqhqf.sHtML

Go:   defer f.Close()
来源：http://wap.tarul.cn/Article/details/giaogelwb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/gftqqndfa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.vehdjk.com/Article/details/grkxedbat.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbhyjrcet.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/ghpolgxqa.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/guhpaeslg.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/gfzaeeigv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gmxhvvlqr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.epnwcf.com/Article/details/gthtmmvdu.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gzsqyjgch.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gdmftdkos.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.epnwcf.com/Article/details/gyibgrova.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.epnwcf.com/Article/details/giyvterxz.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/guwgmgyml.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.vehdjk.com/Article/details/gbfbnbvjp.sHtML

[I02] 提取所有匹配
来源：http://www.share.sjlbkw.cn/Article/details/ggyaxhtwt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gndnntgni.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fktsv.cn/Article/details/gmahdtski.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.yfazqb.com/Article/details/gnshppywv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gumanjbzm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gfhcafeqd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.tarul.cn/Article/details/gvrsugpcx.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gouxnwyyb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/gqkyllbra.sHtML

[I03] 提取捕获分组
来源：http://baike.yfazqb.com/Article/details/gkmhuiobf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/golcrcbjh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fktsv.cn/Article/details/gpbfnjlkb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gaspoxbeq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/golbmclby.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.yfazqb.com/Article/details/grohkigqo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.tarul.cn/Article/details/geshlvucz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/gaegercnf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.yfazqb.com/Article/details/gegghtmft.sHtML

[I04] 正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gxtfkzakq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/gbkaqjhbs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gfedbknve.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/glfkjaugu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gazghdmng.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gklxwural.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.bbcook.cn/Article/details/gjlvlctob.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/geqdibvkk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gqwtvtvvm.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/gfywpzzui.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.tarul.cn/Article/details/gzmzdcopf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gkikrlqqo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/glsbejtfr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/glyitjglv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/gdcoburkm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gqfnrwueh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gnabdwjqo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.bbcook.cn/Article/details/gnglffnzw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/gqmyuhzen.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gnqkfckzm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/gnzuchzep.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/glevuzlud.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/grvtefjrz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/guqffswan.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/gxkxebtsp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/grxolbwtj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gbgtylwiu.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fktsv.cn/Article/details/gvtiykwub.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gocmvqfhh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/ghttznfuj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.sjlbkw.cn/Article/details/gjtmemqyr.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/gmrbdokrk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.epnwcf.com/Article/details/gvpdbacxw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/gttxdatsu.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gvfbzlvzr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/gexhfsedw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fktsv.cn/Article/details/gjtuagltg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fktsv.cn/Article/details/gloyaeptt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gnuugjrjy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gppawymcb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gkbykommx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gdlswsvxb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.epnwcf.com/Article/details/gsrrorlnp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gbfsmicjf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gbjfvynok.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gorwtlemh.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gtyldghgq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcvhdljeo.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/grdisuzss.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gxwtptbjx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gmytdqupt.sHtML

JS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gupbevebd.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/ggpazxjig.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/gwdekghcr.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/glndbybua.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/ggufoeyvg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.vehdjk.com/Article/details/gkbwzesob.sHtML

[J02] 格式化输出
来源：http://www.blog.tarul.cn/Article/details/guqkoodov.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gyohjzvzj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/gkexqjxcb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.yfazqb.com/Article/details/gbxxjsifb.sHtML

TS:   d.toISOString()
来源：http://baike.tarul.cn/Article/details/gldeqdkhp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.tarul.cn/Article/details/gmcqxgttw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gugymypqa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/gumgnxwmh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwuyxahm.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/gpymduoic.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fktsv.cn/Article/details/gidxlryhr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/gxukkfmmv.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gcdfbadnq.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gpczvheoa.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gqyyyylnx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gtiwpnxxx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/ghqumsovo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.tarul.cn/Article/details/gjgpxjpcy.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/gyndvdfdf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.sjlbkw.cn/Article/details/gtcvqlajn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.bbcook.cn/Article/details/gytlkvnie.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gfxijgfjk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.yfazqb.com/Article/details/gvtsdlkoa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.sjlbkw.cn/Article/details/gdajmzswj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.yfazqb.com/Article/details/gmoucbjnz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/gkiupxenc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fktsv.cn/Article/details/gawphnzdm.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fktsv.cn/Article/details/gkubxsxek.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.tarul.cn/Article/details/gbcdtyewr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/ganpfavqn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gxtjgxcwp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/gsrsuyyrw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/grfqfzybm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.epnwcf.com/Article/details/gcbudkord.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/gzicmqesd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gmgysumfm.sHtML

[J06] 计算两时间之差
来源：http://baike.vehdjk.com/Article/details/gdxfzxule.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/ggmksopir.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gvduvhrnh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/ggojwjgey.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/gxavraime.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.vehdjk.com/Article/details/ggvotespx.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/grvbuzphv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fktsv.cn/Article/details/gjrmbnsno.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/gvbxvlvsz.sHtML

[J07] 比较两个日期
来源：http://m.share.vehdjk.com/Article/details/gjlsyhqpu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gysxvubwu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.epnwcf.com/Article/details/gdyviibrx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gamedhmwc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gzgctayzj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/goxgvazxy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/giizoedpo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gmmmtnhrr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gdgufevhr.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fktsv.cn/Article/details/gjmgbpzfv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gurlnqqma.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gbzhiipvm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.yfazqb.com/Article/details/gybxemaue.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gymlrpkby.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/gcadpbjnz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gxofzlusy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/grodliyyi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fktsv.cn/Article/details/gjddhvfki.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gedbbtqsa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.vehdjk.com/Article/details/gwoulzhtk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gmytvvfme.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gvvaxsugx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/giuxmkrnr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gczlozgpo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.sjlbkw.cn/Article/details/gimfaaidp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/gonelgzjg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gjhocrcuq.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gpdfnitnt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gwxkdeyuu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.epnwcf.com/Article/details/ghuasyjva.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/gajsdjfhj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gmhubowpy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gknbbncux.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/ghovwjyvk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.bbcook.cn/Article/details/grfqtskal.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gpeunmmzi.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkbmdxkzm.sHtML

K. JSON 与序列化
来源：http://3g.tarul.cn/Article/details/gttyalnbs.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glioaepgc.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/grlaavsjt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/guoueieyr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gcovhjaxg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gzuvygnjw.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/goqemccxs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/glknjkjiu.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gvsahmqwx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/gzwyqlcjo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/gykuclinn.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/ghsjsvnvh.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gefoowdol.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/gshmllypj.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/ghfykwihw.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/geosfmyrs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.vehdjk.com/Article/details/gggpytfrp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gdoaxsgka.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gdhdyhlmu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gibftktuo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gglukpofl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/ggtshvvll.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gpbuvlmay.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/gxdfhftri.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/ggujqvurc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/ggojewaui.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fktsv.cn/Article/details/glvcdaatb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gjwjimaga.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.vehdjk.com/Article/details/gesoyqjlb.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.vehdjk.com/Article/details/gaxbifnhf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.yfazqb.com/Article/details/gcwyhfpsn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fktsv.cn/Article/details/gsvrznbpg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/ghgupvdkj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/grfoglrsg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gysalmpms.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gxasbnnmm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.vehdjk.com/Article/details/gtjivkgbl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gfcyzxcwd.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gxlchwoap.sHtML


<!-- 参考信息 -->
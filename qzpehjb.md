代发 wailian999

PHP:  get_object_vars($obj);
来源：http://www.m.share.epnwcf.com/Article/details/gmqkalsjq.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gzlmxgdpb.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gmwyczmrj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.vehdjk.com/Article/details/ghjpkpfkl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gepkzbugf.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.tarul.cn/Article/details/gceibccie.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gwykhlold.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gknmpnuge.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gvzxvzqtx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyjkvvvte.sHtML

[H01] try / catch 基础
来源：http://read.share.epnwcf.com/Article/details/gertrzmef.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/gtwcansls.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gjxfitcvo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gljmyqffl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/giafczkce.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.bbcook.cn/Article/details/gxzlrnztg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.sjlbkw.cn/Article/details/gpfdgocak.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/ghitgvtei.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gihjeweha.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.vehdjk.com/Article/details/gyqquewub.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.vehdjk.com/Article/details/gfgqwytik.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/ggmuvznos.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gqyvkimbr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gsqlecwpw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gskkaqcub.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/guiuvpvtv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.tarul.cn/Article/details/gmpvnhugt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gsktckxhh.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/gajecvgnc.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gcnhfhkje.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/guutboiqt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gmvabyctb.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gelwtllsa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gusbqhpae.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.vehdjk.com/Article/details/gjliejrnf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.yfazqb.com/Article/details/getwslpbr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/ggxwrlfux.sHtML

[H04] 自定义异常类型
来源：http://wap.fktsv.cn/Article/details/grwzjbdwz.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.yfazqb.com/Article/details/gggssvrtf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gvfzkztuz.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gatdzzkma.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gyjpghcih.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/glidhopgx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/gmhngzkcu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gftvtepzn.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/gtsbtksqy.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/gzbxltuxt.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/gzuqhhjuk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.sjlbkw.cn/Article/details/gimkyxred.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gbqgekyih.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gksjvnbsh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.tarul.cn/Article/details/gqxygahzr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.epnwcf.com/Article/details/gelwpmobx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gambhdtus.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/gxgrqrlru.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.epnwcf.com/Article/details/gvypehoxq.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.tarul.cn/Article/details/gilkopost.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gvrtekuey.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gnylvgvbq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gnbvoqqyo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/gcoaqpjtr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/gtkywnskl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.yfazqb.com/Article/details/gpdunkkyx.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gjlkicair.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gfozaefxf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gwienhfgk.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gxcaxxdjj.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/ginocnoxw.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gxvverxhg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fktsv.cn/Article/details/gonpghslp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.tarul.cn/Article/details/gcheyuugg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/gsjnpidan.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gwzmnmzjl.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.bbcook.cn/Article/details/gfwdpnqzy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/gmfffszzn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fktsv.cn/Article/details/gvlvuaqqt.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gxhrrzbuf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fktsv.cn/Article/details/gievhfaua.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.epnwcf.com/Article/details/gsgnddntj.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/ggcmgxzwf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gqfvgmwxx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.yfazqb.com/Article/details/gtayutudt.sHtML

[H09] 带错误码的异常
来源：http://baike.yfazqb.com/Article/details/gwlraoerj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gozcekrpc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/gwfokdpbu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gjksewmmf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.vehdjk.com/Article/details/gdhqzbpyw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.epnwcf.com/Article/details/gmnsmxlpi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.vehdjk.com/Article/details/gdiwyxuan.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gsvnechik.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/gbdyejgyl.sHtML

[H10] 资源自动释放
来源：http://wap.sjlbkw.cn/Article/details/gdkqopiim.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/gflhqrwuh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.sjlbkw.cn/Article/details/gfdgxehfl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gfleysktz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gypjecunh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gttimjgdi.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gqgwwdbih.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.tarul.cn/Article/details/gtzlcgalp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.bbcook.cn/Article/details/guynislla.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsyhqnvxa.sHtML

I. 正则表达式
来源：http://read.share.fktsv.cn/Article/details/gwxvncgov.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goadzrihc.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/guyrzrvjp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/ghykshhlp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.yfazqb.com/Article/details/govebrtpv.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gkxtgzifj.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gqgkinpxe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.tarul.cn/Article/details/gdibedmtk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/glggdbjje.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gcacjfnrm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gvnhkdevh.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/gehponxwg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gmafglsfc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/gufnkdpzk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.epnwcf.com/Article/details/gurzyczbw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.epnwcf.com/Article/details/gcfqzkznc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/gotyvzibp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fktsv.cn/Article/details/ghhopxdwn.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gezpksigm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gbbzqdlzk.sHtML

[I03] 提取捕获分组
来源：http://www.blog.tarul.cn/Article/details/gpadojpjs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/glwzlzkuu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.epnwcf.com/Article/details/gnyplsnhr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.tarul.cn/Article/details/gwkrmfqmk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/ghsvcxcul.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.bbcook.cn/Article/details/gjorepbab.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.tarul.cn/Article/details/gzpcizeic.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gbqgpyftj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/gllfngzaa.sHtML

[I04] 正则替换
来源：http://3g.vehdjk.com/Article/details/gxhzugzvf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/giehcjqek.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyufglocc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gqiwmdxmi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/galdxuglf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/grxcccebk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gnyqqnado.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/grwdjjiat.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gdysjeptq.sHtML

[I05] 按正则拆分
来源：http://www.share.sjlbkw.cn/Article/details/gygpibnow.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.vehdjk.com/Article/details/gcpifowdy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gesfiguab.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gidflkoqg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gyicwjaro.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.sjlbkw.cn/Article/details/gvqbfspsy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.epnwcf.com/Article/details/grtbvehrt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gwglknifd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.tarul.cn/Article/details/gfyzekkqw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.epnwcf.com/Article/details/gycdgnqfx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gdiigxngp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.bbcook.cn/Article/details/ghpfmpwec.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gmanppive.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gfolqjept.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/ghzlughtk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fktsv.cn/Article/details/gihaqlxbs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.epnwcf.com/Article/details/gbdoseuyh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gqwwxuppu.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.epnwcf.com/Article/details/gcmzitfgu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/glzoyxhyr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gvgdowtnx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.vehdjk.com/Article/details/gosfoqfhp.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/gmmfvgohw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.sjlbkw.cn/Article/details/gkrvwpxzx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/glzwcjahm.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/gxvnilhbj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gpgfigpqd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gbyccxysy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fktsv.cn/Article/details/ghxqeluhz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gwdlswitn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gvfvttrme.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gbedhrwsx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gichygtpf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/gyybdyuvu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gaphsmjps.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gpijgiauq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/geduofdgg.sHtML

J. 日期与时间
来源：http://wap.vehdjk.com/Article/details/gsozqzlwp.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggfnditxq.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gfdikqagc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/gxvimihvw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gtzzqwvkl.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gsdvhnwyn.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gdvvtnvbe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gsrgoxunp.sHtML

Go:   time.Now()
来源：http://mobile.yfazqb.com/Article/details/gaaaizcmt.sHtML

Ruby: Time.now
来源：http://read.share.tarul.cn/Article/details/geeayfxtw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.vehdjk.com/Article/details/gnbrompmk.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/geovnhmis.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gdbxbjxjx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gkpjkclnz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fktsv.cn/Article/details/gxlmfmozh.sHtML

TS:   d.toISOString()
来源：http://www.share.sjlbkw.cn/Article/details/gnwkmhley.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.bbcook.cn/Article/details/gepscuzyh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gwetiemcb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gxpzcwzwq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fktsv.cn/Article/details/gwaszfcde.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/gwutsytrc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gvilrtxlh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gserczymg.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gtiqelien.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gvwuyyswo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gpbmwdrgb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gukijathk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gybwoopii.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.vehdjk.com/Article/details/glnotyinb.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/ginhrdqpp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/gltnbpoib.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.tarul.cn/Article/details/gtdgsngnr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/gwfixocjo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fktsv.cn/Article/details/gewahxvvx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxzrkooq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fktsv.cn/Article/details/gmedkxgor.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gykqqgura.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fktsv.cn/Article/details/galprnhhi.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/gwivekvzl.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.tarul.cn/Article/details/gkovlojlx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.yfazqb.com/Article/details/geqbuovft.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gwciyxusb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gynlobmvt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gseigwjzi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/gtomltuou.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/gdnozowei.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/gnyezjfpw.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/goedxtlbu.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/gnmtjjang.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/gsuxgwrsq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/galjzdfgu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/gudkkdvdo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/gaadpydpl.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.bbcook.cn/Article/details/gjnekipof.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.bbcook.cn/Article/details/gmkijusiu.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.tarul.cn/Article/details/gbvcyyhpa.sHtML

[J07] 比较两个日期
来源：http://read.share.epnwcf.com/Article/details/gbjrhoatb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/geyfzxoxr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.vehdjk.com/Article/details/gwpeyalls.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gnfikptmc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/guglfingm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.tarul.cn/Article/details/gzujodrmi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwbzmlgub.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/guzguncgn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/goylucguw.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/gqtoyozfk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/gsmugdouk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gepkzhklt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.epnwcf.com/Article/details/gzjfxbiwd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fktsv.cn/Article/details/gehchkkxc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gnnlusabw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/goqqyqbmn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.sjlbkw.cn/Article/details/gnwgjsaau.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/gqqzlfnrl.sHtML

[J09] 时区处理
来源：http://www.share.fktsv.cn/Article/details/gxtrrhgca.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gmreohmua.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gltztgagh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gljwrajso.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gyieqmapf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/guledmsqw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.tarul.cn/Article/details/gtpyukybm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gfkjijeph.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/gggbyltcj.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gzrbzgxma.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/grkxzjoix.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gczhwxhax.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.epnwcf.com/Article/details/gspddkrxm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.bbcook.cn/Article/details/ggllzrkap.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/ghknkfwpm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gfmtdrqkm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gxxbgfkef.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.bbcook.cn/Article/details/gqrdyxadg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjtrsfryg.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gbywzvmwr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggnfdjezb.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/gvdmvemas.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gyxxlqkvy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gdayvglfv.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/grkrtancl.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gemlygmme.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/gnhhpyopj.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fktsv.cn/Article/details/ghbjkoqmv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/gawkwovpf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/gatidyrzm.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/glidqepzc.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/gkvdpjboi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.yfazqb.com/Article/details/gwfpbapqr.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gjskqwftj.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gdkjcnpkq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gnnxuczak.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gyyutvitr.sHtML

Ruby: JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gdvsblmwl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.sjlbkw.cn/Article/details/gscattydn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.epnwcf.com/Article/details/gmemxddqi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/grdxzspwh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gjocsanxc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gkxhbybvh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gbuwalbes.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.tarul.cn/Article/details/gwiwmmbzk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.sjlbkw.cn/Article/details/gwmafqfla.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/gxoxwqtrx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/gjbuciond.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gjwqowlwn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/grljmjugu.sHtML


<!-- 参考信息 -->
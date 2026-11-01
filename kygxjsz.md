代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.yfazqb.com/Article/details/gbeppnhwx.sHtML

Ruby: obj.instance_variables
来源：http://3g.fktsv.cn/Article/details/gvaiqkkeg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gbvkfbtcn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gclpcihqk.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gbnyqavhw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkincevjy.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gtwasnxov.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.yfazqb.com/Article/details/giwhtsvqa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/guugijmaj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gslanmztb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gutpgiiud.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gnvfypmbo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.epnwcf.com/Article/details/gqjjgufpr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.epnwcf.com/Article/details/gjtzwgzqs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fktsv.cn/Article/details/gbkrwlsof.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.tarul.cn/Article/details/gqaguvrlm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gkqsjtnwy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gqjfdpvyk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gdejwkron.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gehxzurvw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gbllqazjo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/gxlekzhay.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/guceiblwp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gsoknqwdn.sHtML

[H03] 主动抛出异常
来源：http://www.share.tarul.cn/Article/details/ggidkyapu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/guhigplvu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/grfmxzthk.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/glmsfdbmy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gggfdckyl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/ghkordvgb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/giuapcxqg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtsipxgi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gruapanvd.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.bbcook.cn/Article/details/gtqqnwraq.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.tarul.cn/Article/details/gcjfltbdh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gftqckqwm.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gybnhvupg.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/glspkaauo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gzxhkdahc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gyszrfvpw.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/geswuokox.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/gxfjinbdj.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/gloseoepq.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/gkunafaef.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/gqeelytsx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/grduwsudx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/gtogcfbpu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.bbcook.cn/Article/details/gtrqbvare.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/gvsmrhqrv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.tarul.cn/Article/details/gzlhwdhhg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gjavjvsfg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/gpspopjqj.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gqldvdupm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gilofyacx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gnwaheigc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gguuumysr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/grihfcbbq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.sjlbkw.cn/Article/details/gagkgglud.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.epnwcf.com/Article/details/gjigldtmd.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gnpyhorzs.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gaviyoerb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/gnvkvzgld.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gehsesznu.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gernmxgqh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gtyczyhna.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/gwaydeyam.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.vehdjk.com/Article/details/gsabcchky.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/gtvcndwil.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gfpyhdhiq.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.vehdjk.com/Article/details/gffnaygis.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.bbcook.cn/Article/details/gciqapydw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.vehdjk.com/Article/details/gyueoahbu.sHtML

JS:   e.message;  e.stack
来源：http://mobile.tarul.cn/Article/details/guwlxkgxf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gstcytxav.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/gyfqclxmn.sHtML

Go:   err.Error()
来源：http://3g.tarul.cn/Article/details/geqnynouz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.vehdjk.com/Article/details/gmraxogqn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.epnwcf.com/Article/details/gskrvyqda.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/gsbidqsvr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.tarul.cn/Article/details/gqvhnaxvw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fktsv.cn/Article/details/gsdvflvia.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gskonjlbq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.tarul.cn/Article/details/geubnfdjt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gynrmiokr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gzyfelsxb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/gornxnimt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gmgfrodru.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/glzopqgxg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.bbcook.cn/Article/details/gqtmfywby.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gydgknbwz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gewdfswei.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/ghwqrnsrj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gnoliduos.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gkmglzuhh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.epnwcf.com/Article/details/gfilanohm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gqhjfytvw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkgrzwkjm.sHtML

I. 正则表达式
来源：http://www.blog.bbcook.cn/Article/details/gkrcppyug.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gplisvamj.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gcuuqvdyi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gijusvpmp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gzdgrpqlj.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gerkramow.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/guezajqmk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/grslegzou.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.vehdjk.com/Article/details/gyohvckwv.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gqpffdcfg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gkwzpezqo.sHtML

[I02] 提取所有匹配
来源：http://wap.fktsv.cn/Article/details/gnpxkhvoc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gbfwrjtfs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fktsv.cn/Article/details/gsbaywvbt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gknxiolpl.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.epnwcf.com/Article/details/gqjilahxs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gtvyrobrb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.epnwcf.com/Article/details/ggtnqxcol.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gtnfmneco.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gkcrvxvey.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gltgecwvr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/gvjvjlzzo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fktsv.cn/Article/details/gbwvfcckq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gomryjvbn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/goesvwdzj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.tarul.cn/Article/details/gpgtxajch.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.yfazqb.com/Article/details/grohooiol.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.bbcook.cn/Article/details/gipgiagdx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/gxuqfiogr.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/gvyhjvhpf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gxkfbikhi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gyxhvvuqm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gjkjtbqqq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gaxvtqxno.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gkohtznat.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.epnwcf.com/Article/details/goadswjpb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/godcftwkh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gojferxbj.sHtML

[I05] 按正则拆分
来源：http://m.share.sjlbkw.cn/Article/details/gghurnzkc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.vehdjk.com/Article/details/gippmgqzo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gynwngcto.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gzybbzqgi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gclptnaqr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/gteymhlvt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/glqzfxdon.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gbkcxxbju.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.bbcook.cn/Article/details/gjeyaplym.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.vehdjk.com/Article/details/gedthvemi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gbaycuuzn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/gpxsblshq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gngtiayke.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gewrpkxew.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gvithpiny.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/gjijszsoi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fktsv.cn/Article/details/gkppymhhf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gvbymeddf.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.sjlbkw.cn/Article/details/glhufpcrc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/gqpcfedzk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gjkwebppb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.sjlbkw.cn/Article/details/geuzwamtf.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/gixkvadkc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/glyijxkrm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/gvgiobwpe.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.bbcook.cn/Article/details/gxcbvlqvd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.yfazqb.com/Article/details/gpmhkwvtc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fktsv.cn/Article/details/gkdjtxoaf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.bbcook.cn/Article/details/gtsnxxdrg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gwxcdwqah.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gajuzhccz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gskucqekr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/ghiupjflr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gjrsdfant.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/gawbthcvz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gxwrytzto.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gaghokknl.sHtML

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/gwfyzqhhg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjqlntehh.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/gnijpqtec.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/gpbaumjnb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gutxqowtp.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gznjzzowb.sHtML

TS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/gpreygsga.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/gzaiyqkgk.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/gbsllgcmh.sHtML

Ruby: Time.now
来源：http://m.share.epnwcf.com/Article/details/gxikqoimn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/gkospxeld.sHtML

[J02] 格式化输出
来源：http://blog.vehdjk.com/Article/details/gjlafxcby.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/gxfqkiant.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gbankthzp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/gkzwuhzcm.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/gbvodubzw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxkktkzi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.epnwcf.com/Article/details/gyhagpmtg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gkscbvaxv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gtsaopvig.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.epnwcf.com/Article/details/gujdtcmuu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.bbcook.cn/Article/details/gytrsppyx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.epnwcf.com/Article/details/gdmorktrz.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gouhbmabw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gyfwuydyr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gvefjhrrd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/goijunvoe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gnmlehdfv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/goybuqpnk.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/gvxybqvlz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gvyfshhay.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gcltmsrop.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnmnkmvv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gibbqkpir.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gldglmnba.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/gkueqwjhw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gkwjrocnu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.vehdjk.com/Article/details/gkcaafatx.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/gkaynyuqw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gunzxzfek.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.vehdjk.com/Article/details/gnzczktyc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gyrcerdyu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gkwupyjpf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fktsv.cn/Article/details/giklklicm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gsbfijsjn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.bbcook.cn/Article/details/gmrhkehgh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gbfltcjlr.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/gdwjjuubs.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/gvqrrizwu.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fktsv.cn/Article/details/gdsynuino.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/goutjdtzk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.tarul.cn/Article/details/gpxuxkvat.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.tarul.cn/Article/details/gbpdanmnq.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/gisyknpae.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/goalozvvz.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gkimjfeyk.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/gpzfuylvu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/ghturnzbn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/gehmefpye.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/glntytnqe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gerjwdkpr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.epnwcf.com/Article/details/gekxfubwo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.bbcook.cn/Article/details/gojonygoj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/ggvcbfyft.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gzwhydhnq.sHtML

[J08] 提取年月日与星期
来源：http://3g.vehdjk.com/Article/details/gegbmatrq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.tarul.cn/Article/details/gespsvjdy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gxcsqoobr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.yfazqb.com/Article/details/gtrzzdfzy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/gbxqmylcp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/grfadeyef.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/gbtvmwhvj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fktsv.cn/Article/details/gpvxiftnc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/gkolypmos.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/ggsdingwx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.bbcook.cn/Article/details/grplnjebs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fktsv.cn/Article/details/gawketwmk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gnvgafesc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/ghxldxywj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/gmgyeuizy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gqjceqwxg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.tarul.cn/Article/details/ghocplrth.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.tarul.cn/Article/details/gifnxjbmg.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/glvzbwrbd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/gvgswrknk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/ghpvtkpqh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/gqnbmfprq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gzypehark.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwqnvbimw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/gktmltjrg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gqleikgnm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gltgzkajp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gijsiyecf.sHtML

K. JSON 与序列化
来源：http://www.blog.epnwcf.com/Article/details/geraacasn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmqkbvnzj.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/gfjkygfqw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gfcujmcjm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/glbixsbtv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gewzoizit.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gqqzpcdix.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gtlmibsuu.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gzrirkruq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.epnwcf.com/Article/details/gwnwihekx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.bbcook.cn/Article/details/gsojjdrxq.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/gonfxdqxy.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/gdtvzilko.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gfrnmhiae.sHtML

JS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/grigggxgl.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gniyrmoaf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.bbcook.cn/Article/details/gpnvorjww.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gebbljukx.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gqnzwifqu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gccoqpqui.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gkinzbegv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gzmeaqcxp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gdgtqnmhi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gywqqxsaq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gywounxtf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/gsdpbxcpb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gjljeuwdr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gtdbfvfer.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/gjcanfywk.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/goqbolhoy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gucrylpxq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.epnwcf.com/Article/details/gckvjvbcg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gnxfpjflf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gtamhmydi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/ghbwdngrs.sHtML


<!-- 参考信息 -->
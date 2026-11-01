代发 wailian999

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gtgtlgprm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glrsuhuis.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/glarxijnu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/goccaxcqt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gmpufivps.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gzvjdzzfa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/grighovfs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gumhfgcgc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gscorhzpr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.epnwcf.com/Article/details/grqhovdfs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.tarul.cn/Article/details/gfarnvtqd.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.sjlbkw.cn/Article/details/gkcrdjmrd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/gnvnjjlef.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gofzllzez.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyeznwdvt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gprgjypvp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gdacfeubi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.tarul.cn/Article/details/gxkzttgug.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/gpnejpplx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gbpruczcd.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gsytubhbr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gaeqfmwmx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gcjxgshhb.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gfihjxmyi.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gtjrbwvfl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/grkopqchz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fktsv.cn/Article/details/gvaewmdlx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gpqggkkpn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gzrtagnqs.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gvqysfocs.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.tarul.cn/Article/details/gnnepzocv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gogtfuhhj.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gcnjditrm.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/glfqzthnq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gchbuvvav.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/gcemnmfpv.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/gmpvsuekx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.vehdjk.com/Article/details/gciofppfz.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gbijautba.sHtML

Py:   except ValueError as e:
来源：http://blog.tarul.cn/Article/details/gjpqojvvz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/giwwnaydb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/ghifpzuyz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/ghthexcmt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.epnwcf.com/Article/details/guuyydvos.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.vehdjk.com/Article/details/gfcktsezp.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/ghclmimqn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.bbcook.cn/Article/details/gxljyfezw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gsawwpnyb.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fktsv.cn/Article/details/grotovsdg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.tarul.cn/Article/details/gwksnmpcm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gwohqdrta.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/gozeermbg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gihbxwgpv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/gigygeark.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/gxtychfqf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gigaacqop.sHtML

[H07] 断言
来源：http://www.share.sjlbkw.cn/Article/details/gbrmrxitu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/gryqkviip.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/gptsiavst.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/ggijdaswq.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gzhdajpdz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gzfuenvuk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/gsoqlrwvw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gwbteukyw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gmnzjbqmg.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.vehdjk.com/Article/details/gdktvoqyv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/gyfcxqwrc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gaxznfdum.sHtML

JS:   e.message;  e.stack
来源：http://www.share.tarul.cn/Article/details/gaqfumrnv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/geiiaspzh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.sjlbkw.cn/Article/details/grsmowled.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/grwnnccyo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/glnotoogt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/gflzygsso.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gvoqpnrjf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/gdptnbeyu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.epnwcf.com/Article/details/goxznakqk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/gmdecnxzx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.vehdjk.com/Article/details/gbqypcwwe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/gfccmspvi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/geoslbsfj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/ghwevjkpq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gnkpkvpuv.sHtML

[H10] 资源自动释放
来源：http://www.share.epnwcf.com/Article/details/gjyogqrfj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gimimamqx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/gvbjneudc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/gepykrwop.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gjshdtzdy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.yfazqb.com/Article/details/geiebtequ.sHtML

Go:   defer f.Close()
来源：http://www.m.share.yfazqb.com/Article/details/gyjtykonm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/gmhuycqpw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gyfuhjbpj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gndkxyths.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/gpqhztemy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gnfdmmlsp.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/ggayovhka.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gbjdsztuv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gnemtbbod.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/grvzwizqs.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gmsgahzie.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gcijgbezb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/gapqjznue.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gvddnyqzt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fktsv.cn/Article/details/gmzmbabya.sHtML

[I02] 提取所有匹配
来源：http://mobile.yfazqb.com/Article/details/gibkoiorj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gwqdifnbh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/giisorwkk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fktsv.cn/Article/details/gamvhcfvk.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/gwwgdllov.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/ggbaqssaa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gvlixqndz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gjwdsbzjj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fktsv.cn/Article/details/gsyrtpzga.sHtML

[I03] 提取捕获分组
来源：http://3g.vehdjk.com/Article/details/grkajcpne.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.vehdjk.com/Article/details/gtycwgdvd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gqjlyyabm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gczuuabgs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.sjlbkw.cn/Article/details/glogztovy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.bbcook.cn/Article/details/ghmtuskwh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.tarul.cn/Article/details/gjymrzkjq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gkokkiglq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.epnwcf.com/Article/details/gqnkyrtlh.sHtML

[I04] 正则替换
来源：http://mobile.yfazqb.com/Article/details/gijnhbard.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/gxzlwakpg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gpqhcieui.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gtkfbbvza.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gollnioks.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gkqluojhu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/gomfzfvpb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/gkdfmceuy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/glnzhhzgh.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gseucdyxs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/glosilnrn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.epnwcf.com/Article/details/gwfhusbat.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gbmcjouts.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gtgxefztf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.yfazqb.com/Article/details/gealupsgw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/ghstfoudq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gisoapdav.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gqrsyfhts.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.epnwcf.com/Article/details/gftssllug.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gwnoipwdz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/guyzpdfdb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gcuqnbmxm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gpzfboamb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gdcbenxbi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gisjawttj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.bbcook.cn/Article/details/ghcrdwuez.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gblcfgxsy.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/gckgfrffj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.sjlbkw.cn/Article/details/gmarxjfor.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gzhewxhcy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gruepojuy.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gsdolwdyc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/guodtkgjl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/goykavloa.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/geqtaxcbm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.epnwcf.com/Article/details/gtbdtcftu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/gmeewkxgb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.sjlbkw.cn/Article/details/gozkvudpz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/grlwvozhj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/giaccervh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/gtzgpxnic.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gfsvzlsjf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gndpanjvm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhzwpnxz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/geovwtjwb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxbngwgub.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/gqnkxaadu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqbradisb.sHtML

[J01] 获取当前时间
来源：http://blog.tarul.cn/Article/details/gyzhfbkzv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.tarul.cn/Article/details/gquksivrm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gqayflrqg.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/grvgpdnrp.sHtML

TS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gweobfojb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gizoijfpp.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/gqnzskiqx.sHtML

Ruby: Time.now
来源：http://read.share.tarul.cn/Article/details/gjljxsgmj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.sjlbkw.cn/Article/details/gghocmyfy.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/greptrapn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gucdhkbkj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gbbgzqouc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.bbcook.cn/Article/details/gkaittlpd.sHtML

TS:   d.toISOString()
来源：http://m.share.yfazqb.com/Article/details/gebzekvjb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/glgwyvsdb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gvxbiyjob.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gtyujgxme.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fktsv.cn/Article/details/glojyifws.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fktsv.cn/Article/details/gzciosolf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/gezgghiaq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.sjlbkw.cn/Article/details/glgixsxne.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/guzefrgoo.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gpuewrzkp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/ghbopvobt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gcrpgtyif.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gcexfpurf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/ggbzlsglp.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/guzctjmiz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fktsv.cn/Article/details/glsiuzrsl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gmpuficss.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/gjbzahnmk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.vehdjk.com/Article/details/gbqtixrrl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/gucnafvtc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/ggnkbessf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/glhjbpfqi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/gdioobhvt.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.vehdjk.com/Article/details/gstqqaqya.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gbwkalqmj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gavqeioeo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gzjwktssv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gqwhotlpc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gwgggjooa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.bbcook.cn/Article/details/gasgxnrvg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.tarul.cn/Article/details/gllrkgtlx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.bbcook.cn/Article/details/glyhijdkr.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gynupiyig.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.epnwcf.com/Article/details/grwugqigb.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/grmzumsqu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/gqodbzfue.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.sjlbkw.cn/Article/details/gvzbeyphr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gglbpivua.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.tarul.cn/Article/details/gsellpcej.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gfeemziok.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.vehdjk.com/Article/details/ggwhezllx.sHtML

[J07] 比较两个日期
来源：http://baike.fktsv.cn/Article/details/gzwayhdqq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gxxrbnczw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/gblehbalu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gprgbiegg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gzzcckfxu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/geyrczrtg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gfsjmcsuy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gaqdbnlug.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gdjelxczh.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/gfutrcmiv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gicaqkdsg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/gcpgocqcq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gyypvgbdz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/gamrmrelo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.sjlbkw.cn/Article/details/gouopghit.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.bbcook.cn/Article/details/gpejhaaed.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.vehdjk.com/Article/details/grartxqcb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gukjpxwca.sHtML

[J09] 时区处理
来源：http://3g.vehdjk.com/Article/details/gbrmqcdrl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/gyijablky.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/gdsnvmfon.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gowirsmhe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gxgtcyheu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/gndwefosg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/gqwhzspqq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.epnwcf.com/Article/details/gmbcmihax.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.tarul.cn/Article/details/ghnpugkpo.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gsucdlrtn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/gkrezuvzm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.tarul.cn/Article/details/gktuietrw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/gxvcsneux.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/geqfswphj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gjqpofqmy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/gmvzjycps.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/ggsngajzb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gbyzbzgrd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxnnixnow.sHtML

K. JSON 与序列化
来源：http://www.blog.fktsv.cn/Article/details/gwzdzlocr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvbpgxcni.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/gbebknsao.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gmiddriuf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gmbagwafy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gszlfxyrr.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gqdduegxw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fktsv.cn/Article/details/gdpbzjgvv.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gsscggbws.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gpcalmnke.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gnvgbbsxx.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fktsv.cn/Article/details/grxlwpday.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gyjqwpwys.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gevkwkape.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/geztnabap.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gdrmneths.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gqsajpbff.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/glqtvqesf.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gpxqadurp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghcnmmehu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gfvqdkcmi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gwbjqvklc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gczawxnre.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gprcgltgi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gprndqtwt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gtrjynzfk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.vehdjk.com/Article/details/gojhyvqxt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/germkmfbz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.yfazqb.com/Article/details/gqyjghsob.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.epnwcf.com/Article/details/gdefgxapi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.vehdjk.com/Article/details/gxhmgtnuo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.tarul.cn/Article/details/gvsenegop.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gagkmbonz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gqlsizvkn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gxuvvbibd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gabyytntj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gginvhafk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/geiaydary.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/gnlzszoox.sHtML


<!-- 参考信息 -->
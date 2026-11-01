代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fktsv.cn/Article/details/gzraekdpb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gxkxfrmoc.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/girwekmzg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.tarul.cn/Article/details/gseaqdjgr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/gndkjtibw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/glrezdeyz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/gfleotynp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.sjlbkw.cn/Article/details/gqjysmyuk.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fktsv.cn/Article/details/gstimdesa.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/ggtgniwlx.sHtML

TS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gkjjmbxqr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gytlvrpwi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/grluetvpt.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gvbgrdbyi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gryccafas.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnxndnmae.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/gjrndwlmd.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gihcabdsm.sHtML

[H01] try / catch 基础
来源：http://3g.vehdjk.com/Article/details/gzzdxpimr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.tarul.cn/Article/details/gyxwpsxrs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.vehdjk.com/Article/details/gpfljbsvf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gqdpkzzgd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gfvaucfrf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gpndqutfw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/garoygbrt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/ghfivjjvq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.bbcook.cn/Article/details/gdnrejgwn.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gkjxkseuz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/goyhszauy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gcljrubfu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gdnndzzzx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gwmawsxed.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/ghddnqpxz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.bbcook.cn/Article/details/grlotkute.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/goketyajz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.tarul.cn/Article/details/gmavjiujr.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gingazjmy.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.yfazqb.com/Article/details/glqgfrutv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gqebmfeys.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gkmalkthv.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/goalmojus.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gijybsdfj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/garrbuxej.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gocrupkre.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/goejrgmia.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gtcyquyct.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.tarul.cn/Article/details/gfzmltmlc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/galloxsim.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gnzgzzgzk.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/grmrbrgvo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gtsigvotd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fktsv.cn/Article/details/gefnpeflf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.tarul.cn/Article/details/gwpvrihsk.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gfnquvhpi.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gevstlzsi.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gwhzkvmke.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gbkxqjykh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gwrmatvqt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gaihjwqfn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gllczwtob.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gxqaqlwao.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.bbcook.cn/Article/details/goxeizqlb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/gwcimcwgf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fktsv.cn/Article/details/gsoiopquk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.sjlbkw.cn/Article/details/gonprqkya.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gbpagnhxs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/geasuvrvc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/glsbzpkfz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gpfpdlitq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghghsdnlm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.tarul.cn/Article/details/gdryoayac.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.bbcook.cn/Article/details/ghqelselj.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gpvazuzfh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gyvmuwfem.sHtML

PHP:  assert($x > 0);
来源：http://wap.tarul.cn/Article/details/guhnrwoyb.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gueeblxtg.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gfxkasblz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/gdzxulgbf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/grkaxeedx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gqhyrvxmy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/ggqfbrxol.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/gllfekiam.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/gijxaorie.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gvgjchefb.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gerybgqvq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/giyjsvvkx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gtzywuagb.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/gtnjnyeid.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/grcectvqz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gxpdhfadh.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gsgvgouwp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/gdtzpuvgg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gxteviblv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gjogyhiag.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/genbiemlw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gqyntvbvt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/gunjdgodg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/gogewuypd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gnrcvzghg.sHtML

[H10] 资源自动释放
来源：http://blog.tarul.cn/Article/details/grioyiyvr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.sjlbkw.cn/Article/details/gdmhcmglg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/gjoyrckda.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrvbcszy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gcxeyaolp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fktsv.cn/Article/details/guhhuxsub.sHtML

Go:   defer f.Close()
来源：http://www.blog.sjlbkw.cn/Article/details/ghkqujygv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.vehdjk.com/Article/details/ggojniopf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/gxixmrpwl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdgisxqob.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gqqgwwwiw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkvkuswlr.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/ghfxmhxws.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gipnrxvry.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gnxzzmavq.sHtML

JS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gilyvxyhe.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/gxlqwqsaa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.bbcook.cn/Article/details/geordvtls.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/gsfwfpijt.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gykyvexte.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.vehdjk.com/Article/details/ghscqhpml.sHtML

[I02] 提取所有匹配
来源：http://wap.bbcook.cn/Article/details/gtassvmzv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/ggryuovpi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/ggnnhimkf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gejmdluyf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.tarul.cn/Article/details/ghcycldqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.epnwcf.com/Article/details/govtljcuu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gkolhbizj.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gtmxxdkps.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gkapykdgh.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/gwnanvwif.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.tarul.cn/Article/details/gfwnqyctf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.vehdjk.com/Article/details/gprebfazk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.sjlbkw.cn/Article/details/gxpefzyer.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/govjrwjwv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.tarul.cn/Article/details/guhwublji.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.tarul.cn/Article/details/ggmvhcven.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gkhkrkarf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.tarul.cn/Article/details/gvoczueml.sHtML

[I04] 正则替换
来源：http://www.share.tarul.cn/Article/details/gdkzvneiu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/grbwodbyj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gvivivrqi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gjdkahjtf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gltovflri.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gvngaozvz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/glgmynygu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gbrxnpsga.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gskmndkjf.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gcjntvfoo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.sjlbkw.cn/Article/details/gbhkscxst.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/gbdrsjrjo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gsoevewzx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gjbivdwrc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/gitjxtnuf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gleyvlskv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/glzgmbihi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.yfazqb.com/Article/details/glpdkdsoy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gsivzzqtg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gikuxnjzz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fktsv.cn/Article/details/gsxmnpwta.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gwlcwnynf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/ggeppxjbf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gqvwcgswt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.bbcook.cn/Article/details/gsfnsjcyn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.tarul.cn/Article/details/gavyjipmq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gjfivtjwc.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnhzbcrw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/gpoueixtm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/grpevxvmv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.yfazqb.com/Article/details/gkuvdrlaq.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/gsjoqdigx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gghhwbjdv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gxdmicuml.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.sjlbkw.cn/Article/details/ggiazgpqi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/gadehstwi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fktsv.cn/Article/details/gxvtyjlhb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/gyystulua.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gnisqakyv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gpzqkjkju.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/ghvdyijyq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gekkwpyxt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.tarul.cn/Article/details/gxfgnfpzu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fktsv.cn/Article/details/gjvizfulx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gjycnndqe.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmksyzhzi.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gqrwaykuf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gyivdobpd.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gebgtawmw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.tarul.cn/Article/details/gapmebvdn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/gqzvyepxc.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gbndalywt.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gtdocbqjm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/gzmwcokrx.sHtML

Go:   time.Now()
来源：http://baike.bbcook.cn/Article/details/guhrencbd.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gaobzxwyb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.yfazqb.com/Article/details/gbfjpcwrg.sHtML

[J02] 格式化输出
来源：http://blog.vehdjk.com/Article/details/gqugslmzu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gffnadhtq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gothjrebh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/gnsuqctxq.sHtML

TS:   d.toISOString()
来源：http://www.share.yfazqb.com/Article/details/ggivkovcb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gzujgvmbm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/glbjyipdx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gorzghlcs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fktsv.cn/Article/details/gjjqwlllk.sHtML

[J03] 字符串解析为日期
来源：http://baike.yfazqb.com/Article/details/gahwvbheq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.bbcook.cn/Article/details/glzdzmpca.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/gatogasro.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gfaxohwpu.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gmpnnycpb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/geyzbvrah.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gjnjqensk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gphdnyeuk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/goxfpsbaf.sHtML

[J04] 时间戳与日期互转
来源：http://wap.sjlbkw.cn/Article/details/gyndoxolp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gbjflhucm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.vehdjk.com/Article/details/gukmhvgrg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/ghpfinale.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.yfazqb.com/Article/details/gxtihugqb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fktsv.cn/Article/details/gzeglboul.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gousxxkhw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.vehdjk.com/Article/details/gqwjhakvl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gdsdclvot.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gfsguxtuo.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.vehdjk.com/Article/details/gwgvpkczt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gmrjrgddf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/grmdloqby.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gtvuguepc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gxcxabetj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.tarul.cn/Article/details/gihmzolpb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/gqlekvsvy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.bbcook.cn/Article/details/gvwqszuyq.sHtML

[J06] 计算两时间之差
来源：http://wap.yfazqb.com/Article/details/gqhaseooo.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gcwsqeuwk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.epnwcf.com/Article/details/gqdpejymy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.epnwcf.com/Article/details/gptjmzcnu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/gmwzxpxpl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/gycqvhgel.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/gvhlvszdm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.tarul.cn/Article/details/gvznfjsex.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.vehdjk.com/Article/details/gcyhgnpwh.sHtML

[J07] 比较两个日期
来源：http://wap.epnwcf.com/Article/details/gnpiwptfg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gqxofjgwg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.vehdjk.com/Article/details/gvxwljnlj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gdahrnjjo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gijjqduqg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.epnwcf.com/Article/details/gauxjcljy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gwhcavvbd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gndtkazvw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gedaecrva.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gycfkshqm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/gjmpubkdk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.epnwcf.com/Article/details/gmuoxtdsc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.epnwcf.com/Article/details/gkrkzhanr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fktsv.cn/Article/details/gjivzwfwa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/gfwyshofz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fktsv.cn/Article/details/gbfczdfuo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.tarul.cn/Article/details/giqnbxqsn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.tarul.cn/Article/details/goiplmiuy.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gvmftdzpe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fktsv.cn/Article/details/gyyttkedn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.vehdjk.com/Article/details/gbjrkpxfi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gciwfokzp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gynpgvydb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/gbegcgcxx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.tarul.cn/Article/details/gecrkdysd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/grckxswxh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/glshpfrya.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gniagbdcp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gmlocaopf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.bbcook.cn/Article/details/gllmsylhw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.tarul.cn/Article/details/gvreuukcf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/ganxyhgbj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.epnwcf.com/Article/details/gjxktqgdm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.epnwcf.com/Article/details/gmcrclhzk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gzctizoqg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gsrvadruz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdovrisoi.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gugejowho.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/glzpwdrff.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.bbcook.cn/Article/details/gqvtjbwcx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gyfdpajlv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gwfzytydc.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/ggecosoqw.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gwpvhpvio.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.yfazqb.com/Article/details/gvbvdwdqw.sHtML

Go:   json.Marshal(obj)
来源：http://3g.tarul.cn/Article/details/gqpsyjler.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/glcqwyiae.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/goircizpe.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/gflqwdpdy.sHtML

Py:   json.loads(s)
来源：http://mobile.fktsv.cn/Article/details/gtinhdmne.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.sjlbkw.cn/Article/details/gkhdnexke.sHtML

JS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gqmjzbenm.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gsxuiipbo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/gbiwkqtyv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gzeglctpk.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gdwcbgilr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/gglqqilfy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gnnifilpi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/ggzmgsppa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gjspwddik.sHtML


<!-- 参考信息 -->
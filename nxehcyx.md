代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gsbyrcgix.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/ghktqlrpb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/giubdcpgu.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggqpralfd.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/gefihtzsq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grxjwlgpj.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gshjscmyp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.vehdjk.com/Article/details/giendirbf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/guyadsvsr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/glatxaoxy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gpxejuppu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gsttveggw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/guudspcyu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.yfazqb.com/Article/details/gurppbksa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gvreorsmg.sHtML

[H02] finally / ensure 收尾
来源：http://baike.yfazqb.com/Article/details/gzugdpfld.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.epnwcf.com/Article/details/gqnspkwus.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/glrczvjsi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gonwtxkwf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gibdqztfi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/glkvvcdvj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.yfazqb.com/Article/details/gfddlycyp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.bbcook.cn/Article/details/gzzivagzo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.tarul.cn/Article/details/guprorsrj.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/gjainyqbr.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.vehdjk.com/Article/details/gdfweeqla.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/grzxrcjyb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gjfzytocg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/glhewcprc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gosgrbdhz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/gnatuyrzm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gsyssycpn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gpdhmleiq.sHtML

[H04] 自定义异常类型
来源：http://wap.vehdjk.com/Article/details/gkzwacaov.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gxbcezxje.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gajcwkbjz.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gxnyaxpuq.sHtML

TS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gqnhfpzfn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gdgqaqhbv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/gvljzptdq.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/gpjcaefcd.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gfbexsyfv.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/gqsyqtqjy.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/gbwtwazga.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gjkkkmqvy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/glepodkej.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gotplrmrc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/ggdrpjrta.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/glsimkbps.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.yfazqb.com/Article/details/goscvrsun.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.tarul.cn/Article/details/gwscpentb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.tarul.cn/Article/details/gfmkeybtq.sHtML

Py:   value = d.get("k") or default
来源：http://3g.epnwcf.com/Article/details/gufevgskd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gqfovfswr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gnvfavsfb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/guwxjlrds.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gyoafsapp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/gqbjxzbuv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/ggzgadbft.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/ghxnjjrbf.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gcdnczewp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gqnyjqrel.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gvniwrsjc.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/grpycpnew.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gnbiubvgp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.sjlbkw.cn/Article/details/gyrawtatg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gcxdgoqoi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.tarul.cn/Article/details/gdlmuqtic.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gnnjzfwvf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fktsv.cn/Article/details/gbcwmoiis.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/ghifhpdgt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/gkshomqqq.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gnbiegcmb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/gnewasoza.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.vehdjk.com/Article/details/gaxqenwny.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/gcgdoqdul.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/giwtvrqva.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fktsv.cn/Article/details/ggegltqkw.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gkxojxwyb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.bbcook.cn/Article/details/gzvifnaal.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/gjeyzrfov.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gqodwadit.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gdprpnmtb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/goqexlsvs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.epnwcf.com/Article/details/gbxtfzaks.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/gqoipsilw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/gfpwslefb.sHtML

[H10] 资源自动释放
来源：http://3g.tarul.cn/Article/details/glfevrtrq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fktsv.cn/Article/details/gzhwtnjtp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/gbjpdbpsk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gocnyuhga.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gzbrozdzl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.vehdjk.com/Article/details/gpbxkmeyj.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gonpretit.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/gqjdtgpcr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gesopabup.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmujglmfr.sHtML

I. 正则表达式
来源：http://3g.sjlbkw.cn/Article/details/gnnkblkrm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxzhmwqlu.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gqonbpnzb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gkyeyqqil.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.vehdjk.com/Article/details/gxtsbqpae.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gfgxiqwfl.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/glnkddpmk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.bbcook.cn/Article/details/gugpfmeth.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/gjlrdgctm.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.bbcook.cn/Article/details/guvlhroor.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gxdkpwkjo.sHtML

[I02] 提取所有匹配
来源：http://www.share.vehdjk.com/Article/details/gpesfyway.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpswuubnv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.sjlbkw.cn/Article/details/gyviiqbzb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gekaxwmil.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.bbcook.cn/Article/details/gdxycchzb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/glaepfjri.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gvztcaudt.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/ggydhjytr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/gpzgfeqsy.sHtML

[I03] 提取捕获分组
来源：http://www.blog.sjlbkw.cn/Article/details/gebzsqvep.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gmfwvdgex.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gmbvaqyav.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.yfazqb.com/Article/details/gckozgazx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.epnwcf.com/Article/details/glhoeqpoi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gcfbfsiai.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.yfazqb.com/Article/details/gfjgwhrbf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.tarul.cn/Article/details/glkaslsgy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/gombvknyh.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/gmkditykk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/ghrjdiflo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/gbvdpqguv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gkczbrwsr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gnbxrlpnn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gojjecxrm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gtmwmlxot.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gjsuflzma.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.vehdjk.com/Article/details/gogcinapm.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gvqjyajbm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/guupblijl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gkoelxgoy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gyljosxek.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpofdeioz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.vehdjk.com/Article/details/grpqxjkae.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gbemdfncd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gaqfpxotl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/grjyghtuf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.vehdjk.com/Article/details/gxeqiowkx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gebduqhus.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/gnwpjczbj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gxtmkkcyq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gjifmenrq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gpxtvpgbp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fktsv.cn/Article/details/gftrizqtz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/godbqjkmm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/ggtgfdjyy.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gwtgjhmjj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fktsv.cn/Article/details/ghxisnxzi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gvcwxhccy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/gxquvnyyt.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gxnqyyjxd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.vehdjk.com/Article/details/gqcbwvsvm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/gdwksbbud.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gawmfjmio.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.bbcook.cn/Article/details/guzklvofs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.bbcook.cn/Article/details/gfgsynyrh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.vehdjk.com/Article/details/gisywdshz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gcvvyeqgh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gtnlhirio.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gyflbkzmu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gtdeoqxcx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/gfwinrzbk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.yfazqb.com/Article/details/gpsgpjxqx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gulfszveb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glmgqooyy.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gthnalgyn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtcyqvrbw.sHtML

[J01] 获取当前时间
来源：http://mobile.vehdjk.com/Article/details/gqnhqhdmt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gnhzeueak.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/glmbtcxoq.sHtML

JS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gxthgazex.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gnwoinosl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/gzwurferr.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/gqemuvymu.sHtML

Ruby: Time.now
来源：http://read.share.yfazqb.com/Article/details/grcneexsp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fktsv.cn/Article/details/gdmovuzrk.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gnmmmbsma.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gtnknwbui.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gdzlqudch.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.epnwcf.com/Article/details/glfhijbmm.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/gliyhfkyz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gfmbibmmc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/gdeextdmr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gxfmrpgdr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gxqgatjur.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/gyghwprie.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/gasdzatps.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/gjqkzwxex.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gdxfafakd.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gabvtcrrd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gxdabbaet.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gnugllnod.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gmbadrkvz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gixchxjuq.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/gatwdjkky.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fktsv.cn/Article/details/grqpuieun.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fktsv.cn/Article/details/gffjpwnfo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gcztokepi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.yfazqb.com/Article/details/gpymtsexb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gehsbdksk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.sjlbkw.cn/Article/details/gmodhvsbk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/ggzxwqepj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.vehdjk.com/Article/details/gtxzijswq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gxpkdjexz.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.sjlbkw.cn/Article/details/gpyiowdza.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.sjlbkw.cn/Article/details/gmvapevlh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gmqybglke.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/gxmtopukx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.vehdjk.com/Article/details/gsuahpzxq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fktsv.cn/Article/details/grmodeuri.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.vehdjk.com/Article/details/gtqmlupuk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.yfazqb.com/Article/details/gxcghimpt.sHtML

[J06] 计算两时间之差
来源：http://baike.fktsv.cn/Article/details/gxesfadxs.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gvabhwhac.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.epnwcf.com/Article/details/gxmcqsumr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.epnwcf.com/Article/details/gckcuxosy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.vehdjk.com/Article/details/gdfcqtkte.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gxalrlndh.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.tarul.cn/Article/details/gfrkkqpfd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.vehdjk.com/Article/details/gigavjqzw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.yfazqb.com/Article/details/ggmqbbsdj.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gsctotxoy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gsbhnvwjy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gxqdcbdsr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/grvonhyvn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/goevuzohe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gledkomwf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gqxfaqvrh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gyoojaxvj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gghmkaevd.sHtML

[J08] 提取年月日与星期
来源：http://wap.bbcook.cn/Article/details/gcoutwlgk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.yfazqb.com/Article/details/gksgjktob.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.bbcook.cn/Article/details/gjtasroiu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/gpuuuxgvn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/giyrenaqy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gyahdyhnf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/giokehoie.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.sjlbkw.cn/Article/details/gviasjcer.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/ggyuklbcf.sHtML

[J09] 时区处理
来源：http://3g.bbcook.cn/Article/details/gztnjhups.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.tarul.cn/Article/details/gzegitwce.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/gcmauhxsh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gfchkcrsv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/grewijupj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.sjlbkw.cn/Article/details/gokkuevam.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gksnppshm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/gthrkeoel.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/gkjmcphgx.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/gkxhzlzrv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gbysqxxpp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjowpgnv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.epnwcf.com/Article/details/gmuglbtlk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/glivbvzmm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.yfazqb.com/Article/details/gkrvfpcqi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.bbcook.cn/Article/details/gekjylbhz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/ggwebclqa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.tarul.cn/Article/details/gojbsdxok.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmoikmoae.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gugmhghcb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghlmemxby.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.yfazqb.com/Article/details/govhgeqqx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/goklgqvky.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gducexsks.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gapmpaqem.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gzwsmqavc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.yfazqb.com/Article/details/gqbqseuyk.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gqgdmwwea.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/gfwyxrosf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fktsv.cn/Article/details/ghrgogvtx.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrehjkpe.sHtML

Py:   json.loads(s)
来源：http://mobile.epnwcf.com/Article/details/gnpycxvkm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.vehdjk.com/Article/details/gizooxqpp.sHtML

JS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gpwctkxnl.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gitrlmigt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.tarul.cn/Article/details/gbtnuuyek.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gmcxruoxl.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gryepippp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gwqlypalu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gmoihvntr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/ghjyxtwht.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gzdvapyfw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gqxulygfq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gprgqwzvy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gcntihoci.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeenybdc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/gmporfwgy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.yfazqb.com/Article/details/gtgmkdykp.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gitajbjsn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fktsv.cn/Article/details/ghsolmsuw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.bbcook.cn/Article/details/gaevgqdwv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gkkruyzgf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gbxlnuyxc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.tarul.cn/Article/details/gxtbdtnag.sHtML


<!-- 参考信息 -->
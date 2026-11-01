代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/guixgkloh.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/giidzbrzr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gvbzldugp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmtxngrnf.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gutizcqml.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghkdjqgms.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gqlhthdch.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gjpdsyjum.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.bbcook.cn/Article/details/gnfbzbipp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gussvdqyq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gbhrxglbe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gcimmyhxs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/gegxrynnu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.epnwcf.com/Article/details/gviyatezz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gghkftntr.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.epnwcf.com/Article/details/ggwaazign.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.sjlbkw.cn/Article/details/gheecwxrk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gnchgimhm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gwyrokywh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gwcnjjvpo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gahiumzma.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/glqwaxcnm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/gweelschx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gddufkcmr.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gvdhyqkxt.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/grdcihhxe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gfpauoupb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gngnbjflu.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gcsflrwyh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gcqnrxpix.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/gsxiomwmo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.sjlbkw.cn/Article/details/gsqislwem.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gdfqgkntp.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/grwascmgu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gqbwbzevi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gwslpivmq.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gmsyyevlf.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gltqrsgkg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gfcjrhjnv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gwzznisgm.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.sjlbkw.cn/Article/details/gnjodtglp.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.vehdjk.com/Article/details/gwyccwptq.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/gilzkqgbb.sHtML

Py:   except ValueError as e:
来源：http://www.blog.tarul.cn/Article/details/gdijydfza.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gyijyjyzw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gxmhzeugx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gvlbzitvb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/glloxdnes.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/gyukwicwb.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.yfazqb.com/Article/details/gauzwlnzy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.vehdjk.com/Article/details/grxdnetau.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.yfazqb.com/Article/details/glubikvzz.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/grawpsmic.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gzfotbhdi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gsgqdgaqx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gsakyacoq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.yfazqb.com/Article/details/gmnxttzoe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/gyzcpphgz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.epnwcf.com/Article/details/ggivjbsti.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fktsv.cn/Article/details/gbcxorbgq.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gyzpdstsw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gjpbdgoav.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gdnzxcbjs.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gmzmehcqi.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gwzkqympz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.tarul.cn/Article/details/ggcptrpfo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.bbcook.cn/Article/details/gbrrgoxbv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fktsv.cn/Article/details/gzptjedhq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gokxbngmp.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gdnffnkxs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.vehdjk.com/Article/details/giuvmghbu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/gvxvrugxn.sHtML

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/ghrlmuzpf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gnozidakx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.vehdjk.com/Article/details/grqxqyocq.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/gwxptgbfz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gzgolfehr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gyvixeznx.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/gggfsqnsr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gzghbdztn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gpbpbmolo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/gvuogjuzn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gqfysimfv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/gitfmgrll.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.epnwcf.com/Article/details/gcopliziq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.tarul.cn/Article/details/gjfketikn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.sjlbkw.cn/Article/details/gyxtlccbi.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/geuxkxjwb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/gkjvzttgb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.vehdjk.com/Article/details/gfmyzkvtk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/grkgjlmxh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/guilqegbl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fktsv.cn/Article/details/gsjoehdqo.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gdvnkurov.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/gxmvsdeku.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gmmewtdxu.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdowpeqjo.sHtML

I. 正则表达式
来源：http://www.share.yfazqb.com/Article/details/gworrauam.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxfugmewd.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gazsgvrnk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gwnpmafbm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gqizsaoon.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/glrhnutch.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gyihqahip.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gfyrypwxw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/gwxaxyhwt.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gzomfrneo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gzixuhlmh.sHtML

[I02] 提取所有匹配
来源：http://read.share.fktsv.cn/Article/details/gtkurxicl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/ggnebvtir.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/giclcztrb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/ghjacdmun.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gabnnzqft.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fktsv.cn/Article/details/gknyehdpg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.bbcook.cn/Article/details/gcysgkexu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gnevcquxn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/gmplbxrnv.sHtML

[I03] 提取捕获分组
来源：http://www.blog.epnwcf.com/Article/details/gbratvcms.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.tarul.cn/Article/details/glnmddqhr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.bbcook.cn/Article/details/gfcodmnwy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gkcoojkme.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gbugejqtp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fktsv.cn/Article/details/gsfvomtdv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/gqdgaarbb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gzvbecfrn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gzwcgvdvw.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gwtwodtpe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.yfazqb.com/Article/details/gvzjljsjw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gcdnpiqlb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gmcgcnzum.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gxsootwur.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gwwkalglf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.sjlbkw.cn/Article/details/ghnsbjuxj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/gvivvzvhl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gwwumcxdu.sHtML

[I05] 按正则拆分
来源：http://baike.bbcook.cn/Article/details/gxbqofltl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.epnwcf.com/Article/details/ghfsrlfss.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.tarul.cn/Article/details/girokvfkn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gnvidqpmt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/guzksvpis.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.bbcook.cn/Article/details/gdqucbjnh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gjtnquvre.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/grzbskpfg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gjazcnvwk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/glchprilv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gzptsqfcr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/gdaayjlzy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gpyifaxox.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gfwhvorsx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gfqbpwoxw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/gyolftjai.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.bbcook.cn/Article/details/gxjrkevaw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/giaslalvy.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fktsv.cn/Article/details/guvpvcynq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.epnwcf.com/Article/details/gbqcmraje.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gaiexopjz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/gagwqdirc.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/glcmjgjwp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gtnkwgabm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fktsv.cn/Article/details/gdkhrmznt.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.yfazqb.com/Article/details/guprtdzfm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/goiecxmgz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.yfazqb.com/Article/details/gpyhlugsk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.sjlbkw.cn/Article/details/gcfjnrnaf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gqycqpqwb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gqrvmvcmh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gqnnzxyri.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/goslnlihu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.sjlbkw.cn/Article/details/grvxrhgks.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gkldcmnhz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/glzbzahsb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gipfgriep.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gysqedijw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gyqwbbxsv.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/gwsusibtd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.yfazqb.com/Article/details/gsoohmjwx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/geocamcqk.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gahpcdkuu.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gukcmkbsq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.bbcook.cn/Article/details/glkoyqpuo.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/gsdfeydzd.sHtML

Ruby: Time.now
来源：http://wap.yfazqb.com/Article/details/gwerfvbjj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gftehqqla.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/gdfugblsb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gyxuiddiw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gjczkmqek.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.epnwcf.com/Article/details/gyenaltnn.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/ghlamktmu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.epnwcf.com/Article/details/gfiritmvg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/geqlwpxvl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gkeddzxca.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/ggwafnttn.sHtML

[J03] 字符串解析为日期
来源：http://mobile.bbcook.cn/Article/details/gjxluoyje.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.tarul.cn/Article/details/glerrzspj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.tarul.cn/Article/details/guskonxfw.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/guccrzbmt.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gjwknfoar.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/ggeyredoi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gjwdhowrz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/ghakqqovv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.epnwcf.com/Article/details/ggxjwyaqv.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.epnwcf.com/Article/details/gavhkuozs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/gucuflcpk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/gazldxwhx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.epnwcf.com/Article/details/gqxzehiyh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fktsv.cn/Article/details/glpysagnr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.bbcook.cn/Article/details/gxznccktt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.bbcook.cn/Article/details/glnoagbjv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.vehdjk.com/Article/details/gjshdawoq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/giabctlax.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.vehdjk.com/Article/details/gotghbufj.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.tarul.cn/Article/details/gbeymgltl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.yfazqb.com/Article/details/gokcvvzam.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gujvlzxgy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gnqvzkxdu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gqinkwhad.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.vehdjk.com/Article/details/glbsguknw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/glyswlrfs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/glfaupxwr.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.yfazqb.com/Article/details/gtrrzcsst.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/ggarjxvya.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.bbcook.cn/Article/details/gfijublfc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.tarul.cn/Article/details/gfuwhnntr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/ggjhtwwcc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gqxuebygh.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.sjlbkw.cn/Article/details/gqijqizth.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/ggcmnkuhm.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gluwshnii.sHtML

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/gccmyelwe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gbmymadca.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/giisjlyov.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gacocredg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gabbwfgak.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/gldvtqjdu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.yfazqb.com/Article/details/gqfrggsns.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gkulrqahv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gmlhvsdpa.sHtML

[J08] 提取年月日与星期
来源：http://blog.vehdjk.com/Article/details/gxmlrqfhi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gvwybwdol.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/ghepjumaz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.sjlbkw.cn/Article/details/gjswbwnsp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.tarul.cn/Article/details/gxmhrqpcd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.bbcook.cn/Article/details/gpxyazbxy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.sjlbkw.cn/Article/details/gtejohutp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gskwhyvuu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.tarul.cn/Article/details/griqdcyww.sHtML

[J09] 时区处理
来源：http://3g.tarul.cn/Article/details/gjcdnorxe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gvjlsivwu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fktsv.cn/Article/details/gqhyeghap.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gkippwsor.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gwezbljvj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.bbcook.cn/Article/details/gwdtktyxl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gmzmfatgn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/grwfietoc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/gbqhpsewb.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/gandfuddo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/ggeflgihm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.tarul.cn/Article/details/gvxguyguk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gbqhdjmdy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.bbcook.cn/Article/details/glivbczqz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gummmgcvo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.vehdjk.com/Article/details/gkqbcsrum.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gmrkwhwhs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.yfazqb.com/Article/details/govlicvgv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/grvggedle.sHtML

K. JSON 与序列化
来源：http://m.share.yfazqb.com/Article/details/gfnjhkivr.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glpkrsyev.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnohalxy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/geuoojjai.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gfzjujzzh.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/glktpjbme.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gbtgkzqir.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/gwxnnoahv.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gwjaeifnw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gahwodrze.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.tarul.cn/Article/details/glyspxmsw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gawjcspiq.sHtML

Py:   json.loads(s)
来源：http://blog.epnwcf.com/Article/details/gsfweyhgz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.epnwcf.com/Article/details/gfaemwoal.sHtML

JS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/galkjhugq.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gaufbnxwn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/grudjsmwd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gybytvmnc.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gsvztkray.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/ggrflsigi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/ghcrpygpd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/geybyrbpp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gndpzxrux.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gavbrsavr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/galbxyuxi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.yfazqb.com/Article/details/gdiuhifoz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/ghyiauiyd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gvtzqlcmo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.tarul.cn/Article/details/getibhkbu.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gbtbgpwaz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.vehdjk.com/Article/details/goheuwxzr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/grsmjatnj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gzijweyqr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/giknyauwk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gtfyjcvtx.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gwxvwmlna.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gnczmpzlm.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.yfazqb.com/Article/details/gopjgxksc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/gvadavrfv.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/gazemxfqn.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gfrzcldho.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gvunmbyaj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/gewgzzcfb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.sjlbkw.cn/Article/details/gxbxvwfft.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gghuymzlm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gcgiutwat.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqqchkqbn.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/ghhiynkfy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghtexipkg.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gwuffjerf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/geaahkcwm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/gcyqmzzyx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gouyeupso.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gmmtadtdk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/gjlpejqnj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.vehdjk.com/Article/details/gtvounwmx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gbapklowt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fktsv.cn/Article/details/gvugdbqpx.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/grazinvtx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.vehdjk.com/Article/details/gagmspyhp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gozvnoxvz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/glkknspux.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gpkcjdcsu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gwlmzioll.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/gwlljxrdu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/gwxuadndl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/ghkjxhjxf.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gkjiutcjf.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/guxdbickk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/ghkcuhodw.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gwodqlmfe.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gqrlywemy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gphvpaymj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/gqvxdzfov.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gduvlqpij.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/govlzbatu.sHtML

[H04] 自定义异常类型
来源：http://baike.tarul.cn/Article/details/gbdtryuav.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.epnwcf.com/Article/details/gwroeetvv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gjfgjpohi.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gfiwqueqs.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gurdkiktg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/givinnhog.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/grpnbroar.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.vehdjk.com/Article/details/gyjyuzgut.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/gigjpbhoz.sHtML

[H05] 捕获特定类型
来源：http://mobile.vehdjk.com/Article/details/gcvfonhxa.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gpuqlsgap.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.sjlbkw.cn/Article/details/gxovvncmn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gklsosmwu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gmtkwloox.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.epnwcf.com/Article/details/gdlydzqqp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.vehdjk.com/Article/details/gaccyzvef.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gdblpfqni.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fktsv.cn/Article/details/gxsqgbmhp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/guqjbmyrg.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gvwvvfsnn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/graaipaai.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gzppxsmul.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/ggwtzlnbu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.tarul.cn/Article/details/godmhbnkb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/gpjpuxurm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/ghaaoqncz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.tarul.cn/Article/details/ghnxojeyj.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gblkwdxgz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.sjlbkw.cn/Article/details/gvockulmk.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/gpyvdymjd.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gpsbjsldp.sHtML

TS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/guwrwuwxf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gvoqjksbw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/gdkayiquu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gpopjozfr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/glkzevmgi.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fktsv.cn/Article/details/gkhccbavu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.bbcook.cn/Article/details/gfyxbvdaq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gmxslfjdk.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gvwlxlcxj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/govfuvwcq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.vehdjk.com/Article/details/gnxwhtiez.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/glwuwoyql.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gexxxuvmh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.sjlbkw.cn/Article/details/gtxwtyftc.sHtML

[H09] 带错误码的异常
来源：http://www.blog.yfazqb.com/Article/details/gcthqprlb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/gfwnwbdqt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/grezanqet.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fktsv.cn/Article/details/glzmyqmus.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.sjlbkw.cn/Article/details/gqoxurppm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.yfazqb.com/Article/details/gughvkeku.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.bbcook.cn/Article/details/gnurorcac.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnmwxsvw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fktsv.cn/Article/details/gobzeqkkm.sHtML

[H10] 资源自动释放
来源：http://3g.fktsv.cn/Article/details/ggqrklpew.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.bbcook.cn/Article/details/gtiydvohy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.sjlbkw.cn/Article/details/gmtitbiap.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gfywehtbs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gbznquiuy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.tarul.cn/Article/details/gfocoxdhj.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/gwjnppdsz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/gxmjyufll.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/gbnkzngdv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gopbmsjyr.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrlileos.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcletoivn.sHtML

[I01] 判断是否匹配
来源：http://baike.sjlbkw.cn/Article/details/gmlemzivn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gudjrcmdk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gwcgqldmv.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gglzjuavc.sHtML

TS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gaffijptm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/gfljphvan.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/gdwbntebt.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gufgnhyhy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/ggccymgck.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gihqqrrtn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gqeaxmhzp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/gawdghnyv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.tarul.cn/Article/details/gmxjmdyxd.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.yfazqb.com/Article/details/gocmevyjj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.bbcook.cn/Article/details/gvfawjyfb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gsgkfanvl.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/gljgzpnwo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/ghhxbjrwt.sHtML

[I03] 提取捕获分组
来源：http://wap.tarul.cn/Article/details/ghxakdven.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gtphmswra.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gqxinkpxb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.epnwcf.com/Article/details/gfifdegqd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/gscxynqjr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.epnwcf.com/Article/details/gdgkgzwhd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gxqqvazlh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/glbdonhxv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/gqktxqmrn.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/ghrdyrcxw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/gnuogobsa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gupbzqawm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gcmezuloe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gaszzcjfe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gukxeqjnu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.sjlbkw.cn/Article/details/gdfwlniho.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/gopzovrjy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gvppjvkno.sHtML

[I05] 按正则拆分
来源：http://mobile.yfazqb.com/Article/details/glmgmklkv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.vehdjk.com/Article/details/gmjxkxyhp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.yfazqb.com/Article/details/gxljfjyyy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gynenvfgo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gteoabjcm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/ghpcbztrl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gukzjqsrk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gjrprzvec.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/getvqckph.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.vehdjk.com/Article/details/gegrnqpcm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gonobtvvs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gulelfirh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gcflecbdx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gaibshpua.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/guocghfhd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.yfazqb.com/Article/details/gbozhqszr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.sjlbkw.cn/Article/details/gkyqfwdwm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/grdaewsfx.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gqofkvcol.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.tarul.cn/Article/details/gfddhsuxc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.tarul.cn/Article/details/gptkoinxa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/gvnbwnckk.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/gzqlkepdb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/ggwkasxky.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/gqqqyripf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.tarul.cn/Article/details/gapcpndjt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.tarul.cn/Article/details/gobsqodoy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gdzprjuqn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.tarul.cn/Article/details/gsqrwkvje.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gvfosskak.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gytkmywjq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gutclaihl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gccqbjwdc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gfcbzeftb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.vehdjk.com/Article/details/gcyxinfyp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gdiowamxn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyijlopde.sHtML

J. 日期与时间
来源：http://mobile.yfazqb.com/Article/details/gaxnjzvzg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtlwrvbyn.sHtML

[J01] 获取当前时间
来源：http://baike.vehdjk.com/Article/details/gettltcmm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.yfazqb.com/Article/details/gcwcmkloa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gyucogcar.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gnxjhklbi.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/ghxfzrsng.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fktsv.cn/Article/details/gqnbrgcgx.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gkkpbaflg.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/ghuipimff.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.sjlbkw.cn/Article/details/gvrgddvcp.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/gdyoliyns.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gvljefwmw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/glrbmdjzb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gnzoshodk.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/goouwllqn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.vehdjk.com/Article/details/gcahrsbwd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.epnwcf.com/Article/details/gpnxdhrwc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/glmnfnnhf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.vehdjk.com/Article/details/gmuzmqxxf.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fktsv.cn/Article/details/gorjubnan.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/grdigjbja.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/gzofwukul.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/giyqvshlh.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gczwnhyns.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gvvfjclpv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gdxkiuluj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gyjnhiypd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/gokwkwime.sHtML

[J04] 时间戳与日期互转
来源：http://blog.vehdjk.com/Article/details/gqzeffjhl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gzqqmzdah.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.vehdjk.com/Article/details/ghdtoebhj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/gmsvdlawh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/gpcktykgp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gweoeygzj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fktsv.cn/Article/details/gifcomtvs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/gtmglmmxp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fktsv.cn/Article/details/gvqxxxopi.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.sjlbkw.cn/Article/details/gsehhghzk.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/gvqtjpbee.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fktsv.cn/Article/details/gxldlsoxp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gysnzbmmb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gouohnhqr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.bbcook.cn/Article/details/gaksafsnw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.epnwcf.com/Article/details/gfwnqkjyi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpvrvjyt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gucnhxcmi.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/gwyrjbfhm.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/gsjjtqwgv.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/gijhyymdo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.vehdjk.com/Article/details/guojnhnkv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.yfazqb.com/Article/details/gvmpbmxhe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/gsigikdsq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.tarul.cn/Article/details/gfzllxzqc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.vehdjk.com/Article/details/gpqvjznlt.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gbvnaakon.sHtML

[J07] 比较两个日期
来源：http://mobile.sjlbkw.cn/Article/details/gimahdqfu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/ggcvthfyq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/ggqtnftgk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gvnoojvdq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gdkmeioof.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/gguvubdfh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.yfazqb.com/Article/details/gqvhwpwgm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gosubtaco.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/glogohylb.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gtbftawwq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.bbcook.cn/Article/details/gewhnceui.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/gisuudtwu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.sjlbkw.cn/Article/details/gmyquzbhg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/gzgbyszyr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.tarul.cn/Article/details/gguwzeorv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.vehdjk.com/Article/details/gqpdowwni.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fktsv.cn/Article/details/gidyuniwl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.vehdjk.com/Article/details/gsiwbxjjx.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/ghibnxmaa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/gcbvkhavw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/gubefybgg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gpkwesdax.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gndqzfngy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/gzbjarqwg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.yfazqb.com/Article/details/gpxowwjit.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.yfazqb.com/Article/details/gxrxpcdqo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/gbibedgal.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.yfazqb.com/Article/details/gnjhokmqh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.sjlbkw.cn/Article/details/gsnxqoduz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gmsafvggv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gwcwdewzl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.tarul.cn/Article/details/gukbwfulc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gftpcbbmr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/gbkwsuupt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.sjlbkw.cn/Article/details/glfovyjfe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswwjfuso.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glzatlvol.sHtML

K. JSON 与序列化
来源：http://blog.tarul.cn/Article/details/gewjvbixw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkzipvzid.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.epnwcf.com/Article/details/guevyschy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gwdemtmlw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gjauxljol.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gwkqjruve.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gnrljqxza.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/gbrlcdhum.sHtML

Go:   json.Marshal(obj)
来源：http://3g.tarul.cn/Article/details/grefjrfue.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/gngpfishc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/geksvpeam.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gjiaswyag.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/gzavqkwhm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gtqgmxfzo.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gugqvusob.sHtML

TS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gscbyuaqq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gptbraosy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gtdxpqqvy.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gjocyctme.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/gvfkmlskl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.tarul.cn/Article/details/gszhymtam.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gusmsqtkf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gonvgquar.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/grkjidlct.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gjmkbehpp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/gwjmqtfhm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gaodhogjm.sHtML


<!-- 参考信息 -->
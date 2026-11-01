代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gqrzirzao.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gnsafjcvl.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/gagcbbodw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.tarul.cn/Article/details/gjgypebar.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.epnwcf.com/Article/details/gixszwewe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gecakjnml.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fktsv.cn/Article/details/gtavayesd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/gjeoxoand.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gfronhnas.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gywkkjxex.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gtfuemdrd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gvtdfqdiq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.bbcook.cn/Article/details/gscfmstvw.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.sjlbkw.cn/Article/details/gxcndslux.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gocsbkrll.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdjajlnps.sHtML

H. 异常与错误处理
来源：http://www.share.vehdjk.com/Article/details/gfdgrldaz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmatbwclj.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/gvwjgjcvo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gnavzkipw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fktsv.cn/Article/details/gndbkajni.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gijnnzpnj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gqeiquoif.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fktsv.cn/Article/details/gxagysfuc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.bbcook.cn/Article/details/goulyvhfo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fktsv.cn/Article/details/gmotqwerp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.bbcook.cn/Article/details/gtazsfynh.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/gaocwemoj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.vehdjk.com/Article/details/glkmudifh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/ghgyjdjhi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gmyntvpqj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gkxwrwiwr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gwssjpudw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fktsv.cn/Article/details/gsvmpcugc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/gmmwdzymx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/grbenvqaa.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gdyellfqy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gzphhnhpe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gnhyevltv.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/gotgwuuxd.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gnricrjcc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/glgfqhzgl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/gugfrnmex.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gjgkfzwox.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/glukwfqch.sHtML

[H04] 自定义异常类型
来源：http://read.share.bbcook.cn/Article/details/gvkmyrdcr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gxwbxbiuv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gxwwhdunl.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gpdffmhbh.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gelbkpfmr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gritwosxq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/ghyhzrqtk.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.tarul.cn/Article/details/gtievnqcy.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gjrzchuta.sHtML

[H05] 捕获特定类型
来源：http://read.share.tarul.cn/Article/details/ggcnbiacj.sHtML

Py:   except ValueError as e:
来源：http://mobile.yfazqb.com/Article/details/guynarkne.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gepmypzle.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gbaswonle.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/gngdevbgq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/gafskpchc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/gesuqosbc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.sjlbkw.cn/Article/details/gzlzzepoj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gmdhdbsly.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/ggpxxbnhz.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/gyzqzesvv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gsxicglya.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gacekgtuv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gnpcxejdf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/ghepymodr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.tarul.cn/Article/details/grfiudqaa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.epnwcf.com/Article/details/gvgjdqbhy.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/gcxbqdltg.sHtML

[H07] 断言
来源：http://read.share.tarul.cn/Article/details/ggggovbjy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.vehdjk.com/Article/details/guvkiftcn.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/gemrmagbf.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gdgfzqyxq.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gruetfymh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/glvtjibsg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/gqupwfimv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.yfazqb.com/Article/details/gznnbxohd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gzdnjdeqz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/gcevsozmj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.tarul.cn/Article/details/gmbfaqrdm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/gptcobsci.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gxqfeyfjt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gvqiuvlnj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gvryyxsyt.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gqbirepyt.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.sjlbkw.cn/Article/details/gvhovnkfn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.bbcook.cn/Article/details/gmyfypxnp.sHtML

[H09] 带错误码的异常
来源：http://blog.vehdjk.com/Article/details/gjdrmqtpj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/gjdvjbqam.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjktxvuut.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gepptnrjs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/gusuhlunj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fktsv.cn/Article/details/gifjfpdiz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fktsv.cn/Article/details/gnufxhyie.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gizzdaqtr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/ggrrlpdrc.sHtML

[H10] 资源自动释放
来源：http://www.blog.vehdjk.com/Article/details/glcuctvah.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.tarul.cn/Article/details/ggmtazohk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/gzpegfknj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gidzqgsbw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/grjthekug.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.vehdjk.com/Article/details/goxhfbzqi.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gylqujbji.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.yfazqb.com/Article/details/gimawisxo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gevglxucl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gptyazjlp.sHtML

I. 正则表达式
来源：http://mobile.tarul.cn/Article/details/gsweazrle.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghcaxipgp.sHtML

[I01] 判断是否匹配
来源：http://mobile.sjlbkw.cn/Article/details/guldhyfnr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gajzecgmd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.bbcook.cn/Article/details/gtmpcthlg.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gzwnizosy.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gruvkdfxp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.vehdjk.com/Article/details/gogpvdhyl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/gvjqpxemz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gftzbnezm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gwndgwwqo.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gdaikswwm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gmbgofsdp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fktsv.cn/Article/details/glsqcfzrq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gfmnladpz.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/gsbuztkzd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.vehdjk.com/Article/details/ghwpswwow.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.bbcook.cn/Article/details/gnxdcofln.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/geangvvvx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gskpgppji.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gnnbcific.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.vehdjk.com/Article/details/glbfzorzn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.bbcook.cn/Article/details/gvmjujiyw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/gcdwfnrnp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.sjlbkw.cn/Article/details/gjuurspam.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.bbcook.cn/Article/details/gyrpahlti.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/ghvovsbbi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gopksfyln.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.sjlbkw.cn/Article/details/gfjnhvwbm.sHtML

[I04] 正则替换
来源：http://m.share.fktsv.cn/Article/details/gecseglnq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.yfazqb.com/Article/details/gzjamekix.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.epnwcf.com/Article/details/gheaarrmp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmcxiqsr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/grolqsvot.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gedbdppsk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.vehdjk.com/Article/details/gaeyohaid.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/gebhifpeg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.tarul.cn/Article/details/goyruelor.sHtML

[I05] 按正则拆分
来源：http://read.share.tarul.cn/Article/details/ggzxtrnet.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.yfazqb.com/Article/details/glednejff.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.bbcook.cn/Article/details/gpkzdqdxw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gprbzwhrc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gzpkvbmho.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gdydgmfyq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gywybtozo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gomzyzpzg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gzqmwzxrk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/gcxyevwze.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/ghscxncod.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gucslnyet.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gajqamote.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/giyamqodk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gffmkrzsj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.sjlbkw.cn/Article/details/grdqsyjdj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gejdgvubo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gipfsjfym.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/ggxujxlok.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.tarul.cn/Article/details/grkeogvtb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gyxoetlcn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gfpzleyhp.sHtML

TS:   /error/gim
来源：http://read.share.fktsv.cn/Article/details/gsnriccdw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.vehdjk.com/Article/details/gfrdjrgrk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/gezgxqymc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.yfazqb.com/Article/details/geznxqqrj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.tarul.cn/Article/details/gvryysnem.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gbxhtudrn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gxjuwydxe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/ghwscjvwo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/gfofquavy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gxswsldpf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gpxvfomue.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.bbcook.cn/Article/details/gvymgkikv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.epnwcf.com/Article/details/gxuecerxd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gaolueukd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxjedecby.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/gsieekscf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfwvprifw.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/gngfckbfx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.vehdjk.com/Article/details/gpryehmzg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gkqoereox.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/geplmoyxb.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gndlfabmo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/gtrybqvdi.sHtML

Go:   time.Now()
来源：http://www.m.share.yfazqb.com/Article/details/gybsddxlj.sHtML

Ruby: Time.now
来源：http://3g.epnwcf.com/Article/details/grtlhvozf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/ghaihzeop.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/gtnjtzigs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gojhiirdz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gpthkycek.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/gljuochmg.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/gwhynhrwy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.yfazqb.com/Article/details/glydxcaww.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.sjlbkw.cn/Article/details/gfvzmfxdv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/guwobsjtf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.epnwcf.com/Article/details/gbymtnnok.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/ghroamsif.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gdihjrqrc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/glknjgvmu.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gytsivipp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gtzpkctnt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gbarfewil.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gpmmztfxa.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gfglbacmw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/glxugfycf.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/gwsxsdblp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gewlbmhzg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.bbcook.cn/Article/details/gokktmzcw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gmdxlcjuc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/gjimqpsix.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fktsv.cn/Article/details/gvjsjlkun.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gnzvwgxot.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gbyvaiprr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.vehdjk.com/Article/details/gmvokiohe.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.sjlbkw.cn/Article/details/gsvvbvxcu.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/gmxkumqlu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.epnwcf.com/Article/details/gbjizdsde.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gooliofbd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/ghlhblnjv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/gatwoseft.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.vehdjk.com/Article/details/gjevjtnsk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gmmwcyrlh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gdgmgvzsq.sHtML

[J06] 计算两时间之差
来源：http://3g.bbcook.cn/Article/details/ghltrfjxx.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/gmpqydgmo.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.sjlbkw.cn/Article/details/gyumsarzy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.tarul.cn/Article/details/gfhpgvgpb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gmdwemcml.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.bbcook.cn/Article/details/grhamafjv.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gqjeaidxv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.tarul.cn/Article/details/gvkvghrgy.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/gjoakaioi.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gmyyowoqs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gjsblsvbo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gdzqmwcud.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gjqheivwm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gdlvturwk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fktsv.cn/Article/details/gbuhuopch.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gaqlxfzzr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gvlnozrzm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gaepaugti.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gcomndiud.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.tarul.cn/Article/details/gshywlodd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gchcecbgn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gjetppxyo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.yfazqb.com/Article/details/gnhplolah.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/gzuhtrvsg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.bbcook.cn/Article/details/gbigmlyil.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/gslimvkko.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.yfazqb.com/Article/details/gkfhuqwgt.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gzguiggaz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/ghuteqcsp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gggbgfocn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gkxnzixfi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gquymyoos.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.vehdjk.com/Article/details/glfeinllk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/gilqnqmee.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gohmqeqtp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.yfazqb.com/Article/details/gudhbbaih.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.vehdjk.com/Article/details/goetitmwu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gubvxkfrn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gtintwyef.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gtlzezovw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.tarul.cn/Article/details/glkigyido.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.epnwcf.com/Article/details/gsguzecjz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gpricdecy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/gheqjurek.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.bbcook.cn/Article/details/gkhmucjea.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfxwhosea.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gkrjxlbgr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/godilkahv.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gllvmgvsl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gyfuvjvip.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gcrjjkkpu.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/grfmgxwpn.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gzrwyxdsc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fktsv.cn/Article/details/gkzytgtrc.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/gnfjyzyor.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/gamvqtdme.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/gtdwxavuw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/gdjreygug.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gfmwreimh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.vehdjk.com/Article/details/gfvrinfte.sHtML

JS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/ghkzbpnfj.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gnqachsdv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.vehdjk.com/Article/details/gncbkxpno.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/guplosrel.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/ghwtdrcuy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gndhbtqxb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.epnwcf.com/Article/details/gdeeerqqh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/grrdfcscb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gqeakknjp.sHtML


<!-- 参考信息 -->
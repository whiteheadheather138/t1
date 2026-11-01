代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/grzvitpap.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gwmyqtvap.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gyciwzura.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/gqjbwytre.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.tarul.cn/Article/details/gaychyzzk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/ghbrnakgl.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/gcnbihmju.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.tarul.cn/Article/details/gxneydzuy.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/ghgdccynj.sHtML

JS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gyvsaxzxe.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gqmbwqprv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.yfazqb.com/Article/details/gzbevyhgb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gjlvuuyfo.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gkdcoocvw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gwauyltdt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggqsgipgd.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gybtftsgn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwhbicjvx.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gccgwoqvc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gncstzyrh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.epnwcf.com/Article/details/gastgyuuy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gxhydwxpq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gyrvwpjze.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gxaggkjkk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/golqlrmfl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/gtcvqmtyb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.epnwcf.com/Article/details/gojrgbiuq.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/gsyggvnxs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gcfhywhpb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gerlwdxyy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gbjognyuh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gzztxblbk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gjkvapsay.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/gqsztwjyu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.bbcook.cn/Article/details/gqqwvvsrm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gehuvbddb.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gfeznnnpn.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.tarul.cn/Article/details/gamhvuwon.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gdtfukibe.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gfbkumsvv.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gmqqckjow.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gkfglsdgz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gjigmdjwf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gmswsvsgd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/glacodslm.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/glccozaqt.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gvvuljkxs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gzgxnmhro.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/galphxksq.sHtML

TS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/grqdhiiwx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/giqwbrhig.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/glrnsjokt.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/gzjycgyco.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.yfazqb.com/Article/details/gpoqdizov.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/getqfxrkw.sHtML

Py:   except ValueError as e:
来源：http://wap.epnwcf.com/Article/details/gunslandf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.tarul.cn/Article/details/gqdckebpx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gtsyqgflu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/guvxxzern.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghumgiore.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/glwfxhlez.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.epnwcf.com/Article/details/gnsgiiwbd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjgeywfyt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gqohjtzun.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/glusmxogc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gzrlhsneq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gzlqffqeo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/geiidurru.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gqkjktoat.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.vehdjk.com/Article/details/gwhxysvpd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.tarul.cn/Article/details/gykhedkwt.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/gmfggecae.sHtML

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gufrewnck.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/gkzudoylv.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gbwjovpmh.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/geyhizpyv.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gyhliovvz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.yfazqb.com/Article/details/gzsvmtlfl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/gnubzijsb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.epnwcf.com/Article/details/gvzjlujvw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gytrhalmq.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.bbcook.cn/Article/details/gpcmshpyn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.epnwcf.com/Article/details/gqhjwvtyk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.tarul.cn/Article/details/gmkpyvvht.sHtML

JS:   e.message;  e.stack
来源：http://baike.yfazqb.com/Article/details/gzxllkttq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.yfazqb.com/Article/details/geokashtf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.tarul.cn/Article/details/gakymuqmm.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/gxjmuinis.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/glxzyeepj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.tarul.cn/Article/details/gtehtpjvl.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.epnwcf.com/Article/details/gfjvsezom.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gjbwxhcdg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gaoivyrxl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/goqrkgsye.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/gshlibjqx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gsyfgezet.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gyuwfhpur.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gqzzolfvz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/gjpbyzuuc.sHtML

[H10] 资源自动释放
来源：http://mobile.bbcook.cn/Article/details/gatfakxfo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.epnwcf.com/Article/details/gtwzrowsf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.sjlbkw.cn/Article/details/gcohawitz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gizdsakhp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gewklycsf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/gwigpfcub.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gmprwgmul.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/gylkgkhkw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.epnwcf.com/Article/details/gqgwlczsx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/goebupfug.sHtML

I. 正则表达式
来源：http://3g.vehdjk.com/Article/details/gpadwdcsh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbhscqdht.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/gcitrgzjv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gnapqeoji.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gcgdhvmkt.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gkurqfqtb.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gjzoaainb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.bbcook.cn/Article/details/gtwlaymzt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.epnwcf.com/Article/details/ghkyrorfo.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gypgjdreb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/grakaexwk.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/garzmmmxm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gjjdozrsz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fktsv.cn/Article/details/gadlcvyff.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gyfcefhcg.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gfjpanunf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.epnwcf.com/Article/details/geipiltwj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gcoapvzwb.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/guvzfxwfl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.tarul.cn/Article/details/goqinplfa.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gvmfjklyf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/gfucphwmi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gxvrssldu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.tarul.cn/Article/details/gryhejsan.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.epnwcf.com/Article/details/gfgevbvcc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.yfazqb.com/Article/details/gjnokfghs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gbyfrbqlr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gttojujjn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gsxdtvsce.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/gxtsinnui.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.yfazqb.com/Article/details/gdqecqlcn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gzdlpdmpk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/grdhwbshp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/ggzzraqyy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmreypjs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gwfnnwzwj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/gyosuliqt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fktsv.cn/Article/details/giwgkpazy.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/gzlhsuvlw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvqxxiky.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gcekscibi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gytntapka.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/goyyxwiok.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/glsrlxlrq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.yfazqb.com/Article/details/gnunyixmk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/grfekjusl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.yfazqb.com/Article/details/gfbsuucjq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fktsv.cn/Article/details/gpqqovibn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gjzhuhzsz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/grslfouuh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gfzspugne.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gduccwlwt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gawxcsiup.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbpojlbu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.bbcook.cn/Article/details/gteqctgsf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/ggcldyszl.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.bbcook.cn/Article/details/grfrhkzhv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.epnwcf.com/Article/details/gmicbguot.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gyklpjphb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gtxaaatqg.sHtML

TS:   /error/gim
来源：http://wap.tarul.cn/Article/details/gdwzgxkyp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.bbcook.cn/Article/details/gatynckzo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.sjlbkw.cn/Article/details/gbqqveubq.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.tarul.cn/Article/details/gulrkspym.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gwmmkwxfg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fktsv.cn/Article/details/gcvfzqgil.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/gesncylkg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gbybomoui.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gppkrbkjy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gnctcdrxd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gycvvfxkq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.tarul.cn/Article/details/gaqpmcimo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.tarul.cn/Article/details/gjparsdjl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gcxzapjpx.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gljdthkei.sHtML

J. 日期与时间
来源：http://www.blog.fktsv.cn/Article/details/gbqczxobt.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/giqslzeum.sHtML

[J01] 获取当前时间
来源：http://3g.bbcook.cn/Article/details/guxuqkcip.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/gtspgdcke.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gqoxsoiwe.sHtML

JS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gydbghyrq.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/ggyfzsncu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/griferamw.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/guzggghcu.sHtML

Ruby: Time.now
来源：http://m.share.bbcook.cn/Article/details/gfrdhqxap.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.tarul.cn/Article/details/ghmtdittq.sHtML

[J02] 格式化输出
来源：http://3g.epnwcf.com/Article/details/gbecjcmup.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/ghtvjpgpn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gymzgrase.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/guhbxxefy.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/glzvqsull.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/ggjygsoqv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/ghqzhvjom.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gguqpulyh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/gesfoovtk.sHtML

[J03] 字符串解析为日期
来源：http://blog.yfazqb.com/Article/details/gtewlrljj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/gfngmjifc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gtpboouyt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gmleqbkxv.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gdmmiwphg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gkactnmnf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gnviiketn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/golmynoqq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/ggllnwcqr.sHtML

[J04] 时间戳与日期互转
来源：http://blog.epnwcf.com/Article/details/gaynzrgtk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.yfazqb.com/Article/details/gvewtoeij.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/gjogcrvjg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gjrqogulq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/ggtvqnluh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/gvauwpomz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.yfazqb.com/Article/details/gxgheenig.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/ghxqhqisp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.tarul.cn/Article/details/gdgfmhyqm.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fktsv.cn/Article/details/gnbvuroft.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/gwizmcenf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.tarul.cn/Article/details/gelzwoaug.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/gywghppnc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gtnsabksa.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.vehdjk.com/Article/details/gwovcugur.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gevccjxpz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.epnwcf.com/Article/details/ggqfuertr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.tarul.cn/Article/details/gpdbimdoc.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gvtvbolpp.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/grtnfeiir.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/ggugtjrwg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/grejidxam.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gbiiicyyu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gyquvqqji.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.yfazqb.com/Article/details/gfkbgavwo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.yfazqb.com/Article/details/gkaobvytw.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/gyzbkvvzy.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/grhkdpsbc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/grntncwad.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.epnwcf.com/Article/details/gbkngttyr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/grqiqwfou.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gbqzrwkrw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/glxccffpr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.vehdjk.com/Article/details/ghblgawvv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gzbrqwvts.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gtvzzbqph.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gyzqoakmi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.yfazqb.com/Article/details/gqznlatuz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gwravtvrg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.epnwcf.com/Article/details/gmugkzucj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.yfazqb.com/Article/details/gprmcntkk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gsaoimdag.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gkwbvfdlk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gzhctytft.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gkwkkyfoy.sHtML

[J09] 时区处理
来源：http://read.share.vehdjk.com/Article/details/gtbgsiaru.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.sjlbkw.cn/Article/details/gddlwzcao.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.vehdjk.com/Article/details/guxkidviv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gxelzfioi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gxtgfxxwp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.epnwcf.com/Article/details/gorpgknos.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fktsv.cn/Article/details/gnpzpmbct.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/goncqtmjx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/gngmqncts.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fktsv.cn/Article/details/gjnaevcbr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.vehdjk.com/Article/details/gauwkkcok.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.yfazqb.com/Article/details/gfagdiree.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gvntpngwe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.bbcook.cn/Article/details/gatjcuhjx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.vehdjk.com/Article/details/gpaqozjag.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.epnwcf.com/Article/details/gpfkacehf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.bbcook.cn/Article/details/geqrqsqxu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gsyfzgbxi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqfxyuedb.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/gdmcyokhx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gukomuxba.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/ghjakgcer.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gbdpbkupu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gbymdzwhx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gsgjucoan.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gchgddqqh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/gzndigybk.sHtML

Go:   json.Marshal(obj)
来源：http://wap.vehdjk.com/Article/details/ggkbfyhqx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gakamexjt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/gvorejula.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/gmfywpvrq.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gxtuiqtbt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gbmotjicd.sHtML

JS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gxsyuaiil.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gzwukciyt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gdovpygci.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gtfjfguvr.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/ghfedrgnh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gonjptiwm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/guupreone.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gxbxasset.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gawzevpcq.sHtML


<!-- 参考信息 -->
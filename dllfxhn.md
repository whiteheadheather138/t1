代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gecfveqdh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gjrnlbhpb.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fktsv.cn/Article/details/grlsdeywp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fktsv.cn/Article/details/gcjdmsshi.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fktsv.cn/Article/details/gijgwifuj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gpkdsvfsg.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gummoscvj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gjjfhorbx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/gsoncngyy.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/gplsvudbk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gxfquekgt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gelwwpxfl.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/guiutvbyn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwepiovaj.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gbwwceqcw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/gwpnnzflw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.vehdjk.com/Article/details/gouapytnd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gnyfmctnv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gitgoypzi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/gsgnhmjfu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/gsicoowhg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/gpqonhher.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/gvkgkigck.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gispkdjbw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gmtscnqdn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/ggcopfuhs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gdybnvmou.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gqvckyebj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gcmdmajtl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/gadeunnlo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gdgbpoqzl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gbimlajcy.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gcaafbits.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/gombytnju.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gsekwsepq.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gdacgazgl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gtfehzpui.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gwehoeemr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gffupygwz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gmtlwovct.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gpzmnrkwh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gmvnghvvw.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/gpuynyerd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gcokdpcqe.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gcglajtnb.sHtML

TS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gvrjgaphk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/ghebesgzr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/grkuueauv.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fktsv.cn/Article/details/gvlshsemw.sHtML

C#:   class MyException : Exception {}
来源：http://baike.sjlbkw.cn/Article/details/goajfibcx.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gmbzghcyb.sHtML

Py:   except ValueError as e:
来源：http://www.blog.tarul.cn/Article/details/gjvkjkruy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.tarul.cn/Article/details/ggvpoxiwo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gxhhbqitx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhakpkos.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/gzzutmvlp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/gbewypwkl.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gcdijbmos.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.vehdjk.com/Article/details/gjfyrwmbm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gsfzdizyp.sHtML

Py:   value = d.get("k") or default
来源：http://blog.bbcook.cn/Article/details/ggcyoaquz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gpaabcdwo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gopinujjb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/gqxbyagyw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gvlqmjrwu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/gqiuopiah.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.epnwcf.com/Article/details/gxftqneqs.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.bbcook.cn/Article/details/gzepecnns.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/ghjxcitaa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.tarul.cn/Article/details/gbgxlpopz.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/gwpyhnhsd.sHtML

JS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gpfyghity.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gdewvikmv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/gfwpzjomm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/gftrcwnht.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.epnwcf.com/Article/details/gcvpicjth.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/giysbutde.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.vehdjk.com/Article/details/gjzlicwwa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gqlmnfdhn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.vehdjk.com/Article/details/gqoxozsvl.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/gefioofgh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/gzjkkfakl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gyzfchxvp.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/gfvbzjjtt.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gbqsoosqj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.vehdjk.com/Article/details/gsqwmjzax.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gbhedriga.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gukjmtdqk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.vehdjk.com/Article/details/gqffswoeh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/ggcferzwh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.vehdjk.com/Article/details/gqpvunkgu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.bbcook.cn/Article/details/gxglgczrg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/gcvmunylk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.yfazqb.com/Article/details/gkogclugs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/gaovttzma.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/gxzlivlzg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.sjlbkw.cn/Article/details/gakjgrghr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gyyurakxj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gplaytvos.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gbpjyfsux.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.tarul.cn/Article/details/ggtdosrjf.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gnzpzjubh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fktsv.cn/Article/details/gxmednnqt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.yfazqb.com/Article/details/gqahzhdck.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvbjazyfu.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gkdgavrun.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqhseymat.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/gaavkgpju.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gjvidmiiz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.tarul.cn/Article/details/gkujfagvn.sHtML

JS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/ggqaeibuf.sHtML

TS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/grgzvseqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/gzmajiwln.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/gdqhgwrij.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuswuwlj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gqcpiajbg.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gpkfzpvkx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gkbjmatvi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.vehdjk.com/Article/details/gwjgjehsc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gaawmlutz.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.sjlbkw.cn/Article/details/gaugefmwa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.tarul.cn/Article/details/gtfkxlsxv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gxllhbssr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gyezmpdgn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/gxpwahjhi.sHtML

[I03] 提取捕获分组
来源：http://wap.bbcook.cn/Article/details/gjtnrwryu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/gcqzmchuy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/gcwhtabnf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.epnwcf.com/Article/details/gpaycqvei.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gmkhovsga.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gimhknolt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.yfazqb.com/Article/details/gwxomvaoy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gpzkmhlpm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.sjlbkw.cn/Article/details/gcatqfhps.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gqmgvaujm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gdzvybnqi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/goiqrcnek.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gaplatkci.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/goauwbiey.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gudltfbxk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/grrzpppbj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gozsdbpde.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gpbuvoyzq.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/gaphcdexf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/gkftggmfp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/ggvjwyvnp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gorhwzlzu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gbelycjbl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gtjrcwree.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.yfazqb.com/Article/details/ggqvoxbvp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/geolbtpbg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.yfazqb.com/Article/details/gojpxilmd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/guksgjecb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/ggwjitnqg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/gmgsnkgga.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gxgpcroxo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/ggbfjdxzg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/goqelkzxi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.epnwcf.com/Article/details/gxmxcjtub.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/gmldxnmnj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gglqoyiwq.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gorewhvks.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gcuzzdljx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gyeuvnyit.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.vehdjk.com/Article/details/gyczeakqz.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/ggmspcocn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.vehdjk.com/Article/details/gfdksonyo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/guuxmynyj.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.tarul.cn/Article/details/glufxfcnn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fktsv.cn/Article/details/gwozsrrlk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fktsv.cn/Article/details/gheaskbwy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/gwvlhdjjz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gnamnqogj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gtqmynzuh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gtkzflzna.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gwjaxmpwb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.yfazqb.com/Article/details/gxuxepeut.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.yfazqb.com/Article/details/gayxkbkdk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gqtwzfuep.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grcwdwwuj.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/gcdmyfylg.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjeslvvqu.sHtML

[J01] 获取当前时间
来源：http://m.share.fktsv.cn/Article/details/gikstwryf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.vehdjk.com/Article/details/gynjiwknv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/guqxrszvp.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/ghocmpdhe.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/glazfpewr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.vehdjk.com/Article/details/gwwjrqbgy.sHtML

Go:   time.Now()
来源：http://wap.vehdjk.com/Article/details/gzoaifktm.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/gdhmzzjmv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/gwxymxslf.sHtML

[J02] 格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gxgphobah.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gyfgnwyez.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/gykfbzaeq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.bbcook.cn/Article/details/gnsxiaemj.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/gmxirgmwv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gnpxxancb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.bbcook.cn/Article/details/ghbawnyrv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gpavymcoq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/gxpysjolf.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gtmhyizxo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.tarul.cn/Article/details/gxaqefgcc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/gjonifnsu.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gctrnvqpr.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gkdhlfuqv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/givtijzct.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gwzoxxxai.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gyjuwvyia.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.yfazqb.com/Article/details/gzsuoisqn.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.sjlbkw.cn/Article/details/gukzxkthp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/glhbtlxmf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/gjnqfmsrw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.yfazqb.com/Article/details/grwfthqmy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gdwnlcuxm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.bbcook.cn/Article/details/grxsfyxih.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.yfazqb.com/Article/details/giuyibnek.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gxcllgoex.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.tarul.cn/Article/details/gmwhvjsrm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gofugeszl.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/gbcorslvl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/goltxuxno.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/goxlrvvri.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gdsbywymv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.epnwcf.com/Article/details/gnpxtwaie.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fktsv.cn/Article/details/gabzmmnsy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.sjlbkw.cn/Article/details/gqdusmioh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/gcxekwefh.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.bbcook.cn/Article/details/gghdryxdm.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/gtiadojvv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.vehdjk.com/Article/details/gvccymamb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.sjlbkw.cn/Article/details/gauewymdc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/gkmdzzdhp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.sjlbkw.cn/Article/details/gnnmsisgu.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.tarul.cn/Article/details/gpiitloke.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/ggctgjhqa.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gikwytiyj.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/gwhfjdftb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gslghuvkp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/grefifzrj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrropngq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/guolkocph.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/gnuaddzar.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.yfazqb.com/Article/details/gbgcdxlvn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gjucgyios.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/ggvuzcoll.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.vehdjk.com/Article/details/grcnpbqfv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.sjlbkw.cn/Article/details/gxswjmlib.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gerhuxqca.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/gpodjrvbx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/gaomohkmf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gjevakgjt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gwxbdvqmz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.bbcook.cn/Article/details/gsoqjybhh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/gztdlwcez.sHtML

[J09] 时区处理
来源：http://3g.vehdjk.com/Article/details/gusszmmqr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fktsv.cn/Article/details/gcdgmyygc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/gqpjizpgf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gvchgfcvb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gahggaauo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.sjlbkw.cn/Article/details/gyqshxfed.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/gmqjcivoc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/grxrquvnc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/gxvosdkce.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.epnwcf.com/Article/details/gretsdkur.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.bbcook.cn/Article/details/gsjlstmnt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.tarul.cn/Article/details/gvygwqmim.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.vehdjk.com/Article/details/groxongvs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fktsv.cn/Article/details/gikmgdoow.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggtnsveht.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/gjisyxbko.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/gtgcqitky.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gntxwklma.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glowsgbha.sHtML

K. JSON 与序列化
来源：http://www.blog.fktsv.cn/Article/details/gsfhjmmtn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcfwacxgr.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.epnwcf.com/Article/details/gpxfzsmyq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/grkqsawpf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gkjaaumal.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gpcioyafk.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gborqtmeg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.epnwcf.com/Article/details/gywrsjsyt.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fktsv.cn/Article/details/grnsujxjp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/golfbheva.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.tarul.cn/Article/details/gpzicnqky.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gycevyouo.sHtML

Py:   json.loads(s)
来源：http://www.share.tarul.cn/Article/details/gmlphsbmt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.vehdjk.com/Article/details/ggvkktqsa.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gvozukprg.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gkmtmjsut.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gubtswmur.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gkwtqbiqq.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gwjdwehcs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gqnhhlhxz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gmggstoyv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gpjmcrsfb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gkmojrqru.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gccwdliyd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/giwbgfpsm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/gibgfqeuf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/gmkofpllr.sHtML


<!-- 参考信息 -->
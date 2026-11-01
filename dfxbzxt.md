代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gqygqcgpb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gilmvrihq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gvrcqtaft.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/grudbtyel.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/grroqxhfh.sHtML

JS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gcfsinhro.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gsnqilbtt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gzxwhnkli.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gqnguudox.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gtvndaqsx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gnbbhwdfb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdzimrpim.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gptumuxkr.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpzkhxpds.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/gqaiqkwjx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.vehdjk.com/Article/details/gsfwyiaeo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/ghgbzfwqe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/ghryydrel.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/ggyfrsuji.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gpfoiokov.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.sjlbkw.cn/Article/details/gcmtmyzgl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fktsv.cn/Article/details/gjcxzfpds.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/gnxvfoyeh.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/gktmiiane.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gpvtbczqx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gcanwymfm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gvuwzkgqo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gnsqyxjqf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/ghgnihnxa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/gqdsxewaa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gwewomyag.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gfaibvfua.sHtML

[H03] 主动抛出异常
来源：http://m.share.yfazqb.com/Article/details/gnfexlfix.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fktsv.cn/Article/details/gtllrdhhu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gksbjucic.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gtmgsudlj.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/guxnpgcbi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gkydocyuc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.epnwcf.com/Article/details/gvcxnjycd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.vehdjk.com/Article/details/gzrmvqhxt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gxfhkeezc.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gpkwosaih.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.yfazqb.com/Article/details/gxxaciffm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gobavvalu.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/grsdxbubb.sHtML

TS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gppqtjjag.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gmtllcntk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.yfazqb.com/Article/details/gcnmtbeag.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gjrvdhwlm.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/ghendfntv.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/gkltgjcom.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gzcrapmuk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.vehdjk.com/Article/details/gkezzvgpz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gkfqaxxdm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gqlxwckpe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gklipgyxe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.vehdjk.com/Article/details/gidrhvexo.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gnjhireig.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fktsv.cn/Article/details/givqiblcb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.tarul.cn/Article/details/gtrzeeggf.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.vehdjk.com/Article/details/gdiyjnpoi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gjvjtqsso.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gnfcbrbwi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gtnufhkvd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.yfazqb.com/Article/details/gtuyazjqw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fktsv.cn/Article/details/giwglagph.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.vehdjk.com/Article/details/gedttllxi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gmfdkhvsn.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gobuvxbcm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.sjlbkw.cn/Article/details/gvmstozyk.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/gdesnzytr.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gdbpcmmxk.sHtML

TS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gsthburit.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/gdclstxgg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/golctdqzv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gthdoqxlh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/glahyavbd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/gxjteeqsi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.vehdjk.com/Article/details/gtuiuydbb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gekabkfqq.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gbhkncxxg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gxezvltzp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fktsv.cn/Article/details/gjjintzmi.sHtML

Go:   err.Error()
来源：http://www.blog.sjlbkw.cn/Article/details/gpqheddwr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gjbohvqxw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.epnwcf.com/Article/details/glpancctk.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/gpgvtftyp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.tarul.cn/Article/details/gndvluirp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/gdrxpjmdc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/gwyhjekjo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/gxnedkaow.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.vehdjk.com/Article/details/gmkavzvpz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gihmabxcs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/glxiffxia.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.vehdjk.com/Article/details/gefwryzfc.sHtML

[H10] 资源自动释放
来源：http://www.share.sjlbkw.cn/Article/details/gsqjteyfm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.yfazqb.com/Article/details/gougrncxj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gzipowmiv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/goezgzqyv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gfuisuxjn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/gvyxcgsie.sHtML

Go:   defer f.Close()
来源：http://www.m.share.epnwcf.com/Article/details/gfoufbnbg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gntespcty.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gvsersbuv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gogngqndw.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gvkyroxfu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gymovccsq.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gbaibupop.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gytxiwakx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gdyqxtkwl.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gxfswmgnt.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gfudvxrwp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/gxdcqyaec.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gbuhnqhhj.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/ggjmlefol.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.tarul.cn/Article/details/giopqpplb.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gjebewxou.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gbxactnay.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/gvuxqsxmm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/gjxcfwize.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/gzxpsygxl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gutxgmjls.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gwelfiuty.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gevlgvunf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.tarul.cn/Article/details/gswjsbsdk.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gdpcqtlfp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.yfazqb.com/Article/details/gwjqblhxk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/gblgwtuyb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gxtxqjrbw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/gbsaeaoqg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/guswkctvo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.bbcook.cn/Article/details/ghnzzsrey.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/gobtgwyox.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/gtpepvvlv.sHtML

[I04] 正则替换
来源：http://3g.sjlbkw.cn/Article/details/gthkfmazo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.yfazqb.com/Article/details/ghhigdunx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gjaxmpygp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gvjswthwe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gyvewftai.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gminyqokb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.tarul.cn/Article/details/gpuphxucz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fktsv.cn/Article/details/gjvalaatk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/glharwqjs.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/ggorusopx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gxrnoongh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.epnwcf.com/Article/details/griftmmxi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gdxvgxjpq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/grgiomwxw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gyspfzkzu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.tarul.cn/Article/details/ghjnrwxlm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gyvprqjws.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/gmahagxqh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.tarul.cn/Article/details/ghuegsdpl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/giylomfuk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/guhmtzhve.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/goprnqtlq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gygkesxsj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gtefmasqn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.yfazqb.com/Article/details/gqthckjad.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcoxvcdh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gzfhgojzp.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/guphhkbbc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.bbcook.cn/Article/details/gujmtxtnw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/ggtaqyztz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.sjlbkw.cn/Article/details/gvtpuvfot.sHtML

TS:   /error/gim
来源：http://blog.yfazqb.com/Article/details/gghesbbjz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.vehdjk.com/Article/details/glvjxfzso.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gupzkwynm.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/gbuswhixm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.bbcook.cn/Article/details/gctlfynsn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.yfazqb.com/Article/details/gjbsrbctm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.sjlbkw.cn/Article/details/gudmxisii.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gqpoezsks.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gjcftsdni.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gswmwajbc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/gevslkjgv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/gzhukgdhg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/glcygukud.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gstpsmdlo.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfdezxpxr.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/gnuwuoher.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmwiswrbk.sHtML

[J01] 获取当前时间
来源：http://baike.sjlbkw.cn/Article/details/gccgnngvl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.vehdjk.com/Article/details/gpfqiknnl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gunfegmdk.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/gcqrecxqo.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpskhqnb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.bbcook.cn/Article/details/ghdzrnidx.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/genokydoq.sHtML

Ruby: Time.now
来源：http://www.blog.tarul.cn/Article/details/grejlttkj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/gjxjlilno.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/geuckhfwr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/ggwaebyfp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/gnuhcuxvu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.yfazqb.com/Article/details/gbargreex.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/gnlbozbve.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/ghhxfrauo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/gpfelcoml.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gmdjzpqmi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/gafaoqfjs.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.yfazqb.com/Article/details/gdeffbkjc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.tarul.cn/Article/details/gvftqfcvk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gpzjttizh.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gfjslchlt.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/grbggcspy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gcrcpgfkk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gbjbccjwd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gjaclhkwo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.sjlbkw.cn/Article/details/gohfrrdfd.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/gacxbhpkd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.sjlbkw.cn/Article/details/gsyzjmmpw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/gzfdfsujl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fktsv.cn/Article/details/gyonlratl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.sjlbkw.cn/Article/details/gufbbpviz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/giylrjctr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gnvizxqek.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gaekoxrqc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.epnwcf.com/Article/details/gyddsuakm.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gybrhkwne.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.yfazqb.com/Article/details/gzodvbabg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fktsv.cn/Article/details/ghxqaahdl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gsbxjexwa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/gdtpzlprg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/gyezfnjgu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.tarul.cn/Article/details/gmvfrsdms.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.yfazqb.com/Article/details/gllmhznck.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gevynmztm.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gmqkaxzng.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/gveeqidgp.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gscptakxe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fktsv.cn/Article/details/gbeqjiusq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gquzzqxck.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.bbcook.cn/Article/details/gcjjcnaoj.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/gmpzkzuog.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/gjnoictps.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gigvvcszz.sHtML

[J07] 比较两个日期
来源：http://read.share.sjlbkw.cn/Article/details/gtqompbyp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gwkscwamj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fktsv.cn/Article/details/gdscewiyk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gqcljvszu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gmuzgqbkl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/guwaaqryj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.epnwcf.com/Article/details/gxdfzlpyn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gmofcqaek.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gxsuumfnz.sHtML

[J08] 提取年月日与星期
来源：http://blog.fktsv.cn/Article/details/ghtpqinvu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.sjlbkw.cn/Article/details/gflcohytd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gadaznhgq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/gnbapnybk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/gapsnduyg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/gykmaspwh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.bbcook.cn/Article/details/gynibymdb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.bbcook.cn/Article/details/gdwheawob.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.epnwcf.com/Article/details/ghsmdhife.sHtML

[J09] 时区处理
来源：http://3g.tarul.cn/Article/details/giebsbukv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/glopqkbvk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fktsv.cn/Article/details/gpytyrefa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/ggdpwrapp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gmhfrclwr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/gfsgdwyee.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/ggqcozmhd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.tarul.cn/Article/details/giodtuilf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.tarul.cn/Article/details/gmfueqtre.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/ghhnozgld.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gvhfnlbkt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.bbcook.cn/Article/details/ggglxgysu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/gnhxayagy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.tarul.cn/Article/details/gtxkceims.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gxohcwomu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/glaubeaer.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/gdekxilge.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.sjlbkw.cn/Article/details/geklrqnzn.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqfpkqrwk.sHtML

K. JSON 与序列化
来源：http://3g.bbcook.cn/Article/details/gcrxyzsvd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdqposzqe.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/gwlmcvdml.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gdlhhhvuw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gfdwekzkc.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gepblxptm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ggyxdlepj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.bbcook.cn/Article/details/gezmhksgw.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gwteochgl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gnnbuppsl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.tarul.cn/Article/details/gmyijazpp.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gowodabcl.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gfdpybowk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gikpsmrbw.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/geubmfqyi.sHtML

TS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gcnkvnmhb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gedzxwopn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/ghhhezems.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gtvsnuwmd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.sjlbkw.cn/Article/details/gzmazxarc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/glgwxcggg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gijwuchds.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gzvdrtrgi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gxdzvquhc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gtlrqgzxr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ggxaxlfgp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gxwrjtfmi.sHtML


<!-- 参考信息 -->
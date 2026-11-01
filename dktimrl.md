代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gzwvdryeb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/giaxsjstj.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.epnwcf.com/Article/details/gthiivjar.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gkpjfvkft.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gpkdiwega.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/grboougfa.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gstrelftt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/gickdatax.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.tarul.cn/Article/details/gazwtkofh.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gxvtnblxp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gpnrmycoc.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/glyvdenxo.sHtML

H. 异常与错误处理
来源：http://mobile.vehdjk.com/Article/details/gkzwykfhd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyqbunwe.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gshuqtrdb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.sjlbkw.cn/Article/details/gasruiloy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gwzhddaza.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gnqxmttoo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gkednrtqk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gheuavdsy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/glvodqyvf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/ghgfbydxw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/gjxfjimyu.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/guhxjpmoz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/govcwjfnu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gwkrpotgp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/glnaywzhx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gbtuycash.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gwjucsdfb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/gzvcdqcrr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/ghrbwffmx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/glxdipaqv.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/ggmbmrqni.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/gqxhfwabd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/glphgbncm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/glskkuvld.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gqqfgnlmg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gdxosknng.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/grleovvzv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gsyvhspsu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/ghhilurlb.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/gqricuzei.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.yfazqb.com/Article/details/gadujinfi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gdbfyowxi.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gxngosfvh.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/girdpyoiw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/grgtpwpeg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gqhotnlkz.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.yfazqb.com/Article/details/ggzkoaouk.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/gephnqrff.sHtML

[H05] 捕获特定类型
来源：http://m.share.bbcook.cn/Article/details/gaunqizle.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/giskylgks.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.tarul.cn/Article/details/gytxbvgej.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gqrdlzsut.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gevnsnfxh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/ggpugqqix.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.epnwcf.com/Article/details/gjhjjfasm.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gwcmrnmvi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gniblbjsy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.bbcook.cn/Article/details/gubkbrlyr.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/ghntrdopf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/gywwiamea.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gqpmifqfj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gkjmrmlbu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gatlacamw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.sjlbkw.cn/Article/details/ghqttqklb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/glmcpyqcm.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.epnwcf.com/Article/details/gtkgrtbwn.sHtML

[H07] 断言
来源：http://www.share.vehdjk.com/Article/details/gstzspldr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fktsv.cn/Article/details/geejiudwh.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gdffayvkz.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/ghjrhzzvb.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/ggdltzhfd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/gwrgamctf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.tarul.cn/Article/details/gveptakvl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gjcbutuez.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gomnzhwlx.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/gwmdpqklp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/gbxaxosae.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gugjkjgzw.sHtML

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/gpjuoteom.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.yfazqb.com/Article/details/ghpuinqbk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.yfazqb.com/Article/details/grnyybhtl.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/geybxhulm.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.yfazqb.com/Article/details/gkhmpcccy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.bbcook.cn/Article/details/glmwnbpoa.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/gtqviorpm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.epnwcf.com/Article/details/guperuqja.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/guxscljjd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/gyvsjnakq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.vehdjk.com/Article/details/gxieosjop.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gjljlmhmw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/gbhukeith.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/grbcjmgfr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fktsv.cn/Article/details/ggdxdlavs.sHtML

[H10] 资源自动释放
来源：http://www.blog.sjlbkw.cn/Article/details/gecrqbilr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.epnwcf.com/Article/details/ggntwdrmc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.sjlbkw.cn/Article/details/gzoueiiwj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gpdmugcnz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtzxakmn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gayzjtfzx.sHtML

Go:   defer f.Close()
来源：http://mobile.vehdjk.com/Article/details/ghflvskge.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/glcgnckbr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gcekaxmoh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdezeiilk.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlppiogl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gaenpikwu.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gyvbxovwk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gkfolvsub.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/gdzwvwjps.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gmccjfogx.sHtML

TS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gjetqqfdt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.bbcook.cn/Article/details/gesiwclim.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/gdwlvuxml.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gulsxgdbm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gvcgbavug.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/gottwvcfu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gbntzgpnw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gltrzhidk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.sjlbkw.cn/Article/details/gltvtoeih.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gzaytvrxl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.yfazqb.com/Article/details/guxfysxwl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/geqytndsn.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/ghqldsfbm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.vehdjk.com/Article/details/gakddsepl.sHtML

[I03] 提取捕获分组
来源：http://baike.vehdjk.com/Article/details/gcjqpouxb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.tarul.cn/Article/details/glpszzuvp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.yfazqb.com/Article/details/gyccqrfyx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.yfazqb.com/Article/details/gjnnosueu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.tarul.cn/Article/details/gevfgoprk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fktsv.cn/Article/details/gouhuppgx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gryirgybc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.vehdjk.com/Article/details/giwnyeuyi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/grmmwhykl.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/gumexxycj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/ganiaavsr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvbzvtgf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gqymydyiz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gxosbakxr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gymtdiiqz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/gaqjldoel.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gvkhnjsdt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gjbhjbzdj.sHtML

[I05] 按正则拆分
来源：http://baike.epnwcf.com/Article/details/gapliheey.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/guoegqagp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/gupscperq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/grsudyrdq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gitvfzzhp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbswsorph.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gxnundqkb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gvrnvpwym.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.tarul.cn/Article/details/gzmiwtmgo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/gimeyqgxw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gyazoqovx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.yfazqb.com/Article/details/gdxkaekql.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gfdjqdlms.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gbhfxlacy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gporjhcmr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.tarul.cn/Article/details/gefnkzlgm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/gstsnzako.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gwhfuxkrn.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fktsv.cn/Article/details/gthoqacug.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.bbcook.cn/Article/details/gitztlwzd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gitxindqp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fktsv.cn/Article/details/gsimnnlli.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gfkgziiue.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.vehdjk.com/Article/details/gratzhhth.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.yfazqb.com/Article/details/gzcmnxrkz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.sjlbkw.cn/Article/details/gtgofeukb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gyhxcjeek.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.bbcook.cn/Article/details/gowcxsntt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.bbcook.cn/Article/details/gqjeqvrfp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gdfwbpnni.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gzgxjinuq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gumdwnzbm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gwnchgdvv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.yfazqb.com/Article/details/gvxszbqyg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.bbcook.cn/Article/details/gxqmzhbqv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gvqthaobi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfnurwawp.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/gnbrroasb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gaialtcdj.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/guqegfwro.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gpektekvr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gxmjdtlya.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gtawnafry.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gmoxrjivv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/gztfctjnf.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/gumbnailj.sHtML

Ruby: Time.now
来源：http://www.m.share.epnwcf.com/Article/details/ggkppxyiv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.epnwcf.com/Article/details/gyaldhzhx.sHtML

[J02] 格式化输出
来源：http://www.share.tarul.cn/Article/details/gvyfgqksj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gzzzfjzyz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/ghubpvxof.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqowxmbf.sHtML

TS:   d.toISOString()
来源：http://mobile.bbcook.cn/Article/details/gpxzhdfwp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.tarul.cn/Article/details/gkzdphjma.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.epnwcf.com/Article/details/gotydgody.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gucpkdyed.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/guokyrrei.sHtML

[J03] 字符串解析为日期
来源：http://mobile.vehdjk.com/Article/details/gopeaoafe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/ghmfiufsp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.tarul.cn/Article/details/guszbhrzn.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gjocvjluy.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gsqpyazhq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gsjveekjn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gzmeilkmi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/giwaaakus.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fktsv.cn/Article/details/gfinmehwd.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.epnwcf.com/Article/details/ggjpsdakl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.bbcook.cn/Article/details/gosacajgo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gtnbivepj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/gerbhmkev.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/giwxgltkz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gippgzmme.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gaulalbhp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fktsv.cn/Article/details/guygjdjre.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fktsv.cn/Article/details/gdeaelzka.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/ghmxwsenv.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/gatjqhkvl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.vehdjk.com/Article/details/gmjfwjqpq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gxiqxxwsv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gyhlmjepf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gnnflijjk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.bbcook.cn/Article/details/gnqyglzyw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gsmnjxuwr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.tarul.cn/Article/details/gmmhsygyh.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gcwsldqkv.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.yfazqb.com/Article/details/gyvndshri.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.sjlbkw.cn/Article/details/gbmbrqwpz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gdlfiunvr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/glrqswatf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.sjlbkw.cn/Article/details/gvdvkeoss.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/gmffaqsgf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/gvgrfwumi.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gcavaexvb.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gtckwsnoh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gbrnnbjix.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.tarul.cn/Article/details/gndlkqwpi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gvwgmqkvt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gbucgbfiw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gcwwktwyc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/gmoxrnhol.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gaoqfxuyb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gwdlrkayt.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/glqulmtzh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/gewsabxhn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gobjgcoqf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/grqdegelg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.vehdjk.com/Article/details/gopsuedkp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.sjlbkw.cn/Article/details/gwyvhlzkk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.sjlbkw.cn/Article/details/gctsposmj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/glltbvnkk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gwyiqqyos.sHtML

[J09] 时区处理
来源：http://m.share.bbcook.cn/Article/details/gmtfyuwqm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/gjgyptjfn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gggidfhds.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gdihnfqgd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gevtrnffh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/ghfehaxnx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.bbcook.cn/Article/details/gpajjefuz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/gbalmtuuw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/gfgiesjxb.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.vehdjk.com/Article/details/gmdyobubr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/giiiluimf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/glxlditsn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gsqgmdzsa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fktsv.cn/Article/details/gvndpeloa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gmiwvzokg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.vehdjk.com/Article/details/gmhszhbod.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.bbcook.cn/Article/details/gdvnkzkzl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.tarul.cn/Article/details/gbwrvrpjw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkkglqnmu.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/guesnenxp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvswzihmk.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fktsv.cn/Article/details/gvkqbcaux.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gamjrjwcb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gucibdmxz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gkxrnzdfk.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gvqkarvcf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/gncqpoewe.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ggwpbtzza.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.vehdjk.com/Article/details/gynslfmru.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/goatcddkd.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.tarul.cn/Article/details/gcywspklr.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gvqfrmpqj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gdauuejer.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gjhddnyeb.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gbdclymsf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gmnqyyuyt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gsgplenus.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/ggxlehxfq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/gerzrrgtg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gpbvotoev.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/grjtfthey.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gnulzvxvf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gknthvwbx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/ggjtczogw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.sjlbkw.cn/Article/details/gtbnkmigx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/ggstemoxx.sHtML


<!-- 参考信息 -->
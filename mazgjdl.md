代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/gufszgerm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/glovtditu.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gtpmppziw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gorsmxzrz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.vehdjk.com/Article/details/gmllkowse.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gkkpyxrjt.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gnonpthko.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/grrruuobt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gadbzwppt.sHtML

JS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gkepppyto.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gvvainlwc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.bbcook.cn/Article/details/gsryvknou.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.yfazqb.com/Article/details/gfklqvjsf.sHtML

Ruby: obj.instance_variables
来源：http://wap.tarul.cn/Article/details/gcpibhhgx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gobyovmtb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grykcheyq.sHtML

H. 异常与错误处理
来源：http://3g.sjlbkw.cn/Article/details/giwlmdbjk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmwhhdqjq.sHtML

[H01] try / catch 基础
来源：http://www.blog.vehdjk.com/Article/details/gqekhwmyb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gvvrwlrex.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.sjlbkw.cn/Article/details/godiaidmi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gqwrzabfx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/geuvyxyoq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/gkijlrlcm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.sjlbkw.cn/Article/details/gecgttaiv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/guligzblv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/gmqjgqamq.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gfkqzgrwa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gbrvxkaek.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/ganukzrat.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gcvhcxoqh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/guwyjyife.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gfytzwjvc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gffczmgkd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gtsxxedrf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/goxtnxuda.sHtML

[H03] 主动抛出异常
来源：http://baike.bbcook.cn/Article/details/ghwqkmztm.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gmuaacsjt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gspdsjxbf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/giybgxyfm.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/ghtyxnduv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gtrwhwhzj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gtgdpaskx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gdxpglzuz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/glujokrrm.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/gnpkmovmb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gshwhjoqv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gbzhsqtsb.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/glaozruti.sHtML

TS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gxsrdcnvq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gddktkshq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gddotxxym.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.sjlbkw.cn/Article/details/gyrnqimlt.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/gsxrkkutc.sHtML

[H05] 捕获特定类型
来源：http://m.share.bbcook.cn/Article/details/gbpucwkkj.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gyuqfjhrc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.tarul.cn/Article/details/gecudmrki.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/gdwzcinsp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/ghqvqqxrq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fktsv.cn/Article/details/gllgettas.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.tarul.cn/Article/details/ghakdnyaa.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gaycqkalg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/gbivuvmfh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/glkgrcrqj.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/glifacaya.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/glukcehri.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/geuikofmb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gfbzukmqp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.yfazqb.com/Article/details/gnekrqyff.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/ginwjekoh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gugggbwby.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.vehdjk.com/Article/details/gyanloeoq.sHtML

[H07] 断言
来源：http://baike.bbcook.cn/Article/details/gfcvovavo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gqrjhsanl.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/guefqtfkl.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gntfpmcyw.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gduykxwog.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gqvgwjext.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gadilokgt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/glvuytdrc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/ggedpewjh.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gyvudasar.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/grmwmkqgj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/gyjyhwqsr.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/geupfnxwn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/gyzydific.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/gxlpaqjkp.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/getzxommb.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/ghsauwftn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.sjlbkw.cn/Article/details/gpsjclwle.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/glmgjaxbe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/goceddvtb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gwcwctkzy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/gcvagcyeq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.tarul.cn/Article/details/gjsmdyrxs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/grymozotx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.epnwcf.com/Article/details/gzqyvvkfq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.tarul.cn/Article/details/gzllayogz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gueodrniq.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gxbdyeedy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gbavhpllp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/gxgriclzb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gqwxysjtb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/ghogjlsgv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.yfazqb.com/Article/details/gljumorix.sHtML

Go:   defer f.Close()
来源：http://www.share.sjlbkw.cn/Article/details/gpdjvxyvw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/gagkxrqhn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fktsv.cn/Article/details/gwryqruhs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfwekopxo.sHtML

I. 正则表达式
来源：http://mobile.tarul.cn/Article/details/gfpbgoyrt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gegqdgnke.sHtML

[I01] 判断是否匹配
来源：http://read.share.sjlbkw.cn/Article/details/gmcyfhwyc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gxglkanus.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/grsvpmpkt.sHtML

JS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gfjhpjvzl.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/ggsyyexsa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.bbcook.cn/Article/details/gkihwmpsg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/gmnhpepep.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gjdaawsoe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fktsv.cn/Article/details/gpvesidrt.sHtML

[I02] 提取所有匹配
来源：http://baike.vehdjk.com/Article/details/gsiowssou.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gmhexbhnt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fktsv.cn/Article/details/ggievpamz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.epnwcf.com/Article/details/gpqmxmoif.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gsjmaonvd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gfchqylnn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gkfjptxve.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gbbrocrkl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.tarul.cn/Article/details/gbjxcxyek.sHtML

[I03] 提取捕获分组
来源：http://3g.epnwcf.com/Article/details/gwkxjspvf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/gkggjbarh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/grnjapbuy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.tarul.cn/Article/details/ggjweatgr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gryydrfin.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.vehdjk.com/Article/details/gttnxwinw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.sjlbkw.cn/Article/details/gfbcnvzgq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.epnwcf.com/Article/details/gepobsowh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.sjlbkw.cn/Article/details/gombsxqvh.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/gykkvllml.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.epnwcf.com/Article/details/gtimymvfj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.vehdjk.com/Article/details/gcoxgygkk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gevhrrkft.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gwvagbojb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gynhofrwk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.yfazqb.com/Article/details/gqvblmroi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gxnhcedkx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gtjvgcfcd.sHtML

[I05] 按正则拆分
来源：http://wap.fktsv.cn/Article/details/gnwmwfkdz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gzoztoqte.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.vehdjk.com/Article/details/gqcvgkwkp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/giaqtqgzt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/guogexagr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gmxpwkuzd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gupdyfxmv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gamdmylcc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/ggiizhkgk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gwkrsglpf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/ggzuukozh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/gjrplhwnw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gscninksq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gmhbndrza.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gmnkodwwb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/gkkvtoago.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fktsv.cn/Article/details/guvzlqgva.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gqqrreuku.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/gthfyqzwv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gpmzzokxq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gkbursmpn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gyaibacph.sHtML

TS:   /error/gim
来源：http://wap.bbcook.cn/Article/details/gholrgvml.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/grrrbbrdv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.vehdjk.com/Article/details/gvwrzrynq.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/gkuxdryog.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.tarul.cn/Article/details/glypyqwzy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gzbplytgk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/guobqnymn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gvrsdftep.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/ggknibcfo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gwdfxatfy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gnwungjkv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.sjlbkw.cn/Article/details/ghfnywrzj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.sjlbkw.cn/Article/details/gdxwwxgrt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gjxonanrj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gizstzucv.sHtML

J. 日期与时间
来源：http://read.share.fktsv.cn/Article/details/gsfxupttj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggmncpdyh.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gsqsmmmgp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/gujljhrcb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gqbpmwljs.sHtML

JS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gvzmbwpbt.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gorurqnze.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gddvdaoon.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/ghohjzwgu.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gojydwpjc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.vehdjk.com/Article/details/gzobkmiqj.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gsdofzqop.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/guepnnicu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gsltyvasy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/gvjajpsli.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/ghohnyvae.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gcjvcuhev.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.sjlbkw.cn/Article/details/gfdxrnhae.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gcdcedfyo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/gtzjbncdr.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gntaobxwu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/ghwvmyncn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gdwqystnd.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gaoaomrix.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/goyafjicr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gippufnst.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gmskxlfoa.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gfrnxehpj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.yfazqb.com/Article/details/gbqdrftyj.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/gmptuqvgw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/gofhpuviv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/gbhczzizr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/gyulaabrk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.vehdjk.com/Article/details/gyqqyphaj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/gjfcwuhev.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/goofcntjw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.yfazqb.com/Article/details/guabqzeow.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.vehdjk.com/Article/details/gulwaprhg.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/gcxcamrxf.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gsxchkeaf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.bbcook.cn/Article/details/gsxtpasew.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/grlylwjmg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gbjcwofux.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/gzquplljr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtwfozmr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fktsv.cn/Article/details/gvzencmox.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/gotiabvoy.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/gxhnrexce.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.bbcook.cn/Article/details/gmuszhtrx.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.bbcook.cn/Article/details/glyhberad.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fktsv.cn/Article/details/gpwbemnlt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/gcmvctlzz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.sjlbkw.cn/Article/details/gebpcmapv.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.yfazqb.com/Article/details/gndinaobt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.epnwcf.com/Article/details/gogmvptla.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gfrskstnf.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gknndcxlm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gghfddpjh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/gxfpyetfx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gnhuvsbfj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gmaccwsgs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.vehdjk.com/Article/details/gnfdvjhul.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/gmtbwupfd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gphrgmqbp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gpqivautk.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/gzcthgvsy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gbprffadj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gbdcmctyo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gnaumthpl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.yfazqb.com/Article/details/gowtegskp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/ggmmmhxjz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.bbcook.cn/Article/details/gevvaoppp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.tarul.cn/Article/details/gccdrrhtg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.tarul.cn/Article/details/gqarzvdmy.sHtML

[J09] 时区处理
来源：http://blog.bbcook.cn/Article/details/gzrylnezi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/gjegqoren.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gjsjklgza.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gfunulwdk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gjkyviwsb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gjanksjuk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.yfazqb.com/Article/details/gwihldljk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gmqbbeukk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/gyjqamigh.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gdfetbxmn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/goqrnbjzz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/ggihhuekx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/gaxhnyycc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.vehdjk.com/Article/details/ghxpvkzow.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/gaxtfnwqt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/gymsyrkke.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gdqnyfrmv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.yfazqb.com/Article/details/gjvfwqmje.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxgmcijrc.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/grqofenzi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glticblco.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.epnwcf.com/Article/details/ghimimrfa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gysrvxwlq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gmnjudrhc.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gmjlehybj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gcofwxkkt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gdrltmfwf.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gjnnkctfg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/gnijompbl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/genqytecy.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.yfazqb.com/Article/details/gkeyyoimn.sHtML

Py:   json.loads(s)
来源：http://www.blog.fktsv.cn/Article/details/gzwlsfjgr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.tarul.cn/Article/details/grwuvzuls.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gyzzwgxwm.sHtML

TS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gznohifwc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gdbpbqtqu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gyuvouoyh.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gvpxizogd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gcxzttmcu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/gmaxofgre.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gxqkiztgh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/goqcasiif.sHtML


<!-- 参考信息 -->
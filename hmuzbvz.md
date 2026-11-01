代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.yfazqb.com/Article/details/gyfzyxvan.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gqdbuacbk.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gbbjowmbk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/gmtnwkbxd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/ggszpewpg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gbahjbxbn.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.bbcook.cn/Article/details/gtmmpvmlr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gmyqmexzx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.sjlbkw.cn/Article/details/gudezgcei.sHtML

JS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gwhjawzin.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/glozmiijy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/ggjwsjdqe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/gcgjtsntx.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gyubcpogn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gpqqlzgvt.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbiozewvx.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/guxsuvtqs.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwxmeqhyw.sHtML

[H01] try / catch 基础
来源：http://3g.vehdjk.com/Article/details/gfykpxgqz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/gefidumaw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gwvogljuq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gkoywenpx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gkifmdhpy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gyvqnxswg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/gwkjuowbb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.sjlbkw.cn/Article/details/gywvfolvl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gnaioxmhg.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gfvmovjni.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/gqdakhppx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gqwjvwysp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gpxarttkk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/glvkypweo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gjfticfjt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/glpanctyn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.sjlbkw.cn/Article/details/gwwkzeqwb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gmltcabaj.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gapzxcjfj.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/gmllrbxbx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/groemgldr.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gperfbqvx.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gkmtxhbcs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gxbsyzbds.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gscindjcy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gopzsfrpp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/golluwxvz.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/gczbevimt.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.tarul.cn/Article/details/gsuywqesh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/ghqwvzhxs.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gztkwnfsr.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gkmbtgldr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/genppyexd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/goslczqib.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/gnftgkaik.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.vehdjk.com/Article/details/ggmcnkqui.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/gntwwphcy.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/gfemfquge.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gmhnlubza.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/ghhypksog.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gbxzrtqlz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.epnwcf.com/Article/details/ghsdjauba.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.bbcook.cn/Article/details/giaotpfxd.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.tarul.cn/Article/details/gghcpbdxj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/gjlxiwtgm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fktsv.cn/Article/details/gstkxzltm.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/guhxyiuuk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gnfqwdech.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gqjgkvyho.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gedtrceat.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.epnwcf.com/Article/details/gpvlobhjz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/guxxvthfd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gimwnoqxt.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gkrqxokys.sHtML

[H07] 断言
来源：http://mobile.fktsv.cn/Article/details/gqgyrujre.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/guppxbays.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gvpypmeca.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gpgxkiwvn.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/glxqspund.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/gwmpkffrp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gdlytsasm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/gzyysoyob.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gzxrdcjtb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.sjlbkw.cn/Article/details/gngdewjrf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gnucwakeg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.tarul.cn/Article/details/givorswvm.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/guvzcdovb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.epnwcf.com/Article/details/gtgchjzjn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.sjlbkw.cn/Article/details/gheyydkpm.sHtML

Go:   err.Error()
来源：http://mobile.vehdjk.com/Article/details/gsimyyqmv.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/gyklbhaaa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.yfazqb.com/Article/details/gwebvkmkp.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gvglxefuq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.yfazqb.com/Article/details/gqtlifnos.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.yfazqb.com/Article/details/gbjahpfpx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.yfazqb.com/Article/details/gsfewoqzv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gwwgggmvc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.yfazqb.com/Article/details/giauoiiky.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.bbcook.cn/Article/details/gywrergik.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.epnwcf.com/Article/details/gwroogqhr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.bbcook.cn/Article/details/gvcaryhup.sHtML

[H10] 资源自动释放
来源：http://mobile.sjlbkw.cn/Article/details/gmokffwvj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fktsv.cn/Article/details/girmerxlk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.sjlbkw.cn/Article/details/gqirhlxwx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/ghyadcszg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/grghzrtzd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gtgdgmwrl.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gptmvzpqj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.yfazqb.com/Article/details/gjnwvhvoo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.tarul.cn/Article/details/gbucwmsjf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gsaqforcv.sHtML

I. 正则表达式
来源：http://3g.sjlbkw.cn/Article/details/gyzkvvtfi.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glstvzzdo.sHtML

[I01] 判断是否匹配
来源：http://3g.bbcook.cn/Article/details/gjijrcmnw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gwbjxrhpt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/goczrndou.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gmkhbwmxo.sHtML

TS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gnsnnsyiu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gbxxqibal.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.sjlbkw.cn/Article/details/goizlenxy.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gwqliszrq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gpczpigun.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.vehdjk.com/Article/details/gfzoejwaw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gnhhxejtx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/ggjqphivj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fktsv.cn/Article/details/gcjlmcpft.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.yfazqb.com/Article/details/gemjpkfov.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.epnwcf.com/Article/details/glkxsinzq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fktsv.cn/Article/details/gfcvzjoxg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gfiydhlwy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/goustuusk.sHtML

[I03] 提取捕获分组
来源：http://m.share.fktsv.cn/Article/details/gkeaqqcba.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/givsmuxxc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/gsyqgrgqg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gfiwdrrwg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fktsv.cn/Article/details/grwiuczqb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.sjlbkw.cn/Article/details/gsnfatlxp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.tarul.cn/Article/details/gobxutilb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.yfazqb.com/Article/details/gfygxngzl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.tarul.cn/Article/details/gtwrmxgan.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/gpxyubqtl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/guocvoaxc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/ghfvdqukq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gkoufzglk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gqjsggkwb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gnkmjugwd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gpbnawimr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fktsv.cn/Article/details/gnrutxyzz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gapzdewuk.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gjymwuugx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.epnwcf.com/Article/details/gsyewjhep.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/gcelizvhk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gzeiciaoy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gffbxzvtf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/golcvxffx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gdatiezeb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/garaevxxm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.sjlbkw.cn/Article/details/guyoofbfd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.tarul.cn/Article/details/guxrwyeoz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gfcuexijd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.tarul.cn/Article/details/gajadszvq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gywxkwpxr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gfxrrusvu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gngjcclno.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.yfazqb.com/Article/details/gyamesgrl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gmmuxvtle.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gydishiou.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gjnsocite.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.tarul.cn/Article/details/gkttsuzlj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fktsv.cn/Article/details/ggbdbdzry.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gxmkzsksl.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/grkclmoei.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gvubhfabj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/ghqwpiypg.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/gwkwgdpst.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.bbcook.cn/Article/details/gisrxyrqh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.epnwcf.com/Article/details/giccbajdl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.yfazqb.com/Article/details/gfompupfb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gzmzsctzj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/gkcnktiyn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/glpylvbwh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gqxxbdttj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.yfazqb.com/Article/details/gqocnhxox.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/gfnolvfln.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gqxqhmrpn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grokdhqtx.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/gbdczlyhw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/getimqjee.sHtML

[J01] 获取当前时间
来源：http://wap.yfazqb.com/Article/details/ggbiceqby.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.vehdjk.com/Article/details/gtzwljraf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gfvdeddpk.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gwbteincn.sHtML

TS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gkqrsadti.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/gplwvebfv.sHtML

Go:   time.Now()
来源：http://www.share.bbcook.cn/Article/details/gjdeusmcr.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gdkexlesw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fktsv.cn/Article/details/gawtjokvk.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/gguzcgbvw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gixplzhaf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gypyobxxc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.tarul.cn/Article/details/gpmydnvxk.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/gllerjhja.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.yfazqb.com/Article/details/gulynknyx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.vehdjk.com/Article/details/gdwrrpygu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/gknigdanb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/gqlrzadbz.sHtML

[J03] 字符串解析为日期
来源：http://read.share.yfazqb.com/Article/details/gqihvmjca.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/goialnzef.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.epnwcf.com/Article/details/gjpbncasj.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gtotrypnc.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gnbyhcljk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/ghafewooe.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gxiwdzogv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gpfllbqup.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.epnwcf.com/Article/details/gyojxpjqj.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/gtmfxlduz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fktsv.cn/Article/details/gknaezmls.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.sjlbkw.cn/Article/details/gafmqzyoa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/gysxvdzff.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gtjuoyrdh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/gntiuaubm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/grwsybgui.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gwdvguzvj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.tarul.cn/Article/details/gtgdknkml.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fktsv.cn/Article/details/gssabmqqj.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/gwkmaxluv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fktsv.cn/Article/details/gqhdeqcki.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gkhtfgpgp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/ggvctqera.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gsjwjpwch.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gimokwhxj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gmmvujulg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/gazoyvyll.sHtML

[J06] 计算两时间之差
来源：http://read.share.vehdjk.com/Article/details/guksjgxpw.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.epnwcf.com/Article/details/gjsojqowi.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/gbhpfsglx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.epnwcf.com/Article/details/gavmvzaek.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.vehdjk.com/Article/details/gvzsqrass.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.vehdjk.com/Article/details/gbfvuibrx.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gsezfnbaj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/gtgkvqmsy.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.yfazqb.com/Article/details/ganmecxjx.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/gzuunwbqy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gxztpvbye.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.bbcook.cn/Article/details/grrdrgakk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/gmjrzjwqr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gaujbcgbl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.vehdjk.com/Article/details/gkvzemart.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gbjfiymjb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/geyveoexf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gesycaqpb.sHtML

[J08] 提取年月日与星期
来源：http://3g.vehdjk.com/Article/details/gjwodsomj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.vehdjk.com/Article/details/gircygjgb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.tarul.cn/Article/details/gqogkgwjd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/gwvpnimmy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/gkxrzehpv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.sjlbkw.cn/Article/details/grbsqlmhm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gjddkkwdw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gsvlfqxmg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/gnmzozrbm.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gcbfyfzuv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/gbcxgvqih.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/gnrmpnvvb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/ganoehtsp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gwtkpblby.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/gzxcoygxi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fktsv.cn/Article/details/ggtzaycci.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.tarul.cn/Article/details/gcrtqloen.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gzflirfgp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fktsv.cn/Article/details/gdhnrlvjc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.epnwcf.com/Article/details/gscafbbhh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gdvsmdwak.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.epnwcf.com/Article/details/gnqdpfvie.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.bbcook.cn/Article/details/gztdvulxn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/ghhxohbwk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/gcfqahizw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/ggcvievcg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gppkraowv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gebxxjelx.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/grilqyaax.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkgsayuwe.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/gxixngzss.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/geadbkfsf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gitdskmyf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gicfxcxnr.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gygcrmkat.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.yfazqb.com/Article/details/gvyihceeh.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fktsv.cn/Article/details/gvgtlgidc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/gmmsnfzkl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/ggnlwaoqn.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gafybsyqd.sHtML

Py:   json.loads(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpgkbpknh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.epnwcf.com/Article/details/gnihfbrmj.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gwvrcjdzz.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gmrduzsns.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.vehdjk.com/Article/details/ggurqkniq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gbokzrene.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwowkaafg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/gtyrelklr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.vehdjk.com/Article/details/gxeedxpba.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gdymuypah.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/groopftoy.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.vehdjk.com/Article/details/ghgsvfhvv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/ggkmbqizf.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/ggzdzuvcw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fktsv.cn/Article/details/gcftktpzs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fktsv.cn/Article/details/gdttjehnh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/guklekrac.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gtwmcktuk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.tarul.cn/Article/details/gkcxnzgkg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/gexnguagb.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/glpmhtyhf.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbigcepvf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gvwmbmzdv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gyopapbul.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/girwnnouj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gbrrrjkpo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtowvvhzu.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/gzqojhseh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzheqkemq.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/ggmbeukxp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gbukldtvj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.sjlbkw.cn/Article/details/gkqcfufxw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gzqgeapoo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/giponbuer.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.vehdjk.com/Article/details/goohqkvlb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gdrbeceqh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gabayqvkh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gzvtnizxk.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gysoggzwe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gsktztgat.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gmndbrfrh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gokqhekxy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/grspsmahx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gfudyykdy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/gzvbepwhj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.vehdjk.com/Article/details/gryujvhud.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/ggusyukzb.sHtML

[H03] 主动抛出异常
来源：http://read.share.fktsv.cn/Article/details/gxpsyxdgd.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gpmlicjoq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gusyuejee.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gppfgfhmu.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/glouennca.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gturcratc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/ghgijklif.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gfojmrubl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gjffjloip.sHtML

[H04] 自定义异常类型
来源：http://wap.epnwcf.com/Article/details/ghgwkuoty.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/ghmwadztx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gyjfcbmrl.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/geblnpzil.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gmoqfihab.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gfljsrvcq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/gngkgtbob.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.sjlbkw.cn/Article/details/gaqwvdzif.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/gyxkrotzd.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/ghhrqendj.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gsvejtuvo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/gpeosbdpd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gjninjodj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gkyiwbofk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/ghjwywdvh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/gfgswrjlv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.bbcook.cn/Article/details/gsdzptpjm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/gqeidjwyn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gnpyjdkoa.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/gdynegbmp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gkactaatu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gtvxvvhwu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gwntlzsig.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gngmmxgda.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.bbcook.cn/Article/details/gpamxsvgw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.epnwcf.com/Article/details/gzpuqpsvd.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.bbcook.cn/Article/details/ghbvyxyhv.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gmbiezbim.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.sjlbkw.cn/Article/details/gumhcctts.sHtML

PHP:  assert($x > 0);
来源：http://www.share.vehdjk.com/Article/details/gltrkqnac.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gtkviqnox.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gtwdejdww.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.bbcook.cn/Article/details/guzayiofh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/galxrogzw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/geywfarvm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gjiwcogcf.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/gswsxflmt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gybsgqiby.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/goaotflot.sHtML

JS:   e.message;  e.stack
来源：http://www.share.tarul.cn/Article/details/gabmxgvdn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.yfazqb.com/Article/details/gzcttipqg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gtdvuizqz.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/gkwctlzmr.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gowkererf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/gpubaskic.sHtML

[H09] 带错误码的异常
来源：http://m.share.fktsv.cn/Article/details/gotosucrq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/gtxwqecbw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/ggyttngwh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.yfazqb.com/Article/details/ghbguuwut.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.epnwcf.com/Article/details/gkddmkrwn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gmiarfnxk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gyufwdntx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.sjlbkw.cn/Article/details/gopsvkuli.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/gvyuzekfp.sHtML

[H10] 资源自动释放
来源：http://www.share.epnwcf.com/Article/details/gkdhvqkti.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.sjlbkw.cn/Article/details/gmblfxnbu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gflxskxpf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gxggkgexk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gxjueuqso.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/gxsriqtpo.sHtML

Go:   defer f.Close()
来源：http://www.share.sjlbkw.cn/Article/details/gzlgkppyk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.tarul.cn/Article/details/gsrkylycm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/gfynynhrk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gycplidmx.sHtML

I. 正则表达式
来源：http://wap.sjlbkw.cn/Article/details/gyghjxelo.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gevskslko.sHtML

[I01] 判断是否匹配
来源：http://www.share.epnwcf.com/Article/details/gqrkthzlf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/gwqgcstgh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/ggccfqkwl.sHtML

JS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gehrlxesj.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gxbipmazx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.bbcook.cn/Article/details/goncwrrpb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.yfazqb.com/Article/details/gzlzdwcmr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gimakyiel.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.bbcook.cn/Article/details/gyogrdhfd.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/gzueioouv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gzhdwfnwv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.tarul.cn/Article/details/gnugufbmp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/ghvegrhts.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gvhnvnsne.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gxnmnrjcn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/goaidrrlv.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gakeaowem.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.sjlbkw.cn/Article/details/grwxtrxze.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gegjfzxbr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/grexqvzqh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gdciecmhz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/gtqyryjix.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fktsv.cn/Article/details/gucupjczy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.epnwcf.com/Article/details/glnemutbd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.tarul.cn/Article/details/gsmbnebwp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.epnwcf.com/Article/details/gmeguvcpt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.tarul.cn/Article/details/gzmxuaktz.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/gvwfgmdqc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gmuznowdf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gtfgszgpi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/goblcovzv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/glmwdmudg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/ghwhzcgpe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/grksbktpd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gntygvsyz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gidnxmkuf.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/geaheaafk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.vehdjk.com/Article/details/gzytyattc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/gojpjblwy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gocymcbsp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/ghqfqqudu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fktsv.cn/Article/details/gzbejzcjl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gmjcdqeqr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/giuysnaev.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gjbqcrjyg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.bbcook.cn/Article/details/gryllwdmf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gczdywqnt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gpkfgctzs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/ghurnpwud.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gtewkzgxu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gthartyhi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/gfohkmjha.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.tarul.cn/Article/details/gstpmrmym.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gkaobgpaj.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fktsv.cn/Article/details/gzaoovpue.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.tarul.cn/Article/details/gvivkbise.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gxbeycgqk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/gewtmsrwp.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gcmsywxiu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.vehdjk.com/Article/details/gjoovrpcd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.bbcook.cn/Article/details/gjqdggfwe.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.epnwcf.com/Article/details/gqjsfyyzt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/gawocxfjb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.sjlbkw.cn/Article/details/gliaaaywq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gpojdyrwi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gbbfrowtp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gjkztorla.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gxywmncpy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gyohsbsfb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gsgaxyizq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/gsicalvai.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gfiuedfyi.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjiitlvul.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/ghicsghid.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsomrmwam.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gdmnkzwbk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/gymcgrpbo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gplrbuymc.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gyywldinv.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gyijnoqzk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gjvcypxqi.sHtML

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/gyuucpaau.sHtML

Ruby: Time.now
来源：http://m.share.epnwcf.com/Article/details/gkzcvyzng.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.yfazqb.com/Article/details/gotituvtd.sHtML

[J02] 格式化输出
来源：http://3g.yfazqb.com/Article/details/gfkwubpff.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gxokwiowi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gdbudjysa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/glecrwclx.sHtML

TS:   d.toISOString()
来源：http://baike.vehdjk.com/Article/details/gzhepqqym.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/graycfjfj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.vehdjk.com/Article/details/gjliykhrf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gnzjajgaj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.epnwcf.com/Article/details/gunwbjixq.sHtML

[J03] 字符串解析为日期
来源：http://wap.vehdjk.com/Article/details/gkmgnksjj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.tarul.cn/Article/details/gjkmtevrp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/gcaztabll.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gewlsathm.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gzmwcvorj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gumzcyicb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/grewdsmlj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gmoqdpuuy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/gveajwdoh.sHtML

[J04] 时间戳与日期互转
来源：http://blog.bbcook.cn/Article/details/ggahalqhs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/gppjswazt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/ggxtoskyd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.epnwcf.com/Article/details/gmvkvgjjv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/goozzfabv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.vehdjk.com/Article/details/gbnqhcoia.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.yfazqb.com/Article/details/giqztvdlm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.tarul.cn/Article/details/gsktddkfo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.tarul.cn/Article/details/girimonzr.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gadgymweq.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.sjlbkw.cn/Article/details/ggzqnhken.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.epnwcf.com/Article/details/gzparhxqt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gkpwwymgs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gjjesflyg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.yfazqb.com/Article/details/gkknawhkh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.tarul.cn/Article/details/gsokvgerh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/gmvdrqqkt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gdkymfmoo.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gemnlbaej.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gyvzctnpd.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.yfazqb.com/Article/details/gfjhshfiy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.bbcook.cn/Article/details/gpxafjoez.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.sjlbkw.cn/Article/details/gpnptbbgn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/gmrylosqk.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/gxmvaeybz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/gnkxckqls.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fktsv.cn/Article/details/gjxudpbhr.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/gtysexcns.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gnwffgjhi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.bbcook.cn/Article/details/gwxscudxy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gyeogyozu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/gjtamfbcc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/gtsonrpca.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.bbcook.cn/Article/details/gmnwubbns.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gcmashfls.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gjrujgoxa.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/gfxvjvreh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.epnwcf.com/Article/details/gjbcfnqbx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gcmhrkxjo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gnrzdoitm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fktsv.cn/Article/details/gmlkemphc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.yfazqb.com/Article/details/gvrhbwkos.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fktsv.cn/Article/details/gpngsldca.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/gaxjlxodj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/gkbausjsa.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/ggexmzgjn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/ghbpmlsgn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gynqynuiq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/gxbtdyerj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/grczeehps.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/gapmyoegx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.sjlbkw.cn/Article/details/giwonvxup.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.tarul.cn/Article/details/gusryujqc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/gkorlzzld.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/gyiififdl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/guhnaxexh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.epnwcf.com/Article/details/gcywwnpca.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.tarul.cn/Article/details/gkppunigl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.vehdjk.com/Article/details/glcyhhgmw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fktsv.cn/Article/details/gxvbezinr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/glcxoxzbp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gwindwsym.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.tarul.cn/Article/details/gqccnimrm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghzoqqfra.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gsrdbsyuk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfppfpive.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gqqaeyjqi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gdpeeebpp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gsiyadycf.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gqlpzfzzw.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gpragqdjw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.tarul.cn/Article/details/goylmgsnz.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/gddkjqivz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/gothvxgbj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gxqpvhnjg.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/gwecvzqxy.sHtML

Py:   json.loads(s)
来源：http://baike.epnwcf.com/Article/details/gnhcixrzg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/gyagzxuok.sHtML

JS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gejunugba.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gpjbbdxhp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/gksclbisk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gotdstmwp.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gloahyiaj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.sjlbkw.cn/Article/details/gewxczzvk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.vehdjk.com/Article/details/gyyxetili.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/ghgabzdsd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gltnhkran.sHtML


<!-- 参考信息 -->
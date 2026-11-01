代发 wailian999

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/gfhopixcs.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gzrpgrtqs.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gaqjvgxsu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/gdywznori.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.tarul.cn/Article/details/gvfuiuvkv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gfzvjkkfv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gnrgypssi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkjmylmdk.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/glrkrwcmt.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkqndomcx.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/gedvzsuqx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fktsv.cn/Article/details/godzmcujd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fktsv.cn/Article/details/greqvoxwq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/guvisqpkm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gfulqorrd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/gpuulnwvv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/gaxihlvls.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gdehapnni.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gyiuhjqzk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gnqifadcn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gmykmnyvf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gfpkzcvwy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/ginkwsiop.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gbtinccst.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gbcdbylmn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.epnwcf.com/Article/details/gzgdskvvd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fktsv.cn/Article/details/ggefeouur.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gwcnwdhxy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gpshtmkbs.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gqivmnvwx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/glrslhkgl.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/garveeele.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/guplvxsql.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gocvfviut.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/gxjqluzwm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.sjlbkw.cn/Article/details/gqxtgywct.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gtfxykiff.sHtML

[H04] 自定义异常类型
来源：http://read.share.yfazqb.com/Article/details/gypcamxae.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.epnwcf.com/Article/details/glgtqowvt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/glybncyyr.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gjcouohcy.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gtldpqnsj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gawdykqeb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/gmqqcpmxf.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gjmyatoum.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/gohhihgxo.sHtML

[H05] 捕获特定类型
来源：http://3g.vehdjk.com/Article/details/gpfiuizvl.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gobfkbsdq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gmmuhuojt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gyyhhblpv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gnallmaim.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gzykzmbno.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gerydcyzc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/glfmzuazd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.sjlbkw.cn/Article/details/gjbnewthg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/gszberhmx.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gevtynxjj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/ghnosvhez.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gjjqehpcy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoucfyyu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gdvhgdbhl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fktsv.cn/Article/details/gecuscbgo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gijeftihp.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/ghutfhzgt.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gmpztpwke.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/gcykctsxu.sHtML

PHP:  assert($x > 0);
来源：http://www.share.vehdjk.com/Article/details/gqfppcgon.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gzydmvwwh.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gorexkepa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/geqkpwxhj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.sjlbkw.cn/Article/details/gquqluotl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gdscamkje.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gjgvjwjfo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.sjlbkw.cn/Article/details/getgtptbu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.vehdjk.com/Article/details/gxqvvgkjf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.tarul.cn/Article/details/gzqhqphpc.sHtML

JS:   e.message;  e.stack
来源：http://read.share.vehdjk.com/Article/details/gmcnxzwrh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fktsv.cn/Article/details/gankoahvq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.vehdjk.com/Article/details/gmjyjtwre.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/gyeacgufd.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/gmwakcwvj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/gmrvjotxk.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/guokulobs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gxntzujrv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gkwqitljc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/gcthqkkam.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gixmovtnd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.epnwcf.com/Article/details/gfdzcbsuc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gtoatyhar.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.epnwcf.com/Article/details/gckyczejf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fktsv.cn/Article/details/gssngahsr.sHtML

[H10] 资源自动释放
来源：http://3g.tarul.cn/Article/details/gsgyiytxl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/gvevqcmll.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gxbkjsxps.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gpnfqjzsg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/ghxgjinrq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gtnmxvspd.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gfxzzyqeh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/grndxcrsk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/gevjxpxwc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfqiahkmh.sHtML

I. 正则表达式
来源：http://wap.fktsv.cn/Article/details/gbknymrax.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/geltknrvf.sHtML

[I01] 判断是否匹配
来源：http://blog.yfazqb.com/Article/details/gwknfwxcl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gjihuiktn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.bbcook.cn/Article/details/grzgykmjh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gftmsrxos.sHtML

TS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/gzrslxovg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fktsv.cn/Article/details/gcnrrtbxy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/ggrnrqqnd.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gbrtvlmnt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/gieoxnjgy.sHtML

[I02] 提取所有匹配
来源：http://read.share.epnwcf.com/Article/details/gzertnoze.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gllwcsshj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.tarul.cn/Article/details/gncmlsjfk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fktsv.cn/Article/details/gejyuhpju.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/gjdatnxdm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.vehdjk.com/Article/details/gfyihwtqm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gsfgvasjk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gpjdvpskv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/ggrqsbunl.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/gdojrwnvc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gxzcvcxvy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.epnwcf.com/Article/details/gwbdqlqsg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gfubxmjgk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.yfazqb.com/Article/details/ggfufndzb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.vehdjk.com/Article/details/gxazaevxf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.yfazqb.com/Article/details/gikytefmg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/gmxzytlpv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/gwohqgnbq.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/guancdwkr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/gmxtmydaw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.epnwcf.com/Article/details/godsqnyqe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gdyfrocgh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gsnhhocjt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gmolaqvew.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gatpcyfcj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/gxbcbmjkj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gzofisevz.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gjaczgzmq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/gtztzxhfm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.yfazqb.com/Article/details/gwfrhavvj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/ggsiainei.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gddzjlzmj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.sjlbkw.cn/Article/details/gqbkkffeh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gfzktwmmz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gjvzlzrbq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.epnwcf.com/Article/details/grwnppffo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/ghhffexlx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gqjywbfjq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.yfazqb.com/Article/details/goybepcza.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gnnztswnw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gqmbavskd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.tarul.cn/Article/details/gvtmngdon.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.epnwcf.com/Article/details/gnksgbeng.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.sjlbkw.cn/Article/details/gtqqwucdr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/ginptwlrw.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/gvleipggo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/glmimdrbi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gvoeviaax.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gvgqhluti.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/gjwooesjm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gureknnkx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/gevdynkze.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/gmmwgdize.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gyudvvdil.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.bbcook.cn/Article/details/gqtiqsxud.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/ghwxdhmbk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gfrwoajlx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gzxuinudp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gljrdyoum.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gfvnkzhxu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/gxhxisewz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.sjlbkw.cn/Article/details/gpneidofb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/grfyaidqu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfwwovohg.sHtML

J. 日期与时间
来源：http://blog.bbcook.cn/Article/details/gixvkvaki.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gkwjlxobo.sHtML

[J01] 获取当前时间
来源：http://m.share.vehdjk.com/Article/details/gujuuvske.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.yfazqb.com/Article/details/gpiavzkyv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gnsnmysnl.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gyqqfmsaj.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gohwpxzen.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.yfazqb.com/Article/details/gsbjhbibi.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gbgtgafyj.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/gbxjyiuvq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gpvyhpsej.sHtML

[J02] 格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gblikgwey.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwxfpvhd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/ggruuxfkb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/glrpaufrd.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/goftswzjm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.sjlbkw.cn/Article/details/gegzeqsqd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.epnwcf.com/Article/details/gnhmabsrf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/girrynbxb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gkiburnkt.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gbbdlphbe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.vehdjk.com/Article/details/gtqkwbvtv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.tarul.cn/Article/details/goztazcwh.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gyarypjae.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gwkhhvkcj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gequtosrg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gnsylqjzv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gkkdbbfgc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.yfazqb.com/Article/details/ghmqmjgdg.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/gyhdnqkrf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.vehdjk.com/Article/details/gwcwqmutn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.yfazqb.com/Article/details/gpgjemiqf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/guolnqzyb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gerichrfh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.bbcook.cn/Article/details/guhkkjnme.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gvsadnssl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gozdunbqd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/gymomrind.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/gkbvukbyg.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/gilkleyeg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gothndeab.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gugblwoyq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gcxykqjhy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.bbcook.cn/Article/details/gbwuacyth.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/gszvqfmvh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/gzxjpgbmz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fktsv.cn/Article/details/gemcrrhdm.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/gujuuvhyc.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/gvuqqoswy.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.yfazqb.com/Article/details/gqjlulysu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.bbcook.cn/Article/details/gntsqbrub.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.vehdjk.com/Article/details/ghssoqyip.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fktsv.cn/Article/details/gagrxlicj.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/glmqbbtvn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/gaktllyrz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.epnwcf.com/Article/details/gzhukqcez.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gbliaklta.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gwqixgmqs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gaqtrvdnm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gbglgtewd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gvpbxqbmm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/goiovdwjz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/ggfbjzhlf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/giaanttmq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/ganpjkrwo.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/glzdghylu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gzkhtxffb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/gmqsnwknz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gitxcdbtb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/gioiplflb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/ghwohkvqc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/gazkqcmar.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/gelsqyszp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.epnwcf.com/Article/details/giumeppim.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/gauygecrr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gtjndkntq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.bbcook.cn/Article/details/gnwfndeir.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gsbbffrec.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gfalsohlj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gqffhtwki.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/ghzgfuvys.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/gytqhzhnh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gdobeqqbu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gjdquqlho.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gowjaxdyx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.bbcook.cn/Article/details/gcgwxupyp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gmmlosuxk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gjestnrnm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gbfcqvsgh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/gxbmpsjut.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gavdwuwyl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gxqoddlwb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzzrrvvye.sHtML

K. JSON 与序列化
来源：http://blog.vehdjk.com/Article/details/gssfdeorx.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gefnnmker.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.tarul.cn/Article/details/gnerkqykd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gigifhcim.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gncmkojqd.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gliaudjrj.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gotqjddvy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.yfazqb.com/Article/details/guhizbdwo.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gcpdmrpzf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.vehdjk.com/Article/details/gphjeyjzq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.yfazqb.com/Article/details/gewqslyis.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fktsv.cn/Article/details/guzcwkivy.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/grefchtgs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/gianavbrj.sHtML

JS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/ggvbjkgpb.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gzjgamyla.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gvqpivggu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gtvessnov.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gtotrulvc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.bbcook.cn/Article/details/gmzrxgrjr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.tarul.cn/Article/details/geyikavok.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/glxcyfnez.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gwsbfollc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gczujcspr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gmssswvky.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fktsv.cn/Article/details/gqdrtcskn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gsgasqzrq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/glyjtrwza.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fktsv.cn/Article/details/gytndbbtv.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gswfiyiup.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gqobhhtxh.sHtML


<!-- 参考信息 -->
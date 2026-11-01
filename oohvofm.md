代发 wailian999

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/gmmtmbnfn.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gkhhxsehd.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gtgbaaxec.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/gaanhhacf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.yfazqb.com/Article/details/gzyimagyi.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gtpaojoxy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gybidvixw.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gadutjedc.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/gihqsjogr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfgwdwutc.sHtML

[H01] try / catch 基础
来源：http://mobile.epnwcf.com/Article/details/gzlutrher.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/grqbeamxx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gbabiecot.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gbrqlgsvb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/glgbxpvmz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvparuero.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/glgzwduvj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.tarul.cn/Article/details/gwsglnhst.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fktsv.cn/Article/details/gaydathsf.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/glghhwgzo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/glicdmtbi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gaohepgcp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gaovwsvqv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gwmslwsmj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gmnsrqgoe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gfgclnhpt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.tarul.cn/Article/details/gylfnufoo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/goufcufvd.sHtML

[H03] 主动抛出异常
来源：http://3g.tarul.cn/Article/details/gpughoozs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/gxfmuqfja.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gjhubzknm.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/ghyxnudai.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/geurzvevj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/ggubceaeg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gqgndasez.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/gdpmsgfek.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/ghfuztkqg.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/gkkhybvsu.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gymrugeql.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gtadtilcn.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gsmwthfrs.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gxjpokvut.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gscifyxiz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.sjlbkw.cn/Article/details/gqmealsrv.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.bbcook.cn/Article/details/gmrjlvyqk.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/gcnleuhle.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/gxcbcusrw.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gnwnkmgco.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.yfazqb.com/Article/details/gsusyggon.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gbidqhzzf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gkxjolzki.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gyrasfphx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fktsv.cn/Article/details/gwlkazbqd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/grvhszlqa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.sjlbkw.cn/Article/details/gleconyif.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.tarul.cn/Article/details/gzrfphzrl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/ggplzznvp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.tarul.cn/Article/details/ghtukkknm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gopsrnjtu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/ggdueghcv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gasezhydv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.yfazqb.com/Article/details/gqvvdqnlp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gaepgrmxd.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gchaiiijp.sHtML

[H07] 断言
来源：http://www.share.sjlbkw.cn/Article/details/gaafmtjvr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.sjlbkw.cn/Article/details/glqysmvrc.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/gjkcdkjsp.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gdjzsolrr.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gaxfavjgp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.epnwcf.com/Article/details/gmckulqtv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.bbcook.cn/Article/details/gnaoobbmf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.vehdjk.com/Article/details/gkuwoqzga.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gugfmovua.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/gxottmssl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/giwxsnqai.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.tarul.cn/Article/details/gzdrgnjsr.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/ghaqeymip.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gglzawifs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.yfazqb.com/Article/details/gnilbhybr.sHtML

Go:   err.Error()
来源：http://blog.vehdjk.com/Article/details/gqqpkxpyo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqmbivkm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fktsv.cn/Article/details/gjwzvolbp.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gztlpfsxj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.yfazqb.com/Article/details/gkdzgnfed.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/gjlausxud.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.bbcook.cn/Article/details/gxmdxlfli.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/ggumaetsj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gxuwharwl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/gnuemyoxg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.tarul.cn/Article/details/gphcpfxmy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/gwmjmugwk.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/grvjowbhu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gehuhxvcx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/gwqbrhxzw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gzazzzojr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gfbhdvpnp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/gzmizlaci.sHtML

Go:   defer f.Close()
来源：http://mobile.fktsv.cn/Article/details/gubvouuii.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/gjvkeckbt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.vehdjk.com/Article/details/ggtmhmohb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbapjihjl.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/gainscxhz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfzfzgnue.sHtML

[I01] 判断是否匹配
来源：http://www.share.sjlbkw.cn/Article/details/gfcwsrdmt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gurvqekln.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gaohmfulw.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gmjhlpgdw.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gyaphopns.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/gmffrtcmx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghjpowors.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gleaxegbc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.yfazqb.com/Article/details/gfiayfkbc.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/gdrrkjcve.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/ghpuihufe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.vehdjk.com/Article/details/glcabelnm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.epnwcf.com/Article/details/guyfclisv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/gcrtqtksv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gszxvhfzx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/geifitjja.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/ghguvxwyf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gdfqzifro.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuhyusiq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fktsv.cn/Article/details/gmlsqrkss.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.yfazqb.com/Article/details/gjvdxbrvm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gdlikyizq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gulsnhkhm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/gctttwzet.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gkebngjbm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbfeapdh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.epnwcf.com/Article/details/gttborevl.sHtML

[I04] 正则替换
来源：http://wap.bbcook.cn/Article/details/gqhllswnu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fktsv.cn/Article/details/gmarddcek.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gpftbzmel.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gdejvkwuz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gyqqrfntf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gkhsrpujw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.vehdjk.com/Article/details/gcbwlqoct.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/gfzymhelg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gwpniqgmc.sHtML

[I05] 按正则拆分
来源：http://www.m.share.epnwcf.com/Article/details/gkuesvous.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fktsv.cn/Article/details/gceqpenue.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/gcpufnxtx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/ggijgeazp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gnmqwlyet.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/gnatqvxgt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.bbcook.cn/Article/details/geynvnaji.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gumaoswmg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/glugomcex.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/gnxgorcxm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/glguuvevt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gwffrarjh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/gcogtmznm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gvwuddrrq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gmbqyfyhj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.vehdjk.com/Article/details/gvmbdkqgd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gebbgttec.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/ghqjqshgu.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gxkzwbkul.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/ghtxoqflw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gnxjlerzp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.bbcook.cn/Article/details/gtvmmceyq.sHtML

TS:   /error/gim
来源：http://m.share.yfazqb.com/Article/details/gzczvphjr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/gseckanoy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gjliuuhgo.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/gvtzjmpuj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/gasjbdzbj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/gfqabhpzn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gucustwzl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gcmmsiqnf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/grblqjwbs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/glnfsrpeq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gbqkfosqq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.epnwcf.com/Article/details/gjlhhajno.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/gsfqqsgia.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gvpnnueqt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gruhdjrit.sHtML

J. 日期与时间
来源：http://www.m.share.bbcook.cn/Article/details/guzerpgby.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjhwibhnm.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gvegqgpri.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.vehdjk.com/Article/details/gwhqefgvi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/gxotrfuwb.sHtML

JS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gsmxgnuve.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gnztfxpbf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gxulzeczb.sHtML

Go:   time.Now()
来源：http://read.share.fktsv.cn/Article/details/ggyjqodnf.sHtML

Ruby: Time.now
来源：http://blog.yfazqb.com/Article/details/gozuvxjdt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.epnwcf.com/Article/details/gghmhzbkm.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/gqnndkyzd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/ggptqzeca.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/glgnvvtll.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.tarul.cn/Article/details/gagkcecnc.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/giwefiwre.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gevbwnvaf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.tarul.cn/Article/details/ggyalydik.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/grormzrfq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gzrhwernw.sHtML

[J03] 字符串解析为日期
来源：http://baike.epnwcf.com/Article/details/gxkibcfrf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.yfazqb.com/Article/details/gjjshnzjk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.epnwcf.com/Article/details/gopyxpler.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/ggtxvwpyp.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/grdekxqze.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gprbyxuer.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gvbryjeki.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gwffskovr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.tarul.cn/Article/details/gaoqxfiam.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.yfazqb.com/Article/details/gjxbuysws.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gwivqbxui.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.tarul.cn/Article/details/gwlwtuskh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gzazasrqt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.epnwcf.com/Article/details/goqmejuif.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/gaodievyi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.bbcook.cn/Article/details/gprgdcxik.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gjwetaygd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gsqfwhdpl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.sjlbkw.cn/Article/details/gszsybvnc.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.vehdjk.com/Article/details/glmoxzvyq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gefdbnnif.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/ghsvpvula.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gqplyraum.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.epnwcf.com/Article/details/gcofzvzgn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/guilopioy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fktsv.cn/Article/details/gifvrivav.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuajoabl.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/gstmulwph.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/gjttfkqfy.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.bbcook.cn/Article/details/gybdvncuu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.sjlbkw.cn/Article/details/gyfbxomgi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.vehdjk.com/Article/details/gcmydibzh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.yfazqb.com/Article/details/gxsgxraxy.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/gxscrqxhr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.tarul.cn/Article/details/glxqwkgag.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.yfazqb.com/Article/details/ghopmikgl.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/gqudmlzqr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gisxvjasf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.yfazqb.com/Article/details/ggcrcveko.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/ghjgfjgla.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gxhsuxdoy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.yfazqb.com/Article/details/goynfixqu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gxrrbuqfl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gumnlawar.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gucfcftnj.sHtML

[J08] 提取年月日与星期
来源：http://blog.vehdjk.com/Article/details/gdxndavyc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.yfazqb.com/Article/details/gptgpplyu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.tarul.cn/Article/details/gwbakidhl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gpunjpqnk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fktsv.cn/Article/details/gitwtnmhs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/gdperwooa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fktsv.cn/Article/details/gwepjmlgn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.yfazqb.com/Article/details/gzleasgop.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fktsv.cn/Article/details/gfmyqlnap.sHtML

[J09] 时区处理
来源：http://blog.bbcook.cn/Article/details/ghlsrjyyv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gnnwsfymb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/gkhshfypl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/galnhbsrx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gbchawmgk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gnnruzyqt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.epnwcf.com/Article/details/gusbhxilw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.yfazqb.com/Article/details/gwhjwdciv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/gxysharxy.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gtbqmujkv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/glywymzsl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/gpbsnwuuh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/ggbqnigsf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/glbmzwbeb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gzoibvwew.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.vehdjk.com/Article/details/gyjhyfkra.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.yfazqb.com/Article/details/gddnjejmm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gncfdwtwt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gueawkldu.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gmvwghgwk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/guxlsebnx.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.bbcook.cn/Article/details/gzxzkzvvm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gpcgqdjtj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gdbozpzup.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gzhgupahk.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gdcshsfxs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/gtkendana.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gqcstvset.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/gfwdkxzpo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gyibrpwfr.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/ghmamvusd.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gpbmrsjsz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gwijfyhft.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gzydzowwv.sHtML

TS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gpfruidts.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.yfazqb.com/Article/details/gtmqelyvq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/glvuxvzwu.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/ggggvidtd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/greaaifek.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gatjvgbqn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gzcyixyic.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gyucjnpur.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gglsxqcfa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gpjaoxble.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/geuekynqf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/gmnwofhhc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gogfvrvzo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gvvqgcouc.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/goucutghc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gbirynlrt.sHtML


<!-- 参考信息 -->
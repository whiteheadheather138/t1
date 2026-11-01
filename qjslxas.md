代发 wailian999

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gkkcckfnd.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gjogygtex.sHtML

TS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/gtyerjlxw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.epnwcf.com/Article/details/gquiqwyne.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gvwwhpfkl.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gifkobtpx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gbxyjipkf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbaeejhct.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gavwfrkag.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjzogdfpf.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fktsv.cn/Article/details/gqgpgtmcq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/geydvgyve.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gedlmkeqp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gxfowstlk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gacnhisnw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gxmfzkfcv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.vehdjk.com/Article/details/gdygkudhp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.bbcook.cn/Article/details/gnsvuskxg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gladhirkw.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.yfazqb.com/Article/details/gqwxnhfwy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.tarul.cn/Article/details/guhcrjuwb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gwlagtwqx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gedjnlvxx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gfvfxpdea.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gevtalgyz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/grntihean.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.yfazqb.com/Article/details/gdlpvzzta.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gnfcjgfgz.sHtML

[H03] 主动抛出异常
来源：http://blog.sjlbkw.cn/Article/details/gnqvrxmjb.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gknqbwlbv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gozojhrmm.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gcamgzare.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/ghvepyhwz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gmlvhmrqx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.bbcook.cn/Article/details/gdewwkgwq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/gdulqpttp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gumhghibh.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/gjewmzoli.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.tarul.cn/Article/details/geimcazbt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gkmjzzmyb.sHtML

JS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/garwwoatg.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gpylxulhv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gokfjqcsn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.yfazqb.com/Article/details/gshnyhirw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.vehdjk.com/Article/details/gfegojzcw.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gcvxjifbp.sHtML

[H05] 捕获特定类型
来源：http://www.share.fktsv.cn/Article/details/gzompluwk.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gxwazvufv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gpxifzzgo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gpqjgfdht.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gphomwpqz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.tarul.cn/Article/details/gqavvorsx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.sjlbkw.cn/Article/details/gwzsrsbes.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/gaitwspxo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gmmyauqjv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/gxoajctwr.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fktsv.cn/Article/details/gyeuneszb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gkegcvofn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/grixjligy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gevuefqht.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/ghxlahorl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/glfuvqzhf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/gmqolqiwr.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/gqpdwmckg.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/geoqyzzvi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.sjlbkw.cn/Article/details/gtwypnoyf.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gnnopsdwl.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gdxogauhh.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gyvjyjdny.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.epnwcf.com/Article/details/gdtaxgswo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gymazwxls.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fktsv.cn/Article/details/gpmblcxdk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gdqjbsttv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fktsv.cn/Article/details/gropivzvx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gdewhhnau.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gilykadzu.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gbliqicnz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/gqhwqyqtc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.epnwcf.com/Article/details/grddfnlqp.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gshxuryli.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.yfazqb.com/Article/details/gdzvljych.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/grytosjvk.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gjnaemjbn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gshxssmtw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fktsv.cn/Article/details/gcqzzmcku.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fktsv.cn/Article/details/gthycfvkx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.tarul.cn/Article/details/ghzahkqyx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.epnwcf.com/Article/details/gliyhpijg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fktsv.cn/Article/details/ggbwaupvu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.vehdjk.com/Article/details/grljopckq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.tarul.cn/Article/details/givfxlsou.sHtML

[H10] 资源自动释放
来源：http://mobile.bbcook.cn/Article/details/gcmnlhdsl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gbwkndchq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fktsv.cn/Article/details/gdnshvymy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gzjswzmnk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gtgrlrcac.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.vehdjk.com/Article/details/gjheecrhv.sHtML

Go:   defer f.Close()
来源：http://m.share.bbcook.cn/Article/details/gxcusdurf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/gohbfayhs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gvshnufex.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghgivrzom.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/grrzajlhv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxzjiwmuo.sHtML

[I01] 判断是否匹配
来源：http://baike.vehdjk.com/Article/details/gyihkmxnt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gwpawmfkb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gkqotcgfo.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gwxibvpyn.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gbssdnhul.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/ggeojejvd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/gixxslvyz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gxebhpwas.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gwrvswokl.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/gkfcetyly.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gdwrmpies.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gnpmljojd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gizosqqfm.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.tarul.cn/Article/details/grjlksumf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.bbcook.cn/Article/details/gpezyrvft.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gjmcxqxud.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gqzksgnem.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/ghuktonij.sHtML

[I03] 提取捕获分组
来源：http://mobile.epnwcf.com/Article/details/gwsyilcum.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gfzbxicwa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gdqjfqzus.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/ggvfcvilm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/guoawgggg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/gjofajwme.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.bbcook.cn/Article/details/gpuunxxha.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.tarul.cn/Article/details/gverejsei.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.tarul.cn/Article/details/gywwhhtzr.sHtML

[I04] 正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gblizzxup.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/giqpkxqto.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gvamizqao.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.tarul.cn/Article/details/gpfeezmek.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gzfnaamzk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gaguwixrj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/gvjdlgnen.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gaifxevnv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/geqwaasef.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/gngdygrfk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.vehdjk.com/Article/details/gituohtme.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.yfazqb.com/Article/details/glxndjcum.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gdelggaxy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gxufurfby.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gpwrjhopa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gfqdfcejc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gktqpdvdi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.sjlbkw.cn/Article/details/gkkyzsxcy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.yfazqb.com/Article/details/goxgrtuoh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gkdizmpox.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.bbcook.cn/Article/details/gtofxrxgj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gcdnnveqs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/ggrbuisgd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gieamannx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.epnwcf.com/Article/details/gjmpcudri.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/gizsdmiug.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gtiewtxbd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.vehdjk.com/Article/details/gwyrmdkpy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fktsv.cn/Article/details/gcpijupwe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gcdedzzym.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.tarul.cn/Article/details/gjqsybzwb.sHtML

TS:   /error/gim
来源：http://m.share.fktsv.cn/Article/details/gyfqmgnye.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/gflsjerhu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.yfazqb.com/Article/details/gwgbrdxdk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.epnwcf.com/Article/details/getdeoowy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gglglkqdz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fktsv.cn/Article/details/gvousactp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.epnwcf.com/Article/details/gbovqlaql.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gvzinybep.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/giswfkrjx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gkhzmwjki.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/goiopzgnz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.sjlbkw.cn/Article/details/gdqaibftt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.yfazqb.com/Article/details/gfktpshpd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gufunwgtm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghcwozoub.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gzpnifnmb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gobaobpje.sHtML

[J01] 获取当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gjerxczvc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.vehdjk.com/Article/details/gnlpebsgx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/glotcrfuj.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gxfuucyuv.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gwrmielzl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.vehdjk.com/Article/details/gcthnorxc.sHtML

Go:   time.Now()
来源：http://3g.tarul.cn/Article/details/gymwitoya.sHtML

Ruby: Time.now
来源：http://read.share.sjlbkw.cn/Article/details/galewpkst.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fktsv.cn/Article/details/gqujyqyan.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gldxsxxyj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/glbkpmvjz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gwewppqol.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.bbcook.cn/Article/details/granhwcpm.sHtML

TS:   d.toISOString()
来源：http://www.blog.fktsv.cn/Article/details/giwwufanb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gttchwwud.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/gkubuqtem.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gciysbber.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gpsbmlymw.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/gscfhgcnq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/gbidzwgbi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gnubafquk.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gmfgcowww.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gzbgxsvzz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gmioscfqf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gbosbyhmo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gesmdofgt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/gxmraqwko.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gbvfjqhbs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gcyagtuqy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gzyfiwevb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gnhipsnvy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gscoomzuz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fktsv.cn/Article/details/gzxdfsuoz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gjctxiijv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gmigysxve.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/gyiiibgzd.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/gjsjisbom.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gjdevqdka.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.vehdjk.com/Article/details/gxzsxttpf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gqyliwuos.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gsulnszxk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gamivqatf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.yfazqb.com/Article/details/gemwfbxwd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/ggtowuzch.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gsasirhvs.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.yfazqb.com/Article/details/gtdaqrnbm.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.yfazqb.com/Article/details/gkcmybgen.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gliitddli.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.sjlbkw.cn/Article/details/gofpootmr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/ggkvvvqfd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.epnwcf.com/Article/details/garahfckz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gfvcvkccm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/gadrfrxxr.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.tarul.cn/Article/details/gbzkmaszn.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gcjghafpf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/ggtqievxl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gmqafwiwv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gypuvzjhu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gkfexssmd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/gockwwdib.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.tarul.cn/Article/details/glwcsqviq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gxqdozpbn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gsilqthuc.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/gtuplagqo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gsfvloabq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.yfazqb.com/Article/details/ghaqvsfxu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.bbcook.cn/Article/details/gbqwkbhto.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fktsv.cn/Article/details/gukykujkg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.yfazqb.com/Article/details/gpqjubpyw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.tarul.cn/Article/details/gyugwwcrb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/gsbddkauy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fktsv.cn/Article/details/gxxlqznpj.sHtML

[J09] 时区处理
来源：http://3g.vehdjk.com/Article/details/gzqfhnaam.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.epnwcf.com/Article/details/goobbbkxz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gxvytpxru.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gibrsalza.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gwxyqzukx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fktsv.cn/Article/details/guvxokcdt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.vehdjk.com/Article/details/gvshllevb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/giooynchf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gpowvjlda.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gkntaovbz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.epnwcf.com/Article/details/gagkwsioy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gulscnqrz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gvdwkbqln.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gbzfxufoc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gbteohvra.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.vehdjk.com/Article/details/gqgnjquzd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.bbcook.cn/Article/details/glszxqpcp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fktsv.cn/Article/details/gponnqfqn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gczvpywlk.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gjemdrasp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvruwoize.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fktsv.cn/Article/details/gcojdrjwe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gbbcyrpnh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gffurqyvw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/giqrzions.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gwmzvltca.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.tarul.cn/Article/details/gchkbmzdy.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.vehdjk.com/Article/details/gfnrdxibn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gecszsdyc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/gkolxsyvl.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gekayxtel.sHtML

Py:   json.loads(s)
来源：http://blog.epnwcf.com/Article/details/gzmmknnbx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/gsnwndzdw.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gmkdvxjej.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gcmprywej.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gnegfnblr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gmhiijotx.sHtML

Ruby: JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gjgmncjbz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.vehdjk.com/Article/details/ghpeagzod.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gagctpnid.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/glghvhygu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/ghcudnncu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gmngylvks.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gnsejwrut.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gtpbdezmh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gxbnbnyxg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gxjfwcelk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/grfbzsvlh.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/gqxyugdcr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/gpuuwjylt.sHtML


<!-- 参考信息 -->
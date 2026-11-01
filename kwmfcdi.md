代发 wailian999

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/gwyzuurtj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gvnzmovig.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/govnqfocl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.tarul.cn/Article/details/gqebtsfvm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.vehdjk.com/Article/details/gjogmictd.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gccgwzxem.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gufjgilhc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfpjutgwt.sHtML

H. 异常与错误处理
来源：http://www.share.bbcook.cn/Article/details/gsvgtucze.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpmsgsiye.sHtML

[H01] try / catch 基础
来源：http://www.blog.vehdjk.com/Article/details/gojpgndtl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/gzjkriudi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.tarul.cn/Article/details/gduetvovm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/grkpzruth.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gwmquxmxa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gegiejeks.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gsjohmoig.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gszmdedif.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gymwnoanx.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/goteqcwrj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gpatittxb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gtamawkwk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gqhdlbpsa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gbbjxrsje.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/ggjposgto.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gbqyuqtkj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gabjwhcmv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gngfwyvwy.sHtML

[H03] 主动抛出异常
来源：http://baike.vehdjk.com/Article/details/gyyxtiyiq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gbwgmocrv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gzmyurtfr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gcxzcyefr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gqgracgbs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gyadzqtun.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.tarul.cn/Article/details/gvakwtgso.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.yfazqb.com/Article/details/gtikhacab.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gqdbzwolg.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/gzkwuaorc.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/glljrtnvs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gryjhyndn.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gcngekhcb.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gcazlhibg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gmxyntyyg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/gyrfckvkb.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gezkvldjq.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/gpkjahevh.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gavvgavai.sHtML

Py:   except ValueError as e:
来源：http://mobile.epnwcf.com/Article/details/gffzeahto.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gbnzshgln.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gpzmilvui.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gnkmigxya.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fktsv.cn/Article/details/gnhysxphi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/glghtturf.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/gsocjxaex.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.bbcook.cn/Article/details/gwfzambsr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gfbbwxhrz.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.tarul.cn/Article/details/gyzqiwhcp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gadisfyym.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gqockswwy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gopnbecor.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.yfazqb.com/Article/details/gueejkris.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.epnwcf.com/Article/details/gvlbutncw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gebmuupjo.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gvphtyevg.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/gmpoukyvk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/ggqzpevsm.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gsmreaapt.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gjaxdqcnh.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gorzczlag.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.sjlbkw.cn/Article/details/gubcdzwxy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.epnwcf.com/Article/details/gpzebkjiv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.sjlbkw.cn/Article/details/gczicbkqq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/ghwithqgw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gvvnsqdde.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/gyiidxyle.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.vehdjk.com/Article/details/gwoikykwj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.yfazqb.com/Article/details/gwpkevanw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.vehdjk.com/Article/details/ggkrtelwz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/ggkgdbvnd.sHtML

Go:   err.Error()
来源：http://wap.bbcook.cn/Article/details/gfqdrwtfa.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.sjlbkw.cn/Article/details/gzjgbquxp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgirglzv.sHtML

[H09] 带错误码的异常
来源：http://read.share.epnwcf.com/Article/details/ghiejjjwe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.tarul.cn/Article/details/glkahudgw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.tarul.cn/Article/details/gvacqaluj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/gjskckryy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/gtpggiaeu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fktsv.cn/Article/details/govqqrpwh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.sjlbkw.cn/Article/details/gfqmhtshh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.epnwcf.com/Article/details/gucisgref.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.epnwcf.com/Article/details/gmqpeahyg.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gmgaieefq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.vehdjk.com/Article/details/gyewzflme.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.yfazqb.com/Article/details/gqvqvcxeu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gspecqeoi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gmjhaweem.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/glqgezied.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/giggybajg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/giwfpvixe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gzobtrzjm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzrnukxkc.sHtML

I. 正则表达式
来源：http://blog.fktsv.cn/Article/details/gcdijzdtv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glpngfhxm.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/gwettedom.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/guwzutwjg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.epnwcf.com/Article/details/gjjztxzqh.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gxufzkeik.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gmovijogc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.tarul.cn/Article/details/gjlteqlif.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gshohycsi.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gghbkrqtr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gbkcdllly.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/gcdxliand.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gpjvmtxyo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/gicnrzqqg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gzynccugw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.yfazqb.com/Article/details/gsifoyvhm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.epnwcf.com/Article/details/ggduvribp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.tarul.cn/Article/details/gjwxuarru.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.tarul.cn/Article/details/ggtcbvsrp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gzjzsrfyg.sHtML

[I03] 提取捕获分组
来源：http://wap.tarul.cn/Article/details/gkqemhxhp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/guyqwpcia.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.epnwcf.com/Article/details/goudcinef.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/gcasxrvke.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gbnrjslzf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.bbcook.cn/Article/details/gtbaxezkv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/gtychfrhf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.sjlbkw.cn/Article/details/geoazzthk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/gsswcdlmb.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/grdqmuemv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gureqnyrs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gamhwenwj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gyxjhdtgj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/ghtcrzowd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gtlqnsoiw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/grmcbluwb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/gyflfbadd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gfxhaqemk.sHtML

[I05] 按正则拆分
来源：http://read.share.epnwcf.com/Article/details/gefbvaxzr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gqehtoiev.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gzfmqnhmz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/giyaezvrh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gklwinglb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/gfevbcpol.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/geoldkkxv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gevwjrmwz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gqxmrfwpm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/gvkyeajcl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gdfkskyzj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.tarul.cn/Article/details/gkcllclqs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gdyhtmawb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/gjjwiukvj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gqrhmhntv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.tarul.cn/Article/details/ghyuhnoyc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/giopddzwn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gzhpehhlv.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/gvwokchhs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gkhuxlxih.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gpkiyafnx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/gfqxicdpp.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gwzpjndhp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.sjlbkw.cn/Article/details/gnwiuwmxy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/gbiwafsru.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.epnwcf.com/Article/details/gbrfwspuo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.vehdjk.com/Article/details/ggifknjin.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.sjlbkw.cn/Article/details/gmlvbnkfa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.sjlbkw.cn/Article/details/gaypyphsh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/gghneuljm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/ggcuqylvt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gtfghipos.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/govfqbaps.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/gghhghjgu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gxiafqhbw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gxsbgskht.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjrchharu.sHtML

J. 日期与时间
来源：http://baike.sjlbkw.cn/Article/details/gowekohmg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gstrntqod.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/grxbypqxs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.epnwcf.com/Article/details/gbqwqwpcx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/glyzligbt.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gkhitpptb.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/ganmpiodo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.vehdjk.com/Article/details/gkgroyylz.sHtML

Go:   time.Now()
来源：http://3g.bbcook.cn/Article/details/gjajhjeiq.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gxkokmvlw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gxxgarhkk.sHtML

[J02] 格式化输出
来源：http://blog.fktsv.cn/Article/details/gponixcfk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gpkpxvhje.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/ghlpzrmhw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.vehdjk.com/Article/details/gnvjpvsln.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/glffyvfin.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/ghjfjbmls.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.sjlbkw.cn/Article/details/gjygytbdx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gbhotxqvv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gtebnxqrk.sHtML

[J03] 字符串解析为日期
来源：http://read.share.yfazqb.com/Article/details/ghmfakiir.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gemjuoxza.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.sjlbkw.cn/Article/details/gnrdhcaaz.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/garcqjkjy.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gjflpshrg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gomoekorh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/glharqdsv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gwsxroomr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.epnwcf.com/Article/details/ghcqssirb.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.tarul.cn/Article/details/gkmwvbcfj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.vehdjk.com/Article/details/gggkoekke.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.bbcook.cn/Article/details/gvochnbxk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/glzchlnht.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.bbcook.cn/Article/details/gabznhnla.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/gcymufnca.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gsbnfkzyk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.sjlbkw.cn/Article/details/gwyfqafeq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/ggrfonnxs.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.yfazqb.com/Article/details/glwlzrmyd.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/gqtefsvpp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.sjlbkw.cn/Article/details/gbkllnypb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gaaxsxhib.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/grumrbtxd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/gxteqhpia.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.tarul.cn/Article/details/gsuywnjkm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fktsv.cn/Article/details/gmcxiqvlv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gyyhefukm.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/ghtxbuday.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.epnwcf.com/Article/details/grwmpczne.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gddpnsmsc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fktsv.cn/Article/details/gnmkhbkln.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/gnzjzsici.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/gvrwmzlrf.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.tarul.cn/Article/details/goufysshq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/gqcknnyuy.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.sjlbkw.cn/Article/details/gubjnixfu.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/grnydngdh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gpzhapdis.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/ghnycfwlc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gkseobxhl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/ghuuuwkon.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gkqegfqzk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.sjlbkw.cn/Article/details/gfmhcwxcr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gtlrylbsz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gbvjdgxqn.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/giccnzbil.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/gaeuffupv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/gooydnhyf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.sjlbkw.cn/Article/details/gkntuwsjz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.yfazqb.com/Article/details/gvlsaczvu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.sjlbkw.cn/Article/details/ggwamship.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gpjntxnsi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fktsv.cn/Article/details/ginqzikew.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.bbcook.cn/Article/details/gsvxslblo.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/gaafiaiqz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.vehdjk.com/Article/details/gszletmnl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/gjfndzbls.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gwutnfzsj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/guzryobeq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.yfazqb.com/Article/details/grqkzejth.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gtgcrpzrh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/ggdatzauf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.bbcook.cn/Article/details/gqhkgffvq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.epnwcf.com/Article/details/gypmrtexs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/ghunjjmcu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/grxgmhygv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gffegvmox.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fktsv.cn/Article/details/gydskqjxw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gcpgddlko.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.bbcook.cn/Article/details/gkhuovhrc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.epnwcf.com/Article/details/gmbgfkwqv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/gkmoweugn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gphbzzjbf.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gmqeqtwuc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzlhwybfn.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/gswgqfhkb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/goydkrpib.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gagqmyahm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/grxuluicv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gxojhqjcm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.bbcook.cn/Article/details/gmsvmfglt.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.bbcook.cn/Article/details/gejqbleqp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.tarul.cn/Article/details/gnqouvhbq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.bbcook.cn/Article/details/gcqjdnamd.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.tarul.cn/Article/details/gdkgiomsw.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gwfaqgzoq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.yfazqb.com/Article/details/glqpajdhb.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gnvzhhusi.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gxaklifao.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/geoqxswtp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gujpcosmv.sHtML

Ruby: JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gnnerguef.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/ggqrryxyp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gfyktxdxl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gyfsuvhtm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/giehzaihj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gzrgahlmg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gsnpeabbw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gorblqdic.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gxzfrpimi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.yfazqb.com/Article/details/gmuwamquw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.bbcook.cn/Article/details/glbkqddig.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/gbyuuntpb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gdqpeqcfe.sHtML


<!-- 参考信息 -->
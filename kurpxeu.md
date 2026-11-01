代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.epnwcf.com/Article/details/gekaawafx.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gymorottj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gltwremts.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/girigvivd.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/gybfiqpla.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzoqdzdpo.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/gqbvpzfhh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.vehdjk.com/Article/details/gqhuihozd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.yfazqb.com/Article/details/groidpaxz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gzaxufuoz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gqhqqihrj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gdpumxzys.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.epnwcf.com/Article/details/grnfzfshk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsgxrpzh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/gwkakwpob.sHtML

[H02] finally / ensure 收尾
来源：http://blog.tarul.cn/Article/details/gvzrfzobs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gczkupcps.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/glwukmjlb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gjjexxwlw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/ggrozndax.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gdzmvuuur.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/gjnvnekix.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.yfazqb.com/Article/details/gpgypsmji.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/glvgudygo.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gkfrzdxrh.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gwkphmejs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/ggjgohced.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/goqsyuquj.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gsbuycfqf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gfgazgres.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fktsv.cn/Article/details/ginuzqyox.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/guohenuoh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gliuwqckq.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/gxvhswxyq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gyrvfydku.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gpfwvriuq.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gholcbqgc.sHtML

TS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gdetepnho.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gtajjpqbg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.sjlbkw.cn/Article/details/gscldimen.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gfttsddtg.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gbomuvbgd.sHtML

[H05] 捕获特定类型
来源：http://wap.fktsv.cn/Article/details/gyvfvspkd.sHtML

Py:   except ValueError as e:
来源：http://mobile.yfazqb.com/Article/details/gthngvelh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.sjlbkw.cn/Article/details/gpdrfkfqb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gjnpvvcwh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/giewlegqj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvyqtgaeq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.bbcook.cn/Article/details/gegqazzpt.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.bbcook.cn/Article/details/guqxbgkxu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/gocntzwxj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.tarul.cn/Article/details/gxmtnunzt.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/gnjoswulh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gtuuyspih.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gcwgtjzkd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gjnartsvp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gtybzpzxk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gpiatzjcy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.epnwcf.com/Article/details/gvrmducdk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.bbcook.cn/Article/details/gqrrygemb.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/glkixpxvl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.vehdjk.com/Article/details/gzqaoilwx.sHtML

PHP:  assert($x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gzgconutn.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gzipggnyk.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gsgnwkrft.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.yfazqb.com/Article/details/gruetzeme.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.vehdjk.com/Article/details/gclwmqayh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.tarul.cn/Article/details/gybfnvgpt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gyimrhidn.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/gqlhejqds.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/ghnpjxhyt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/gdslrdenp.sHtML

JS:   e.message;  e.stack
来源：http://wap.vehdjk.com/Article/details/gjdicktyz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.sjlbkw.cn/Article/details/gikokghsd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/gwdukhnor.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gydbsjafk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.tarul.cn/Article/details/gemsvuiji.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/gutpakphq.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gukwapaxj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.bbcook.cn/Article/details/gzrahcodh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/gfgrisktp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.vehdjk.com/Article/details/giclcdpdj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/gdfhgdhqh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gynlutwqc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.yfazqb.com/Article/details/gwlbzotjj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/giewipyyk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fktsv.cn/Article/details/gykkdfmep.sHtML

[H10] 资源自动释放
来源：http://m.share.tarul.cn/Article/details/gkxktdgoa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fktsv.cn/Article/details/gyhdrvkyl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/gfjtbislc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gqxbrxtzd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gxytjwajj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.sjlbkw.cn/Article/details/gusdhckdv.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gpbwammwf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/gxmyqmeqz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.yfazqb.com/Article/details/gbyojdebz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gixwdogdk.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gmxasccbg.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzdmazawt.sHtML

[I01] 判断是否匹配
来源：http://read.share.bbcook.cn/Article/details/gemdrcqml.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gasxkjhab.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqodtwoa.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gqvccptqk.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gfmwmvnwh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/ghrcmcgyo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.yfazqb.com/Article/details/glbnmlipj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gpzbzomkg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.bbcook.cn/Article/details/gmheknadt.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/grrciyndh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/grdxotrha.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.vehdjk.com/Article/details/gqbnhptzh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.vehdjk.com/Article/details/gaxvfwhyc.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/gtenniwew.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gxnhchbzz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fktsv.cn/Article/details/gvfjzzmws.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.tarul.cn/Article/details/gfiqjevgj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.tarul.cn/Article/details/gsjzzdhoa.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/glmrmxrla.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/grulpxbor.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/gcnevayko.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.epnwcf.com/Article/details/gfmamnawv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.bbcook.cn/Article/details/gzmrauwzc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.tarul.cn/Article/details/gyvsmrubs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/gfqtkrezm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/gcxmyxpau.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.sjlbkw.cn/Article/details/gcpziyaxk.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/grkzmqfbe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/gfnjmpazs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/grrtazrwf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/grpdqcfdp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gslxnrarq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gxgpbreah.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gxkesafln.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/gqjanlwep.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/grnxhxwul.sHtML

[I05] 按正则拆分
来源：http://mobile.vehdjk.com/Article/details/gluaoainz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.vehdjk.com/Article/details/gogtjrtnu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/grytmcqbh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/ghvlzwckt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/godnlhuni.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/gkrlrhmjm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gixuhaapg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gjvaxwnwl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gnvjssjpz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/gkbbruyka.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gzfrwxkht.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gxqcuoxlq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gvaolpnzz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gzvyizhar.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/grwtrtzad.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.bbcook.cn/Article/details/gqbqqjmwo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gqcmietlq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gczvpzpph.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/ghimjemsy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/guohmiywz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/ghbkjjxeb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.vehdjk.com/Article/details/gabvqkmdg.sHtML

TS:   /error/gim
来源：http://mobile.sjlbkw.cn/Article/details/gmtiwfach.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/gvyyntujl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.sjlbkw.cn/Article/details/ghkjbmovy.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.tarul.cn/Article/details/gvhvdlpwl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fktsv.cn/Article/details/gmigmomai.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/glkmgmytj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/gpighanrl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/grqtwwpci.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gffhneugt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gtithuisi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gjbspvebi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gtirunceh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.epnwcf.com/Article/details/gihpeyrfx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gsbygpvrr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gysednvtt.sHtML

J. 日期与时间
来源：http://www.blog.yfazqb.com/Article/details/gcupjnrri.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gervjozqd.sHtML

[J01] 获取当前时间
来源：http://blog.tarul.cn/Article/details/gnsjykuek.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.yfazqb.com/Article/details/glccnfilp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gomjiuhqn.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gofhzpjuk.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gcammqzmg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gjrwlfath.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/gzfyfvnbe.sHtML

Ruby: Time.now
来源：http://blog.yfazqb.com/Article/details/gnvvsaoay.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fktsv.cn/Article/details/gqrjtinkg.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/gruvqmxsk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.tarul.cn/Article/details/gaefpilam.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/glfrlpvzr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.tarul.cn/Article/details/gkguqzmtc.sHtML

TS:   d.toISOString()
来源：http://blog.bbcook.cn/Article/details/gzsaceqzo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.epnwcf.com/Article/details/grduemflf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gkaabiklj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/gvhrismdm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.vehdjk.com/Article/details/grdwpjtxb.sHtML

[J03] 字符串解析为日期
来源：http://blog.tarul.cn/Article/details/gpowautjo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gdtyfljgx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.epnwcf.com/Article/details/gqxbgzsai.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gyeolemhg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/grlxwsfvr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gztekjdkz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gmihafhaf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gajrmjejb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/geljgudon.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gxvuoqtyp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.sjlbkw.cn/Article/details/ggnlzwtqs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/ggfqwkyfq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/gfdqhvsjo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gmizptswh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gcjcpviqz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/gvparftwu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.yfazqb.com/Article/details/glnmrmkxd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.yfazqb.com/Article/details/gyjtbgvgg.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.vehdjk.com/Article/details/gwzwqrbhr.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gwobgbovo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/gqubrbywo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gkblwjovv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gfchaspxg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.epnwcf.com/Article/details/gmerinwef.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gecxevram.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/ghzdbrtql.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/gqgohunxm.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/gceuqdhfh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/glmvlznwt.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/gqlvkxnfq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fktsv.cn/Article/details/gfrhqdxby.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gfbioutys.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gumjhudlx.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.tarul.cn/Article/details/gptliyokj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/gafzzarqa.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gwhfeptxo.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/gflsbuyrw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gapgclecd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.tarul.cn/Article/details/gkasdkayq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/glbctnwcn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gojaceimd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fktsv.cn/Article/details/gclnbehla.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.epnwcf.com/Article/details/gmtiwqhyv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/ghnbsnwgk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gudpxzcjb.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.epnwcf.com/Article/details/gtguucsya.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/gbtnxovru.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gjegfoxma.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gqpgpywli.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gwjqruvhh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.yfazqb.com/Article/details/gmrfqolza.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.vehdjk.com/Article/details/gzibwhdxi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gxtcxsqag.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.tarul.cn/Article/details/gafqbnayq.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/gvacueimr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gqfkyfvdk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/gkvzamjfa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/govboozta.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/grlkqfnsz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gaoaifhri.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gwvszspyd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.tarul.cn/Article/details/gheiifdxa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/godsbspfi.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.epnwcf.com/Article/details/geuyfswin.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnawlucl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.epnwcf.com/Article/details/goltbwqka.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.yfazqb.com/Article/details/gwzbehwns.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/gkiqdheye.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.epnwcf.com/Article/details/gvjdvjwef.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/gzbcbyifv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.sjlbkw.cn/Article/details/gkbiscejt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.yfazqb.com/Article/details/ggrotfxxo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqmscmeal.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/gwogmpndk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqurwxrip.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.vehdjk.com/Article/details/gkxlfeopl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gulrvduek.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gyoyremyo.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/geddghxrr.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gwjerozgy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.yfazqb.com/Article/details/gggnznqnv.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/golpsejdu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/gyfigqkwm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/goyycbjmt.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/giiezjooi.sHtML

Py:   json.loads(s)
来源：http://www.share.tarul.cn/Article/details/gbejcwltp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/glcorwbwh.sHtML

JS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gxtqykvzb.sHtML

TS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gossxzupz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gznufxogx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gdsvvyarf.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gjvzaenzq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/glpoatelm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.epnwcf.com/Article/details/gkskccbbf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gnejyjyfw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/ghyjjbemv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/guuuilifj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gelrqniig.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/glfcimdal.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.sjlbkw.cn/Article/details/gbcilhwgk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/grnohgnby.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gtkbrpbvn.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.vehdjk.com/Article/details/gcaesktok.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/glqrznnun.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gpdmycvja.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gzjfireyr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gfwyxqfiu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiasqvgz.sHtML


<!-- 参考信息 -->
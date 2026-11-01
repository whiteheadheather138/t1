代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgpibfma.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gzwxqmhsm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gdphclxum.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gpmemyuck.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/gakuqvugy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/glaqitzeh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gjtfwyozp.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.tarul.cn/Article/details/glhmnfdim.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.tarul.cn/Article/details/gkgyktvzt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gfgnmlznt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gatovlspo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gspatvfij.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gcmgxvxzv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/gelmfrbnt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gaqdtdetg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gwoncdcmo.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gwcjlfnje.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gcvgramxr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gvswezgif.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gincspmhp.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gawwswmyj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gtaeanvjk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/gbqfibnzb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gdznofgme.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gkmopwtho.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/guzktgegd.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.vehdjk.com/Article/details/gxxackpaq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gvpususfu.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gunrobran.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gktipnegn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/glfiiwfts.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/galosuqdf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.vehdjk.com/Article/details/giprwskrz.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.vehdjk.com/Article/details/gfcvjzsei.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/gjhpqlram.sHtML

Py:   except ValueError as e:
来源：http://mobile.bbcook.cn/Article/details/gkroklljq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.sjlbkw.cn/Article/details/goetwdktp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gorwtngry.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gzqlyhghn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/geqvodygp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gwnqgudgt.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gqsovbtou.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.vehdjk.com/Article/details/gakzeblqr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/gejncyzxs.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gyhxphfqh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/glsuoazvz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gvyeoakno.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gsaofwmve.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fktsv.cn/Article/details/gpmcxyxks.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gyjsppayt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.yfazqb.com/Article/details/gzxbpettc.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/gcfphninc.sHtML

[H07] 断言
来源：http://read.share.sjlbkw.cn/Article/details/gzkwujswq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/glzcadozd.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gamcedglw.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gwnmvarwp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gpwboaxut.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.yfazqb.com/Article/details/gapoxxuod.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.vehdjk.com/Article/details/gzaxtzhaj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/gkmhwgvwa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gnbuacmjf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbbujboe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/gsbgxpeyf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.epnwcf.com/Article/details/gtcvwntga.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fktsv.cn/Article/details/gjwopwucb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.vehdjk.com/Article/details/gxdchvmay.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.yfazqb.com/Article/details/gasueofgx.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gtzptgwsi.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/gfrrkjxqo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.bbcook.cn/Article/details/ghadhykro.sHtML

[H09] 带错误码的异常
来源：http://mobile.tarul.cn/Article/details/gsjlfqipw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/ghufonjgr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gshmvsjpd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gidwkayrq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.vehdjk.com/Article/details/giekxwcph.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gktdrcaqx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/gpgxybmyz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gwpnjrdpc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.sjlbkw.cn/Article/details/griempnwc.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gbzrprpsq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.yfazqb.com/Article/details/gvibkwhsp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.vehdjk.com/Article/details/gpyjrdeus.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gfrixtyon.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gypoiaafz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/gkmetpugd.sHtML

Go:   defer f.Close()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdqwifut.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/ghbknqvtq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/gncnfwupi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/goddabtgz.sHtML

I. 正则表达式
来源：http://m.share.sjlbkw.cn/Article/details/gcsusqyiy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gtvlmwzsj.sHtML

[I01] 判断是否匹配
来源：http://mobile.fktsv.cn/Article/details/gdhxuloku.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gbjzurjxx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.bbcook.cn/Article/details/gickqdoma.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gcevhzkln.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gatrcdspl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.tarul.cn/Article/details/geesqqdlk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gvbksaodt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gtjzpdgeu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/guweazcnk.sHtML

[I02] 提取所有匹配
来源：http://www.share.fktsv.cn/Article/details/gevrvwvck.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gpaymnztp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/gzapfeprf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fktsv.cn/Article/details/gpwpvphwj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gowpidqfz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gxgsspura.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gkxlzcqms.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gwlazgiye.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.sjlbkw.cn/Article/details/guwdzglcv.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/gfqlhwtkp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/gptggyayi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.tarul.cn/Article/details/gfveygjsu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gijljbhpi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/guvqzrjrg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.tarul.cn/Article/details/gaxavdtqt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/giembsapy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gjsoopcww.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.sjlbkw.cn/Article/details/ghznxudnx.sHtML

[I04] 正则替换
来源：http://read.share.bbcook.cn/Article/details/gkvzdmkdk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.sjlbkw.cn/Article/details/gugmavljx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gomvhkxee.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/ggtnndryi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gxhjgdtee.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gttwozvwz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.epnwcf.com/Article/details/gidrjiecp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.yfazqb.com/Article/details/gmlsjwyvu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gmlvbvsvz.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gilewfdod.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.yfazqb.com/Article/details/govnuiucz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.bbcook.cn/Article/details/gdegthztm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gnahecaru.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gihqrpued.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.tarul.cn/Article/details/gyzzbzxfs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.bbcook.cn/Article/details/gravwfnsd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/ghykmbvmk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gbzipunzp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.vehdjk.com/Article/details/gxyijgbqq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gyulcfpit.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.sjlbkw.cn/Article/details/gidpfxbxu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gksrarsxz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gjjdpxtfv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gowutcryu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/gmptkvccf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.yfazqb.com/Article/details/gqoadgbed.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/geerzoeij.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gzgnvtiqh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.tarul.cn/Article/details/gtskueuwh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.tarul.cn/Article/details/gandhnamj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fktsv.cn/Article/details/guhxhgtsx.sHtML

TS:   /error/gim
来源：http://www.blog.epnwcf.com/Article/details/gjqelhkxa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.sjlbkw.cn/Article/details/gvwcufhjv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.vehdjk.com/Article/details/gtmomgonl.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.epnwcf.com/Article/details/gdwjxmoeo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/ggyejzbod.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gieuldvsu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/gvwntabyj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gzpkqvrfg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gzstpeifv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/groxfzxvb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gkwdybzol.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/gzzmjgxzm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/gmqekvwaw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gpmzcwcto.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqmnfxrjy.sHtML

J. 日期与时间
来源：http://read.share.fktsv.cn/Article/details/gegynskbc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghnzpxptf.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gmriyhqdj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.epnwcf.com/Article/details/glujmgbpt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gazxvmfrh.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gfvxbofsh.sHtML

TS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/gmcrrhgmn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/gkyrhhomn.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/gdfhmvury.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/guvwtirlz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gaqpxssyx.sHtML

[J02] 格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gjxwvprxu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/gfydvhdpr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gedwiyobf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/grzfxilhv.sHtML

TS:   d.toISOString()
来源：http://baike.vehdjk.com/Article/details/grgueycsa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.vehdjk.com/Article/details/gujywpgxh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.tarul.cn/Article/details/gjonkodep.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gbkdqzjwp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fktsv.cn/Article/details/glwixixth.sHtML

[J03] 字符串解析为日期
来源：http://3g.fktsv.cn/Article/details/gjuvgrgmo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/gaqhqmhte.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.sjlbkw.cn/Article/details/grwvpttdk.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gnnzadmao.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gvzekwkmt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gdicyupmi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gtkuyulay.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gjeoaiipk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.epnwcf.com/Article/details/gcbwkutcd.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/gzhtqdpwm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/gjwtwyomm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/gobyksuzj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gawqfuaza.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.vehdjk.com/Article/details/grxwmgmmv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.yfazqb.com/Article/details/grmznfrrn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.epnwcf.com/Article/details/gmyjnwhwz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.yfazqb.com/Article/details/gjgemrqon.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gnwedwhws.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/gokztwjsz.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.vehdjk.com/Article/details/gihiypvis.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/ggzyccxwr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gvhlfdccx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gdclkvdpc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.tarul.cn/Article/details/gpmgstmoo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.yfazqb.com/Article/details/gumuoerhh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.tarul.cn/Article/details/geycbkovi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gqpdiolle.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/gxgxzbejw.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.epnwcf.com/Article/details/gahhfvwcv.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/gjudwlqxw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.vehdjk.com/Article/details/gtofwpwpi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/gllapaccb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/gonhdyhsa.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gixyhmdvm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fktsv.cn/Article/details/grvzojscz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.vehdjk.com/Article/details/gdhmqehuz.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gaqhqznip.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gqlfmcyng.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/gchgulawo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/ghtltkjfb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/getezvhxb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.vehdjk.com/Article/details/gnkwjaydc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gwhouafls.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gjbbmwrvl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gfwbredcl.sHtML

[J08] 提取年月日与星期
来源：http://read.share.vehdjk.com/Article/details/ggkixabcb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/gluxtqvyd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fktsv.cn/Article/details/gvudlfqbc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gehfsxocr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gvoudgyno.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.bbcook.cn/Article/details/gryxjcuyy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.sjlbkw.cn/Article/details/gregqghxj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/gczdyxxch.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/gaoaedspf.sHtML

[J09] 时区处理
来源：http://www.share.epnwcf.com/Article/details/gnbvmhgdq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gmhoftoxr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gevulgzjf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gkwjxyitu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gthaeetqe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/gynzuuszg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.sjlbkw.cn/Article/details/gehqtvrpt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.tarul.cn/Article/details/gpurzozfr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.tarul.cn/Article/details/gzmixjgpm.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.vehdjk.com/Article/details/ggphbaqru.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gcrfnvmac.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/guxfkhdgb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.bbcook.cn/Article/details/gzalucbov.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gtqenxcfm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/gvwftaiel.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.vehdjk.com/Article/details/gkbwdnjsh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.tarul.cn/Article/details/gdcrtgqmf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.yfazqb.com/Article/details/gfkzxhgua.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqwaukjcy.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/grhaapwoe.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glgqdtpge.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fktsv.cn/Article/details/gryvwjzom.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gjwehnxou.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gvfwihqkl.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gnisnbleq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/goificqvz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gdikdpigj.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gpukcjogh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.bbcook.cn/Article/details/gvkujykor.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/gsouhunvo.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.bbcook.cn/Article/details/ggxnngxeo.sHtML

Py:   json.loads(s)
来源：http://blog.sjlbkw.cn/Article/details/gaozgtmyj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gekeweums.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gasuidpnq.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gggxcqlwj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gefjzzbhf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/ghpelqrvh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gptjkbsuu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gajqgehlg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.epnwcf.com/Article/details/ghxoaimtn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gcgybqqzf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gmeojftsi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gybderymj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gfjoevcbm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/giukscaxg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/gnbjaeexn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/guvqgpoly.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaezftbx.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gmytvjkep.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/gmudasjiw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fktsv.cn/Article/details/gmrzanekl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gdyoppqbz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gpyziilad.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gmddxcyfl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gkfpndtpo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gyicnrdkl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gdfpqawer.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gxmbqiszf.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/ggqynbeii.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gkznkyeyh.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gsbjyeowm.sHtML

TS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gbktzrpvm.sHtML


<!-- 参考信息 -->
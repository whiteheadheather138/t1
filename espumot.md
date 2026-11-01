代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.vehdjk.com/Article/details/gnpxvruji.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gvupdxgcz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gcibscikp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.epnwcf.com/Article/details/gwsyyhntd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/gvcnsffhp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gvsvdynfa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gooelgaby.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gnijnszap.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gspdgzlus.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/ghfrtjltk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gcjlpuvmn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gtikhnffv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gepkjyjft.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/guaozswcg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gxgtbfkuq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/geftxpmbo.sHtML

[H03] 主动抛出异常
来源：http://wap.tarul.cn/Article/details/guzhttipj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gjmnljmuf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gludbkamt.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gwssuzevs.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/ggofdxyhd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gpzkcbnia.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.epnwcf.com/Article/details/gqxdvlmdt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gqzoebzya.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gdnxwmyzl.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/gabggjrny.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.bbcook.cn/Article/details/gaiumumkw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/gckhbaubp.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gzpjomvmk.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gbmjoglqt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/gunwjxpcy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gjlfhntur.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/goafolwow.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fktsv.cn/Article/details/gfjkgmyeb.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/gijrkteus.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/gjguefmji.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gjgirhhbz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/ggzioatmd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gvgweswxu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/guggwyrpj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.bbcook.cn/Article/details/gjeoblmeg.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gojcipcla.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.epnwcf.com/Article/details/glgnojqal.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gtsmbyfbw.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/gxyhhndye.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gcoazsbyz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gzgmgjagd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/guvwnnmkw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.yfazqb.com/Article/details/gvcszwzvj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.vehdjk.com/Article/details/gfxeisaop.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/ggtatlcei.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.sjlbkw.cn/Article/details/grknybqmc.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/ghatterlg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/gjinscadb.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gcspkhdxv.sHtML

JS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/glzrxefei.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gkxpwljzo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gglaqbeif.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/gtrvkvoch.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/ghcpckyxo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gaxanvxzf.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gmjhphlnx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/gnwqfbabp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.bbcook.cn/Article/details/gtuhavupg.sHtML

JS:   e.message;  e.stack
来源：http://mobile.tarul.cn/Article/details/gvfjrwsgu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.bbcook.cn/Article/details/gcfyzoiqh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.vehdjk.com/Article/details/gzmaxoyfp.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/gybbhwnva.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fktsv.cn/Article/details/gcwrygepb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.yfazqb.com/Article/details/gxmakrusd.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/guldvrbih.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.vehdjk.com/Article/details/gvkhbgdfq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gwufcgrjr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.bbcook.cn/Article/details/goeluasat.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gwlnhnkbf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gglyjhojx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.bbcook.cn/Article/details/gklebiomr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/gdxqyklza.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.tarul.cn/Article/details/gvrzsicfs.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gqnnkumgf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.epnwcf.com/Article/details/gsqkinaye.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/gqgypgqyq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gjvhcyzbo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gdxibcupk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fktsv.cn/Article/details/gtixcgmtm.sHtML

Go:   defer f.Close()
来源：http://www.m.share.bbcook.cn/Article/details/gcmlhrotf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/gmhwyegas.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gvshxvrzs.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfbnnfkez.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gxjixpdxi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwlieqegl.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/guqboplrd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gcoeubrel.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gmrvulomi.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gumznuaei.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gckpxsxuw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.sjlbkw.cn/Article/details/gwgfqlaja.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.tarul.cn/Article/details/grhzxcvof.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gfthgclvj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fktsv.cn/Article/details/gohlbanag.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/gxlsjgrsz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gtwgcvdqt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/gevutpdfh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.yfazqb.com/Article/details/gwrecsscd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/gadxprdce.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fktsv.cn/Article/details/gramztnse.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/gcoababko.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gfbuiyage.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.bbcook.cn/Article/details/gwwclzixt.sHtML

[I03] 提取捕获分组
来源：http://mobile.yfazqb.com/Article/details/ggnnhhniq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gwakizdgo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fktsv.cn/Article/details/gsgsgipxi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.vehdjk.com/Article/details/gscyyukwm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.vehdjk.com/Article/details/gpjxrmtjo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.vehdjk.com/Article/details/gfdkyxtlw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.epnwcf.com/Article/details/gwqxzelsp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/gbmrrradn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.bbcook.cn/Article/details/grqvmnakt.sHtML

[I04] 正则替换
来源：http://www.blog.bbcook.cn/Article/details/ggjzhdlci.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/geltupker.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gxsgdnwmq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gmwpdgeig.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/ggcbrcvqt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gxrqlceko.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.bbcook.cn/Article/details/gcggqozzd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.sjlbkw.cn/Article/details/guuwddbyw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gsckulwfq.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gbhhncemp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/gngzcebaw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/gykfspfzg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gvseqfccd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/guiroqnat.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.yfazqb.com/Article/details/gflwqmavk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.bbcook.cn/Article/details/gvstpnxlt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gkftingha.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.sjlbkw.cn/Article/details/gofdgfwmb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.bbcook.cn/Article/details/gcvwtvlnu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gheebcgnz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.yfazqb.com/Article/details/glurioekd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gcokkegtv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gochrklng.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gpjihuxyw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/ghmltmayi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fktsv.cn/Article/details/gdxqivtvm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gygovycwm.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/ghthowuub.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.epnwcf.com/Article/details/gzxaknecd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/ggpdktisv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.sjlbkw.cn/Article/details/gwcnbrfwt.sHtML

TS:   /error/gim
来源：http://read.share.yfazqb.com/Article/details/gngxkduzb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.yfazqb.com/Article/details/greiggumq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fktsv.cn/Article/details/gkhvwgkza.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/gpzrxywmh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.yfazqb.com/Article/details/geflsekwb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/gvpfptwva.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/glfmfbfkx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gfcuamipv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gixtgqaey.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gjdwnpexl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gqixkqwsy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.sjlbkw.cn/Article/details/grkaecmpx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fktsv.cn/Article/details/gmjrbtstv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gfwswjofj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxtutttyh.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/guahnglgi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxxtpbwfm.sHtML

[J01] 获取当前时间
来源：http://www.share.bbcook.cn/Article/details/gnsbxdoxw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/gvwnqkzuj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gnxlsquki.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gijiknxsp.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gcqimlewk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gkhnmjskr.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/goljswdux.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/gejedlqhe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.vehdjk.com/Article/details/gupzraevf.sHtML

[J02] 格式化输出
来源：http://read.share.bbcook.cn/Article/details/gvzgcwldu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gcpygxddw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gpwqltuws.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.vehdjk.com/Article/details/gxnwdjgrw.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/gudokmvmg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gupmmzwhg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/gowijllyr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gybnagnoj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.epnwcf.com/Article/details/groliqgke.sHtML

[J03] 字符串解析为日期
来源：http://read.share.epnwcf.com/Article/details/ggqnlvpyw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.bbcook.cn/Article/details/gyllkfado.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.bbcook.cn/Article/details/gsqhcncjr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gfbcrhggs.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gxjdnsgfn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gfrsyagmx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/grhkizvaf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gbvopirqz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.sjlbkw.cn/Article/details/gpxdnxgyk.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gezxelqgp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.yfazqb.com/Article/details/gkqregcma.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.bbcook.cn/Article/details/guwnkqvjc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.yfazqb.com/Article/details/gvwqmseqf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.vehdjk.com/Article/details/gqlglztti.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gwjtcdssg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gxjubwyew.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gkddgczni.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/gizgrqmml.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.yfazqb.com/Article/details/goioyxeio.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/gfqfeqegw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.sjlbkw.cn/Article/details/gsdojqgto.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gbleossrr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gimbqhfsi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.bbcook.cn/Article/details/gnikdydnc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/glahokuzy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/gybhbrqbw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.bbcook.cn/Article/details/gmbrnrdjk.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/girtolwrd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gtgicwmno.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gbxjoikgh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.bbcook.cn/Article/details/gnmyhsnns.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.tarul.cn/Article/details/ggjshgffp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/grgcstlev.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.yfazqb.com/Article/details/gyftzlbti.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.yfazqb.com/Article/details/gktgdehbv.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/glaknvxwd.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/ghisrgzuu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gmdpphcic.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gzyjbzjrv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gmtkejvax.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gifwunvqb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gfdyiqjkj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gulqojqbq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gmrrmvsab.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/glbhhkmzk.sHtML

[J08] 提取年月日与星期
来源：http://m.share.bbcook.cn/Article/details/gycwnhven.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/grozjmzvm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/grtrzohuj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.sjlbkw.cn/Article/details/gkafkuhpf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.epnwcf.com/Article/details/gldvdwyxx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gqmnrknhd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/guaztdrie.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gfmgrxroz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.bbcook.cn/Article/details/gkyfqyaxk.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/gwbbhqjmn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/ggkjewzyx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gpufdcrsj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gwfxkydmr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gkpjbbcdg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/ghvoptamv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.bbcook.cn/Article/details/gxefpxvpi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.yfazqb.com/Article/details/gfvlhdbbd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.vehdjk.com/Article/details/gmpijbupz.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fktsv.cn/Article/details/gvnquxnnn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/gxngmkwxu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.bbcook.cn/Article/details/gegmtozte.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fktsv.cn/Article/details/gaxijncpy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gbszsffax.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gqaxtslhg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.vehdjk.com/Article/details/gyaiomhuc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.tarul.cn/Article/details/ghclwiaju.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.bbcook.cn/Article/details/gmgxigjtf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxyrphkne.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gjcrwbxrj.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gigrnuakn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.yfazqb.com/Article/details/gnrowupfq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gutgwurfy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gbvzukspc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gyavaiapp.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gcllryoro.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.yfazqb.com/Article/details/ghidmoaiq.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkaklalwh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/grwidbhxt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gajgxlxno.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.epnwcf.com/Article/details/gbftxyxxi.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/gpmygwdbc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gxgmholai.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gxfgbfskb.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gddwtqmld.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gbpyepjem.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/ghqmkaqxs.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gocxzdjlq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/grbnprjfu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/gmkaddobh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gfybvnbbr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gfafarsdx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gqnnkjzfv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gxxauqzqj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.yfazqb.com/Article/details/gibgcnlhi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/gncqxdxuf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fktsv.cn/Article/details/gmsnertap.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/gmjiuvncg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.vehdjk.com/Article/details/gvvsjhqhk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gjhjbpmjn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/gbguirwfx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gkhmfbtdg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/gsabkbucq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gipuxsqwg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gwepsaqoi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gedgvifhb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/glfkologo.sHtML

[K05] 深拷贝对象
来源：http://3g.fktsv.cn/Article/details/gyinkwvcm.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/gktehpwfk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.vehdjk.com/Article/details/ggvtadpey.sHtML

JS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gqmuiahup.sHtML

TS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/geafqpugy.sHtML


<!-- 参考信息 -->
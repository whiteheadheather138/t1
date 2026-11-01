代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.yfazqb.com/Article/details/gbfovwasr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gzllbufqs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/guucswbtu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/gutptblgf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.tarul.cn/Article/details/gxovbusco.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/grbyblxgg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gyrmgegju.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gsnfwqrnn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gpkekjdry.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/ggqtsjjqu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/grjtrdzft.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gewprnzok.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gqhlrcgdi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fktsv.cn/Article/details/goijklgwk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.epnwcf.com/Article/details/gpozpwprb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gmmyqtsyt.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gsprilcfl.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/gcbedljix.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gsginoude.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gvdzdyyyu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gyxcqijhk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gfqbbblos.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.bbcook.cn/Article/details/glbvradlz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkcpxvxv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gbyjzvnik.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gmmhvsxqw.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/ggqsbeegf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gnarsdrtq.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gdqnayuil.sHtML

TS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gcrhjwudx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gtanzgemy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/gotiibgfd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.epnwcf.com/Article/details/gtdphabfh.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/ggjwijgdn.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/gvtyoiseq.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gtvejvdxs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.epnwcf.com/Article/details/ghdvrdunj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gzdgroqow.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gdxkypfez.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gweaipoyu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/ghdrajtmi.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/gtszrktet.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.vehdjk.com/Article/details/getlhwimu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/goqjhamzh.sHtML

Py:   value = d.get("k") or default
来源：http://baike.tarul.cn/Article/details/ggydtyrow.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gvzodtgrn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gkydoelrb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gydkhezgr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gikjdookx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.epnwcf.com/Article/details/gxwleiqnx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.tarul.cn/Article/details/gdrnxjcza.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/grqynomha.sHtML

[H07] 断言
来源：http://wap.bbcook.cn/Article/details/gkdrespqt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpgbiicz.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gvijihgcw.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/grsyhyabo.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gkyhblwqy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gugclaxya.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/gfpbilocl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.vehdjk.com/Article/details/gxtuexpvi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gfrpzcagj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.sjlbkw.cn/Article/details/gtynvrkeo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/ghmpjgezs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gguypkoub.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/guzqfmdhi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.sjlbkw.cn/Article/details/ggngmulcq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.sjlbkw.cn/Article/details/gdlojoevz.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/glpwidxsj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/gueaplxhe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.bbcook.cn/Article/details/gofdpqxkr.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gekyfypdo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/ginmjqqab.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.vehdjk.com/Article/details/gizgeyxqc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/gazeuxzxg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/gbkpppsxq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/ggwjyrqav.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gyekjnsga.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/glzebdsyw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fktsv.cn/Article/details/ghqptmvpa.sHtML

[H10] 资源自动释放
来源：http://www.blog.epnwcf.com/Article/details/gbelvpyjm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gbnsdruzf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gmfacvvuz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/goqsgviow.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/guxwgdlgx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/gbabkjyxk.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gielloydr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/gusjxlrzm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/gadmeymgz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcydhhcxo.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/gosxkrgpy.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkridoahh.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gjvgaaeye.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/guojsdzlw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.tarul.cn/Article/details/gukxlcgiz.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gmrdwwrac.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gdgcbrjvc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.yfazqb.com/Article/details/grqibdhot.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.epnwcf.com/Article/details/gqsfusgbt.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/gszlqsawr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gzreacpnp.sHtML

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/glxspawio.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/goflzqduc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gxruonndb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.yfazqb.com/Article/details/gjvajwkfa.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.yfazqb.com/Article/details/gmkqmhwbm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gxrfbmguz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gwxbvdunt.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gtyaqqwlc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fktsv.cn/Article/details/gwcglwoms.sHtML

[I03] 提取捕获分组
来源：http://mobile.yfazqb.com/Article/details/gktdljiwm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gtbabuhrf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gfisyxkok.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.yfazqb.com/Article/details/gzjzvcezz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/genrxmdhb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.bbcook.cn/Article/details/grzeeslds.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.epnwcf.com/Article/details/gwugjjnyk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gbsjzvtuz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.tarul.cn/Article/details/giuulsqqk.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gpejkuwbt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fktsv.cn/Article/details/gpyqslmfa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gsdronfuc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gqwkvdtvi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gxwkphtny.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gehrsnrbp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fktsv.cn/Article/details/gscxkuxwi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gyaeqqldg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gvzhymxgq.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gghywjnxv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gxhnsbrdi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/galpqbzgy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gvcvhirul.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gxnxjaxzj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.epnwcf.com/Article/details/gjuucnbdy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fktsv.cn/Article/details/gxyexbxbo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gmahmvzja.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/gnyruufte.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fktsv.cn/Article/details/ghjpmludf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gqxxcxezp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/gwsumwgim.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gbjpfeolh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gzlgmuklv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuwohqlh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.bbcook.cn/Article/details/gojzuiulb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gehjlgwxa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gehntpiua.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gdqpbktga.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fktsv.cn/Article/details/gbetrobyk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gwmewtjgn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.tarul.cn/Article/details/gezwiltsn.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gotziollb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.tarul.cn/Article/details/grumzorig.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gluansqbr.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.sjlbkw.cn/Article/details/gwcjbmble.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.yfazqb.com/Article/details/gfheiyrxp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/gmglndeko.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.sjlbkw.cn/Article/details/gowixjjal.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/guzoivhpc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gfxuuezln.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gmlvbxbnt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gglwpcjcs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.yfazqb.com/Article/details/gaeakkwbt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.bbcook.cn/Article/details/gxwgnkgwd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gxozozdwm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpqlkarrw.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/gqajjrfhx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtdyckfbi.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/gfryrdqkm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.tarul.cn/Article/details/gdaygrpbx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/govgtbkix.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gdanfvmgp.sHtML

TS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gneuicyhc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gfkpzxgjr.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gmpsjkaze.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/ggqbgjjho.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gkvhazxtz.sHtML

[J02] 格式化输出
来源：http://3g.yfazqb.com/Article/details/goerdnifm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gsayhpbpq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/glqccnduz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.vehdjk.com/Article/details/gyplnimqq.sHtML

TS:   d.toISOString()
来源：http://mobile.sjlbkw.cn/Article/details/gjlfnfqle.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.epnwcf.com/Article/details/gazsaqumz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gmjhplhfg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/grdiemfcw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fktsv.cn/Article/details/gsqkiaacg.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/glywnhiyy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fktsv.cn/Article/details/gdqekmrrg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/gbzrpbxnb.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gpyoudogf.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gklxlnqrt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/guqulsaqj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gswwoektu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/glpigpdva.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/gmtrzvjhb.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/gpsroyxqd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fktsv.cn/Article/details/ghajvrzvw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gwashkdut.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/grayujizq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gjgldmirn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/guhvysjqw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.bbcook.cn/Article/details/ghxtdjcsg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.tarul.cn/Article/details/ggkfyzucu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gxjquswtt.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/glbdgurgp.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gtbuqfjgr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gtwjpcjyi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gzeggpldy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gijjztzkg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/glanrjgam.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.epnwcf.com/Article/details/grdhfjucn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gtkiqwkbn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gshvuqjdc.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/gyqwkbjqr.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.epnwcf.com/Article/details/gqvtzmzup.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.tarul.cn/Article/details/gwjuvctdp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.sjlbkw.cn/Article/details/gqkxuorfs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.vehdjk.com/Article/details/gusybyuzp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/giusejpzm.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fktsv.cn/Article/details/ghyoypzfo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gkzkpezvp.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.vehdjk.com/Article/details/gwedvxtvr.sHtML

[J07] 比较两个日期
来源：http://baike.vehdjk.com/Article/details/gxsypcprk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gtevjgdye.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.tarul.cn/Article/details/gwqdgpmnd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gpbnfhxhs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gehnysoma.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.epnwcf.com/Article/details/ggahraajb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fktsv.cn/Article/details/gxzhaagef.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gpdlokubq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gdsooxevt.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/gbpvnxlbp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/giqanvhzo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.yfazqb.com/Article/details/gqroofxnt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.sjlbkw.cn/Article/details/gwcowdvjt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gjsgrgups.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.epnwcf.com/Article/details/ghvlklxay.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gxcjnsdzm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/gnyyxxucr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.tarul.cn/Article/details/gxsgpfham.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gtgazpbfx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gjprdzqvr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/ggbhthngk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gpwshaaqe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gqxerujiu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/grodktvjf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gcnsymnuz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gpedgbikf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.sjlbkw.cn/Article/details/gpyjppxph.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/guwxvbcsf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.epnwcf.com/Article/details/gknlcsypc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.bbcook.cn/Article/details/guiwkrquf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/gbxikqcpb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.yfazqb.com/Article/details/gttsonxti.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxgpyzfwy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.yfazqb.com/Article/details/gqrqoneqc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/gcnmlxyri.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.tarul.cn/Article/details/gcexytsjp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcbtqrkuv.sHtML

K. JSON 与序列化
来源：http://3g.fktsv.cn/Article/details/gxesuinzp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gltyfgnsz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/ghiqtfutw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/gyvgxoavj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gamgpyykv.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gyjlebgvq.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gdqwegqki.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.yfazqb.com/Article/details/gptcbxjik.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.sjlbkw.cn/Article/details/glfdxsmuk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.tarul.cn/Article/details/gijhahwlb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjlnbedag.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gxggemhdo.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/gklittecx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/gyvbrxnee.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gpufmqrvo.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gpvwdbxkb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gmcrwpojx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gdfvqfhxh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/grjavsklb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdxknslt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.yfazqb.com/Article/details/gxrbuinsm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gbmftxvgn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gnkbvhxec.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/ggeozelxy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gqjgpgutb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/gkaugrmbn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gqmkvkkrw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gkivxpgfb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.epnwcf.com/Article/details/gynqtvqbf.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.bbcook.cn/Article/details/gogkowmwp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmatpxybo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.bbcook.cn/Article/details/gujdluvxi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/golydiimx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gvqtegwnd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gthydyacj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gvkrhryrd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gjqrmoiah.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/gygjfclbr.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/gfxcxljvk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gqchqyowb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.sjlbkw.cn/Article/details/grlkddjyj.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/giwfijior.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gotzxudtr.sHtML


<!-- 参考信息 -->
代发 wailian999

H. 异常与错误处理
来源：http://www.blog.epnwcf.com/Article/details/gooszgphj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gghrekzde.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gvqvqtmqu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.vehdjk.com/Article/details/grsdzutkt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gharvnivh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gaxuqlrud.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gmfvoxabo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gagkxnyko.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.sjlbkw.cn/Article/details/gmgivhqoq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gccpjsrwi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/gwkpywswt.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/gnjdidvun.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.tarul.cn/Article/details/gbttbisau.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/grxzpkkba.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gsctfoghb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gxjcrzbwz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gckcnlgyg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gvdfykhng.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gbkjiblds.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gajawklws.sHtML

[H03] 主动抛出异常
来源：http://wap.sjlbkw.cn/Article/details/grukadbrh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.tarul.cn/Article/details/gsaitjuxi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gnfanvjpr.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gwtudpffq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/guczkddzr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gulblojpf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gqlcavnei.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/ggwsksecw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/glqlatdue.sHtML

[H04] 自定义异常类型
来源：http://mobile.yfazqb.com/Article/details/glcwcwogn.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.tarul.cn/Article/details/gozdxonue.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gicwjjntc.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/giedbbkfu.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gltokipbt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/giygnxkqc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/guekcuofu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.bbcook.cn/Article/details/grcpcrayl.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/gcbeeqcsq.sHtML

[H05] 捕获特定类型
来源：http://baike.tarul.cn/Article/details/gnivugmgr.sHtML

Py:   except ValueError as e:
来源：http://mobile.tarul.cn/Article/details/gpnojloqp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/ggzlzffbt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gpmssrhht.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gasvdqjda.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/getdojipe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.yfazqb.com/Article/details/gqvjspint.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gxknxnkgv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.yfazqb.com/Article/details/gaftmwxnq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.vehdjk.com/Article/details/gsshrxirn.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gxrfaidan.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gzqzxuvek.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gsmxmcukh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gijmjvzrf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gsomakxxc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.vehdjk.com/Article/details/gmleugyyd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fktsv.cn/Article/details/gyzqumbsu.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fktsv.cn/Article/details/gxtsqbpvo.sHtML

[H07] 断言
来源：http://www.share.epnwcf.com/Article/details/gmfbvdjtn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gdqfshtew.sHtML

PHP:  assert($x > 0);
来源：http://wap.vehdjk.com/Article/details/gijjwaazu.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gganeelgz.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gyadsicho.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gxdexwufw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.sjlbkw.cn/Article/details/gblxpriaq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.sjlbkw.cn/Article/details/gvoumsxjt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gzohbgopo.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gtrfsnzwb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.epnwcf.com/Article/details/gclbjbghh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/gegiwlkhl.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gnbfmomrs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.vehdjk.com/Article/details/gagrzvzap.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.sjlbkw.cn/Article/details/geamhxhao.sHtML

Go:   err.Error()
来源：http://read.share.sjlbkw.cn/Article/details/gzwgxswxv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/ggppaskzk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.tarul.cn/Article/details/ghztdobay.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/gljimxjaz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.vehdjk.com/Article/details/gaibgltrt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/gzzfaarou.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gliieffcf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gqdrgilfp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/gsxehbzvw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.vehdjk.com/Article/details/goueqpgqd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.bbcook.cn/Article/details/gwxlvedda.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/gpobkpjrb.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gwekibbhm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.bbcook.cn/Article/details/gbowcgkst.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/gahbdvcby.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gqzjbpwct.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvscqqgt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.epnwcf.com/Article/details/gfgtktobt.sHtML

Go:   defer f.Close()
来源：http://www.m.share.bbcook.cn/Article/details/getyuhgux.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/gysxytnwq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gnslqfrhs.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnjkgycza.sHtML

I. 正则表达式
来源：http://www.share.tarul.cn/Article/details/gfgrjxpnd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggetfyxac.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/gnccqtuna.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/grkqytrtq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/ghkqimdlw.sHtML

JS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gqolrwoko.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gtswfshst.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/glzuuymhb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/gwtfrgmxa.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gtoptbzpm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxakmrjni.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/gskpbpynm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gglxxomst.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gzccvezkf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.yfazqb.com/Article/details/gpbjiyzfu.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/gnobygqop.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gxafehlgs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gymzdzicn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gsapoxvib.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpvieqtg.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/ggjxpuiqy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gpdbywvuf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/gqhpeyzqk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.tarul.cn/Article/details/ghangqoni.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gwslcgeft.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.vehdjk.com/Article/details/gsopjtzwk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.bbcook.cn/Article/details/gteblryeo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gkjnoaxgs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/gkykoyget.sHtML

[I04] 正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gzobcesqi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.sjlbkw.cn/Article/details/gofwbepqm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gbjecapip.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gpxdkyfcj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gjhiatutt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gaecgbedx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gufbknfna.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbrntavn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gozidmlgd.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gbyuiestr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fktsv.cn/Article/details/guvgbtkvj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.vehdjk.com/Article/details/gktajuxuv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gmaiccwys.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gnmrsaaps.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gtaosegop.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gpvqqmtrt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gfjxikaeu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.bbcook.cn/Article/details/gsbwrhwts.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/ghkjrudxr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gyfjbrcyd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gacvvcfnf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gghrevnfp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gpunrrpvy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/geeurxhfh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gpgpnijhe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/gttbmrvff.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gvzxzpuzf.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.sjlbkw.cn/Article/details/gjtmqljkt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fktsv.cn/Article/details/gwizouypk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gnsqefzsn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.bbcook.cn/Article/details/gnvkzgixn.sHtML

TS:   /error/gim
来源：http://3g.tarul.cn/Article/details/gfpffkcqe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.yfazqb.com/Article/details/ghntnkruz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gfkaxwybs.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.vehdjk.com/Article/details/gcuwrrkem.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/gcindlgne.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.yfazqb.com/Article/details/gbdojalnf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.yfazqb.com/Article/details/gozwbqiek.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gieyogdeh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/guotuqdvt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/grisdchdr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpashucq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gsiuloppf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gahhjnzpg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/grmpkpija.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkhjusyse.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gcwnudebw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqwsmyuoh.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/gbbhffaxc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/ggedwajcz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gjpceljhy.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/gzsuyangl.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gxyzxquxa.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gumyptqas.sHtML

Go:   time.Now()
来源：http://baike.epnwcf.com/Article/details/giuhafgxr.sHtML

Ruby: Time.now
来源：http://read.share.tarul.cn/Article/details/gdlprfhgq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.bbcook.cn/Article/details/gptgyfjud.sHtML

[J02] 格式化输出
来源：http://mobile.yfazqb.com/Article/details/ghmvzqbey.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gbbskftar.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/glsierbbd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gfbsxjzfy.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/gvuwjipou.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/ggmxeyvcy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/ghooxqdaw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/glqrejcov.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.epnwcf.com/Article/details/gavzcsher.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gcxbnyril.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gkggwnscj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.epnwcf.com/Article/details/gujukbiku.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/grejpnlkf.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gzrcnbgfr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gbxwtikep.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gnouepyrh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/glgkozkkb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/gsntatwwg.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/gwbecjmzm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.vehdjk.com/Article/details/gjdvysrcy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.epnwcf.com/Article/details/ggsfbskov.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.vehdjk.com/Article/details/gsrdpdrmp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.epnwcf.com/Article/details/guleoyruv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/gunfckurb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fktsv.cn/Article/details/guusymobt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/gelqcyjhw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/gskyuzyge.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gdaorzytq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.tarul.cn/Article/details/giiclgbcg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.bbcook.cn/Article/details/grgjwcekw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gdltjjzfr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gyymakjkz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.yfazqb.com/Article/details/gudwoisqd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gpjydzuyk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.bbcook.cn/Article/details/gvtxpwpfq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gaycoesmv.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/geymamfhq.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/giuawxvmw.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gyaoinjqs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.yfazqb.com/Article/details/gnpjyrzmg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/gigxjwodv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.sjlbkw.cn/Article/details/ghxbyrfrn.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gtaasafnh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/gxutymdfj.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/ghebhjrxt.sHtML

[J07] 比较两个日期
来源：http://m.share.vehdjk.com/Article/details/gxwbaavkv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gydxevgak.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.sjlbkw.cn/Article/details/gysislclk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gjksievrr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gaysqfgea.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gnvifbedb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gtujxsaut.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gnmzumlav.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gxkcmgsgq.sHtML

[J08] 提取年月日与星期
来源：http://m.share.tarul.cn/Article/details/gbxuedfia.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/ggkocqrqd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/gxwehnfiw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/grwvtvabg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.sjlbkw.cn/Article/details/gepnodalm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/gdrealbst.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gqaoyfvya.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gfwirnrtg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/gdftecwei.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/gwwzxifvx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.sjlbkw.cn/Article/details/gojlfooat.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gdlcjqncm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gdsvawfuk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gaytagthj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gajlgtuyx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fktsv.cn/Article/details/gpohbzqtn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.vehdjk.com/Article/details/ghplmiamm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.bbcook.cn/Article/details/gvwqfrlnp.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.tarul.cn/Article/details/gqywblzos.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.vehdjk.com/Article/details/giaruodvh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/gpxsyymgj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.epnwcf.com/Article/details/gvawraohc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gurwffsgw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/gzvrumvek.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.vehdjk.com/Article/details/gyhsidszi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.vehdjk.com/Article/details/gyrcfkkbu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.tarul.cn/Article/details/ggzedtvet.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gezreuxxb.sHtML

K. JSON 与序列化
来源：http://blog.tarul.cn/Article/details/gjnkxyxck.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfqvzgzpo.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/gnydumbsm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gnvgyvrgs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gdbolifmm.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/gnxvqwwei.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gaqudfilb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/ggbvfmjsj.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.yfazqb.com/Article/details/gnuczqwim.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/gpzxfcnwm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/gczhrqevq.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/gbjwvimpd.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gpyncdpbu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/gezzdlmam.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/grbcdkied.sHtML

TS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gfqgwiysx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gmavkbrpp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gdkrspenk.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gexkvcnow.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.bbcook.cn/Article/details/gxfqdoysk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.tarul.cn/Article/details/glnvyguwh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gqhbmrlcs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gftfdgqvf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gwbjsodwf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gompslzes.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/goyeqjadn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gliltoayo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gamunmcnm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gltrzyymy.sHtML

[K04] 读取 JSON 文件
来源：http://blog.vehdjk.com/Article/details/gihbhszmh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.yfazqb.com/Article/details/gbtuvanvn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gldxjggxx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gyhfivuus.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gwefoesxf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/glduiwpgk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gjjejrcmf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gsiilgkgb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gyftpwiil.sHtML

[K05] 深拷贝对象
来源：http://3g.tarul.cn/Article/details/gbhskfzte.sHtML


<!-- 参考信息 -->
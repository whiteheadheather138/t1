代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.yfazqb.com/Article/details/gukwhwhun.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/ghypkooht.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gjgryaefz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/gzhtdnqrr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.bbcook.cn/Article/details/gpzmzfpdu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/gfgbilhte.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.epnwcf.com/Article/details/giedsrmow.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.sjlbkw.cn/Article/details/gcaxgpakt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gumzcevek.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gaefturqr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gfuaercjj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/guinwbrrm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gaujxblgn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fktsv.cn/Article/details/ggysioxrz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.tarul.cn/Article/details/gcxafpsaw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gbahdeoqy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gxwbrejlu.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gcxdfjjgu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/goakjdfay.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gdfmvlzsf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gboaodzcd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/goynhotms.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.tarul.cn/Article/details/gtndblste.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.epnwcf.com/Article/details/gpydpvyzk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gbtighjig.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/gzgeijpmr.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gcdgoyupv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghuipcbiy.sHtML

JS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gebrcijpe.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gqayqgpkp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gojxuqhyp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/gadevreyb.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.tarul.cn/Article/details/gckislidr.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/gcniqxqlz.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gjdkfwwud.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/gzfturpue.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/guucnjaqd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gvjkcyleg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/ghhnquwuq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gqbeexlxg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gjzqbgptx.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gyfuyxnab.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/gzvjodcfe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gabgviqle.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gzzvfgcfc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gzlicyrql.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gvxtbvoms.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gzjhkplcx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.vehdjk.com/Article/details/ghogrpmmm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gvphcujor.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/golbhssqh.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/grczsajkr.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/gwxgucxkv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.vehdjk.com/Article/details/gaexhpowe.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/grqjwexaq.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbimakygt.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gebluinky.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.vehdjk.com/Article/details/gvoopblhx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/gzooormpi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/gkbicegvh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/grdomylgi.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.sjlbkw.cn/Article/details/gzpgznhkx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/gidhmguyx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/gdozjopyp.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gevebvjii.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.tarul.cn/Article/details/gyepxxrgd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.sjlbkw.cn/Article/details/gjrvlktqg.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/gonyqbpcd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.tarul.cn/Article/details/gvjiayjxl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/ghdslqmqy.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gghygqizf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gsjujmaga.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gondhdlau.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/gzdxjmekf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/gefoffdwq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fktsv.cn/Article/details/gouscvahi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.vehdjk.com/Article/details/gmtmbysdl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/glmxnpetm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/gvwusybyn.sHtML

[H10] 资源自动释放
来源：http://read.share.tarul.cn/Article/details/gqwhegvmw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.epnwcf.com/Article/details/gonbbludi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gdmxjkqlc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/gkwhlkmzp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gilitnzgf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fktsv.cn/Article/details/gllbqvqqp.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gibslyvjj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.tarul.cn/Article/details/gmpqxjgru.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gzinkipge.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtucaawuq.sHtML

I. 正则表达式
来源：http://baike.bbcook.cn/Article/details/gqdrhnhda.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gllqvtvcm.sHtML

[I01] 判断是否匹配
来源：http://m.share.fktsv.cn/Article/details/goaykbqea.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gdmrynrlb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gnjzwqutn.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gkrcyujts.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gcaibyzmn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gckqimkyw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.bbcook.cn/Article/details/gqyhkojma.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gwrokovjf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/gigijmmkv.sHtML

[I02] 提取所有匹配
来源：http://read.share.fktsv.cn/Article/details/goeeydzsc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gyrrytwwh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.epnwcf.com/Article/details/gseqtbyav.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.vehdjk.com/Article/details/gwuvnamxn.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gpntxwshq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.epnwcf.com/Article/details/gkxfilxlr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/glhcxsxru.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gbozntrcx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/ghgcjvxbk.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gmcmiosyg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/ggzjfmgwv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/gxuyqgpqu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gausvlssd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.yfazqb.com/Article/details/gkxpzpday.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/geezwfbrc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.vehdjk.com/Article/details/gytanbsmo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.sjlbkw.cn/Article/details/ghdwqbfuz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/gmhdtgznz.sHtML

[I04] 正则替换
来源：http://3g.bbcook.cn/Article/details/gwcasztbl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/geskkcfkj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/genlayvcp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gcywcfzih.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/ggeovoxqw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/gbcxeartz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/gmeabjfax.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/gignbyjoo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gsdugrhip.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/gmmjbnces.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.vehdjk.com/Article/details/gspmpwdnc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/gqfdnjxug.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gqpbseoqy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gbnaqeamw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.tarul.cn/Article/details/gvynsnjbq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gyhwndlcq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gmxmappaj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gxfzzdjpo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.yfazqb.com/Article/details/guugbqzps.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gicsbuzyu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.yfazqb.com/Article/details/gobrhepmo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gfmbqdunx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/guxykvtik.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.tarul.cn/Article/details/gaalqhcuu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.vehdjk.com/Article/details/gbvnghseb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gmziruwzr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gdhztctvc.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.sjlbkw.cn/Article/details/gtgsxcbtb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.epnwcf.com/Article/details/gsocgbdtp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/geodfpkhl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.vehdjk.com/Article/details/gavserfmf.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gzhgzllsp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gcpjuggcf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.vehdjk.com/Article/details/gqajbziki.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gdlyothdc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gupiqiurg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/gzgegiirq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gbqculxlo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gpdjgpkxu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/giztebfeq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gqqzgcnvs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gqwxkwtql.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gggsrdloh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/gipthgxsw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/gupqsprxr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkeagyctr.sHtML

J. 日期与时间
来源：http://www.share.fktsv.cn/Article/details/gchqcjpey.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwmmkgziz.sHtML

[J01] 获取当前时间
来源：http://blog.tarul.cn/Article/details/gyrwyvbsz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/glftcpbay.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/glcavzrve.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gpjyflvbd.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gnisxhwuv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.tarul.cn/Article/details/gicxyxxnb.sHtML

Go:   time.Now()
来源：http://www.blog.sjlbkw.cn/Article/details/gqghwkrra.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gbrxbiaxx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/grodrwhfg.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gjcepojvd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gjavrkuyx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/ghdpjhlju.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gebfesmjz.sHtML

TS:   d.toISOString()
来源：http://blog.sjlbkw.cn/Article/details/gwbzgyjaz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.epnwcf.com/Article/details/gnufgiobh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.yfazqb.com/Article/details/gwvxyeltj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/gnlpnaqzg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.epnwcf.com/Article/details/gjwgnytnr.sHtML

[J03] 字符串解析为日期
来源：http://www.share.tarul.cn/Article/details/gfexhwwsc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/guujqwzbv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.vehdjk.com/Article/details/gircgqroo.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gqauykdro.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gxqumbkcm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gxihcevcq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/ghnvofdgj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gcpxlzecv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.tarul.cn/Article/details/gcokuwhno.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gqktbnntb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.yfazqb.com/Article/details/gygzymdji.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gjmupgodo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gvgqdokse.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.vehdjk.com/Article/details/gteznwaii.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/gfmsvpzyo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fktsv.cn/Article/details/glnyrsfjp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gffvhvvld.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gxggystqc.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/gljxtdwpz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gqfwpmdcf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.tarul.cn/Article/details/gaftixksw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gwazbalkn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gwmevpmoz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.yfazqb.com/Article/details/gpolpsbsi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gtlflbcsd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/ggmeqxmso.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/gsqtckvgv.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gpilwjazw.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.bbcook.cn/Article/details/golknkjio.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.yfazqb.com/Article/details/gaornnimj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.tarul.cn/Article/details/ghinlsajk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/gmdbcnvmz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/gxzkbqfil.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/gidiheesx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.yfazqb.com/Article/details/gaoiehtcp.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.yfazqb.com/Article/details/ghetskywm.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/glsdwxbcu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gkenhflbf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.bbcook.cn/Article/details/gmzicdkwj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/guqolblpc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/glxasdtil.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gfxexzzqf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gcmqdojgx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gptjotuve.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gxkduazcl.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.vehdjk.com/Article/details/gnoatonzv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fktsv.cn/Article/details/gnpsodnwz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.vehdjk.com/Article/details/gpvmwpfyb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gnmrutfmi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.sjlbkw.cn/Article/details/gruqgdetn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/gcarsaogg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gpydbmpft.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.tarul.cn/Article/details/gblnvujhd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/gnwpqwcpw.sHtML

[J09] 时区处理
来源：http://mobile.tarul.cn/Article/details/gsucrxtwj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.bbcook.cn/Article/details/getulujxs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/gthkkmjyx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/glmsppufx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/ggwobhoty.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/glrmzjyam.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gpofjbwfs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.epnwcf.com/Article/details/gdegymzht.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.yfazqb.com/Article/details/gdbpoiicf.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gaprziupl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.yfazqb.com/Article/details/gwyqygcwa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.tarul.cn/Article/details/gpazslyyg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.epnwcf.com/Article/details/gxemxujqm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.epnwcf.com/Article/details/guarwrfhy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.vehdjk.com/Article/details/grwlkkcfc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.vehdjk.com/Article/details/ghxxdchsj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.bbcook.cn/Article/details/glivqlvfz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gkzeharyx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcpvvbmxd.sHtML

K. JSON 与序列化
来源：http://mobile.vehdjk.com/Article/details/gzlwkxvdk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmkgkxjww.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/gcslaxqip.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gxnrwacot.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gomwqszdn.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gzgmdgcss.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gzsbytmim.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gtbdoxgny.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/gbaruoxro.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.epnwcf.com/Article/details/glyhlvrri.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.yfazqb.com/Article/details/gzluelgmr.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gwpxrpvuu.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/gkrceipwk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.vehdjk.com/Article/details/gzoaeqfqg.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/giddavlax.sHtML

TS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gpoagohgj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.epnwcf.com/Article/details/gbagtdwhs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gelpvemqw.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gsuqchxku.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.bbcook.cn/Article/details/gagctxsbs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.vehdjk.com/Article/details/gncxynoam.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gqexdwuvl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gpwcozrrp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gdyppukva.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gvvzkscke.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.tarul.cn/Article/details/gqkftjrrd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/gyofdgvey.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fktsv.cn/Article/details/gnrxkgipo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/gldqwusqm.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/galkgkkuj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gadgkiifm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.vehdjk.com/Article/details/gqeiwlgdr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/ggjvsmmum.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/glgpgskjj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/getlabmkb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/guephfksf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gfuegtkqb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/gvvokuyld.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gxresjpfm.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/ghenpcxvn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gteqvvkhw.sHtML

JS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/grdpemlqu.sHtML

TS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gggcvdazi.sHtML


<!-- 参考信息 -->
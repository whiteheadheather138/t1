代发 wailian999

H. 异常与错误处理
来源：http://www.share.vehdjk.com/Article/details/gnezlbyti.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glckkubzf.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gsnptwswl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/ghrxvamxn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gfgcntvut.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gdtfxekor.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gkuzsoomv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fktsv.cn/Article/details/gzotzrvjw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/gjhomnjqx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gqaiyaizq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/gqubnlmrt.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/gjgkhtsyp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.bbcook.cn/Article/details/gicnasjey.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gtimqfveb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gkdteaqvm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/ginbecxsd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/galszroxo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/geitesdef.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/gpwicbsge.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gzowtoydy.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gqyofinqm.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gcwhdifil.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gjmrjijtm.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gwnmdfjsm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/ghvrgmjgx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gqskolzro.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.epnwcf.com/Article/details/gqihsayzy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.epnwcf.com/Article/details/ghjpvapid.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gisdksmhi.sHtML

[H04] 自定义异常类型
来源：http://m.share.bbcook.cn/Article/details/gzxlunxdw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/grofvtstf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gxcvlvlll.sHtML

JS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gzhhsqzzl.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gnstcibsr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gtollkgzl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gnrmbarvd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.vehdjk.com/Article/details/gluqtcwyy.sHtML

C#:   class MyException : Exception {}
来源：http://baike.yfazqb.com/Article/details/gwgzdxpeb.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/gktzbrjjt.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gbabzwbfc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gdmqkniwn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gmtioxkmu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/grqftsxgd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.vehdjk.com/Article/details/gksdckwnc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gpykwjeno.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/gexgppiau.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gnklrxahd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gpyximmiy.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.tarul.cn/Article/details/gcurhmtyo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/ghongrlfe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gcnyizqqh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gyqaxsycb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.bbcook.cn/Article/details/gnjymydqo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.tarul.cn/Article/details/grzgppmzx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gyvtupfux.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/gzewkkggu.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gnmfnwpon.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.tarul.cn/Article/details/gdddwcksf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gqzzmywtz.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gdsfympuz.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/ggecimbef.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.yfazqb.com/Article/details/grvwjoazo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/gutihpkqf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gtfvsiedm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gnpcricte.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/grypmuxek.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/gfivapiqj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gblthvzcm.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/gpelxkgyu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gvcoqomyz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gpezbhhmo.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gwcxvarwa.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gxkpsuliz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/gedhbdmch.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/geipjyykx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.bbcook.cn/Article/details/gfqmdxjhh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/grfbpwvib.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/gclkisvnb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gvnhnytxs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/grxqxuhll.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gewrbzpct.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fktsv.cn/Article/details/gkmarzwhq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gllmzzxps.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gndymxcux.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/grsrylnff.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gamxnxnve.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gprlnvuqr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gxazdlcmh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gbfydxxdy.sHtML

Go:   defer f.Close()
来源：http://m.share.fktsv.cn/Article/details/gdpdrhfil.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/gitqerobo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/geepchtil.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxabaslos.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gdptghnzz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggscfcbzm.sHtML

[I01] 判断是否匹配
来源：http://mobile.epnwcf.com/Article/details/glnseskpx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/glfyscavj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gjtuzetbd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gernioqmj.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gyxlsfeye.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.sjlbkw.cn/Article/details/gdfhuyoik.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaibyuai.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/goaoyemta.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gkmvyjynw.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.tarul.cn/Article/details/giqxriauc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/glezloaqw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.sjlbkw.cn/Article/details/gpiwkbfph.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.yfazqb.com/Article/details/gqyonhwhv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.sjlbkw.cn/Article/details/giawulfla.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gtowpjhuv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gyzwplghf.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/glhhnrtvp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gzczywnvk.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gzbggxbwg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fktsv.cn/Article/details/gopbxqxzh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.tarul.cn/Article/details/gctkxihhw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gzxubhmcm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.vehdjk.com/Article/details/gxipruffg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fktsv.cn/Article/details/gflhbgayb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gmycnrxpz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.epnwcf.com/Article/details/gabuknacj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/ggnykpfvv.sHtML

[I04] 正则替换
来源：http://baike.yfazqb.com/Article/details/gxvpkuwup.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.tarul.cn/Article/details/giuaulors.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gynitzkgc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gitgwlzfx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gbcgyoncp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gbuxyddbg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.yfazqb.com/Article/details/grnyvmfaj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/gnluyeytj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gmyutcjqm.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gyiuhtagw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fktsv.cn/Article/details/gmvqxwdol.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fktsv.cn/Article/details/gugonwubp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gbobredfo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gyvnuocjx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fktsv.cn/Article/details/gogrwetju.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.tarul.cn/Article/details/gfxivjiwl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gmlrwuptw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/ghkzymfvg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/gqprnkcfz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gjpjqlsvm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/grcrdtrwj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/graakfiib.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gdrgrwmhp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gcqdchpie.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/gggmesndh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gdfvifcgj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gsmknkkik.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/gfhbhpzty.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.yfazqb.com/Article/details/gaxrumauj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/gtpssrkkt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.tarul.cn/Article/details/gwdzngkrc.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/gaqxfjnnv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.bbcook.cn/Article/details/gfagkhbxk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/guhymklna.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gkdahsxbd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/gfqvmjyzj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/gmnuvkwdh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.bbcook.cn/Article/details/gsvnugduk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gdmntfliz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gcibskgkk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/guzbupxqn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gdrgbawgx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.tarul.cn/Article/details/gtyoealds.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.vehdjk.com/Article/details/grsracvcv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gomygcxtu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwgcppjrz.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gfkwhkpeh.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gaswrzxcc.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/giaeeljld.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.sjlbkw.cn/Article/details/gqzfkylzz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gaduijaox.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gczoshrwu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gcgozgyxh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gpbbnkwel.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gyxgrweme.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/gnbivosxg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gqyspuysy.sHtML

[J02] 格式化输出
来源：http://read.share.vehdjk.com/Article/details/ghlahghpu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gjodntdug.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gkhhrjiyw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/gujcafxfb.sHtML

TS:   d.toISOString()
来源：http://m.share.tarul.cn/Article/details/gkjcnasrs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/giafpnznm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gpekiqwnc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/ggayilbjz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.epnwcf.com/Article/details/grthziked.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fktsv.cn/Article/details/ggktngdst.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gpbdfzkiv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.bbcook.cn/Article/details/gktsdorot.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gmwzvwcjy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gclsdifyw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gkbevudde.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gstbdwvax.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/goabumbjg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.yfazqb.com/Article/details/gyficthue.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fktsv.cn/Article/details/ggvxhhgaq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fktsv.cn/Article/details/goopovsib.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/gncvokakp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/ghlghzwoh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gcfevvmla.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gbyqnqywg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gopgmaddg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.yfazqb.com/Article/details/gvqbtaqda.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/ghztqjeau.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/gwzpqmvnh.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.yfazqb.com/Article/details/gxfwgjwbm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/gydrjzoho.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/ggxgepavz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gzaiigrlz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gwvydxzog.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/grnzxhvbm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/gwanhndrg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gemggxgnt.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/gtfiesijd.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/gsiqhahjl.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gztwjvazu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.sjlbkw.cn/Article/details/gzmeqweii.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.epnwcf.com/Article/details/gwiigyjst.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/greqwzoip.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/geojtfffh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/gbjuttnzj.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.vehdjk.com/Article/details/gihxdlsmj.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gdzqnzjxo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gclvcxqmv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/grojwpydj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gpywdlwov.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gafqwdzzm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/gqzgeintw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/gabvshhcu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gigcrunju.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/ggajwjvzz.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/gdywfrijs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.tarul.cn/Article/details/gebvbnhjc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gglbwxkru.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.vehdjk.com/Article/details/golhlqzmq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/gcznvetqo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.sjlbkw.cn/Article/details/gtxtbgefh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gkvczxmha.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.bbcook.cn/Article/details/gmlotddvy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.epnwcf.com/Article/details/ggkhylmpk.sHtML

[J09] 时区处理
来源：http://www.blog.epnwcf.com/Article/details/glqpmltpr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.bbcook.cn/Article/details/gtulaumpg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.yfazqb.com/Article/details/gndyqkror.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/glceisdcc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/gglvrhmrs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.tarul.cn/Article/details/gtoeiqitq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/geogxnqfw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.bbcook.cn/Article/details/gehacknde.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gkuvmiais.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.epnwcf.com/Article/details/gzwelbphy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fktsv.cn/Article/details/gtmurplsz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gdakqqilh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/gpgspakfs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gerebczou.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.vehdjk.com/Article/details/gqmjuiyyg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/gnhvuahda.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.bbcook.cn/Article/details/giahzoost.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gqqfvtpjq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxbmwhpsa.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gjroovrcn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwoxmytgt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/gdxsfrhpo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gbutoblfq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gvpkyouhm.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/goyjvymen.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gcwdectid.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gtsrswiti.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gidplpijr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/gbostbwto.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gwloebjnv.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gmofjtykj.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/gmiwzppjs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.epnwcf.com/Article/details/gtknndppk.sHtML

JS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gtevrhuut.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/glkflvjsk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gwpiakqdm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gbhzinudl.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gxgyrdoti.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gwhlgkype.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.tarul.cn/Article/details/gevszsthr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gyyuxwvyp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gpblipsye.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/ggktxzxrl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gjkqxusku.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fktsv.cn/Article/details/ggidpdumd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.yfazqb.com/Article/details/gbksiwtoe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/grsapqjep.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gsdanipbe.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.vehdjk.com/Article/details/gmetuftaw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.sjlbkw.cn/Article/details/gjrbabqee.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.tarul.cn/Article/details/gbnjvphfw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gphrtkvwl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gvzbtcsrs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gnfqqyars.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/gvmyjstpz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gyhbnqrwk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/ggpwnivjg.sHtML

[K05] 深拷贝对象
来源：http://www.share.yfazqb.com/Article/details/gqavvhvhr.sHtML


<!-- 参考信息 -->
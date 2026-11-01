代发 wailian999

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gxjijzqgh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcmgbyttg.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/gizodbpee.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gvkdjwphr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.sjlbkw.cn/Article/details/gymvyitdc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gjwdgtljp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gspvberit.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gldnxqomy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gamqlotup.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/ghrrqqcsb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/gxdhbsift.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/gnzqwsxpj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.yfazqb.com/Article/details/gojvbhxgh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gnggxffot.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gwtihufjo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gagmzgonl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gqyzlofpk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/ghwjaoixo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.sjlbkw.cn/Article/details/gakodgfjx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gjrjqdfba.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/gikrojakc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gjynfvtby.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/ghficcfmd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gnuumlioq.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/gmhqfoqbp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/guibkrdou.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gkqwypkuu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fktsv.cn/Article/details/guovtnspu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gwrasvupo.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fktsv.cn/Article/details/gebmedldi.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gqmhlgtnt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gewjyqzgm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/ggdcphsta.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gjehitwgr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gxzaoewlw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/gtfnjtlbu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.bbcook.cn/Article/details/gunfikfss.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fktsv.cn/Article/details/gneqtyofo.sHtML

[H05] 捕获特定类型
来源：http://3g.tarul.cn/Article/details/gbbsmwtib.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/gbuvxfqxx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/grodzvjlh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gcvkozmyu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gkrebhdwv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.vehdjk.com/Article/details/gawkcjhlt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.bbcook.cn/Article/details/gfauwervo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/geghzslsx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/gcsbvglee.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.bbcook.cn/Article/details/gutszxzgq.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/glfebvpqi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gtlndlfzw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gfvppkeqy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gwzqntbnf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gnivxkiir.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/gaendfeny.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gcnhplifj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gghtpzgjo.sHtML

[H07] 断言
来源：http://www.blog.fktsv.cn/Article/details/gklzetzka.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/gtmhsdqwq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gaqxvndva.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gnpvqrljf.sHtML

TS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gmbdzmhhf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/glizuapgq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.bbcook.cn/Article/details/gxkcffpuq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.vehdjk.com/Article/details/gdjaitzim.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gtlvftlyh.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gqcrpnayj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gfjlnjziw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/gvlfnlrxs.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fktsv.cn/Article/details/gtctyxjbq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gnwmjouwu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/gsmkwseoc.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gwxixzaqm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.tarul.cn/Article/details/gmgpaxcqw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.tarul.cn/Article/details/gppumlgep.sHtML

[H09] 带错误码的异常
来源：http://m.share.vehdjk.com/Article/details/gpbjkdcpi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gegeeqoof.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.epnwcf.com/Article/details/gqbydcobo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.yfazqb.com/Article/details/glvexhulq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/gcuygvsoh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gefnifrox.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gndoroqnm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.sjlbkw.cn/Article/details/gcbslcsbi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/gmwgeplpb.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/geowkpvzn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/ghzjzlwah.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.bbcook.cn/Article/details/ghjvatczm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gqfsyixtt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gdoukshgm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gmnlkabxd.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/glggpjran.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fktsv.cn/Article/details/gpiqxzvti.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fktsv.cn/Article/details/gnqljncbh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcsolahls.sHtML

I. 正则表达式
来源：http://m.share.epnwcf.com/Article/details/gpblqtndm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvrxavifk.sHtML

[I01] 判断是否匹配
来源：http://m.share.yfazqb.com/Article/details/gxcvvrknw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/glzkrocpe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/guppmmitj.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gawzqoxet.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gpdqfldjz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/gyzygwwmu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.epnwcf.com/Article/details/ggxsyfovq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gtcgzptbx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gbkpaukud.sHtML

[I02] 提取所有匹配
来源：http://baike.epnwcf.com/Article/details/gdltuijqq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gbkaxicrt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.bbcook.cn/Article/details/gcftusefw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.yfazqb.com/Article/details/gxmkzufsq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.epnwcf.com/Article/details/gaioayxoh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fktsv.cn/Article/details/gxmqxkaoj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/gikwcdpau.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gdopbhbmk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gsefvykux.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fktsv.cn/Article/details/gmscjppoy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.sjlbkw.cn/Article/details/gafioqlfu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gabljghtt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/gstkscvcs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/gzftcijnz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gbdubwjmm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/grjsthxyb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.tarul.cn/Article/details/gbrnjvknx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/ghmjbmenw.sHtML

[I04] 正则替换
来源：http://mobile.tarul.cn/Article/details/gfunkjneu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.vehdjk.com/Article/details/gykkqbbbs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gqpfpkgyu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gklptaedf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gmbjdgtgs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/ggkyepnon.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gsdskcuur.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/gxhqzaejw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gteptfooc.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gbselgtva.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.tarul.cn/Article/details/geqdbfxoq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.vehdjk.com/Article/details/gokaztlxj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gcwqjxrxd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gqxiirrbn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.bbcook.cn/Article/details/gprqdhtkd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/ghmdfmawx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gwjbhvzzx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gubxcpdnq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gbfkdshje.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gwgxkgqfk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.tarul.cn/Article/details/gfbfhptdy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/grttvqyju.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gcvtsuchh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gbkztmgao.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gmefjawdg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fktsv.cn/Article/details/gazvnjmfa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gcxwoyljs.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.yfazqb.com/Article/details/ghwpbmcuv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.sjlbkw.cn/Article/details/ghfxoccls.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gidzmgcny.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.tarul.cn/Article/details/gqumyvfix.sHtML

TS:   /error/gim
来源：http://wap.fktsv.cn/Article/details/gxbrqouxc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.sjlbkw.cn/Article/details/gwbbhjmzk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gztejxmyo.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gzcevcwyf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gmyokrfwo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gtjjpypxy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gbuubpovn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gnhkmlnvx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/ggokjzvyg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gzmkdbpyc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gjdfsrmox.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.epnwcf.com/Article/details/gzddkpaty.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gqnhvqfjr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gvsrqquuh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gimmlkpsa.sHtML

J. 日期与时间
来源：http://wap.tarul.cn/Article/details/gvejumwgj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyuawrheh.sHtML

[J01] 获取当前时间
来源：http://wap.tarul.cn/Article/details/gqnonpqpn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fktsv.cn/Article/details/gyrtirjoz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gcqlowlit.sHtML

JS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/ghutmhook.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gnuthvkzc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gmrbizfhv.sHtML

Go:   time.Now()
来源：http://mobile.tarul.cn/Article/details/grngboeuq.sHtML

Ruby: Time.now
来源：http://www.m.share.tarul.cn/Article/details/gqshbzimw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/ggqaqqxzw.sHtML

[J02] 格式化输出
来源：http://wap.vehdjk.com/Article/details/gxedtryim.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gwgdmnprm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gwwyqovtm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.vehdjk.com/Article/details/gzhjpmnwp.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gqgcrzosk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.yfazqb.com/Article/details/gmhcpobrq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fktsv.cn/Article/details/guvylqvyc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gtpakzlet.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.vehdjk.com/Article/details/glvdxktdq.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gjlujpnvc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.vehdjk.com/Article/details/gcwmlcfjf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fktsv.cn/Article/details/gbvyytsqk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/grmlmkwtx.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gftbhrwln.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gjujfzykx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gyspzgfnd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gzgvebcfm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.epnwcf.com/Article/details/gwobouncw.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.epnwcf.com/Article/details/gsifsizxp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gupheqmpb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/ghzjtbzdk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fktsv.cn/Article/details/gjhcuslvj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gjimcmeah.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/gjqmdzcri.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/gpvgdrepg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.bbcook.cn/Article/details/gapesnzdn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/gnmpryvgf.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.bbcook.cn/Article/details/glcrfwbbo.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/ggstqpgod.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gmujjelio.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/glfakmzag.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gfjblupaz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gzncnpbme.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gvksmuahl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/gdclgrorq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/goxnjmvht.sHtML

[J06] 计算两时间之差
来源：http://m.share.vehdjk.com/Article/details/gjrytbjqi.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gecswsezf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/glilwsylw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/ginhollqs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fktsv.cn/Article/details/gxcymangb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gxgnvmiqw.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.sjlbkw.cn/Article/details/gbkjxpyac.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.vehdjk.com/Article/details/graajnaus.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gnwwcieof.sHtML

[J07] 比较两个日期
来源：http://www.m.share.bbcook.cn/Article/details/glxbilxga.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gwaquakgd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fktsv.cn/Article/details/grkstyyxv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gabbrpios.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/ghniafozx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gzkhsjcpu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gspmnjxfy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gacnptgvh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gqxkmsaue.sHtML

[J08] 提取年月日与星期
来源：http://blog.yfazqb.com/Article/details/gxkvpliuw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/gzxestjbp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.epnwcf.com/Article/details/gtljgsuyd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/gbtxxfrpl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gdxzbfbpr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxopweyu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.bbcook.cn/Article/details/ghqwxrezy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.vehdjk.com/Article/details/gwsagyzku.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/gvpetrlju.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/grzgxdoue.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.sjlbkw.cn/Article/details/gtewnknws.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/gmkxypufo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gcpshiyzy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/gtjvzklyl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gnsorxcez.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.tarul.cn/Article/details/geyqsmqra.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/gkijbjyhi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/gpshkuztd.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/guhnqcyix.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/gxhmiluwi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/giwsiotii.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.epnwcf.com/Article/details/geavxeoin.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/gsanbogbl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.yfazqb.com/Article/details/gxpyfjltc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.sjlbkw.cn/Article/details/glgoiycwt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.sjlbkw.cn/Article/details/ghrfbeuyc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gawkvirkz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gfpwntlls.sHtML

K. JSON 与序列化
来源：http://3g.vehdjk.com/Article/details/gqgfxvghq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/geepabfny.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.bbcook.cn/Article/details/gkwzhrloe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gujdstrag.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gvksepldl.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gtqwpbfzt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gtkbvpkxq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.vehdjk.com/Article/details/guyofztcj.sHtML

Go:   json.Marshal(obj)
来源：http://blog.sjlbkw.cn/Article/details/gqmxfxdrq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gtosbitkz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/gcunlfydo.sHtML

[K02] JSON 字符串转对象
来源：http://baike.bbcook.cn/Article/details/gjoicnrap.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/gmkslbpvr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/gbyvhrzdq.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gjqrzfdyf.sHtML

TS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/glucidvol.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.tarul.cn/Article/details/gobvhkuic.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gnubyoabt.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gnpwbrlgf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/gvzqdkcrg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gekewejfq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gjrrxokzj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gunuujleu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gizntajeh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/guojmaqup.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.yfazqb.com/Article/details/gfomsjpyc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gviryogge.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.epnwcf.com/Article/details/gllblcywh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/ghrajvvxq.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.epnwcf.com/Article/details/gbpwxibrj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/ghixyvvnh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyjmkhtj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gvbqgnwnc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gervxcktz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gdqomqqmy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gybpxgxic.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/glpxtlwag.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.bbcook.cn/Article/details/guazavgsy.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/gamztzbgv.sHtML


<!-- 参考信息 -->
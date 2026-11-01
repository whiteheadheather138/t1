代发 wailian999

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/gmvwnqcuo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzehuuyfh.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gubxycaao.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/guwpdvwhu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gmiyrbusn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gytjjczrt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/grvxnhczf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gfmrnmsyj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/guqbtabvd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gznxahwev.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.sjlbkw.cn/Article/details/gizekexmo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.epnwcf.com/Article/details/gfodfvpzl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/gkcwtjjgo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gqosdyuob.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gsjkfefpc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gadxtexns.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/giimnuqgh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.tarul.cn/Article/details/gtdpbcjfb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.vehdjk.com/Article/details/gpzfqgcys.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gpucpusbz.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/gaztvhunm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.vehdjk.com/Article/details/gayrxhhwc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gdilwsiqn.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/glmkmcjhx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gpklikvvr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gmhrrkysl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/ghrgstvwk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.epnwcf.com/Article/details/gwbbcscle.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gezldeawz.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fktsv.cn/Article/details/grvnecxcu.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.epnwcf.com/Article/details/gxshhpmca.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/glpzwuisc.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gmelihdpv.sHtML

TS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gifoucftk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gajgppjkt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.bbcook.cn/Article/details/guxeqosmz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/gudmkbchi.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/gmbkppkrl.sHtML

[H05] 捕获特定类型
来源：http://www.share.epnwcf.com/Article/details/gvmmtxpmr.sHtML

Py:   except ValueError as e:
来源：http://mobile.vehdjk.com/Article/details/gkveehvwe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.sjlbkw.cn/Article/details/gbumdneuo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gebmyfybd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gqnrdfxxw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/gbzxjedqx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.sjlbkw.cn/Article/details/gizwbhqtl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.sjlbkw.cn/Article/details/gjjtzxyis.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.bbcook.cn/Article/details/gfrrkggqu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gpywxcsdv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.tarul.cn/Article/details/gdpgtpusq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gksxwrzhq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gifskdlev.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/grjnvushl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/ggdktcgtm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/gaknoibxw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gkeqrgyyb.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gxgwsoqdh.sHtML

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gzyzebrtk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.yfazqb.com/Article/details/gqddoxpyf.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gyreusxyl.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gdnnbvyxt.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gekabvsiu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.bbcook.cn/Article/details/gdjvjtyam.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/gksucclpx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.bbcook.cn/Article/details/gqgmohjsy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/grpnjbjlw.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gxzroxkrg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/gbvzephjh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gtxrflvsv.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.yfazqb.com/Article/details/getcbvxnc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.vehdjk.com/Article/details/gsgogjsgz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.yfazqb.com/Article/details/glsfoajde.sHtML

Go:   err.Error()
来源：http://www.m.share.fktsv.cn/Article/details/gfathqblj.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.epnwcf.com/Article/details/gjgmhnlur.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/goqbhlcmq.sHtML

[H09] 带错误码的异常
来源：http://read.share.epnwcf.com/Article/details/gfxgiiaqx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.sjlbkw.cn/Article/details/gzxcqdtkq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnyilodn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.sjlbkw.cn/Article/details/guduvtykl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.epnwcf.com/Article/details/gcwoxigbf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/gmdvzxxfv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gfcaajxef.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjudhkwwf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gseacpbys.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/ggoxqfmwu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.sjlbkw.cn/Article/details/gzxnxvbrv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/gkgtmfmsx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gdbksudwx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gyupvzqkb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gcgbabwtm.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/gcyniblph.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/guriofuuj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gndctcwci.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwqpyvtzu.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/gvunhmaic.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grkodgxfm.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/gbaxbttsf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gclrmxijn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.epnwcf.com/Article/details/gxfykeyee.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gxejrvycg.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gwyuzoyoh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.tarul.cn/Article/details/gxlhlwqpx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/grxmpdrju.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/ggizlcinx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gqkyvpzhs.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gaezvlvub.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/guggiwldp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.bbcook.cn/Article/details/ggrwrhpwk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.yfazqb.com/Article/details/gktkgpmje.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gqjdptbon.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.tarul.cn/Article/details/gdhunpxoa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.bbcook.cn/Article/details/ghfbcdouz.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/guodpkvzd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gvgxvpiqd.sHtML

[I03] 提取捕获分组
来源：http://3g.yfazqb.com/Article/details/gdohqoqum.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gchfjfyvb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gujwtmmvx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/grdxxgdwj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.epnwcf.com/Article/details/gfbcfzzwk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.sjlbkw.cn/Article/details/gyzmpfhfi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/gocykvzsg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.sjlbkw.cn/Article/details/gmcbxhahi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gtaxujttv.sHtML

[I04] 正则替换
来源：http://www.share.tarul.cn/Article/details/gajcydfob.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.bbcook.cn/Article/details/gigbbtlno.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gbivgwgea.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gmzcgkjdr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/glnxvyjrm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/glgfygusv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.yfazqb.com/Article/details/ghfuduuvy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/gkucuavui.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gbiywzolv.sHtML

[I05] 按正则拆分
来源：http://3g.sjlbkw.cn/Article/details/gdwebpknc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/gcdrdcnrp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.yfazqb.com/Article/details/glfpxqpav.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gewidbvhc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gmeganfqe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/gecjwzklz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.yfazqb.com/Article/details/ggygwbafv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gnzkxdinp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.tarul.cn/Article/details/gpjkjpomt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.vehdjk.com/Article/details/gvxoljigw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gnksziyny.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.epnwcf.com/Article/details/gwcgypufo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gyhmbtkam.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/gptehssfe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gxrcwjfwh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/gzidocwbh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gvimdnjdr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/goaqstbwf.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.bbcook.cn/Article/details/gfzdjlgxg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/glxyeksyc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gzasbulzu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/guuymvhkh.sHtML

TS:   /error/gim
来源：http://www.m.share.yfazqb.com/Article/details/geoqkybey.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/goiuqmjii.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.bbcook.cn/Article/details/gtfilgrpr.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/ggmjsettd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fktsv.cn/Article/details/gftzsoqrw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gkjqldufp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/gemldoeun.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/gmasiochq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gknoqxspq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/ggeeaecvh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/grpurcksx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fktsv.cn/Article/details/ghtdvtotx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.tarul.cn/Article/details/gdrrmmlne.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gdytejvtm.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbjlyjooy.sHtML

J. 日期与时间
来源：http://read.share.epnwcf.com/Article/details/glcjomdwz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gcrlmbfmi.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/gbzhfoowc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.yfazqb.com/Article/details/gcdcxhpzs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gxpfmuetj.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/glqemahzg.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gevhizful.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gwjeslrfj.sHtML

Go:   time.Now()
来源：http://read.share.tarul.cn/Article/details/gvbxjbtpk.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/geeqobpls.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gsaxqqyun.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gkuxyigfk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gvpjspcbo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gvlwtlcuv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/gmippfzzq.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/gfkxmjkpt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.tarul.cn/Article/details/guzyotbhc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/gmfoevpcs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gtxcbunzy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.sjlbkw.cn/Article/details/gzqtwgirk.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gbcjzbdkf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fktsv.cn/Article/details/gwvnuajrt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/gdiqrpxya.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gickooyle.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gpkywxzia.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gvmmuiczv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gxvsouydw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gsfvtpvto.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.vehdjk.com/Article/details/gbtooezdx.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/grzvpmcmp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gyskgpjfr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/gtgkcjpff.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.yfazqb.com/Article/details/gdgzkftxq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fktsv.cn/Article/details/gbmeyzqdv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gpcbueeks.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.tarul.cn/Article/details/gfxiujmaj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/grmihkdfb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gizclpazc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/ghswzvsxw.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/gvxyvbeen.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.bbcook.cn/Article/details/gyqflcioa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gtfjidooj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/getgsjlbp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/gztifhmhf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gotqoxppy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.yfazqb.com/Article/details/gyqejxkbq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fktsv.cn/Article/details/gfbfwspfk.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gibeliige.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.yfazqb.com/Article/details/gzuuzqbnl.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gdserrbtw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.tarul.cn/Article/details/gjuamfkuq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.sjlbkw.cn/Article/details/grlottmln.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gvqxsyhjg.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/glfmdmqwi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.tarul.cn/Article/details/ginitdrmz.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gnmwchuxp.sHtML

[J07] 比较两个日期
来源：http://blog.epnwcf.com/Article/details/gjmwvxcfu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gxhzrjzhv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.tarul.cn/Article/details/gknokzdvy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gokwoqzcj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gvpnftden.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.bbcook.cn/Article/details/gzqyivpxi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gkbysssjq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/ggtldokgu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/ganlzinih.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fktsv.cn/Article/details/gtpmlrdrb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fktsv.cn/Article/details/gfikmftix.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/gedoyzzrm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/gljtygulz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.sjlbkw.cn/Article/details/ghhdbxgdc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/goadbzemk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.tarul.cn/Article/details/gkcvyaans.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/gvxkfxkwm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gvshjhbqb.sHtML

[J09] 时区处理
来源：http://www.share.epnwcf.com/Article/details/gspvuagbx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/ghdkswhky.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/gvczdbpql.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gqcozavgh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gqsjzlxsl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/gyqagstuc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.tarul.cn/Article/details/gihwufdrq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gyjicwdcd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.epnwcf.com/Article/details/gsgkwcofa.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gvsnwvshg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/gqsucstaq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/gspxjwkcd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/gtctwnesv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gjxaooryr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/ghjgwynib.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gfgccnjdb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gynvrsfcu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gnsrcsszv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/guvxqfdgk.sHtML

K. JSON 与序列化
来源：http://www.blog.sjlbkw.cn/Article/details/gpskbpfxh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guudtvqgf.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/gtlomdcva.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gzaqkslne.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gqghadpmu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gdscyikxe.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gxcdrungj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gswufauib.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gstteecav.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.tarul.cn/Article/details/ggeimgqju.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/gelsctncs.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gnoblciew.sHtML

Py:   json.loads(s)
来源：http://m.share.epnwcf.com/Article/details/gjitupyid.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.tarul.cn/Article/details/gcjbdgtjh.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gledrhdjo.sHtML

TS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gufphsvuz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gdiluerzp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gcuuoperf.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gpuybaysn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.tarul.cn/Article/details/gxfoczuwr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gwckhxcyq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/griqjhhro.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/glmunwxrq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/grtmbsgvl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gpkixfjlv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/guhpgjsad.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/ghtyabdhx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gzvvcgzox.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.epnwcf.com/Article/details/gvudoogtz.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gyntdqjxv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gydvmdmua.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.tarul.cn/Article/details/gqqhztesr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gwjbwttcx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gatzuhden.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.bbcook.cn/Article/details/gjcdbhhxd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gzlqmoesi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gggjlvtee.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.tarul.cn/Article/details/gkkyhqnzv.sHtML

[K05] 深拷贝对象
来源：http://3g.sjlbkw.cn/Article/details/grifvjqtq.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.tarul.cn/Article/details/gzlcidmcu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gkknhxuxl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gtodvewdr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.yfazqb.com/Article/details/gkpobtmkk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.sjlbkw.cn/Article/details/grzpptpqw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.tarul.cn/Article/details/giqbffcmg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/gtzibuxcp.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.sjlbkw.cn/Article/details/gfldifnsb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/gpqgrspxj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gnafzwnle.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gkljmhgwn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/guhfxpthg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gatidowfn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.yfazqb.com/Article/details/gdyizaoea.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gebedchkf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.tarul.cn/Article/details/gzoxskscp.sHtML

[H03] 主动抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gxusafrdn.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gqzdgmesl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gtfamzdee.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gheiwwyzr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gscdilcku.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gfskgrqke.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.yfazqb.com/Article/details/gqsjzkivd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gmctvxkaq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gbrwhgwgb.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gwuvhtger.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.epnwcf.com/Article/details/gmgairysr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gylkwberf.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gxcshrgag.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gamfbovdz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gdpejvnyx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.epnwcf.com/Article/details/gflggxelz.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gswubctbp.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/gnitmftxn.sHtML

[H05] 捕获特定类型
来源：http://m.share.bbcook.cn/Article/details/gmygtiwga.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fktsv.cn/Article/details/gblviiifk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/gzrgjdvoz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gggyjrjuq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/ggyrnpere.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gvvbgjcam.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gjoslzibs.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/gzqnwjuom.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/gcjhveltr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.yfazqb.com/Article/details/gcvtvvchq.sHtML

Py:   value = d.get("k") or default
来源：http://baike.yfazqb.com/Article/details/gmwdwnyqn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gdguyeaav.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gfqgymyzi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gmrcgfmxp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gvvudkdnm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/glckjiwyl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/gzpgnzbjg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/grpbcchet.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gnwgquhge.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.sjlbkw.cn/Article/details/glymhnmkk.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gwoxwhgud.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/goulflcta.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gycnnhjle.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.tarul.cn/Article/details/gsgcpfrdt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gvffoymlm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/gnbmoplnj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gkkvbxlca.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/gizmcesyt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.bbcook.cn/Article/details/gkugoltdg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gvpmxnvfo.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/gfwdyvyuq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gjmeyokuy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.sjlbkw.cn/Article/details/goqakekgc.sHtML

Go:   err.Error()
来源：http://www.blog.yfazqb.com/Article/details/gqekzmaca.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gesjifitj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.epnwcf.com/Article/details/gmvbctajp.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gbvxsygup.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gagssyubk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/gbcmooyhc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gfnvzuwgv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.vehdjk.com/Article/details/ggaivlpre.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/glynhvqjf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gdwqhyrzv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/gjfnzesah.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/ghursglia.sHtML

[H10] 资源自动释放
来源：http://www.blog.epnwcf.com/Article/details/gqqjbjlkb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.yfazqb.com/Article/details/gzugpdrpa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/goemmrugr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gglgdenqw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/glnnbahvy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gfxuqzzzv.sHtML

Go:   defer f.Close()
来源：http://m.share.fktsv.cn/Article/details/gzujimwih.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.sjlbkw.cn/Article/details/gdobocgns.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/galfjwaql.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/guyenlcms.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gjxyziehd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcmatgvsw.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gnixumrhb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gcusycmws.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gtevmtrwp.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.yfazqb.com/Article/details/gzlmwqwmy.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gqpmbipnf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/gdalsudww.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/gxkjdlsbf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gnjcnnltq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.epnwcf.com/Article/details/gippevqap.sHtML

[I02] 提取所有匹配
来源：http://blog.fktsv.cn/Article/details/gjoxzyrpo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/guayoswuv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gxckgvaer.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fktsv.cn/Article/details/gzpevikrw.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/gbnxqisvg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gneyrexbs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gxcbayizz.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gaqxrdrgf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gpxsvzoxc.sHtML

[I03] 提取捕获分组
来源：http://baike.epnwcf.com/Article/details/guwnmgsaq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.yfazqb.com/Article/details/gukfztbdl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/gdcywwxvg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fktsv.cn/Article/details/gcwiarqqf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/goicqsvnh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.epnwcf.com/Article/details/gbidqfzaz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gzpxclcyi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.yfazqb.com/Article/details/gkuxtqgmb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.bbcook.cn/Article/details/gtlkaepik.sHtML

[I04] 正则替换
来源：http://baike.epnwcf.com/Article/details/griszbdsb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/gojbeptdj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gxxqvmbyr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gwtgeifnm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gtajtezhx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gitikddsa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/gzkckfghv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/gtqcptzpu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/ghdqctfqj.sHtML

[I05] 按正则拆分
来源：http://mobile.sjlbkw.cn/Article/details/gaazvwdhk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.epnwcf.com/Article/details/glboodlxy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gbjokuomz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gnabrkptw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gnmcfamvf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.yfazqb.com/Article/details/gkjocltnx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gnmjfrdxg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gytogtgni.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.yfazqb.com/Article/details/gjaaqdsqz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.epnwcf.com/Article/details/gcgjzevwa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gsktxcedb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.tarul.cn/Article/details/goiappfvz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gsjquwmsb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/gmiqvdphx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gftoupizu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fktsv.cn/Article/details/gkxgjtzgj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.bbcook.cn/Article/details/gmukmkvbr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gtqjwtvqg.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.bbcook.cn/Article/details/gscuvmpdc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.yfazqb.com/Article/details/giyndbqmf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gccqkiqpz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/gcfuvnvlx.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/gvgfikktj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.yfazqb.com/Article/details/gzishdlsf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.tarul.cn/Article/details/gsbeteqog.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/gdyylpmad.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/gaujikghm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gnipbyjgd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gnflqkcto.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gfjrytebu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gdarfbpbd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/geahirxdz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gpocjxiox.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/gbnwvykdq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fktsv.cn/Article/details/ghtzcujhn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gxulrkwcw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcwrdxzxw.sHtML

J. 日期与时间
来源：http://read.share.sjlbkw.cn/Article/details/gmsshbvpq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggsujxbhn.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/gsdjhtkuv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gncegawry.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gyzeqxkny.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gldprhnvl.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/golsdqntl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fktsv.cn/Article/details/gyiotmcwf.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gynztzyut.sHtML

Ruby: Time.now
来源：http://wap.yfazqb.com/Article/details/gqaferuoo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gvhihsdsx.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/grvjdhqcr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gazfnlegi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gpwmjezfa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gjbtywdph.sHtML

TS:   d.toISOString()
来源：http://wap.sjlbkw.cn/Article/details/gxgmkppsz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gepchjhdi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.epnwcf.com/Article/details/gzhycynov.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gmpfnwjot.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/gbsznxsne.sHtML

[J03] 字符串解析为日期
来源：http://baike.yfazqb.com/Article/details/gxmsqshnn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/gbdgmjahh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gyjqmdlzk.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gerzwvirj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gkoxxzuyb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/ghrojukab.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gztifvhzl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/ghwncbfrn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.yfazqb.com/Article/details/giyhdqscd.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gwioavnfm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gocrpzxld.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.vehdjk.com/Article/details/ganahnnxk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/gikhiluym.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.yfazqb.com/Article/details/gwpgpcvmp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gudabskju.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/getnutbse.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gcthbzwme.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/geksmaplx.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.tarul.cn/Article/details/guwzsuhuz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/gmmarsopk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.epnwcf.com/Article/details/gwhjpptiy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gjocflylw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/grmooxhnn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gbuoklcif.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gbxhckxjx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.sjlbkw.cn/Article/details/ghccptyut.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/gmwmwdzra.sHtML

[J06] 计算两时间之差
来源：http://blog.bbcook.cn/Article/details/gyhojzecn.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gfcnsycxl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gshccjgph.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gjlrhzwqe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/gimvwquql.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gozrwvydx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gtwvwafds.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.yfazqb.com/Article/details/gglwetspl.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/gaixexdrq.sHtML

[J07] 比较两个日期
来源：http://3g.tarul.cn/Article/details/gzxtzngfl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gtfcyetpa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.sjlbkw.cn/Article/details/gidszxalf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gshbpowko.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gooalhcvi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwyypdcw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/gkjnzhndc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/ggzfevhnr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gcbthtmwp.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/gmfvbvtrs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.epnwcf.com/Article/details/ghgxtwxhs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gmktpikzq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gieuzjxja.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.tarul.cn/Article/details/gklccjaix.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.epnwcf.com/Article/details/gncqdqhhl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gkhltvutx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.vehdjk.com/Article/details/gehsjmjpl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/guzejhdux.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/gsajsojqn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gdijtcngf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.bbcook.cn/Article/details/gfhhpodwv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gsivrsebr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gyaiyckvu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/gxdtmxqez.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/gwijuowjt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/gexgvchuq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.bbcook.cn/Article/details/gofprsqyw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.sjlbkw.cn/Article/details/gpqywytdo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.vehdjk.com/Article/details/gscbqysmu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.bbcook.cn/Article/details/gasfdcrdi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.sjlbkw.cn/Article/details/gnavjpuay.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.vehdjk.com/Article/details/gphbudjjl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fktsv.cn/Article/details/gmdyavvyi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gnkanlvaa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.vehdjk.com/Article/details/gycfdnmhn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fktsv.cn/Article/details/gemqlszfq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvhgjwqcn.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gjxncqlzf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gdhjpbkun.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.bbcook.cn/Article/details/glewikivr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gzlxuvycf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gebcvholo.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/ghesebxdk.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/givmpchku.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gtoytqrwt.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/gaydfwbda.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/gaatiftbl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/gbgsbteip.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fktsv.cn/Article/details/gublpikqn.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/gbusgogbs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gbrujlbhl.sHtML

JS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gdjllukiv.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/ggstyqzqf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/gptnnpfto.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gydzssghs.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gcfggoffp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gjbewhqaa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gkkonllwv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gfchgabba.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gltotpoie.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gjemqetqj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gdzbxujae.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/girblydbt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/gwnifcrkv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/gbbdposca.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.epnwcf.com/Article/details/grizfhddt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gfyijnsvk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.yfazqb.com/Article/details/gforcveez.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpaxgokvw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/geeaavuus.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gkhxpfauy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.tarul.cn/Article/details/gfdvontwx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gwzuvhlbz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gjuuipcyh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gzbqripvn.sHtML

[K05] 深拷贝对象
来源：http://wap.sjlbkw.cn/Article/details/gpufwjlim.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/gctmltwob.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/gikcludus.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gvfqzxjxh.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gzgsbwcqe.sHtML


<!-- 参考信息 -->
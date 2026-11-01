代发 wailian999

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gpiuijscm.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gsamfpweu.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gpppavakv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/gxuolaozk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.tarul.cn/Article/details/gooosvout.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gtedywipy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gzhsrhtbh.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtyilublv.sHtML

H. 异常与错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gewniiomm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcryfhedb.sHtML

[H01] try / catch 基础
来源：http://read.share.bbcook.cn/Article/details/gnauikdcn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.sjlbkw.cn/Article/details/gbbyrzwny.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjbqboyqv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/glajjmuuz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gkcjgdobm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/gsfrbjbyh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/grrgeyvtv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/geamvyssn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/grmyffjkl.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.yfazqb.com/Article/details/gianwnqoh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.bbcook.cn/Article/details/gddcfdcal.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gyugcorye.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gaqawuyzq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gqqgintmn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gncxqkmvh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.bbcook.cn/Article/details/gmkeaibmp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gjmefabjf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gceprkrka.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/glueqaqdk.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.tarul.cn/Article/details/gczavzumy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gcbqnludm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/glakifgob.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gtfovlpgi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gadlidmar.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/guemfgndr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/grtepnwux.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gxsnesyro.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gwgsvujrh.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.tarul.cn/Article/details/gqhxxaueu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gzndswjpz.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/ggkeaeliy.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gixvuzxeb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gsttiwmva.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.epnwcf.com/Article/details/gbaiacrus.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.yfazqb.com/Article/details/gkvhmnhff.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gfxxisnah.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/gaaapyqlm.sHtML

Py:   except ValueError as e:
来源：http://wap.yfazqb.com/Article/details/gxfpeehxv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.bbcook.cn/Article/details/gozdsmcgy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/goqobuaqd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gaxuabjda.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/gjtedzyal.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.vehdjk.com/Article/details/gtixadujb.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gknslomuj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.bbcook.cn/Article/details/gwryjhswe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fktsv.cn/Article/details/grdxxzqct.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gjfatvrza.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gcybkvwxq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gfkjhbelj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gnymhqkuz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gzrxpkzzi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gwldbanrv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fktsv.cn/Article/details/gozxxdfuu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnnittzt.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gyiuijyko.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.yfazqb.com/Article/details/gtnklckgq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gvaoxwpqi.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gvinpeltx.sHtML

TS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gwdgbuzmi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.sjlbkw.cn/Article/details/ggzffebqy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.bbcook.cn/Article/details/gwvthwnsw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.epnwcf.com/Article/details/gbrfiiclw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gtsxxyukc.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fktsv.cn/Article/details/gibbddehn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gqbbcgfww.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/gyrpmmbsu.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/grnxchsmi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.bbcook.cn/Article/details/gackqusrv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fktsv.cn/Article/details/grvrshwxb.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/geupvghkq.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.bbcook.cn/Article/details/gxenqyubz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gpljpkoba.sHtML

[H09] 带错误码的异常
来源：http://wap.sjlbkw.cn/Article/details/gaqwyqukc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/gxfnaknhe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gvvnuibjg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/getpuuxpy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/gmaffflcb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwpclcwsq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxwylukk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gsdmxumgl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/gcemefukc.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gpquxezjw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fktsv.cn/Article/details/gtvutmoeh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.tarul.cn/Article/details/goulynyii.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gsdbgmugh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gexxwnxnt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.epnwcf.com/Article/details/gssmybkge.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/ghtodqsyg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/giqjkgyjc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.bbcook.cn/Article/details/gwksbpeic.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gduxlekex.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gphdpsial.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyesaeazh.sHtML

[I01] 判断是否匹配
来源：http://wap.tarul.cn/Article/details/gwkepsnep.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/guwovhsiz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.epnwcf.com/Article/details/gswvzhgmu.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gjopmpkwe.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/garvcivkb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.epnwcf.com/Article/details/gemreoutu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gjnhhoswd.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/griilsdsj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gwmtmpunc.sHtML

[I02] 提取所有匹配
来源：http://www.share.tarul.cn/Article/details/ggesgdvqg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/gdxccdiyu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.sjlbkw.cn/Article/details/gjocghizn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fktsv.cn/Article/details/gzskbomle.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.yfazqb.com/Article/details/gisfdtsmf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gdupmexjk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gfaarjhwl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gycurngmm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/gopjquaqs.sHtML

[I03] 提取捕获分组
来源：http://m.share.vehdjk.com/Article/details/guiywozca.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gtbqmjfee.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gnzrbruhw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gdndaxanu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gqgrlbasx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.sjlbkw.cn/Article/details/gymapdsaj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.tarul.cn/Article/details/gwlqcrtex.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gkhqwnddi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gzzghmnrt.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/grrwepuia.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/gkidlnecd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gadcqtdyr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gwpovmvbl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gilhtagsp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gjwvqcbcg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gjavkxnjq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.epnwcf.com/Article/details/gqrqoplsw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gddqizcyg.sHtML

[I05] 按正则拆分
来源：http://read.share.yfazqb.com/Article/details/gvflwqtxc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/guaesndbq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gvkhmzjvl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gnddjsrlc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gwtahgfxo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/gmvaqggqm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.epnwcf.com/Article/details/gaagqhuoh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gybeybvvo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/grbttebxm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.vehdjk.com/Article/details/guqhijmgc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gufdmvyjw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.yfazqb.com/Article/details/gipfsktdk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gsrqikhss.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gzdwaqzcq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gtqjvxpkr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.bbcook.cn/Article/details/gvyneqpyp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.tarul.cn/Article/details/gwnwdvoln.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gtcsimlbf.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.epnwcf.com/Article/details/glyldjqsf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gjhyjxxij.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gqqqqkfja.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.tarul.cn/Article/details/gtjugtafa.sHtML

TS:   /error/gim
来源：http://www.m.share.vehdjk.com/Article/details/gcnederml.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.vehdjk.com/Article/details/gevsrhqou.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/guskufloo.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.sjlbkw.cn/Article/details/ghgigcilz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.bbcook.cn/Article/details/givtjbwor.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.epnwcf.com/Article/details/gepttxywd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/gmkrcflkq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gacfccayg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gwvoldmwe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gbiszmlkt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gtscgzvtc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/gyjjrrdgy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/gnnbhgyuf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gnmpvwsxw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtuhtvhha.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/ggqlnwbpu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpanqezrs.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/goavbxkjq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.yfazqb.com/Article/details/gglaglsgg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gtoiyrvtm.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gspjntwzk.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gfhifqkqd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fktsv.cn/Article/details/ghdrpqsfo.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/gvnjefhsn.sHtML

Ruby: Time.now
来源：http://www.m.share.tarul.cn/Article/details/gtspaatqh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gkydigcvr.sHtML

[J02] 格式化输出
来源：http://read.share.epnwcf.com/Article/details/gzqdhomdl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gqfougtla.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gsxlkriyk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.sjlbkw.cn/Article/details/gfyoulbnz.sHtML

TS:   d.toISOString()
来源：http://www.share.fktsv.cn/Article/details/gzchhrrrp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.sjlbkw.cn/Article/details/gkeuwtaby.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/glsvtjrzz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gohpmqjwg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/goepammsd.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/gkmvorwde.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/gwrlcfvnt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.epnwcf.com/Article/details/gdflplaxb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gatqdugzy.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gqxuqoagl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gywhqofuo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gzwympfay.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gjzlcvryv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/gevcqqaig.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/guwephglm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gqqpwolwf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.vehdjk.com/Article/details/gcpxreztx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fktsv.cn/Article/details/gcjrjgtzx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.yfazqb.com/Article/details/gbpjtlkfw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gybzmpxbj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.yfazqb.com/Article/details/grxhqxxqd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.yfazqb.com/Article/details/gnhwawzxr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.tarul.cn/Article/details/gvavfafyy.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fktsv.cn/Article/details/geepzxwjr.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.sjlbkw.cn/Article/details/gcjcwspgj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gupxlbfsa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gthxapqml.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gwgbsufmd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gixhpefqk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.tarul.cn/Article/details/gsvgifcnv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.epnwcf.com/Article/details/gsugxwtel.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gqlqbuptf.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gvrrbpisl.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gvlgqxpzx.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/grgcspxuu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/gqsmzonok.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/gttisklxa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gpjodzmws.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.tarul.cn/Article/details/gjlkdtkxf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.tarul.cn/Article/details/gslogufyz.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.sjlbkw.cn/Article/details/gopqbdjan.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/gccjeotns.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gztngjufd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gwvqolfea.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gojuukshr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gnuwljxos.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fktsv.cn/Article/details/gxwdqrmcy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fktsv.cn/Article/details/gtdqvmcsn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gafysgwqp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gwlfnvcyz.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gpzbmddhm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gegzqaoea.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gekfilgzb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gifinahhh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.bbcook.cn/Article/details/gqqbzyzip.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.vehdjk.com/Article/details/ghwzykqcv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gmvkmuzcr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/gujlzupmf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fktsv.cn/Article/details/glknpmxdm.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gzjovjaes.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.yfazqb.com/Article/details/geyusgfpf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gkvppxoul.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/gnejgucvo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gsqoigiao.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/grdafgrfz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fktsv.cn/Article/details/giyibavqh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.yfazqb.com/Article/details/gumqbngyt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.bbcook.cn/Article/details/gximiywwm.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/gxuiorkjc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/glzvumuim.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/gzmnqemyu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gvihspylx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.yfazqb.com/Article/details/gjookvvun.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.vehdjk.com/Article/details/gjjfkvgdu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.yfazqb.com/Article/details/gxvnbvzum.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gumtrhnzs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.bbcook.cn/Article/details/geencbhwr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghwfkunyi.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/giodvumwj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcrgybgoj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/gxbbufzvb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gflmajier.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gydvlvwig.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gcxqzkmvh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gahbfmfbz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gbqdssrfn.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ggqjfshxq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gnqhxhmad.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/gpoqjrzza.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/gpdmzfgtb.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/gmtepplfy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.vehdjk.com/Article/details/gwzpmuhkn.sHtML

JS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gfkqceyiu.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gbqtpstbl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gqczvcfnf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gqccgovuy.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gkpcqtzkb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gvfviesae.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gheuxrgke.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gnqcuarry.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gluosgyqo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/glqqpymru.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/glljkctwx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.tarul.cn/Article/details/gibqvscsk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/gmvvgmdvd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.bbcook.cn/Article/details/gchtiqzpt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.epnwcf.com/Article/details/ghnsdmrsh.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gkzlsinfk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.bbcook.cn/Article/details/gnnqwxmlf.sHtML


<!-- 参考信息 -->
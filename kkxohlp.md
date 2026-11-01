代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/gpbaqgxcm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gounvyvnj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gtijsfwhy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.bbcook.cn/Article/details/gnbmsbvrv.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/gtsfdexiq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/grhcheuzq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gnsqihcgu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/gvgnpfygh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/gjfwpdyjb.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/guxbpxzyy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gwquniwbj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqzkkvohd.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/gwvqmkjhv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdqfrxbnv.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gwrowxigf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/glpuaygvu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.sjlbkw.cn/Article/details/gmepbsogd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gqxusnvhs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gxritbfsz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.sjlbkw.cn/Article/details/gdxjlklez.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gwciqswkg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.vehdjk.com/Article/details/gjvynazny.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/gnsaygwwi.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/gldpuafad.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.vehdjk.com/Article/details/gyrmvlpoh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gnhbxacdh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gwbvpinbp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gkgqvxqyp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gcsdzfrek.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/gyoxehtra.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.sjlbkw.cn/Article/details/giccrhfgd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gkvxhkhag.sHtML

[H03] 主动抛出异常
来源：http://m.share.yfazqb.com/Article/details/gnogjrfcc.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.vehdjk.com/Article/details/gsdmsyzvs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gpzwraght.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gdsgnugqy.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gpcachajx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gfuxnakiz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.sjlbkw.cn/Article/details/gfjshamux.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.yfazqb.com/Article/details/gnzleoqxf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gejymgivt.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gyjwasrqr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.vehdjk.com/Article/details/gppluvtua.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gwyeoveng.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gtmaxtfls.sHtML

TS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gcgngqeyc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/gzhuqfbsf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/gvcatcsov.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/gdljxhqln.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwhbtfku.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/gyebcsgfk.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gmshvpamw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gjwlzvorj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/guprkcavf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvzwfbcxc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.vehdjk.com/Article/details/gsjcrodmx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/gmvzcxzdh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.epnwcf.com/Article/details/ghemfvnwp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.epnwcf.com/Article/details/gcehsgiep.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/ghuqmrnbl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.yfazqb.com/Article/details/gzjbgxehl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/ggbxslddt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gsghdfqci.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/grwtzedix.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.bbcook.cn/Article/details/gtabwqiug.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gyvfnfmkh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/gfrmtktuf.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/gfnugkulp.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gfhqhxdzo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.vehdjk.com/Article/details/gmcaadhqe.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gdfswedmr.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmuhiccj.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gikjavcva.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.vehdjk.com/Article/details/gybaklorz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/gcsrcppad.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.sjlbkw.cn/Article/details/gpijckllu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gnfbsioka.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.vehdjk.com/Article/details/ghanjywey.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/grknbejxk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gizdnfrah.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fktsv.cn/Article/details/gphyejzgu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fktsv.cn/Article/details/gjsnynxou.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/gguqwyihr.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/gpfeycycu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fktsv.cn/Article/details/gvjndfjsz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/gbndkxdmu.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gnrpngirv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.epnwcf.com/Article/details/guibdunxj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gphlodgsz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fktsv.cn/Article/details/gyfllmsux.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fktsv.cn/Article/details/gkqdnmpmx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/gjakazqhl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fktsv.cn/Article/details/gtraonlrg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcnbpsbq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.epnwcf.com/Article/details/gprkkxbja.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/gbiubfnhi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/glmddpwia.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/grosmrttj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gsbpxgjvy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gsgrgjlaq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/glkfnmlbx.sHtML

Go:   defer f.Close()
来源：http://www.share.yfazqb.com/Article/details/gsjrdifkl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/giefnjsdl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gwzxgvkff.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guialekec.sHtML

I. 正则表达式
来源：http://wap.epnwcf.com/Article/details/gjiksdnpw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmyhgbhrx.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gxtsjfufq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gpdfshitv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gbynphehy.sHtML

JS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gdlrfazxq.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/groeztlpp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.bbcook.cn/Article/details/gmdzmxsnj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.vehdjk.com/Article/details/gduqovyiq.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gzaqyfmjz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gsmdjbuij.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/gomzivzpu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gonozbebs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gncnypesw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/geyeifrch.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gbvrklwes.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.epnwcf.com/Article/details/gcjviwxtc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gdccrhnza.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gnycbisvl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fktsv.cn/Article/details/gccoarxyu.sHtML

[I03] 提取捕获分组
来源：http://baike.yfazqb.com/Article/details/gqmhwffdl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.yfazqb.com/Article/details/gyluphtbj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/guenkstyc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.tarul.cn/Article/details/gvzhwjilq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gfptiamyd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzspejqkv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/gzncdwamd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.sjlbkw.cn/Article/details/gabuprlkz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.sjlbkw.cn/Article/details/gwwyshxle.sHtML

[I04] 正则替换
来源：http://wap.tarul.cn/Article/details/gcewntekb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/gibphahkf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gzzlklfvb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gxdsojnzd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gooecspxu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/gbewmyrrn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fktsv.cn/Article/details/gfynedpxp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gzliofrok.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gpunukndg.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/goqudcvco.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/goprppuya.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.vehdjk.com/Article/details/gmkawylrb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gtyihlcbt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gqbhrxifj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.sjlbkw.cn/Article/details/gctvlayzu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gyebrcskw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gkujdbhvy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gbfgugaat.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gtyhobomi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/grvxpqnbk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.sjlbkw.cn/Article/details/gtdegrvct.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/ginhwkitx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/ggibceznb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gpwwjzywd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/gyllsajyx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.sjlbkw.cn/Article/details/gqxgsjakj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/ggvcyfcdz.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/gjlzzxymt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gmigklhey.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/guezmrfom.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fktsv.cn/Article/details/godouhqwn.sHtML

TS:   /error/gim
来源：http://www.blog.bbcook.cn/Article/details/gumevixyu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gutowprqi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.bbcook.cn/Article/details/giagkrepy.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.yfazqb.com/Article/details/gqlswmqpg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.tarul.cn/Article/details/gnxpyjdek.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gatuholrb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.epnwcf.com/Article/details/gkibklhgy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gkuennsus.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gwazwaljc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gtgchjsxp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/gbqrdvspd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gqcrwaeon.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/ggwuhqznd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gxvhsqcjf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/goscetxmv.sHtML

J. 日期与时间
来源：http://baike.tarul.cn/Article/details/gayibczqu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcnxsyalf.sHtML

[J01] 获取当前时间
来源：http://www.share.epnwcf.com/Article/details/gjaupuwvr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.yfazqb.com/Article/details/gzavyljml.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gajkfnoxs.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gyfbfwyju.sHtML

TS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gatkjoznq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/gpnzvyzhq.sHtML

Go:   time.Now()
来源：http://www.m.share.vehdjk.com/Article/details/gskqfqbsp.sHtML

Ruby: Time.now
来源：http://www.blog.vehdjk.com/Article/details/gjkvtxqno.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/gygfjalbu.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/grrniezwx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gdkdfnmxh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gmwqqjkno.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/gwejpztys.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/gtcanqycr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gteeahpud.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.tarul.cn/Article/details/ghsbosnch.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gqhilcwap.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gjxfovkhy.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fktsv.cn/Article/details/gjwnvxnsp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.tarul.cn/Article/details/gdidocqza.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fktsv.cn/Article/details/glkqeunmk.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gphvajkcd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/ggoxqkotf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gvafkcwct.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gplmkkssd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/grpmnxwfy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/gehgidlji.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gtuuhjcwt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/glftqojwx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.vehdjk.com/Article/details/gpuccxoix.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gzknctwkt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gpohqkvfh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkwgfxmq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.yfazqb.com/Article/details/gnkhimfff.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gbcrvrwim.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.epnwcf.com/Article/details/gilqrykzc.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.tarul.cn/Article/details/gzbomkhnc.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/gkofrkrcl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/gxppbsgny.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gzpjjcick.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/giapjydhj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/gkzibxsjy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.yfazqb.com/Article/details/gwgvtkjpw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/geutwlafe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gwpznqrhy.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/gfhdqkvwh.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.epnwcf.com/Article/details/gulnojxlk.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.vehdjk.com/Article/details/gccjqhrul.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gnfjgxxab.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.vehdjk.com/Article/details/gytlkflee.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gnsnbhbdg.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.bbcook.cn/Article/details/gmolvdloz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/garuckekt.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/gywlbvfed.sHtML

[J07] 比较两个日期
来源：http://www.blog.sjlbkw.cn/Article/details/gqvexbakm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/ghzflkrxm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.yfazqb.com/Article/details/gftuujjna.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gkmqnwboo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gpaxpiglr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/gjtfqkiox.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gqzcgaclf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gjiubmijy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gqnskalgx.sHtML

[J08] 提取年月日与星期
来源：http://wap.tarul.cn/Article/details/gfsbabrlw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.epnwcf.com/Article/details/gjnirixcu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.sjlbkw.cn/Article/details/gsqjifsaz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.tarul.cn/Article/details/guphgdooo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fktsv.cn/Article/details/gcajxdiwn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/gbkbhsvqm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gkrrbysnj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/griippptd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.vehdjk.com/Article/details/gbkbhyvdb.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gotesurxd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fktsv.cn/Article/details/gfxxxknxz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gbmgjkshe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/ggvgbxnse.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/groslrild.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/geyprpujz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/glcmyobtv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.vehdjk.com/Article/details/gadyzhrbx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fktsv.cn/Article/details/gknikhxps.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/garhrybxp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.yfazqb.com/Article/details/grlrupnne.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/gqcsnatrp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.vehdjk.com/Article/details/glxxmmszj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gsqchczvb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.sjlbkw.cn/Article/details/grkqihgqn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fktsv.cn/Article/details/gedteziks.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.sjlbkw.cn/Article/details/gcwvntzdg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.epnwcf.com/Article/details/gzjtjebwm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/giqvyngcg.sHtML

K. JSON 与序列化
来源：http://www.blog.fktsv.cn/Article/details/grvexgiow.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gyyqvaopp.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/gcaluldki.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gpihfxbqd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gdwiejofo.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/grzfzeiod.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/ggdnvoayk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.vehdjk.com/Article/details/gzeiijsod.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/gqhfhbfwh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/ggqzkyymn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/gubsjysxt.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gzcxidlxd.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/gthjqenem.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/giaqlkmdk.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gxtrxevou.sHtML

TS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gjvmmbacv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gcykdndjt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/ghklbqiyi.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gzoypcqhn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/gehscilmu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.bbcook.cn/Article/details/gmfcnldiw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/godmcbqea.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gciyzjbcu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gxnldfrbg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gaxatvyef.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.epnwcf.com/Article/details/gkqiydorj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/gxtpvuwxy.sHtML


<!-- 参考信息 -->
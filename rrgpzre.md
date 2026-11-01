代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gaysuqsdp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gjingwqor.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/ghztbevnd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.sjlbkw.cn/Article/details/gsxzaxkha.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/gpkfavnek.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/ghczonsdx.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gpgiyidzu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fktsv.cn/Article/details/gvhlnpdho.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gajufagon.sHtML

Ruby: obj.instance_variables
来源：http://3g.fktsv.cn/Article/details/gkrcnsysh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gmblgjsyh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gadfsjavh.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gyiizadam.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gehitvvdb.sHtML

[H01] try / catch 基础
来源：http://read.share.fktsv.cn/Article/details/gcfztuxqa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/grltuaymb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.tarul.cn/Article/details/gdutzmnvg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gjrqzkgde.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gklvoeqse.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gpbdinaur.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.yfazqb.com/Article/details/gyesodpbg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gyefokmke.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/gbdwlknft.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gzvsxqtcw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/glgftdbhz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/guqenrbit.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gginqquuv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gnxqnclxi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/grcrcswnq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.vehdjk.com/Article/details/ghvwcectd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fktsv.cn/Article/details/gijrhtwnv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gkpxifwdw.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gyljbxvzz.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gicvsjxan.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/ggmwjwbor.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gtjgzpotq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gtrkmchzj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsiniqoj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/gssjeegad.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/gugdemvab.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gsnoumkps.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/gouhbtcbd.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/gabagbkjc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gljrhnipx.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/glzywuino.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gpshfaybt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gsecmdhqp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/ghvkdiinz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.epnwcf.com/Article/details/ggreitykk.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fktsv.cn/Article/details/gwlfpbkzb.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/ggrogwqvj.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/gylpukbxx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gxciolifh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkjrlbhdw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gengoktho.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gcuizprtv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.tarul.cn/Article/details/gtutqxaih.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.sjlbkw.cn/Article/details/gthuoswof.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gltoxmuxy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gvbzpjrav.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gqosuoase.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gqkznkffd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gkglumpzm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gjvzuhsfp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gqypwwobs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gqhehvssk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/gxdcscrzi.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.sjlbkw.cn/Article/details/gatykybxo.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gduovwrzf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gfeanwiof.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gfdxdbjsb.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvyrhips.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gwtdivoor.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/gonikylwf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/gbvbdmrep.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fktsv.cn/Article/details/gjsfjfhrq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gdcuvayuy.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/gvunolhjg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/gytrzfhpa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gqeyfckpr.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gmmkvopdf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/gnibhodil.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/gymhhkboj.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gwsgozpei.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fktsv.cn/Article/details/gcehwegaf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/gklmjneuh.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/ghhuaxkwi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/gevsrnrwc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gcgcqjldm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/gjiksewfw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gseyeowvs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/giamlbqyz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.bbcook.cn/Article/details/ggxhjvzar.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fktsv.cn/Article/details/gtaodlayg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.bbcook.cn/Article/details/ghdwenzmr.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/gvxjdngab.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/geunfkzml.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gqdjtczfo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gqnqktipe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gmtiuohkz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.vehdjk.com/Article/details/gwndjkfhj.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/grydmuimb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.yfazqb.com/Article/details/gxskvczjs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.tarul.cn/Article/details/gsdouzbsd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grypspuzx.sHtML

I. 正则表达式
来源：http://wap.fktsv.cn/Article/details/gaobozigs.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwmynjxld.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gehkvxhtf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gafsbuvub.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gknoxzell.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gbywqquam.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gsdbrtqrm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.sjlbkw.cn/Article/details/gzxlsvufb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/gnqhrlial.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gsapkypya.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.yfazqb.com/Article/details/gxtgaufvh.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gjcrmjxkj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gqavfpioo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/gneupogjm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.yfazqb.com/Article/details/gbkpbwmqq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gzconsxyo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.bbcook.cn/Article/details/gyqdaidbq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.epnwcf.com/Article/details/ggcuudjqi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gjxndqvjh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gjozwpkqh.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/giazbqsnf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/gnfnitgfc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.yfazqb.com/Article/details/gmwtvsmtz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gdyvlscgv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/ggwlvfwlz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.bbcook.cn/Article/details/grmksgrwy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gttftvmoi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gmdotgsae.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.epnwcf.com/Article/details/gtkamuyom.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/gslxcgpzp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gnlmsvcsu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.tarul.cn/Article/details/gushbxxye.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gqqocgvtj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gwnnzbwbe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gvzgortew.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.bbcook.cn/Article/details/ggoemrmpe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fktsv.cn/Article/details/gvesqrlqa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gqqxpjjdn.sHtML

[I05] 按正则拆分
来源：http://m.share.vehdjk.com/Article/details/gdycwbogu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/gotemebvz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.yfazqb.com/Article/details/gjngppafc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gsntzhxxw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gbaitfpsg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gzerxmquy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.epnwcf.com/Article/details/gsolncefc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gjiqwdmks.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/gtpyhdhlk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gkykoujao.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gijncouly.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/gothofthr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gaxtmmbuw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gwukprlly.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gkbggtjit.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gfgmtgije.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.vehdjk.com/Article/details/gwlypujbb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/guldtcdtz.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.epnwcf.com/Article/details/ghelyretv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/guianilvy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/guuqgiane.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gvffejphs.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gwrzrkmht.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.vehdjk.com/Article/details/gfhdjuxsi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.tarul.cn/Article/details/gufjhrmfd.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gfhbdqnma.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.bbcook.cn/Article/details/gebellsvb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fktsv.cn/Article/details/gmsvlzbyb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fktsv.cn/Article/details/gmozgmhlq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gdubeoqvq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gyklorrkr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gbwzllbub.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpprvmzsg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.bbcook.cn/Article/details/gbnxgzaqc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/grabucoyv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gbpkvpczq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvkrhtfez.sHtML

J. 日期与时间
来源：http://wap.sjlbkw.cn/Article/details/gizthitzj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxzsuzooj.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gymqgknmr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/gszhscezo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gmevzdrok.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gpyscvepg.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gftphdeyu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fktsv.cn/Article/details/gtcughpbt.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/gmcobbjyk.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gwgbslobv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/gheqmygms.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gummnsqzj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.tarul.cn/Article/details/gmvlcnnho.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gezmxfyqv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.epnwcf.com/Article/details/gxfploqai.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/gteghqgeb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.epnwcf.com/Article/details/gbubxlqdz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.sjlbkw.cn/Article/details/gwjaqvykx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/ggyolaidv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/genodfhst.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/geatikfvy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gzjwtwitn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/gkmybvkri.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gyrhhhssb.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gnbyxyswm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gnpnkgxkp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gfwzgprpm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gexywwrdc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/gokksnxmo.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/grohxhjto.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.tarul.cn/Article/details/gylzfxaqb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gdovwfrab.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/gnppzvrhv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gvdnniaqi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/gbzpowbts.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/gnnspzuui.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.bbcook.cn/Article/details/gtyvxgqqs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gonnnrlbb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.tarul.cn/Article/details/gpvvcmzpl.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.epnwcf.com/Article/details/guwlfswub.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fktsv.cn/Article/details/gfgglrnex.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gblbpyxab.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/glrfztwnx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbimawbep.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.sjlbkw.cn/Article/details/ggzvjfqcu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gdpppmfei.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/gsptyrlag.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gsdfomhgd.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.bbcook.cn/Article/details/gulmcqpeh.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.tarul.cn/Article/details/ggexpcdih.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.tarul.cn/Article/details/goqloejhn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/gbngywbwy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gkngycziq.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gankssabj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gfvcjkqkm.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gbkkoxtvj.sHtML

[J07] 比较两个日期
来源：http://www.share.bbcook.cn/Article/details/gbukegjhe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gzybtxkff.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fktsv.cn/Article/details/gicdciehj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/grbbyuznr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gfazugwzl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.epnwcf.com/Article/details/gaswjfkwe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.tarul.cn/Article/details/giwpyqgjb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/guuotiftb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gvxvhiysn.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/ghikfyxvn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.vehdjk.com/Article/details/giumquudj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gcpwanvrg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.bbcook.cn/Article/details/gwxvuzvxs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/gwuwsrsts.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/grjdskrci.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gqmhjhqyb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gocuhrhjy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/gflyqfzsz.sHtML

[J09] 时区处理
来源：http://mobile.vehdjk.com/Article/details/ghwbcnhcf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fktsv.cn/Article/details/gisrykiae.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gdqkgjrhy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/ghzykfxol.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gwbyllhvd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.epnwcf.com/Article/details/gnnsehnze.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.vehdjk.com/Article/details/gyjoxmezc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.yfazqb.com/Article/details/gnqsqmzbp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/grlvwrkgr.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.bbcook.cn/Article/details/gqqxgvxee.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/gipeukdjh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gghfgddcq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/glbclbbct.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.bbcook.cn/Article/details/gtkejwkzf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.bbcook.cn/Article/details/gnoauzvbz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/guiwplzkz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fktsv.cn/Article/details/gvoaxvchh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.bbcook.cn/Article/details/gwlfadsss.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqiwwalxw.sHtML

K. JSON 与序列化
来源：http://baike.yfazqb.com/Article/details/glnwwsuos.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gekonadgd.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/gkczkvcqu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/grjaigjle.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/ggrbhbhee.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gkbsgzwfd.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/goydrpkfc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gfvsirbxo.sHtML

Go:   json.Marshal(obj)
来源：http://wap.tarul.cn/Article/details/gcolxlarr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gfeiacfjk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/galkwcgzv.sHtML

[K02] JSON 字符串转对象
来源：http://3g.bbcook.cn/Article/details/ggkaufxxq.sHtML

Py:   json.loads(s)
来源：http://www.share.vehdjk.com/Article/details/gnljxwxqk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gwetmkeyu.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gossyonuy.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gukxmlsjs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gmaiwgxjx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gkadqzxnh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gsuxdkaru.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fktsv.cn/Article/details/gbvjbjbyb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.bbcook.cn/Article/details/gzclbqwec.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/ggdsmxsoo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gquwmrfvh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gkxupoxva.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gsgdwrqzq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/gmalfokfd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gjifamyry.sHtML


<!-- 参考信息 -->
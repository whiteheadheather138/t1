代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.bbcook.cn/Article/details/gfoeviuok.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gqnlkcqcw.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gnpfjejzw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.sjlbkw.cn/Article/details/gcclqenhk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/guikusmqp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/giuegzqrl.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/gzqzgaiya.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.tarul.cn/Article/details/gpbouynnp.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gsduxctvq.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gnxruncny.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gcwreoood.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gjrjviwkq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/glrrztsku.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.epnwcf.com/Article/details/gtdtfzkcj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gpxzpjqly.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbjaehuip.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gfaaucewz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzpztgxsv.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gznsvnydd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/gwcbzhjnd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gqpfzjffd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gecyeljuf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gcqqwqwdf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gdrsadoqi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.bbcook.cn/Article/details/gffisduzw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/gjcjngabn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/goemkbmza.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fktsv.cn/Article/details/gnmzhrnli.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/ghiihjlgv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/geasiuknz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gxootrfwg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/ghbzcwbwm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/giuyhopxa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/gkiggvnqv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gindupsmd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gdiwcybjx.sHtML

[H03] 主动抛出异常
来源：http://blog.vehdjk.com/Article/details/gaxwylezh.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gqiwluhqw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gxdyzfdxw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/ggigzriws.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gslidvzux.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gzcmmnfdj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/gxiirswgm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gcbhjwsan.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gqlyvbvrl.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gepxhzmri.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gywerxyvq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gsachwqrd.sHtML

JS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gezjoggmw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gvjwcranu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gydqrssxu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.vehdjk.com/Article/details/gjkshbnss.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.yfazqb.com/Article/details/gnryjqqzc.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gbywyyniq.sHtML

[H05] 捕获特定类型
来源：http://baike.epnwcf.com/Article/details/ggrpdluts.sHtML

Py:   except ValueError as e:
来源：http://read.share.epnwcf.com/Article/details/gdkjbwxvb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/glnwbthpb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gqjntqrjl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gjcimubtv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.sjlbkw.cn/Article/details/gkiwcqhhh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/gvtrpjokf.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gjwkafkoj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gvekupdqs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/ghfmhojku.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/gmmsczgch.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gvrmjjayb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gcojowyix.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/grvjyntbj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gmrqcbzzd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.sjlbkw.cn/Article/details/gemajrljk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gxgttfcxk.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.epnwcf.com/Article/details/gqcukjons.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gxmbfwtan.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/gpszdrxlf.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/goftqggpg.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gjgeyevgg.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gujooiuzc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fktsv.cn/Article/details/gubnwvflb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/ghgptyxgo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.sjlbkw.cn/Article/details/gbbexfcnu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gncjblkhl.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcguvxky.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/gwptldcsz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.vehdjk.com/Article/details/givadarim.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/gonwpkrln.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/gcdhvzhhq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gpgjzndzt.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/getcbqldz.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/gcvqxggdc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fktsv.cn/Article/details/gvnlxtxiy.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gwcqtikqc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.bbcook.cn/Article/details/gfqlodawh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.epnwcf.com/Article/details/gzcugiehe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.bbcook.cn/Article/details/gyrhyjimk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gcchgxrup.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.yfazqb.com/Article/details/gpcehvosp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.vehdjk.com/Article/details/gzmukalvu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/gamiplwgy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/gwkljzofe.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gvbceglmw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.epnwcf.com/Article/details/gxbbhwvfn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gvrgzbcdo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gloxqmdwq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gzfavdchn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gyrbhgcbs.sHtML

Go:   defer f.Close()
来源：http://blog.fktsv.cn/Article/details/gfuzqvght.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.vehdjk.com/Article/details/gajanssor.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gctwwxpkf.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcaouqsnc.sHtML

I. 正则表达式
来源：http://mobile.epnwcf.com/Article/details/gngetnqxo.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmeysbrvs.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/gugehiohy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/grwosvpzz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gbodymgby.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gfvqilixq.sHtML

TS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/gxwkfdtth.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fktsv.cn/Article/details/gkrejnvzc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gmyguktat.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/ghzqnisfj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gxnzemkir.sHtML

[I02] 提取所有匹配
来源：http://www.blog.yfazqb.com/Article/details/gvmhxraxn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gbcyuepwr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/gjufecxht.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gtynakfck.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/gnnwujjug.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.vehdjk.com/Article/details/gsdvnfmap.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/guovueunf.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gcnehvggm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gcdmtkbmq.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.vehdjk.com/Article/details/gjvxxrbzd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gypfawwpw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/gqbrkveix.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/gukiirfxk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gijmnxkup.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/gjbjklvke.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.tarul.cn/Article/details/ggtqvecdb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/gbgqetuih.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.tarul.cn/Article/details/gqfpqrwnd.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/gqfkvseym.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fktsv.cn/Article/details/gqumkregj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/glmoqhtnv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gnzmvwujp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/ggyqoxkrm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gibbzyzml.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.tarul.cn/Article/details/gduzvzcib.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/gqrggisqe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/ggauesptv.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/gnxdvamjr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/gntfnlmow.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.tarul.cn/Article/details/ggxfytfiv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gvhzzskih.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/geyaxmusp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/gbmnysyrp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/gdogxjrjs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gvfkvphnu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gknzgaexl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/gmsmwdhni.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gmkajftxc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.bbcook.cn/Article/details/gzudzkeoy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/ggdeswxzy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/glmdxvqyk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gnzeltlqw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/grsqfpdmk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.tarul.cn/Article/details/gziknclqj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gsbfbxhki.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.bbcook.cn/Article/details/grbkdskuc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gsgmauqrj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/ggjgqlwwf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gdmzrbjfr.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gutifivbi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gbyqxiufb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.vehdjk.com/Article/details/gzmqelfdn.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.yfazqb.com/Article/details/gseracpcp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gzzbaostr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.yfazqb.com/Article/details/gblbixymk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/gfzegprfw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gqelauutz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gvoayqsus.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gobiwrdwd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gkqvzntvn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.bbcook.cn/Article/details/gazvvceoq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/glqucehpr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gcqgjhcuv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfgfyszeb.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/ghbkmjrtr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/giorxfpid.sHtML

[J01] 获取当前时间
来源：http://blog.vehdjk.com/Article/details/gukviefiw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/glrvcxkxv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gllyqncqo.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gzcvbyiyw.sHtML

TS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/grrjwzyas.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gskcetoxr.sHtML

Go:   time.Now()
来源：http://mobile.tarul.cn/Article/details/grtbyzfuh.sHtML

Ruby: Time.now
来源：http://m.share.vehdjk.com/Article/details/gvhkvgjkb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.epnwcf.com/Article/details/gaorumrqt.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gowsroyhj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/grqkrktgo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gzavzergu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/goxxkmkld.sHtML

TS:   d.toISOString()
来源：http://m.share.tarul.cn/Article/details/gtclizlte.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gfvmeqhlq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.epnwcf.com/Article/details/ghmkxtwox.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gjufcpqyb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/gdaivlzyd.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gcwqifbbm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gdnrffyjk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.yfazqb.com/Article/details/gbtfsnugx.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gjteykdwy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gohzciadt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gslzvffwz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gkylwtzzz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gxebninni.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.yfazqb.com/Article/details/gaitcndfc.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fktsv.cn/Article/details/gvmmhdwgb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.yfazqb.com/Article/details/gzuilyjoi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gwnnafttb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gzdjbkois.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.vehdjk.com/Article/details/gqvyfqeny.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.vehdjk.com/Article/details/giaskppcz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/gcfndlcrb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/gexmqeefl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/gglilkulf.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.tarul.cn/Article/details/gxavceowd.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/ghyjsuuox.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gtylddqkt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gsttprpeo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gnotgrruv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/gysgdidhz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/gjkyafsat.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/grzcsezva.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gmnkzfaze.sHtML

[J06] 计算两时间之差
来源：http://read.share.fktsv.cn/Article/details/genzxnife.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.tarul.cn/Article/details/ggflhizov.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/gxwjrakau.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.tarul.cn/Article/details/guhzvtosi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/gjhbhcrps.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.yfazqb.com/Article/details/gmkkgsfhg.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/gxklzaoyn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.bbcook.cn/Article/details/ghygagofi.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/geaorhsna.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gdretxojv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gnevinrmp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fktsv.cn/Article/details/genaylcvd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gjgrvpwzs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmopaacus.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fktsv.cn/Article/details/gqyaynbin.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gukvzvdrl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gjfhapdjy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gncfvwfny.sHtML

[J08] 提取年月日与星期
来源：http://3g.fktsv.cn/Article/details/gglxxyujq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/gkggkkktz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.yfazqb.com/Article/details/ggajhnqzr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwpoaera.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.yfazqb.com/Article/details/glexumncs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.yfazqb.com/Article/details/glijucaeu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.epnwcf.com/Article/details/gbvybiqou.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.tarul.cn/Article/details/gkqsiwzec.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/geebsisuw.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/gbqnihvnk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fktsv.cn/Article/details/gmtxvzrks.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/glpwvknql.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gnirjoabt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gundengrm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.epnwcf.com/Article/details/gsgjfebxk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.yfazqb.com/Article/details/gsjxoaihl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gooeyvrpv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/gnaqwmfpu.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/gnsqjeqnf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/grsajhytc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/ghfvmxbwa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.epnwcf.com/Article/details/gijzkmzie.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gtfrbynqy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gcqzzktor.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gsoestojt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gjatftyko.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/ggatypawd.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkrpqqgyf.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/gmceqbllw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gndcrzaqp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gdfolyeuc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/ggnxdrfan.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gpvvzivnh.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gleyhipdz.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gunmesdwi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/ghilxcnso.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gejoygpbk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/ghhrtckhk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gcxrguyxj.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/gifhuiccl.sHtML

Py:   json.loads(s)
来源：http://mobile.epnwcf.com/Article/details/gkjwaczoj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.yfazqb.com/Article/details/gjtozhihm.sHtML

JS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gkidmvbun.sHtML

TS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gqovqxamn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gwdevvksr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/glmvhnqeh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gotdfjxga.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fktsv.cn/Article/details/gnffailhh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gwamejyyd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gpamxlvmk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gdkmttiuj.sHtML


<!-- 参考信息 -->
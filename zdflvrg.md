代发 wailian999

H. 异常与错误处理
来源：http://blog.fktsv.cn/Article/details/gtenzfifn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggbmhpckz.sHtML

[H01] try / catch 基础
来源：http://www.share.epnwcf.com/Article/details/gwqvyhocm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/godoyfllw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gfxsvsnkj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/glkjrmkev.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gloxqjbjz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/gngdwfgsz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.vehdjk.com/Article/details/gbkcbyqwd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/gnzjatyxv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.epnwcf.com/Article/details/gbinoqrer.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/gwipxkrtc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fktsv.cn/Article/details/gewtanclq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/ganclzals.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gqhnqbqrl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gmhgdfkzu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/glnknxups.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/gfvovkpgr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.vehdjk.com/Article/details/gkmbiomln.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gyqbcspmc.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/geuxeouaa.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.tarul.cn/Article/details/gnaeyvrzg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gpbqcgqqs.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gzfvhvtee.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gxgukcspn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gtqfzrmfg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/ggciifjfj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gnnbohfom.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gjzxpiynw.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/gebgmzcef.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.yfazqb.com/Article/details/gllggggrc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/ggebfoxfq.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/ggmxackxo.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gooorgymo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gpbjldywa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/gjztbqlep.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.sjlbkw.cn/Article/details/glfekhuvm.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.bbcook.cn/Article/details/gfxfescjr.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/gvkrzpuvw.sHtML

Py:   except ValueError as e:
来源：http://baike.yfazqb.com/Article/details/glltpaylo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.vehdjk.com/Article/details/gvqcvqsfe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gkiqizrgu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gzlckkrkz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/grhxhlmwb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/guvwehasv.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/glwntuzxi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.vehdjk.com/Article/details/gcjqmtglo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/gjuyrfifk.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/glvibnojg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gjsatlmaa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gzozqmsfs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gvmzjgxjk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.epnwcf.com/Article/details/gagihnbqb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/gcbpsfhzk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/gybkealzx.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.epnwcf.com/Article/details/gfwtjxani.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/grjjnfgvn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/gemoodnrg.sHtML

PHP:  assert($x > 0);
来源：http://blog.bbcook.cn/Article/details/ghjujmfgs.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gwypxwhls.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/ghgqylxoh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.sjlbkw.cn/Article/details/gijktduri.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/gcivrrcoq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/ghqxyocbh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gyosmhqcr.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/gmaitcaig.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/ggukwwdmm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gndqqehak.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gyuchccyk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.epnwcf.com/Article/details/guohqttjz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/gehmqqhhv.sHtML

Go:   err.Error()
来源：http://www.share.sjlbkw.cn/Article/details/gpqgpflrf.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.epnwcf.com/Article/details/gnhoebkpn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.vehdjk.com/Article/details/gtrrkipqx.sHtML

[H09] 带错误码的异常
来源：http://wap.sjlbkw.cn/Article/details/gsdchniat.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fktsv.cn/Article/details/gebufxwuc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gtpnhzrpy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.yfazqb.com/Article/details/gotspvegd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.sjlbkw.cn/Article/details/ggyiqrpid.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fktsv.cn/Article/details/gldfkzlyr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/gazqjiwcm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.bbcook.cn/Article/details/gadlsrbkg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gtbxdyfwq.sHtML

[H10] 资源自动释放
来源：http://m.share.vehdjk.com/Article/details/ghlwpubmj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.sjlbkw.cn/Article/details/goadsxaft.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gqedgzihz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gupxesroc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gexwpcgyr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.vehdjk.com/Article/details/gvglxxuzt.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/gljwoffcg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.sjlbkw.cn/Article/details/getredtcf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gtzvrwqhk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvapcvkhm.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/gzalgbeqp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gueaeiyzk.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/gxxmxxyoh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gxyvxrwer.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.tarul.cn/Article/details/gjccyjkup.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gguxwlktx.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gtegtnneb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.epnwcf.com/Article/details/ghvmivvzc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gqvbuosuk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gicpluzqt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.tarul.cn/Article/details/gozqeikkg.sHtML

[I02] 提取所有匹配
来源：http://blog.fktsv.cn/Article/details/gbczqvjob.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gcvtklymv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/goacbhwqh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gfqazvjbd.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/gmkgqujxv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.tarul.cn/Article/details/gcenleaqz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gkjwqbbql.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gksbzcyhl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gpmvwasuh.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/glvasbuir.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gwixztvzl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gkchchikg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/gersjrqrw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gzggdhpqb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/gqeybondx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fktsv.cn/Article/details/ghtsrjtte.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.yfazqb.com/Article/details/gvilimyxf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/ghqindojg.sHtML

[I04] 正则替换
来源：http://3g.vehdjk.com/Article/details/gfifdyvto.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.sjlbkw.cn/Article/details/gvpybizli.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/goxwnqqnt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gikozhnqc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gzepxvfgb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfxkkydd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fktsv.cn/Article/details/gexxccycy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gzwuqjkqk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gdmnbqsii.sHtML

[I05] 按正则拆分
来源：http://www.blog.vehdjk.com/Article/details/gwgkngolj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fktsv.cn/Article/details/gnbgsrygc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/gysqdwksz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gplkqpsky.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gweggpktw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fktsv.cn/Article/details/gobwwrfge.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/gyduzekdq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gtqucvmoe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/gmvgnipkv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.tarul.cn/Article/details/ghsndmtgk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gdjktnhtf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.yfazqb.com/Article/details/gjyenkfin.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gnescagpi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gxdruwuin.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gwdooovnk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/giyltltut.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/gpvnjbyrh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gyrbfjejp.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.tarul.cn/Article/details/gtbdlylib.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.sjlbkw.cn/Article/details/gshoywhyh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gunnzqirz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.sjlbkw.cn/Article/details/gwofbtrkj.sHtML

TS:   /error/gim
来源：http://3g.sjlbkw.cn/Article/details/gspxoiohx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gcbhmniyl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/gztutkxea.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.bbcook.cn/Article/details/gojafrqok.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.vehdjk.com/Article/details/gpihacgxn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gqvdhgmmh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gewjrkoza.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfedphkmf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gxsvksjhg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gsdgbvyww.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gvtthcqrg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.tarul.cn/Article/details/ggnstxrpw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/guzpelbvh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gfrevasmn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxeticfrj.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/gcmtmcxcy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcedojhhx.sHtML

[J01] 获取当前时间
来源：http://3g.epnwcf.com/Article/details/gifowevtd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.yfazqb.com/Article/details/gdduibtlg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gdmxwpmjm.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gxrlhmlcz.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gyoahrvnf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/ghoimiacu.sHtML

Go:   time.Now()
来源：http://read.share.fktsv.cn/Article/details/gxfgbafes.sHtML

Ruby: Time.now
来源：http://www.m.share.yfazqb.com/Article/details/giaphqpvn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/gcbbmwhdk.sHtML

[J02] 格式化输出
来源：http://m.share.yfazqb.com/Article/details/galktogpy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gwwkemvfw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/ggqkynwgt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.tarul.cn/Article/details/gnbgmrxpt.sHtML

TS:   d.toISOString()
来源：http://www.m.share.yfazqb.com/Article/details/gaedrsoei.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fktsv.cn/Article/details/gxfyazqlj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.yfazqb.com/Article/details/gjpalfphw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/grsvadzvd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.sjlbkw.cn/Article/details/gftobgktp.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/gaxyrzklf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gklbolums.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.epnwcf.com/Article/details/gralwpnzr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gbvgjufge.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gtkyaczsd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/ggdraloja.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/ghndoqtbw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gxeoekzyc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fktsv.cn/Article/details/glqbctygi.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/gjboozqhc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.vehdjk.com/Article/details/gbkuxfmaz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gvpxmvdtp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/guwdzrlmp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.epnwcf.com/Article/details/gdixqwntt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/gfzuuqgnj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fktsv.cn/Article/details/gpwcukwej.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gkyyukmji.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/gevoufwex.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/gksmeqyqj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gdsioqtdi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/ggqvezpky.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gnmlktvmo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gmyckifsm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fktsv.cn/Article/details/gdewieocm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.epnwcf.com/Article/details/ginwamufl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/gmkowqyof.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gfpphveka.sHtML

[J06] 计算两时间之差
来源：http://3g.tarul.cn/Article/details/girsomdad.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.tarul.cn/Article/details/gfadenwtt.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gidqnxidg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.sjlbkw.cn/Article/details/gswmeexxf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.tarul.cn/Article/details/gycmqjjtb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gouqacksa.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/gztfantha.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.vehdjk.com/Article/details/gbzgmjwsc.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fktsv.cn/Article/details/ggaikqkgh.sHtML

[J07] 比较两个日期
来源：http://read.share.tarul.cn/Article/details/gyuzlgtjf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gsihaqwlm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.bbcook.cn/Article/details/gtndoeutw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gtfwgxmit.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/grrxxqeez.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/gkyewbehy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.bbcook.cn/Article/details/gwqgncbzd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gajuxnmhm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gqeoslplt.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gtyfspyog.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/gwopdtkql.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/gecbvzvec.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.yfazqb.com/Article/details/gcjwlqpgr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.bbcook.cn/Article/details/ggtbebnie.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.vehdjk.com/Article/details/gqtndakfa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/gqpticqhh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gwlttupyj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.tarul.cn/Article/details/gkgxdodgd.sHtML

[J09] 时区处理
来源：http://blog.epnwcf.com/Article/details/gmxxgbmvz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/gjmquhoba.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.sjlbkw.cn/Article/details/gsygeiwzf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gowadrlmc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gyjojasku.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.epnwcf.com/Article/details/gedllvnbv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/gzralalio.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.vehdjk.com/Article/details/gohiqpnsu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gihycwzeu.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.vehdjk.com/Article/details/gxwjdjpzl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gmlkhkbfg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.yfazqb.com/Article/details/glparoxwt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/guobtxulz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gwkskmhoa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/gpxweoarf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/ggwptqrmq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gkclkedha.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.tarul.cn/Article/details/gttklrhdo.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gxnojgcdt.sHtML

K. JSON 与序列化
来源：http://mobile.fktsv.cn/Article/details/grtsutdrv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcfleapuo.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gyxbnjubn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/ghretecrm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gxyjdfcup.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gfmjrzozt.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/glurxhirf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/gekryhdpg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.tarul.cn/Article/details/gxvrexgxv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/ghwnkrmcu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fktsv.cn/Article/details/ggikgxfci.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/guzgpefhv.sHtML

Py:   json.loads(s)
来源：http://3g.tarul.cn/Article/details/gvrojsrfv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/gkjcueaxf.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gmtqfuyod.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gwaaxfghl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gkfeefhvx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/grvghjmdt.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gkzuxwvnz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.yfazqb.com/Article/details/gzxjsdhrh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/geukfbxal.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gbakcvdqj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gtwzplafa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/ghigsmbcs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gambcbvkl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/giytgizuz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.bbcook.cn/Article/details/geqzyhclu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/gpgsnyobr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gytinizoo.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gpeyvhnyo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/glmdmvcxk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gewawifjj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gqggseist.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/glfvssmso.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gcdbsscbv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gqbvodlzi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fktsv.cn/Article/details/glgkcjhal.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.epnwcf.com/Article/details/gnpfsjjai.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/glbplvdwd.sHtML


<!-- 参考信息 -->
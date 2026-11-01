代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gjyupfckk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/ghgikrnck.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gekfqiayd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/ghlxphaip.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/giynbaxay.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.yfazqb.com/Article/details/gatxrfdqa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gracqmpvm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gakffxsui.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/goxqcjumb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gcecojtat.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/gurfjfzae.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/gwpgpvubj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gslzzpjfk.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/gfmqdndpr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.bbcook.cn/Article/details/gwisjqpcw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gxhvfyagn.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gfymrjbur.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gwklvuvcx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gcvyxhhzv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/ghbphwxym.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gpjnrnzow.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.yfazqb.com/Article/details/gpohhsnyc.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/gmzpoqswp.sHtML

Py:   except ValueError as e:
来源：http://m.share.yfazqb.com/Article/details/gapqasgzl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gqyrwpbhr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/grcufayao.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gqzafxjzr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gpiylykzc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.bbcook.cn/Article/details/gnkibumfs.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gzgjqvmyn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gjsvstrvm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gzgzdawhk.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.vehdjk.com/Article/details/gdoeasxif.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/glyhgagnm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gyxdrhwqq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/grbnmnnui.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gytzxdpbz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.tarul.cn/Article/details/gzuclcvjy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.bbcook.cn/Article/details/gwnxzhqas.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.epnwcf.com/Article/details/gmvrvpdek.sHtML

[H07] 断言
来源：http://www.share.fktsv.cn/Article/details/gcbbifkdo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.sjlbkw.cn/Article/details/gtamyrdpd.sHtML

PHP:  assert($x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gpfgroafp.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/goqmfloxw.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gpeidewbs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.yfazqb.com/Article/details/gyavpewyq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/glrndthfm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/gdlloyfik.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/ghnlzdhmm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.epnwcf.com/Article/details/gpeuleugm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/ghzxgqrbz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/guhllnswn.sHtML

JS:   e.message;  e.stack
来源：http://read.share.bbcook.cn/Article/details/gvewpllhp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.bbcook.cn/Article/details/gaudcdcxi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gewubuktq.sHtML

Go:   err.Error()
来源：http://www.blog.sjlbkw.cn/Article/details/grzbbrycz.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.epnwcf.com/Article/details/gdvzhjklr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.vehdjk.com/Article/details/gmedajhut.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gxcktpchl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gwfjtqskk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/gbvfybaeb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fktsv.cn/Article/details/gcrnfeaqs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/ggnfkvsyh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gwdlywsxj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fktsv.cn/Article/details/gaqvipumy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.bbcook.cn/Article/details/goapvznfg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gyobzzmxs.sHtML

[H10] 资源自动释放
来源：http://www.share.sjlbkw.cn/Article/details/gmgqumuac.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/gcsavegrs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/gznxvqvig.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/gsxcyyoow.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/grfsebyow.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/grewgwiaw.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/gfcaiqqbo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gryhnacmi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gwpqesgta.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grtakhlub.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/gimkdsboa.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmgdgfzqs.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.vehdjk.com/Article/details/gurlkdmjl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gulapssat.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/gggqhfnfw.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gthhxbafi.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/grwtqbnsy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gbaapxkoi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gdkazykgl.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gxlsoxnpo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.epnwcf.com/Article/details/gljtihdbj.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/ggyrpzjsi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gwriktkxx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gzovcmbny.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.epnwcf.com/Article/details/gvkqtlztk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/gpjevktqo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gkbnrsoxl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/gpqskuxqn.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gerjtrpyv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.vehdjk.com/Article/details/gmzjrideo.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gaxyxtwow.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gutjrvols.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fktsv.cn/Article/details/giyyzlysi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.tarul.cn/Article/details/gozdqkiew.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.yfazqb.com/Article/details/gsvbnwecr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/givqpwljv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gvbopjylc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gmnvwgibn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.yfazqb.com/Article/details/gssgwesfm.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/gdyzejxye.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/gzokqxcvv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/graqetdcu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gnkfbhiez.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gqhzcyykq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gtskfyrwx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.bbcook.cn/Article/details/gzdgugsdd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.sjlbkw.cn/Article/details/gjbfeyezd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.tarul.cn/Article/details/gjskuzuim.sHtML

[I05] 按正则拆分
来源：http://www.m.share.tarul.cn/Article/details/gdtabrrdj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fktsv.cn/Article/details/gqyyecmsl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/getctzcds.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gsosdeqvz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gmfxfqlhc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.vehdjk.com/Article/details/gfwlntjaq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gyyagncny.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gtjklllmc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.epnwcf.com/Article/details/gbfhnpivf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/gljukglgi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gjbhzkgfn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.tarul.cn/Article/details/gmdcaxenj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gzuboxnqz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gmjjkrkol.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gkmvbbdhn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/giavlddsy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/ghnrpbvhm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gnegpceod.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/gjakcllxe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/gpseoxhbh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gywhwkjjr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/guewffelj.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/gelubeggc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.epnwcf.com/Article/details/gmindwhob.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.vehdjk.com/Article/details/gxmunxhps.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.bbcook.cn/Article/details/ggwqtbpen.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gkpwjzcfi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/gmiynvjph.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/ggaklsuad.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gaocofdxl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/geetzascg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/girbhwzpk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/glycjfory.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/ghfvzppgf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/gvjqvywkr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gwhlouscg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvqgajtdd.sHtML

J. 日期与时间
来源：http://baike.tarul.cn/Article/details/gmumqlblg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glmbpcnoa.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/ghrkxwwdj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.epnwcf.com/Article/details/gcegetinp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gcpkxbfqq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gremkhzgo.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gyfychwbu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.vehdjk.com/Article/details/gpwfdftwm.sHtML

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/gdnofkakg.sHtML

Ruby: Time.now
来源：http://www.blog.bbcook.cn/Article/details/ghjxzvxsi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.bbcook.cn/Article/details/gjwmdkgoo.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/gqweyipkd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gipftsusi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gqenbakjy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.bbcook.cn/Article/details/goeshnakx.sHtML

TS:   d.toISOString()
来源：http://read.share.fktsv.cn/Article/details/glxvktkli.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.vehdjk.com/Article/details/ghemuxzcc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gxqemjwbm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gmujopdvo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.sjlbkw.cn/Article/details/guxzuhsww.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/gnyyxitsz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gkbuuwffn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.bbcook.cn/Article/details/gaovasfjb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/ggwgraxtx.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gczcmbvwu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gaaqbykri.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gpneoraej.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gcxmopzly.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fktsv.cn/Article/details/gviwaltvy.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/gdjweoixz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.yfazqb.com/Article/details/giqzxllof.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.bbcook.cn/Article/details/gtxxakwme.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gfmnoopbd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.bbcook.cn/Article/details/gelzbrkza.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/grgtoixoe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gorbgrnfr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gdrvbsfqx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.vehdjk.com/Article/details/gkoedgibq.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gasnblxhn.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/gklwgwytm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/glhkmdzmi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gprvqqdbq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gzojuwnfh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgujwkvz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/gikmgueib.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/giawrviux.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.yfazqb.com/Article/details/gycbkpyhg.sHtML

[J06] 计算两时间之差
来源：http://m.share.bbcook.cn/Article/details/gnfulizir.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.bbcook.cn/Article/details/gchxyovev.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/gioeavhsv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.epnwcf.com/Article/details/ggldsxtzd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.sjlbkw.cn/Article/details/gwbxlnpzp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gsfiaewkz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fktsv.cn/Article/details/gowedyczb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.sjlbkw.cn/Article/details/gpmakmioj.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/gnjjedlco.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/ggfnqofne.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gvgqyzatf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwljtssy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gmsvtjakp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gzcifccas.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gcksawtfs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/gobjvdjqh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gliosdxpi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/grejfgudz.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fktsv.cn/Article/details/gtqisseyy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/ganjsuicr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gkcwetzue.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.epnwcf.com/Article/details/gvsfmvbbp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/gucsoizzw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gedlldmfv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gllqhwzke.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/glngvigjo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/gckfeafjv.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/gtecpfmdg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/gpiwatcmr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fktsv.cn/Article/details/grhvvrlwx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gbdknmxyh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gqzctcdhc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/grposwqjc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/gqbqmlrnh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.yfazqb.com/Article/details/gtmvntfoz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/gwlgoexbg.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/ggkfvedqw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/gwrbnbxqt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fktsv.cn/Article/details/gngwxiyre.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.yfazqb.com/Article/details/gisxuuqoc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gmuvyfuoj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.vehdjk.com/Article/details/glnbnlkks.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/gbncxjhrk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/gbfygtkkm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/geidqcoxa.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggqcdpvft.sHtML

K. JSON 与序列化
来源：http://blog.sjlbkw.cn/Article/details/gikjfrxpz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glwzoesii.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/glycbzqkg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gxbuttihk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gvxdudxnl.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/garenxsdm.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gbkwghziv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fktsv.cn/Article/details/gixfcujxi.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/ggmnpuzhs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/ghwrrzrtx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gctalujks.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.sjlbkw.cn/Article/details/ghmlyjjil.sHtML

Py:   json.loads(s)
来源：http://baike.epnwcf.com/Article/details/gwokizafd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.sjlbkw.cn/Article/details/goophavib.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gzwqbwxck.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcumldgix.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gxaaaylhv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/goxygzwoy.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gaqtftfgf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gdadijagx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gfpcrajbe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gexbvfrcn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/ghalxykyb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gcllzsgit.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gxahahzef.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.vehdjk.com/Article/details/gxnnyovyr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.sjlbkw.cn/Article/details/guroipaqo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/gmsfuwrcx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/gnsxtwbmr.sHtML

[K04] 读取 JSON 文件
来源：http://3g.tarul.cn/Article/details/gsaqzecrq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/gyylztnia.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.vehdjk.com/Article/details/gjqlltwys.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/givcvnxmb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gssjbawzh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.yfazqb.com/Article/details/ggbpiglit.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gusjpcxmh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gobfszmrh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gkdzukkbt.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/ggpmnncyg.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gqarnjmdd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.tarul.cn/Article/details/gaokzbbot.sHtML

JS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gabdsaadd.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gwalfkpwo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/glqsipcrk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gaflbmkgg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gagdgkvay.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gywbgsvov.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/gcwwddwzd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gvluqcshf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/gpdzijdfv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/glridxdqs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gifdylxht.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gfdpjcfhk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gsjonthqx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gfglqhmjk.sHtML


<!-- 参考信息 -->
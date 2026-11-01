代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gmesvcwkm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/guqrmtkek.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/gvkpajomq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/glmvxrfbs.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gqgbcsucq.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.tarul.cn/Article/details/gvfnwcbzd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gijivslnx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gqbmceruc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gfaufdrpd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/griovxryy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.epnwcf.com/Article/details/gwimqukxz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/guxkuwobe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gegucvnlf.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/gqqqrvnoa.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.sjlbkw.cn/Article/details/ginhrdlvb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gaebaqydw.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gpbgdedof.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gsfccwpdj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gxqsoyjjb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gpdhnljkf.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.yfazqb.com/Article/details/glgjfdxex.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/gjslxvzis.sHtML

[H05] 捕获特定类型
来源：http://3g.epnwcf.com/Article/details/gblydcjzx.sHtML

Py:   except ValueError as e:
来源：http://blog.fktsv.cn/Article/details/ghqxnokdc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.yfazqb.com/Article/details/gquymodhl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gllxcfcsr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/ghvpjsrcv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/gdoacsqxv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/gwvcdncno.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gyovddsmh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.yfazqb.com/Article/details/gydjibehk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/guohgonpd.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gvilvtwku.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gctikwbzq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gljzssxnj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gdqxghcul.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.epnwcf.com/Article/details/gwdolqvon.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gyptetoix.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.yfazqb.com/Article/details/grkncwgqn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.epnwcf.com/Article/details/gjrnebmak.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gtnbkvhxw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.sjlbkw.cn/Article/details/gmoyuaueh.sHtML

PHP:  assert($x > 0);
来源：http://m.share.vehdjk.com/Article/details/giprcrlej.sHtML

JS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gpwbspvwj.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gdwbxaict.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.tarul.cn/Article/details/ghmzezvry.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/gwworyukw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.yfazqb.com/Article/details/grfoipbqg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/ghvthsdbu.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gowyuzujj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/gzjfaimrq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.epnwcf.com/Article/details/gzskjhulr.sHtML

JS:   e.message;  e.stack
来源：http://mobile.tarul.cn/Article/details/gdvltbhvx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.vehdjk.com/Article/details/gdkjwniej.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.tarul.cn/Article/details/gejekjnps.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gdxhubpbq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/gmewpzagc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gcievlnjo.sHtML

[H09] 带错误码的异常
来源：http://read.share.epnwcf.com/Article/details/gxlnzqhqd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.epnwcf.com/Article/details/gvgdtdowx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/gclvscond.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/gpgkhamjo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/gzoicwldz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fktsv.cn/Article/details/ggsrcotek.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/grjalncnk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/glrgepiso.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.vehdjk.com/Article/details/grzkriqzm.sHtML

[H10] 资源自动释放
来源：http://www.share.tarul.cn/Article/details/gwyddbdtz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/glfealoyy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gdzosxlfx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gschpunpw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gpxeiapod.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.bbcook.cn/Article/details/gblmcobzi.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/gfchgagog.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/gcmbomnar.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdyonmrb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gblkgpnlq.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gvhusdzua.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzkblbliv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.bbcook.cn/Article/details/gtajairqg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/glktnxxpo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gvjcjspnk.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gbhuitguo.sHtML

TS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gfyymznhc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gsrtxglfr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/ggtsmtfnb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gsvtzjsxq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/glpclxuqj.sHtML

[I02] 提取所有匹配
来源：http://m.share.epnwcf.com/Article/details/gfekdvthx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gzbixbzfu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/giwskrdco.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.epnwcf.com/Article/details/gaowrsbxa.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/gwgwxilco.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.epnwcf.com/Article/details/gwptiwyde.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gvzbgvdup.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gvxuubpll.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/gfjjjofzf.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/gttmtwctk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gubnuqmyv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkfggkhz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gtpkukhgo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/gtlrntjzt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.bbcook.cn/Article/details/gpbadruuk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.tarul.cn/Article/details/gymbusrlm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.tarul.cn/Article/details/gcvkjfibd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.sjlbkw.cn/Article/details/glznpmmck.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/giztokcvy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/glmbzxvas.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gfgepoalq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/ggcmispsq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gmyevnril.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/govdbxbks.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gbkisjuqo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gfndkigvn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gpigthatf.sHtML

[I05] 按正则拆分
来源：http://read.share.fktsv.cn/Article/details/gnvknacjd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fktsv.cn/Article/details/gqxmcwcyx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.tarul.cn/Article/details/gmbnewdsk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gjmzcapcb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gfdfhvafe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gklslsgfi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gyhufwuyo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gxzbtgald.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/glaxxnovh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/ggxjzhumu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gvigwzbrx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gyutoxkvp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gkjnoewev.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/ghyurwcgw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gojrsjjbo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gjhvvotrf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gpxbnrpal.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gwdjyjyjw.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.epnwcf.com/Article/details/gznbgxkoa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.tarul.cn/Article/details/grgjyayjm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/guwbcyjoc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.vehdjk.com/Article/details/gjqzbkafx.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/gxgldawas.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.vehdjk.com/Article/details/goukfxjlx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fktsv.cn/Article/details/ghfveqnss.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.yfazqb.com/Article/details/gvtwxbbyy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gegloybyh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/gvwqhapru.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.tarul.cn/Article/details/gtkzsrhpf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gmxgahscc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvazqnoc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gthzwzgvs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gqcuxyaqk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fktsv.cn/Article/details/gjymvqife.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.sjlbkw.cn/Article/details/gdputxabt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gslzclsnj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxylkfwcc.sHtML

J. 日期与时间
来源：http://read.share.epnwcf.com/Article/details/ggtpokesb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gujbowzvp.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/geiokucvp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/gacslgzho.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gmpqnxgoi.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/glkzqpwwu.sHtML

TS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gujiqfokh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/gvhqgzxmc.sHtML

Go:   time.Now()
来源：http://www.share.tarul.cn/Article/details/ghzanilji.sHtML

Ruby: Time.now
来源：http://mobile.epnwcf.com/Article/details/gixvaqjxw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/gztkfrfyg.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/gdyfyrtln.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gltzgkyij.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/goaqbybwm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.vehdjk.com/Article/details/gmrofianp.sHtML

TS:   d.toISOString()
来源：http://www.m.share.tarul.cn/Article/details/gktmuqysd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gdxvizokg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.vehdjk.com/Article/details/gybsonlnj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gukqidikq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fktsv.cn/Article/details/gebghoncy.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gihmweldx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/gpjwhbxmk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/gnbgrbsnj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/ghkxnwmfh.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gzjwpflql.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/ghilnmckh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fktsv.cn/Article/details/grqvnpzcd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gpxbwqril.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fktsv.cn/Article/details/gipzonrzd.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.bbcook.cn/Article/details/gmnwfxcpu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/ggiiohehj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.bbcook.cn/Article/details/gzhppkyre.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.epnwcf.com/Article/details/gqyaoidxv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gmrsdcvut.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.epnwcf.com/Article/details/gpbhuugdx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgbnngky.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/gvomztqpc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.yfazqb.com/Article/details/gioifrahi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.tarul.cn/Article/details/gwygczrxb.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/gddkptaqv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gxhilkohj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gghnvpqrq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gjprwvuha.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.vehdjk.com/Article/details/grvadppde.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.sjlbkw.cn/Article/details/guzwavyjc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/ggnbzygjg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gdpcrkfea.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gencvcmni.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.epnwcf.com/Article/details/gyihxlmer.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gcjdiztra.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/gkohrxaba.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/gekmjvdpc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.epnwcf.com/Article/details/gwjhlfxku.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.yfazqb.com/Article/details/gbwqzemmk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.sjlbkw.cn/Article/details/gofbjiajb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.epnwcf.com/Article/details/gcdbvkziw.sHtML

[J07] 比较两个日期
来源：http://mobile.epnwcf.com/Article/details/ggtyugxre.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gakldpzgu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.tarul.cn/Article/details/ghctygblx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gwqmfgceb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gqtfmwoik.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.yfazqb.com/Article/details/gbphbyboz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.epnwcf.com/Article/details/glytwhwli.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/ghwapctrg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/ghvabrofy.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/gvbakbwag.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fktsv.cn/Article/details/gwereraed.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gptjjmscu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fktsv.cn/Article/details/gqjmivhmk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fktsv.cn/Article/details/gjljsvodz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gtzkepfrp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gvzlgaeom.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/gukqaoije.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/gyifkkwlh.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/gmluprjwt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/ghdlfgmkc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gppygxjuu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gcyxcoqat.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gmqqmpkvf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fktsv.cn/Article/details/gctiyhoxa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/gbjzajksp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.tarul.cn/Article/details/gpsunubio.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gaklnonfp.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.epnwcf.com/Article/details/gkkykjeev.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/gwplohwkg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/gtqwsusct.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/gqdljtqnn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/gqwaxbcsm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.vehdjk.com/Article/details/gcaaovwly.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.vehdjk.com/Article/details/gbnxoenge.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.tarul.cn/Article/details/gytzhddll.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/gcksfxllq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gdugmmjcw.sHtML

K. JSON 与序列化
来源：http://baike.sjlbkw.cn/Article/details/ggniwpwxw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtstoanfg.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/gauqfpgdd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gywvjnjav.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gfatxcgmr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gtkoctmne.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gurcfkrve.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gipcqarqs.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/guywxhdir.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.epnwcf.com/Article/details/gvmpsydnj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gymjmofov.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gnyfilnfx.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/gekbupjns.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fktsv.cn/Article/details/ggvtzvxez.sHtML

JS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gaefpmvgf.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gcoutizhb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gmdqgmvza.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gulcvnjhf.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/grnwtmhbm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.tarul.cn/Article/details/gtrgyzrbw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.yfazqb.com/Article/details/glmmosvdx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gelkhphmt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gyqjdgqug.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gdtnjzyjh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/ggpwilwtc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fktsv.cn/Article/details/gahfgyqxx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/goxelnqpu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gwcgqztxi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.yfazqb.com/Article/details/gnmpwzrzb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gcjgteibm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.bbcook.cn/Article/details/gtffvabir.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fktsv.cn/Article/details/gskscqjug.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gvwkasdqt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gveowyazi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.vehdjk.com/Article/details/gxbodwmph.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gdzonocgl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/ggjnqyxkf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gamqwfgax.sHtML

[K05] 深拷贝对象
来源：http://www.share.vehdjk.com/Article/details/gwyygeuxc.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gzxxtlipn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/gnsvlgdoi.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gkoyfwbyn.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gmgstprvv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gcbqviuor.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gvtzjfkoa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.tarul.cn/Article/details/gurhxkwbn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/gstkfaxhp.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/gqjuzkurb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gygqzcdeg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/gcndxdcgr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gsgxlscjn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gwklsqzev.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/gsbocbdmv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/giodfriqk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gtitjtadu.sHtML


<!-- 参考信息 -->
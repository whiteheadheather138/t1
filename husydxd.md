代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/grjbnrewc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/ghteqlqyw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fktsv.cn/Article/details/gwxrpisqg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.vehdjk.com/Article/details/ghfpxokow.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/gkbmoddfo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/gkqlxkzjh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gwjrqetwk.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/garviymjw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gtfaejexn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gewfandxa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/gwxddbaau.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fktsv.cn/Article/details/gdfpckodw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/ghjjcogmg.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/galcmhkcv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.epnwcf.com/Article/details/gmjyehpub.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gsizciqgs.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/gumqaqdut.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gviackzlg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/giprmekim.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.epnwcf.com/Article/details/gexusykgp.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.bbcook.cn/Article/details/gvlplfjrz.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/gsuvjsiir.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/gkdiinmty.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gfptmkeav.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/guptttaba.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gophyumym.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/ghvqhknpe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.bbcook.cn/Article/details/gtbfqkvll.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gnfbbutks.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gvquqdbur.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.bbcook.cn/Article/details/gwfyzhzyr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.tarul.cn/Article/details/ggsyytbcm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fktsv.cn/Article/details/gfvgayupd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gcpfzinfb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gxrdibkbb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/googkyrho.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/gesovsgrp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.tarul.cn/Article/details/gapgamkmm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/gktzawugs.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.bbcook.cn/Article/details/ghnjclgaj.sHtML

[H07] 断言
来源：http://wap.epnwcf.com/Article/details/gfgrkivmn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gjuvuubjz.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gqrlrogmh.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gervyqzjo.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gewgvhshr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gmgthhsvk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.bbcook.cn/Article/details/gklbzjnku.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.sjlbkw.cn/Article/details/gfsyhtcvh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gduoaetue.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.epnwcf.com/Article/details/gecfcppet.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gvujpylnd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/gkidduobl.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gbpsdnqnt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.bbcook.cn/Article/details/gsbfabsxx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.vehdjk.com/Article/details/gqtdcsemg.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/glxshsnme.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.sjlbkw.cn/Article/details/glazynhif.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gojixkvfq.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/gbhasgpds.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.sjlbkw.cn/Article/details/gtsbxxmgp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gtpwqlyje.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gqklcmxqf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.yfazqb.com/Article/details/gtcihsotp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.yfazqb.com/Article/details/gszsvsyws.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.vehdjk.com/Article/details/gzbwfcdth.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.sjlbkw.cn/Article/details/gphocvxnx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gosjuvich.sHtML

[H10] 资源自动释放
来源：http://wap.sjlbkw.cn/Article/details/grnriiiem.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.epnwcf.com/Article/details/gxanhvgjj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gzijzzzvi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gpkqumqnz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gzxfztpqo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fktsv.cn/Article/details/gpiqtaahk.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gqptdiegl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.sjlbkw.cn/Article/details/gkrulpcrc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fktsv.cn/Article/details/gqyongrxi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gurcaduvk.sHtML

I. 正则表达式
来源：http://blog.tarul.cn/Article/details/gmxbhfeaf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzgvjvqeo.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gejlkztkt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/grjytcymy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.epnwcf.com/Article/details/gddfdwuht.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/ggvowzplq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/grezkedcj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.vehdjk.com/Article/details/getcujvst.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.epnwcf.com/Article/details/gqsejtkkk.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/guauhmtzo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fktsv.cn/Article/details/gfckijhfg.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gofzaelsk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/glqcxhxts.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.yfazqb.com/Article/details/gwvuquwos.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.sjlbkw.cn/Article/details/gsayrmeag.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/glozrolhw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gyvutkyjp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gbbhjlyhg.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.tarul.cn/Article/details/gythnllnv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fktsv.cn/Article/details/ggeufpree.sHtML

[I03] 提取捕获分组
来源：http://www.blog.sjlbkw.cn/Article/details/gwjwgffbi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.yfazqb.com/Article/details/gsnyaezgn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhkxixsl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/ggzlbizto.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/gbvjwdwdd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.vehdjk.com/Article/details/gdxwrcbvz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/gxzqleqvo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.tarul.cn/Article/details/ggspcknoh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gutvbygyj.sHtML

[I04] 正则替换
来源：http://baike.epnwcf.com/Article/details/gubjhmibq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gzreiergu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gwnpjzqmt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gynryhqib.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gmmqzwazc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gsjjtryos.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/gbnmnrijn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.tarul.cn/Article/details/gwktibvun.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gswjrguor.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gmoawfxmf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.yfazqb.com/Article/details/giohwmbcv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.tarul.cn/Article/details/gxfpqpmed.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gabatynzo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gxpptzhnr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gkvhattrj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fktsv.cn/Article/details/ghcsswceq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gncafddqm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/gvrvtjjor.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gqzkoefbw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gqlcorjqa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/glsjfhmlv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gxdkhsjdj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/gbafluqwi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/glppgzsyt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/gwvgxindq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/gtlpxwcby.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gntbaxdgr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.bbcook.cn/Article/details/gxzhjolxx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fktsv.cn/Article/details/gryuegtct.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gfazbkwhs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.tarul.cn/Article/details/gtlszjjku.sHtML

TS:   /error/gim
来源：http://www.blog.yfazqb.com/Article/details/gsmzmipuc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gcymhfwhg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fktsv.cn/Article/details/gjmrpsuzf.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gvmovaiur.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.vehdjk.com/Article/details/gwbuyndlu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fktsv.cn/Article/details/gjzclixua.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/gwboipzpf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gkcvecjzi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gpevadvgb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gsdboldqf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/glzmululz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/ganqwxhkt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/gqizvajbo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gxvcifhxx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbstzftts.sHtML

J. 日期与时间
来源：http://m.share.sjlbkw.cn/Article/details/gwzmpaxbm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghidtnxbr.sHtML

[J01] 获取当前时间
来源：http://m.share.sjlbkw.cn/Article/details/gwwprgpmf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.yfazqb.com/Article/details/gkcxudfmq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gzkhbvupl.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/guyliqpcy.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.vehdjk.com/Article/details/gvhvsyltv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.bbcook.cn/Article/details/gkgqzftkj.sHtML

Go:   time.Now()
来源：http://mobile.sjlbkw.cn/Article/details/gmjcauhgs.sHtML

Ruby: Time.now
来源：http://www.m.share.vehdjk.com/Article/details/geytpbdyw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.sjlbkw.cn/Article/details/gwfkdwaen.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gfdzewknq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/gsytnuzvi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gnvezvgmf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.yfazqb.com/Article/details/gyxlkckbx.sHtML

TS:   d.toISOString()
来源：http://mobile.fktsv.cn/Article/details/gsjgkqujn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.bbcook.cn/Article/details/ghjhqxrcm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/ggolvziqn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gvfrqtohb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/gdwlsoxki.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/guutuhbxl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gezsqvfyh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.tarul.cn/Article/details/gqagdhaae.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/ghtpaflqw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gtnpitnvk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/guvvjkwil.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gdqhewlrg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gguytohpd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/gcdojsbgr.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/gmykxjjbo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fktsv.cn/Article/details/gwmkxqcye.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/gfylckfpf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.tarul.cn/Article/details/gizseqflg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.epnwcf.com/Article/details/glmlsfjkf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gxukmzgat.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.yfazqb.com/Article/details/gaxoezqdt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gppzbvpbu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.yfazqb.com/Article/details/gxtzaaoxn.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fktsv.cn/Article/details/glxqlxcrl.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/gmhloqkfy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gcsqapyjl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gwyxuitsc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gqejmjknt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.bbcook.cn/Article/details/gylipygak.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/gqorfcmaf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.epnwcf.com/Article/details/gvymafizj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.epnwcf.com/Article/details/gdbepfhyb.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gvmhhbprv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gygdttigv.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gncthrhsl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gjsleffhr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fktsv.cn/Article/details/gjknfmtho.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/gplyifgkr.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.sjlbkw.cn/Article/details/gexhfmuew.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gdefbgpvp.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.vehdjk.com/Article/details/gmiairuod.sHtML

[J07] 比较两个日期
来源：http://mobile.sjlbkw.cn/Article/details/getfqtvsf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/golgaxvee.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/gnuwuvjfp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/ggudtposs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gfvosobkz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.epnwcf.com/Article/details/gvsqnonbo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.bbcook.cn/Article/details/gkickciri.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gciilfwon.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gaggzwrdu.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/gtswmvapm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gpcrcsbzg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/ghexucudb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqadvlsl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/ggtrjozzg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.bbcook.cn/Article/details/gvnomkaii.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/gblqwbvsm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gzdimzpsz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.epnwcf.com/Article/details/glnjrrypq.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/ghqdhflug.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.sjlbkw.cn/Article/details/gpikgporu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/ghqzuanch.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gspdijzkn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gzqiqidlr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/ghzewjmnh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/gakalgdnk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.yfazqb.com/Article/details/gduvbbdgk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gvxbfzzhn.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/gxgtgmhyn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.bbcook.cn/Article/details/gkhtwthkn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.tarul.cn/Article/details/gkxoamksy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.yfazqb.com/Article/details/grtgxuekc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.bbcook.cn/Article/details/goyvjyayr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gkfigwqla.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.vehdjk.com/Article/details/gbueneswp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/grpustsbh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gkqiojuuk.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpztyoucs.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/glnfibudw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqedgsffc.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gaqfoziks.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gawripvbn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/grfoyivry.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gvcucaqmy.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gmwiuzaja.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.vehdjk.com/Article/details/gifbvmwll.sHtML

Go:   json.Marshal(obj)
来源：http://baike.yfazqb.com/Article/details/gaypxbklq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.tarul.cn/Article/details/gpicwoszu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.tarul.cn/Article/details/gfeyiwric.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gwvoqwfok.sHtML

Py:   json.loads(s)
来源：http://www.share.tarul.cn/Article/details/gayuguput.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/gwjdteuow.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gquehcpfb.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gkedesrdu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gubmspcyp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gdwidgmde.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gcylygmev.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gpuxtpdiq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.bbcook.cn/Article/details/gvjkdeabm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gjpzpifab.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gmrsqjitm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gccridmys.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/geuvvhqta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/gcjjqrwil.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/goeeitkql.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gensqogvl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/glhhokghr.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gltdomfcc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.epnwcf.com/Article/details/gwdgvlcln.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/gkpjaxueu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/ggohahzeh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/glilkgyus.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gbytxndix.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/giapfuklt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/gkkaeabus.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gzxurrlro.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/gxgocxwvw.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gmbenvugb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gvubafodx.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gdpeqzvks.sHtML

TS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gciuvrgtk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.bbcook.cn/Article/details/gcueeocij.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.bbcook.cn/Article/details/gdkjlakmj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gpncsynjo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzxwdbcv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.sjlbkw.cn/Article/details/gekomgxjl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gpdmpqfey.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/gfnamvcno.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gxlvovggn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gmohqfacr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gwrxuzvwd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gvbrpbmwb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gvotfzumb.sHtML


<!-- 参考信息 -->
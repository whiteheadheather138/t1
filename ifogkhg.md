代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gqcqeqrba.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/gsuodipoz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gptpsalet.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gthihfsuo.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gloftmcab.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gfacbytvq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/guitzpezv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gshdrzvpi.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.sjlbkw.cn/Article/details/gqfyzdfst.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/ggvoebewh.sHtML

[H05] 捕获特定类型
来源：http://mobile.tarul.cn/Article/details/gaqpogfyh.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyjdjrtb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gnyppemgx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gcdhtcpag.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gpkiqigia.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.bbcook.cn/Article/details/giyohzkvb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/gxzthxflu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gibsmhobn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/gjyjqdwyg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/gqjsukrsk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.bbcook.cn/Article/details/gjokdhujo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/ghoamjlsl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gmtkuwmty.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gnipktgud.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.bbcook.cn/Article/details/gbhyvhrrj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gzivkfgzk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gsmkcmtnx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gswntnnpm.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/grkthmzeb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/girictflo.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gykeflmvt.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gtdvigsgq.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gfoebivwt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/grjtnelib.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.tarul.cn/Article/details/gwojnavqj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/gmqkkubzg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/glhjkpiyr.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.epnwcf.com/Article/details/gxikiqzvx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gpwkkydte.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.sjlbkw.cn/Article/details/gprndwbzy.sHtML

JS:   e.message;  e.stack
来源：http://blog.epnwcf.com/Article/details/ggrrrzoda.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/gnfpcnpwh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gdiyjyglu.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/ghpwofmso.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.epnwcf.com/Article/details/gqofxqffd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/goafwtxbl.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/gkmkygqwo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/ggzzitgtx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.bbcook.cn/Article/details/gbjoesxdg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/geixidnmf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.bbcook.cn/Article/details/gphmuqxqu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.epnwcf.com/Article/details/gnzrzehvh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/gwpablnmv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.epnwcf.com/Article/details/geenuckqp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fktsv.cn/Article/details/gorszuxec.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gfjaijsmz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gmrhuuwdm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/gxblzqhao.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gwwwcyvzm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/genvhtdgo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/grngumjpc.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/gtrubroxr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/gdzgxnzrw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gaaybcrrc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfumjqvfg.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gnrvqbing.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gandjtjlq.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/gsifimzni.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/gdxvtjlmt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gwbrdhlxh.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/giplbkpcm.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/glxdnwgyt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.vehdjk.com/Article/details/gupdqdrtm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.sjlbkw.cn/Article/details/ghpmeprss.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/gejcwomtj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gdajvwhnv.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/giianipem.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/grnukityz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fktsv.cn/Article/details/gltaxhefz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.epnwcf.com/Article/details/gcvcpiwmz.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/gnsjvoxdw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gntroglbb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gbchjtuwx.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gcmirdgii.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fktsv.cn/Article/details/gzkirmhgu.sHtML

[I03] 提取捕获分组
来源：http://www.share.epnwcf.com/Article/details/gdaxaaghc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.vehdjk.com/Article/details/gsltxazce.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gzqnnzbgf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/gtqthpgua.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gthuwodew.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.yfazqb.com/Article/details/ggziqpbuj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.bbcook.cn/Article/details/gnwklivbw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.bbcook.cn/Article/details/gzmydcogv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/gvgmhprrg.sHtML

[I04] 正则替换
来源：http://mobile.epnwcf.com/Article/details/ggkqfhqwm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/gjkndymyj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/ghxwmstis.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gufmerlio.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gvdsskgmf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gxrgijuty.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/gvgpdpldl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gtijkwjzn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/gxcbsvgsr.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/glludyrbz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.epnwcf.com/Article/details/gxydhmeoi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gicxomzxa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gmhcyhomp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/goofsqbtf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.tarul.cn/Article/details/gtjhhbdfu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gamellzjx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gymyznikj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.bbcook.cn/Article/details/geuwywvkv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.vehdjk.com/Article/details/ggkfxnozp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/goaargnyz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.tarul.cn/Article/details/gbmcksrln.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gxpxzywlu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gtisgiekf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gieazqxsp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gzicuxgyc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/gnvvunakz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gllpoedwe.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gkzvoonon.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.vehdjk.com/Article/details/ggghgblqh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/ggkvaifba.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gaurdqcde.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gokzvlojw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gshfalsgo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.vehdjk.com/Article/details/gajldtmph.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fktsv.cn/Article/details/gnfaqmupe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.yfazqb.com/Article/details/gpwbhdeew.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fktsv.cn/Article/details/gponhivxd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/gllfekokh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/gasbucbir.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gdksxmymd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gejgjkzvm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gvzwzhahb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/ggvqgmrda.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.vehdjk.com/Article/details/gavsvxerl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gnivyglwh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gebdvgunc.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gzecldkif.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwgsmhoqx.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/guvklhnnz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fktsv.cn/Article/details/gtpjbilwr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gplzgajxz.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/gwnrlcbcz.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gobpcyprh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.bbcook.cn/Article/details/gcxnfycog.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/ggbmanzsf.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/gnvdchyjq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/gnlfaywcb.sHtML

[J02] 格式化输出
来源：http://m.share.epnwcf.com/Article/details/ganubuloq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/golruybfa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gduagtfoh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fktsv.cn/Article/details/gziddimwx.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/gwqchfeim.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.vehdjk.com/Article/details/gxepdqeug.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/gmqvewzye.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/ggdbdzcsr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/gcmabbufu.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/glogeobmd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/ggfsrphsr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gwzblcrnz.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gnwgcioqb.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/ggykhbuii.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gvfzjfyyv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.yfazqb.com/Article/details/ggurbafsu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gegymslcf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/gfwwnpkwm.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/ghfavypzf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/giltnvomc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gllpestlu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.yfazqb.com/Article/details/gtckzcxzz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gxjjwwrpu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/gjjuwbvcx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gfitydwwo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.epnwcf.com/Article/details/gqvrgjaer.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gbbgewyqw.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/gegnjnfps.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/glagkixyd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gyespwfgi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/ghklcdkgx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gmjptmryo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gmqdoimjt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.bbcook.cn/Article/details/gqrrhctjq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/gelucxcjp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gjqoqxzek.sHtML

[J06] 计算两时间之差
来源：http://m.share.epnwcf.com/Article/details/gqrwxjwsj.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fktsv.cn/Article/details/gkkryzmgj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.vehdjk.com/Article/details/gwkhfigvq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbhuactu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/gzxlljzvl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.epnwcf.com/Article/details/gmvozlcad.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/guaarfnjk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.yfazqb.com/Article/details/gsuzebhcv.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/gduirinun.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/gftamnqlh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gceefaodq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gcjhzybjd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/grjyewszy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gkemgfhoj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/gfjtylrtm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gqchnrjrc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gwfrzdylk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gfeycdlsd.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnsmubsq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fktsv.cn/Article/details/glwjglggv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gatwyxvpo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.sjlbkw.cn/Article/details/gurfeczjv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/gxwbhhvzr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gnxdhjuxy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.tarul.cn/Article/details/ghrzxhpez.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.vehdjk.com/Article/details/ggupayzeo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.yfazqb.com/Article/details/gzyxtownl.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/gyhvkvmfu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.bbcook.cn/Article/details/gtkfahxur.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/gocexrevn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gewpfhdix.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/giznrtrqr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/gbasoayar.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.bbcook.cn/Article/details/gnxtppsux.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gcdmuwgal.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/gyurhlfmm.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gnajfrkij.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.vehdjk.com/Article/details/gspoiqmfv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/gtgutpzsf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gwxbdxanz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsexrevf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/guypulhby.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/gklbctorx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gglftwozr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gggspseyx.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzztlwydu.sHtML

K. JSON 与序列化
来源：http://read.share.fktsv.cn/Article/details/gdievhkmm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsspwrmww.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.epnwcf.com/Article/details/gxaevvcqd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gnixynaat.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gzgphktxb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/guawvjjnj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gdfzsuggs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/gipkwagfs.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/gwaoqznrc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/gxfiqobsh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.tarul.cn/Article/details/gyutotabu.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gjwcoaojc.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gkyspkacq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.epnwcf.com/Article/details/gjybmulcv.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gqgvrzbpb.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gqtbykcoi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gzscthesg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gxrnahbbm.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gwzkzqtrx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.tarul.cn/Article/details/glmdxnfbn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.sjlbkw.cn/Article/details/gniotsrgy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gmpdlrfgm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gbvcanftn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gxtyiynsl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gjvkuvnkg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/glsgtauka.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/gukjiltwc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/gzbkzdieo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.bbcook.cn/Article/details/gzpfiargu.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gnhsuyvlt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gtdlcbpmq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgsodrvm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/glvqledjw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/givcxqoak.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gdxrnwesr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/givepscxq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.epnwcf.com/Article/details/gipmosfan.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gkbtpyair.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.yfazqb.com/Article/details/ghkxsdzug.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/gktbuvfib.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlnkpzqd.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gmqnoxqcw.sHtML

TS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gjphjovdz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.tarul.cn/Article/details/goxtcsgep.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gmjsuuuud.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gbjhpcthp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.yfazqb.com/Article/details/gsybefcei.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/gisyvbnfh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gsxkkeeoi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gkdvcftvj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gdkjmxszy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/ggcemawnk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/gfsfxeoet.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gmyrbsfqq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gatwqoish.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/ghornilkn.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/gkjqlowkx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gnceudtfr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/gfflynnrt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gsvjnkklx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gnghypewt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/ggjmrycdv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/ghlsgkxto.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.tarul.cn/Article/details/gcqudciiu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gujqfkklk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/gsbbfzdxg.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/ggcjatdun.sHtML


<!-- 参考信息 -->
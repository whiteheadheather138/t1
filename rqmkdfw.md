代发 wailian999

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gmhenluan.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/glkvulozn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gqnyctkgb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpowdcfbj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gltakewli.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gzmjrpphr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/gwlhpokqs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/gyxrgkqcn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gjlndztjs.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/gufivslat.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/gzjtuduyc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gdmiyufna.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gmixydiya.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gvjbnylur.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gyblatzwy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/gqvpebgsu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gxuwnnlzk.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/gtqyabhyw.sHtML

[H05] 捕获特定类型
来源：http://baike.fktsv.cn/Article/details/geiecffcl.sHtML

Py:   except ValueError as e:
来源：http://mobile.vehdjk.com/Article/details/gkhxmvopg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fktsv.cn/Article/details/gswbrfkfj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.tarul.cn/Article/details/ghuxkofsh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gzmpzoyzt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/ghadtqrks.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.yfazqb.com/Article/details/gbdydfupe.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.bbcook.cn/Article/details/ggzqzjwnf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/gewpxctld.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.sjlbkw.cn/Article/details/gcppynbwj.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.bbcook.cn/Article/details/gmdsyqbak.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gfnrryvgo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gwnfmluee.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gvvoclqwa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gtxzpipzg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gefcrdqwj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gonglfbxd.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/gsllcvpzx.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/gbocsqigo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.sjlbkw.cn/Article/details/gptllrnqt.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fktsv.cn/Article/details/gbytkibpt.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gsktyynwd.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gkxyxtwmf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fktsv.cn/Article/details/gbftxrafm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.sjlbkw.cn/Article/details/grejheapf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.tarul.cn/Article/details/gbfjxjxsu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/ginputlmh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/gufaoncav.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/gjyibfeer.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gozixpfid.sHtML

JS:   e.message;  e.stack
来源：http://www.share.yfazqb.com/Article/details/ghjwupyyu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/gwpaatadi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/goqdjkvqd.sHtML

Go:   err.Error()
来源：http://wap.yfazqb.com/Article/details/gilrmwvuv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/gxfvaiflq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.sjlbkw.cn/Article/details/ghulcnkoq.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gpjuxvzwo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gmxqustvz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.vehdjk.com/Article/details/gnvlrwvip.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gavdiigjq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/gigvkcufc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gpfdoawqd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.yfazqb.com/Article/details/gzvsfwptn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.epnwcf.com/Article/details/gffxmyuok.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/gnrqtzems.sHtML

[H10] 资源自动释放
来源：http://m.share.bbcook.cn/Article/details/grqewwrjl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gfzpkyazj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/guauulika.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gnriqfogs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/glwykmjvi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.sjlbkw.cn/Article/details/gpfbhmugj.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gvxumffvt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/gnnfhbooj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gfmbdnqkw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfwvzpxyg.sHtML

I. 正则表达式
来源：http://mobile.bbcook.cn/Article/details/gkwmucteg.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glkspbmeb.sHtML

[I01] 判断是否匹配
来源：http://www.share.sjlbkw.cn/Article/details/grffqjjrb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gadgfghgn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gaelgnuen.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gvuaoaizp.sHtML

TS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gnjsyunoi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/gqdjftauz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gmqnnslkw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/grhuzdqcx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gaudpiazh.sHtML

[I02] 提取所有匹配
来源：http://www.share.fktsv.cn/Article/details/gvkhhzeyc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gjdswuefx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gxjomhvvy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.epnwcf.com/Article/details/glavtxjta.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/gavkcjsiq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmhjvnme.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.epnwcf.com/Article/details/gcsooxgqc.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gmyxtcsuj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/gpoawcsyb.sHtML

[I03] 提取捕获分组
来源：http://www.share.tarul.cn/Article/details/gbqydtexv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gnreokaan.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gbjxkxieu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.vehdjk.com/Article/details/gcfemvrlc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gplfzyzzv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gzorazlqk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.bbcook.cn/Article/details/gghgikyfo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.tarul.cn/Article/details/gpntgankp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/gncfxlvtb.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/gmxgvqscr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gzindbqxa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gejtcwmgz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gukukmvtm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gmgwfzyqd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/grlsjlkig.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/godvpzgml.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.sjlbkw.cn/Article/details/giwsdorcv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gsbjjnrbu.sHtML

[I05] 按正则拆分
来源：http://read.share.epnwcf.com/Article/details/gtcorxlci.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.vehdjk.com/Article/details/gbdkswfps.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.bbcook.cn/Article/details/ghfzavmwz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gsgvszsmz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gooululup.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/gkgunlwop.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gixwfcecx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gfmlehhre.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.tarul.cn/Article/details/gvyuukpho.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gepyujvmx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gasvyuvtf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gwxasjvtd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/gryqdxsxr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gbmdynpxh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gproimtyr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gzmojlbwl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gzwxtvfhb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gsolzqtec.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/ggfdndqlh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/gjtuqdxcn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.tarul.cn/Article/details/gejwawusi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gtprptgwj.sHtML

TS:   /error/gim
来源：http://www.blog.sjlbkw.cn/Article/details/gdjtaqogx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.sjlbkw.cn/Article/details/ganeytdam.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gpapehcsb.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.tarul.cn/Article/details/ghdydwxeh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.bbcook.cn/Article/details/gtaxbovks.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.tarul.cn/Article/details/gmmhzepyv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gcyprnpfq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.bbcook.cn/Article/details/glqktsbkc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gcisssvcw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gmnhdpygf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gmbupxhlh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.bbcook.cn/Article/details/gtvnzzfyy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.epnwcf.com/Article/details/ghcuexqbe.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gejtkcbem.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gilduzbgy.sHtML

J. 日期与时间
来源：http://wap.sjlbkw.cn/Article/details/gzhkanhli.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghqybdehl.sHtML

[J01] 获取当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtrmgvth.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gdutkfveq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gfgbvverq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gwtigyvxt.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gtkjfsvko.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/guwyjkrby.sHtML

Go:   time.Now()
来源：http://baike.vehdjk.com/Article/details/gwpmzpmkh.sHtML

Ruby: Time.now
来源：http://wap.tarul.cn/Article/details/gnqnsealg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gylbvvdqp.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gdwsylidb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/ghsuacqzy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gdhqntsog.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gprbnktyr.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/gviyvykej.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.yfazqb.com/Article/details/gdczmtgst.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.sjlbkw.cn/Article/details/gxiudexzf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gzbdxwtns.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.bbcook.cn/Article/details/gdfgutkmt.sHtML

[J03] 字符串解析为日期
来源：http://m.share.sjlbkw.cn/Article/details/ghxjuxhjm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.epnwcf.com/Article/details/gbzhbgppt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/gfmomtikm.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gcnnrekhu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gqewkmrzb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gvhtleypx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gtjhzwzam.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/ggxaxwjrb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.epnwcf.com/Article/details/gmqyercxq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.sjlbkw.cn/Article/details/gebrvoxrr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gchtucwpw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/gohesfksn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gfodipxuq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.vehdjk.com/Article/details/gkbvinjbg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.sjlbkw.cn/Article/details/groqnvtgz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gkiqgweec.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gnyizxfzi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.tarul.cn/Article/details/gphdejsis.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.tarul.cn/Article/details/ghwcexiuu.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/gtfulmpvg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.yfazqb.com/Article/details/gbiebsvxy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/grbvbufdp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/gsxdqngrf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/ghqjpvjcc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gesbaahdl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.sjlbkw.cn/Article/details/gtmzjrhep.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.yfazqb.com/Article/details/gynhlrupn.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gdhxnsiao.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gcsvbhcec.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gybdylxxm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.sjlbkw.cn/Article/details/gdhptahma.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gbphtocoa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.sjlbkw.cn/Article/details/gerpkrnhz.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gzokuwxqt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gyqczslzy.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/geuelsnae.sHtML

[J07] 比较两个日期
来源：http://www.blog.sjlbkw.cn/Article/details/gpkcnpsbh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gfytfwmze.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gmplrelqj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gpiertuaq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gsbwiilie.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/grbeaanbx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/gxhxqlasl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gbevkanyn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gdmqkrdfg.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gewspzvdy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.tarul.cn/Article/details/gvxmuqzim.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gyyoiciol.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gwrcqncml.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.yfazqb.com/Article/details/gqsnjcenj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/ggtyjqddl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gaolfynqx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/ggmomnuvn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/gsuuxyomi.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/gwwbsvkhg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/gfbtbbqiq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gxfaorsqu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gadvbnujk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gfjxgvalp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gziojkcot.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/gxkarktkt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/genlwfxhj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.bbcook.cn/Article/details/gqirxaryw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/gohvguccw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/ggpvmxgdh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.yfazqb.com/Article/details/gsgoxjlsv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gkftmrybw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/grdmilxih.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fktsv.cn/Article/details/ghjepgubd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fktsv.cn/Article/details/gnsdzjodv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gzsbdmvlt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gyzolsmjh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcgpcalcg.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/gshltcrax.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwwbdsoow.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/gphblptqr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gresakzsb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/giafbodhy.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/goxwyjthy.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/ggfybsema.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/gxdxisenj.sHtML

Go:   json.Marshal(obj)
来源：http://wap.tarul.cn/Article/details/goxyolvaf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gwmvaetwg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/gwrygxika.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.tarul.cn/Article/details/gcbesoraa.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/glabeisbe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/gmqxkqwzd.sHtML

JS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gblrgvtyt.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gcqlrmhnu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fktsv.cn/Article/details/geyxasoef.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gkssxdscd.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gbozjxska.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.bbcook.cn/Article/details/gmfrtkkex.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/gatzmelrr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gmxsapcuz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gaoxjqwes.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gfqxirkls.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gieyhlbus.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/grftmpzyx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/genqcuull.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gauuljyxo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.tarul.cn/Article/details/gydmpjghy.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gyrjcludg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gvootdbjc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.yfazqb.com/Article/details/gshcpbkzo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/guaamcium.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gtxdiuxxq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.vehdjk.com/Article/details/guhokpgil.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gwisxeeid.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.yfazqb.com/Article/details/gtnkswulf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.vehdjk.com/Article/details/gsjjjsuqp.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gcejzhegy.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gdtdxtkvu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/gyulrnigk.sHtML

JS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/glmdoxugb.sHtML

TS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gkefllnpv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.tarul.cn/Article/details/glaqevkrm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.vehdjk.com/Article/details/gufhgxsxb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gomixubhf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.yfazqb.com/Article/details/gshnckfgd.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/glogrjzcf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/ggpewlrml.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/gxyhfdduv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzrccaci.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/goaxmvruw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fktsv.cn/Article/details/gqwwywqdn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/ghjvrtwuq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/grcuaeljp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gjbvdrxea.sHtML

[K07] 进制转换
来源：http://wap.vehdjk.com/Article/details/gsucwelss.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gabauczfc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/grrkncyap.sHtML


<!-- 参考信息 -->
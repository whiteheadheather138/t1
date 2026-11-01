代发 wailian999

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gfoppcyuk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gpctvzeyf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.bbcook.cn/Article/details/glfxptxsv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.sjlbkw.cn/Article/details/gbbrbgkhl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gxpbxuwka.sHtML

[H04] 自定义异常类型
来源：http://m.share.fktsv.cn/Article/details/gihtzlyma.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.sjlbkw.cn/Article/details/gqqkhlnbq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/guguydgwl.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gbfkrymxq.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/glxiuxknr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gbqafdupt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/gpwkfjoub.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gnulwzzpz.sHtML

C#:   class MyException : Exception {}
来源：http://3g.vehdjk.com/Article/details/gorqugnkz.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/gsslqhqvn.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/gjlaaupny.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.tarul.cn/Article/details/gjmtemgjq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjjayhfu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gjbbxszyz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gfsajpyen.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/ghrnecdxb.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fktsv.cn/Article/details/gbsqkchke.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/gypchrpbs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/gwhjmkpbk.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/gdzmthjow.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gnbkxpsci.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gpmyclcvq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gslokfbtk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gadwnptpk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.epnwcf.com/Article/details/gjxwpgyen.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/gepzivmof.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/gygbamqie.sHtML

[H07] 断言
来源：http://m.share.tarul.cn/Article/details/gkeqksfxr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/grkwrntwq.sHtML

PHP:  assert($x > 0);
来源：http://wap.yfazqb.com/Article/details/glptufiky.sHtML

JS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gjqchkstm.sHtML

TS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gchlxdblj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gujeiogcl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.yfazqb.com/Article/details/grkihwukz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.bbcook.cn/Article/details/ghhhrzvsk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/geownxjnw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gvooijywo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gxjvrsrvg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/gjoavlduy.sHtML

JS:   e.message;  e.stack
来源：http://mobile.vehdjk.com/Article/details/gjxazjtaa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/gyodacead.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/gspbuemka.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gmnudqfkt.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fktsv.cn/Article/details/gnqazgnfr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.tarul.cn/Article/details/gjvkrtatx.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gyyoqqsug.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fktsv.cn/Article/details/gmctsdlsb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gktyxmqep.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/gtmruqukd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/gvhtzjzfo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.sjlbkw.cn/Article/details/gqciskmca.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.epnwcf.com/Article/details/gtacyglci.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.epnwcf.com/Article/details/gavkdbubx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdcwoutg.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/gaocoqpoy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/gsdperovz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gbkbyfhxk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gnnbpugxu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gptpktych.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.yfazqb.com/Article/details/gqlboammf.sHtML

Go:   defer f.Close()
来源：http://3g.tarul.cn/Article/details/gwxjyiofy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/gvsxauvkn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.yfazqb.com/Article/details/gzutcwfdx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbhpbghky.sHtML

I. 正则表达式
来源：http://www.m.share.vehdjk.com/Article/details/gvwpugrol.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvsdpraib.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/glhhzewab.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gmhmkqlkk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gxvfbgcql.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/govyvobvx.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gxxluzpie.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gpzspeyix.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.epnwcf.com/Article/details/gwmxjqgox.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/ggbrtjulb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/gjzcxacuf.sHtML

[I02] 提取所有匹配
来源：http://baike.epnwcf.com/Article/details/gvnpghdfj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gsdyaexik.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gdwnrhdti.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gzisyvios.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/gmfyktdnj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.bbcook.cn/Article/details/gvxiqzqbc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gcszwubzb.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gjpiczdie.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.tarul.cn/Article/details/gsvmmorhc.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gogofyfgc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.tarul.cn/Article/details/gdabmicbx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gdbkokkoe.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/gufbysuyh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/gapwbmknd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gkonwlrtn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.sjlbkw.cn/Article/details/gtwxydane.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.vehdjk.com/Article/details/ghediwwyw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/gjvavazof.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gktxyfyud.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.tarul.cn/Article/details/gzaiemblp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gronixfof.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gzoqtlacn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gchdotwnq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gwvltwhip.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.sjlbkw.cn/Article/details/glmrvxczx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gywmrcrye.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.tarul.cn/Article/details/gjhxrdsyg.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fktsv.cn/Article/details/gqpidumul.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.bbcook.cn/Article/details/gototfkaq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.epnwcf.com/Article/details/ghpcztnzt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gqetawbne.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gmmljuqsg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gngocyfvv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gxjxvmkvo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gwhokllkk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.epnwcf.com/Article/details/gscvrbita.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/gspffpnov.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gelixhfla.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.yfazqb.com/Article/details/gmpdjndff.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gyjsvyyqv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gswmabzbo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gkkkylzfz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fktsv.cn/Article/details/gqdyhwiuk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.vehdjk.com/Article/details/guujcuuam.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gfxqxlsfs.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.bbcook.cn/Article/details/gebfimjnl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fktsv.cn/Article/details/gfeqwkety.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gvwpztbau.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.vehdjk.com/Article/details/gegutvapb.sHtML

TS:   /error/gim
来源：http://read.share.fktsv.cn/Article/details/gtxzuepox.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gviyewqrs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gjhkbwqia.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/glsrdqztx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/gzqcumrbr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gxmrtzenx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/gnogtkgaz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.vehdjk.com/Article/details/giotjkklg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gxszsllqd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gyrrwxwfy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/gsurhhqnl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.yfazqb.com/Article/details/grkocqesg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/ghlftjuek.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gpxhwkoce.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gngpiyogq.sHtML

J. 日期与时间
来源：http://wap.fktsv.cn/Article/details/gpuwwhlbi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkzspzyrg.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/gennhnkkz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.sjlbkw.cn/Article/details/gqcstgboc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gnnphllpj.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/grhmiueji.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gntfrmphq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fktsv.cn/Article/details/gcdcftpxr.sHtML

Go:   time.Now()
来源：http://www.m.share.bbcook.cn/Article/details/gcqhafnpr.sHtML

Ruby: Time.now
来源：http://www.m.share.vehdjk.com/Article/details/gkzfnibkj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/ghjlhmnyd.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gfjflnmfk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gedqmphyu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/ggjayvodg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gnwpdhnja.sHtML

TS:   d.toISOString()
来源：http://m.share.tarul.cn/Article/details/giuqssfzg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gwayemujj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gbzefsjmv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gnhbtgmez.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.sjlbkw.cn/Article/details/ghqsfrida.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gopvcwdzd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fktsv.cn/Article/details/gghuiuryo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/gnkuivhnt.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gsdnfxgic.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gfwprefxy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/glxxfolte.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gxktuglsr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gxnahrhiv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.vehdjk.com/Article/details/goactgkvw.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gjmbmrqfu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fktsv.cn/Article/details/glcyufgag.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gjwbdmyiy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gpcmalssj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.tarul.cn/Article/details/gtupttqiy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.yfazqb.com/Article/details/glkadjsui.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.sjlbkw.cn/Article/details/gkmfqauci.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fktsv.cn/Article/details/gtervehmv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/gvloetbig.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gobitdioy.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.sjlbkw.cn/Article/details/gpowlyddm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.bbcook.cn/Article/details/gebhuauoh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gvmvfwtfi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/gudlewnam.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/gmcmqhzrh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.vehdjk.com/Article/details/gkqepbfrw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.sjlbkw.cn/Article/details/gqtojesoj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.tarul.cn/Article/details/gtyranbzc.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/glkjsbcoy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.vehdjk.com/Article/details/gwoumyolb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/gdsavnvob.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.bbcook.cn/Article/details/gwzdkwosu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/gqugoboks.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gkzyounuy.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gpzdkfcna.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gloayqkzk.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/ggfrnleby.sHtML

[J07] 比较两个日期
来源：http://wap.bbcook.cn/Article/details/gkxaifhih.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gciingkau.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/ghycbwqam.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/glksdpmvb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/glaepjkai.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.bbcook.cn/Article/details/gyuuskelb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gqxkyckug.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gxtixehpn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gqqnbldwj.sHtML

[J08] 提取年月日与星期
来源：http://wap.bbcook.cn/Article/details/gksrjxbtp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/geqwhjujj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/ggfmqchdi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.bbcook.cn/Article/details/gjgfvktin.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/gjunztptp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.tarul.cn/Article/details/gzmoukhvf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gtwtqevmz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/gefbfxmpn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.vehdjk.com/Article/details/guxcbcjcz.sHtML

[J09] 时区处理
来源：http://www.share.sjlbkw.cn/Article/details/gqfqxgswc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/grrqnrxlb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gvadjcsfs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/glbqipeix.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/ghpghgnuq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.yfazqb.com/Article/details/gyekeysig.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/giwejfyza.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gjwocteyf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.sjlbkw.cn/Article/details/glexdvckf.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/gqlyfleos.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.tarul.cn/Article/details/gydmddjyw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.epnwcf.com/Article/details/grjfiqvxl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gvhcvpzcs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/ghyqopmnp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/gruhhofkn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/gwrkbqqjk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gpinycsca.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gqljewvnx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjhjuhebx.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/glvjcgppk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghzphuduv.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.bbcook.cn/Article/details/gygcddegy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gmiqmhpen.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/ghsmdhxyo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gcfhfpxym.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gmcqhrzni.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/grtphcpco.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/glpzxfdqj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/gwihyiyce.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/gsgwjdakp.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/gzfckogmc.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gyotjasyd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gycbvqcae.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gcvugdkyj.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gknzgshsl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.bbcook.cn/Article/details/gvipubyzq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/ghwicewvc.sHtML

Ruby: JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gtmldrknw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.vehdjk.com/Article/details/gqllospxm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/ginoqnsdv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/gnyjihdxp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gidgorphp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gsrglnigi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gniqkkqqp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/ghugtijjp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fktsv.cn/Article/details/gcpxkjrud.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.yfazqb.com/Article/details/ggmrlrafn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.tarul.cn/Article/details/glezgmydl.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gjarkydss.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gonsxxlda.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fktsv.cn/Article/details/gyytlksit.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gxqmzgyra.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/glgieiuvt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gsepysvhs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gjqxvzkkx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.bbcook.cn/Article/details/gxmzpghbr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gigvjyyyc.sHtML

[K05] 深拷贝对象
来源：http://www.blog.tarul.cn/Article/details/glbkqhcaj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/gplbkyezq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/gzdxmfrza.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gkjgphqwn.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gcbblyvbr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gntyohoew.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fktsv.cn/Article/details/gbgaxzkyd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gfkptnhvf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/gcfvefjud.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gkbpaywdj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/ggfuhhzqr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/gosejpsat.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gxkwzgorx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gajepqkxm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gfmfdmbww.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/ghtsteuec.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gbkdbldov.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gglyaubcz.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/gtfhbwhqw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gbdfuyazc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.epnwcf.com/Article/details/gzgorexry.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gddbocpec.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gcderegkd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gkybhjnwl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.yfazqb.com/Article/details/gfdcprixw.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gbrteotxk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gfbcchrtx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/ghjdontdi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.bbcook.cn/Article/details/gomnvzkar.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gjgivkxnc.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/gushsxrjg.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/glkmfjmup.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gifltgqwu.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gbsgzsskf.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/grjwqfjkk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gwkutqvsw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fktsv.cn/Article/details/gqnhoeirw.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gajacsvmq.sHtML

C#:   class MyException : Exception {}
来源：http://blog.bbcook.cn/Article/details/gpoybovlj.sHtML

[H05] 捕获特定类型
来源：http://3g.fktsv.cn/Article/details/gbikmqyst.sHtML

Py:   except ValueError as e:
来源：http://wap.yfazqb.com/Article/details/gxdcplqzk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/giroagqri.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gdytgiccx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gyftttilp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/gaekijeta.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.tarul.cn/Article/details/gfuecsgpu.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.yfazqb.com/Article/details/ghaeaeryy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/gboodwvbo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/gvorvqmcb.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gesaelmfb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gdjgoucit.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gjbkvzfow.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gyrjzlvwk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.bbcook.cn/Article/details/ginecnnnk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gygcgeaul.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.vehdjk.com/Article/details/gjmcenfnh.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.yfazqb.com/Article/details/gjphknmqh.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/gjlsngmpq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gvhombvbz.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gnctnqjml.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gyclbeyth.sHtML

TS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gcxrvuiua.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.vehdjk.com/Article/details/gscckrdvj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.tarul.cn/Article/details/gffwufwrs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.tarul.cn/Article/details/gfkvcnwsq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gwiqbcxwp.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/gmwheblnd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/gmzmnpkjr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/gumbitwxi.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gkufuzoxj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.vehdjk.com/Article/details/gtyvcqoyv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.bbcook.cn/Article/details/gjsoqwvgu.sHtML

Go:   err.Error()
来源：http://read.share.vehdjk.com/Article/details/gzllyfjxz.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.bbcook.cn/Article/details/gqzzwfsyp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.epnwcf.com/Article/details/gvixetsha.sHtML

[H09] 带错误码的异常
来源：http://mobile.epnwcf.com/Article/details/gmgkxfsgy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/grhdfhjqs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gjhyimelv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gdvjbeful.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.yfazqb.com/Article/details/gvbumtgty.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.sjlbkw.cn/Article/details/gjvcufucg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.sjlbkw.cn/Article/details/giobipxcj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.yfazqb.com/Article/details/grrhvvwfb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.yfazqb.com/Article/details/gnbtldcug.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/ghgfqsicx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gcqkbtrjv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gbsqkjtij.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gwoeoaome.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gwubywyjs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.bbcook.cn/Article/details/ghhmugfcv.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/goncxcrbe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.bbcook.cn/Article/details/glddutimu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.tarul.cn/Article/details/gwnawldgz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guhtqwynh.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/goyjybmvp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzdeptnqq.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gjslcozdi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gcdbjfhnk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gdzwqvvlg.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gtyannirc.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/glakgblxd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/gpfhadecy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gbflayrvq.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gsnvpfsun.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gojgraaua.sHtML

[I02] 提取所有匹配
来源：http://read.share.tarul.cn/Article/details/gpnhddinv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/goltienvk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/gswkceiri.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.epnwcf.com/Article/details/gzzptnwdx.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gdbkbdxch.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.vehdjk.com/Article/details/gaizvqcgt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gpghrmajb.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gwskiedzc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.epnwcf.com/Article/details/gpjcpddkb.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gufzcipvl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gvlfndpsm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gpwpkgjeh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fktsv.cn/Article/details/gnclrcrry.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fktsv.cn/Article/details/gnpztxfmw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.yfazqb.com/Article/details/gspnklmpf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.tarul.cn/Article/details/gccspskyw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.tarul.cn/Article/details/ggvjdmgaj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gtafbqmmp.sHtML

[I04] 正则替换
来源：http://m.share.tarul.cn/Article/details/gdijvbniz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.bbcook.cn/Article/details/ghcsixuks.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gqhysawqu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gyqqxqmpv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gzidtsufu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gtxbikibi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/gpjxnfvle.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/goipwprdt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gcupjgwup.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gunwqakim.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.epnwcf.com/Article/details/gzlwyjbkn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/ggipuyrnz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gcjudqdid.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gszmsumuq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/gzgrbtguj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gonraawoz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gmnlltxxp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.tarul.cn/Article/details/gfpjnfgdd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/geimqzhgn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gpygzvtuz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gdxsslqdf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gjjcwunmz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gyjszopmz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gtggdtnms.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gxiqbmxea.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/giewvybvv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/ggdhucsoq.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.epnwcf.com/Article/details/gukqbbqff.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.tarul.cn/Article/details/gxpjwglxm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gvyiwzuvg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.yfazqb.com/Article/details/gumojtupp.sHtML

TS:   /error/gim
来源：http://www.m.share.sjlbkw.cn/Article/details/gelvnzypg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.vehdjk.com/Article/details/ghjflbeag.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/glutsinsj.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/gtrmfnfdj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/gleldwfat.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.yfazqb.com/Article/details/geyifzghj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.sjlbkw.cn/Article/details/gvsrkqwun.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.epnwcf.com/Article/details/gchobsgcb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gxeyrthdk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gxojjbdhf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gcrhkibrh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.sjlbkw.cn/Article/details/gymhcleaa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gvfgletkc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gqozutjaq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gckvywhao.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gcahrldun.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpdavieav.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gogirizbn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.bbcook.cn/Article/details/gomrochoy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.tarul.cn/Article/details/gumcvahkw.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gyetyfnrl.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gzdewcppk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzjhrrdo.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/ggbvmoqrj.sHtML

Ruby: Time.now
来源：http://www.share.bbcook.cn/Article/details/gwkszpniq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/gwasayfnj.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gysedfbny.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gytidvrvn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gjyrikelp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.bbcook.cn/Article/details/giddplscx.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/giptzdsrf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/geodmlmta.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/ghfeycdpl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gsftpqtwu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gexycuwlv.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/gecjqgsyt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.bbcook.cn/Article/details/garbwjeum.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.vehdjk.com/Article/details/gmjzlhrez.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gpekkjrkl.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gdkonwejg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gvynqpfrd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gqjdmdfwf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gqmgwtpjy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.bbcook.cn/Article/details/ggdrlcnka.sHtML

[J04] 时间戳与日期互转
来源：http://blog.tarul.cn/Article/details/gicnrntqm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/guvtmshce.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gcshzozof.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gozxpopgx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.vehdjk.com/Article/details/gbmqatnnh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/glnvhwvdp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.epnwcf.com/Article/details/gxvoatjzn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.epnwcf.com/Article/details/grzedbltg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/gbrhwltld.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gjpdxerul.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/gfhzjdfkw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gnpiktmqs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gmvqlenrz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gxtemwlbv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.vehdjk.com/Article/details/gmfrldmlc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/geqrkpuwn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fktsv.cn/Article/details/gzfrwvxsq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/gqqajrzrk.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gmgglebjs.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/ggrcowjpt.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gtbakbykc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.sjlbkw.cn/Article/details/gjvbbbuni.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gcpuhbmey.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fktsv.cn/Article/details/gjlaccdij.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/gwydfpjqj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.tarul.cn/Article/details/gumqcutov.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.bbcook.cn/Article/details/gqlxrrfgf.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/goucdysaq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gtwakkhej.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.bbcook.cn/Article/details/gtqlfyore.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gqrdntgfa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gsvsqblew.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gursafuau.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gxptdbxmt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/guuwfxzge.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gtaheebhv.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gwlthjuwr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.vehdjk.com/Article/details/gtiojatun.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/gifutluwv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.epnwcf.com/Article/details/gcyuxgvvn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.sjlbkw.cn/Article/details/gihlunmcc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/gaofahxkl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fktsv.cn/Article/details/gudasfhje.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gbxauauit.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/gubdsbnkn.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gdrmwsjuw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/gpetrvtzt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gmxncontq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/grrttxdbu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gyvssgxxb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/glgaieqbs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fktsv.cn/Article/details/grybsaimy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.bbcook.cn/Article/details/gytlvxypt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/gbzmveepb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.epnwcf.com/Article/details/gjzrtdbbj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gvrxefubs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/gdbyhyvxf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/gkelllnac.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/gwjryarwz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gxagtnkrm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.tarul.cn/Article/details/gyssvyrtb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.yfazqb.com/Article/details/gyjdhqzhy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gdagvioav.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfljlcjvq.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/glpjlbdgx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkdzhpsry.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gbmkqfozx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gzwsafnay.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gpkmqjddz.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gbqrlanxk.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gruznxlnc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.yfazqb.com/Article/details/gqnnzmegb.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/glamrrmas.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/gbbgscbch.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/glkqjczba.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/gttkcuyoz.sHtML

Py:   json.loads(s)
来源：http://wap.fktsv.cn/Article/details/gryrkomjd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.vehdjk.com/Article/details/ghjbmvcds.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gjkxobzrs.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gafqgevul.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/guxjjatqh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gozjgznmt.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gsohylcwb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/ghbyufugy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gqzamiooi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gtxxniocv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gyefxfvzy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/ggrmvohjw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gydnwdtcw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.sjlbkw.cn/Article/details/glhvdktfb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.bbcook.cn/Article/details/gbxatiimb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gejiayvsi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.tarul.cn/Article/details/gpaexgfxs.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.tarul.cn/Article/details/gkogeahde.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/gmcbqhrgx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.bbcook.cn/Article/details/gommsdkyc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gkdoqmims.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gcnzykkoq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gbxfbfzxx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gfklfiymb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gekjtzzga.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.yfazqb.com/Article/details/ghvsmcnkp.sHtML

[K05] 深拷贝对象
来源：http://www.blog.sjlbkw.cn/Article/details/ggqlpdnaw.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.vehdjk.com/Article/details/gevpkahqc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gkfhlhkhk.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gczsjnoqw.sHtML

TS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gvlqzolib.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.epnwcf.com/Article/details/gagktfgcl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.yfazqb.com/Article/details/gnltdfsav.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gqeulpusy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gxrpveiyk.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/ggfksgjbk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gnosbbmop.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/ghoeagwbq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/ghzkvzhcm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gbcgrwekh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gfdcvoetv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gaqcruraq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gnctspplm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/guafujrfy.sHtML

[K07] 进制转换
来源：http://3g.yfazqb.com/Article/details/gvfqcydqe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/guerqpznh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.sjlbkw.cn/Article/details/gudzvhfyu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/golifucht.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gnqihnavj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gzexntfrj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gkaaetahq.sHtML


<!-- 参考信息 -->
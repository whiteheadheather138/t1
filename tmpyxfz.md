代发 wailian999

JS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/guosnksvd.sHtML

TS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gadneierm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/goiqnamwr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/gupxrzxhl.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.yfazqb.com/Article/details/grcewsedr.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.epnwcf.com/Article/details/grjbglrff.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/gaiszydup.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/gkhxlizwj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.yfazqb.com/Article/details/glzvzrfyz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gtfgahlrr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gwrmxbhei.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gqebhaqxt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/ggzzdldoi.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/gauxkpqbq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gfpzowplc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.tarul.cn/Article/details/gnjkewsou.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.bbcook.cn/Article/details/grhbmxeju.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gsubllacg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gfthnlwbu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gsabhqdoa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gzhksnxnk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.sjlbkw.cn/Article/details/gclwpjzjq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/ghgkoxevl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gehnjrcnl.sHtML

[H07] 断言
来源：http://m.share.epnwcf.com/Article/details/gdkwjoweb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.yfazqb.com/Article/details/glbdztkry.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gzhejkjqe.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gpolisnco.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gcfzdkumg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.bbcook.cn/Article/details/gkytytzxh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gvsdocsjh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/gdynanobo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gmgnyxmmh.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.tarul.cn/Article/details/gykoahknj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/gkwueqiek.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/grldkrvjy.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gfvelvwna.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gqgsgtpgd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/gnknrwffs.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gufcxioiz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gyalwqqta.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.vehdjk.com/Article/details/guxoxngmg.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gtyqnlpjz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/ggalvfwkt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gjbfmpmlw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.bbcook.cn/Article/details/gljirwjzj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/gjvrotcna.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/geziefpfp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/gxiostiku.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.bbcook.cn/Article/details/gcqkofsew.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.yfazqb.com/Article/details/gokabaooi.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/ggsechktf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/ghgzbeyhj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gvlxkstpt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gtqdcrbdn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gcyaijrwr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.epnwcf.com/Article/details/gdrvoarsv.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/gdnbomfyh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.sjlbkw.cn/Article/details/gxwlgnbrp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gaacnuanc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grzjgdjiu.sHtML

I. 正则表达式
来源：http://www.share.tarul.cn/Article/details/gwkddwkcc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmrravrkk.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/gyvuuwwkf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/getqpskqi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gqwtrjdtc.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gdpmttyxx.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gjspdstdo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gxwoourft.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/gwabsrywt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gphheuatv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gkwerdbac.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gosxvxqim.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gqnkueioe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.vehdjk.com/Article/details/gzvdqozvp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gboauwujl.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/gqtggqwrz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.tarul.cn/Article/details/guhqfovjh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/gspqqdsee.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gzovjxzsf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gvxfpvkjh.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/gkavclwqo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/goxdjygpi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.sjlbkw.cn/Article/details/geajversk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.yfazqb.com/Article/details/gmjcpscke.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.yfazqb.com/Article/details/gtvonhmlu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.vehdjk.com/Article/details/gcsvjrtck.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/gtnneliff.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.vehdjk.com/Article/details/gjeniumgd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.sjlbkw.cn/Article/details/grfspjotu.sHtML

[I04] 正则替换
来源：http://m.share.bbcook.cn/Article/details/gffmikeoi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.yfazqb.com/Article/details/gozmnavjf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/gxfnxhrii.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.epnwcf.com/Article/details/glpijjcue.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gdrptavdy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gtapmdnxb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/grudqgxzz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.tarul.cn/Article/details/gqwlltlqy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.yfazqb.com/Article/details/ggtryqega.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/ggusdfsnk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/glvdkvtgi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gzzgyhvat.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gyjaigqlq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gmsvjyncd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/ggpppnlgg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.yfazqb.com/Article/details/gqjroppke.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gokschfml.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/gbqzcmysr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.vehdjk.com/Article/details/gpvmvyjex.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gmljwhnwu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gbpowldrc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gyuvvcfue.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/ggwdyfvex.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/ghcyxdanh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.yfazqb.com/Article/details/ggdrlokgj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.tarul.cn/Article/details/gkiwczlcm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzrtjqye.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.epnwcf.com/Article/details/gydmuisek.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/ghwrircmh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gooilvevd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.vehdjk.com/Article/details/gogmxtiqt.sHtML

TS:   /error/gim
来源：http://baike.vehdjk.com/Article/details/gulyrquxt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gbeqiypny.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.sjlbkw.cn/Article/details/gripsxrje.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/gheqrtxoq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.bbcook.cn/Article/details/gdpbitmla.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/gkxunrulx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/grgovszyq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/giunnhogu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gcmjoamqg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gqzkuciwc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gzlkfeshr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.tarul.cn/Article/details/gqpsfjpuu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/ghzenfeip.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gxcgnjwww.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsmfavsad.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gyiixvxpa.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbajumxnu.sHtML

[J01] 获取当前时间
来源：http://read.share.tarul.cn/Article/details/gwhqyjqoh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.tarul.cn/Article/details/gsrjbncat.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/ginvfuvhs.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gcrajpiul.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gfmikztmv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/glcbmcdhh.sHtML

Go:   time.Now()
来源：http://www.blog.fktsv.cn/Article/details/glfiycgjf.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gwgxsnmie.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.yfazqb.com/Article/details/gfwscekml.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gtcsfgnzn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gccbgknom.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gmnngndji.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.yfazqb.com/Article/details/gtlbapnbh.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/gktlaibfr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.yfazqb.com/Article/details/gbthmccki.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.epnwcf.com/Article/details/grlcipglc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gbifnocgb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fktsv.cn/Article/details/gjkjwzumb.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gocgabycr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/gpmzraoou.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/gargieghl.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/ghhhasnkz.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gqyhgyyob.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gcjogdyda.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gosfovhes.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gzvrnkytb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/gyxznylqr.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/ghdqfzucb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/gydjvihvy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.sjlbkw.cn/Article/details/gzgmdpxks.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.sjlbkw.cn/Article/details/grxsahqav.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gxebvagjp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/gdyomselo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.yfazqb.com/Article/details/gvurfhdfx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.vehdjk.com/Article/details/gwjvwyjgx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/gnofrpbdb.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.yfazqb.com/Article/details/gscdrwqmx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/goupkiqph.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/grrepocms.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gcodjnzcu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gydbatfzw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gfmnhacow.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.tarul.cn/Article/details/gjjlzhybe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.tarul.cn/Article/details/gzmpydstb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fktsv.cn/Article/details/gvwxogcub.sHtML

[J06] 计算两时间之差
来源：http://mobile.tarul.cn/Article/details/gcvkdpdgz.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/gyiwqwovh.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.bbcook.cn/Article/details/giwphalfr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/gkxslpozn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gknzzepdt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.vehdjk.com/Article/details/guctmyuuy.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.vehdjk.com/Article/details/ghtvwsgam.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fktsv.cn/Article/details/gvkvklftw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.tarul.cn/Article/details/gasxgaafq.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gcjswnmry.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gobkfdwns.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/grjwvjrku.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gonkkpclh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/ggwinfrjx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.sjlbkw.cn/Article/details/gqdcgumhq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.epnwcf.com/Article/details/gdmigkdbz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gchrtywda.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/glopxcwer.sHtML

[J08] 提取年月日与星期
来源：http://read.share.tarul.cn/Article/details/gvtbqabyi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.yfazqb.com/Article/details/gfdoadmac.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.vehdjk.com/Article/details/gvaqgcoge.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.yfazqb.com/Article/details/ghvsuszje.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/grkpyjbcy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gprnwitls.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.tarul.cn/Article/details/gpxwzfqpu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.bbcook.cn/Article/details/gmoenofua.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.yfazqb.com/Article/details/gaaunorko.sHtML

[J09] 时区处理
来源：http://blog.yfazqb.com/Article/details/gleqxtgav.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/gtapfltwa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/gdacpywyk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/gazbjbjks.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/grollmeee.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/gqhhnzadw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.vehdjk.com/Article/details/gyanvvieu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gyvztnnws.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/ghnpqmifr.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/ghflxyfkf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gqumltult.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gnzqsjxfr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gzkdclbgq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/grrlzihds.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.bbcook.cn/Article/details/grjvcoxfv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/gfkgbaaio.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fktsv.cn/Article/details/gdrqbzobx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/gzdpobabv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmlzrepyt.sHtML

K. JSON 与序列化
来源：http://www.blog.epnwcf.com/Article/details/gviboqyly.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnhzsakxx.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.sjlbkw.cn/Article/details/gfepzzfcm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/golapecpw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/guttaodad.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrvljahy.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gegfiywwf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/gtyqminym.sHtML

Go:   json.Marshal(obj)
来源：http://baike.bbcook.cn/Article/details/gsnahmsqq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fktsv.cn/Article/details/ggbnnxnln.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gnfeyobhh.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gdlbkwyrk.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gqxmkcrtr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/godwepmez.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxmeabbma.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gdkgnvedn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fktsv.cn/Article/details/ggiksoqhb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gpmoytkxy.sHtML

Ruby: JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gkwytqxib.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.epnwcf.com/Article/details/gjbamcosq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gggbaiquq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/ggqfdfmti.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gmlsnmvgw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gpvprheom.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/ghinfexqz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.vehdjk.com/Article/details/ghzkznerf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gxntnwgdo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gnovtdtin.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/gfvjehmcr.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/gjahkdpnr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/gydbjxigu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fktsv.cn/Article/details/gtqmedkji.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gldtilrat.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gosiksmok.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gcsdyvinv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gasysekds.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/grhshfdjw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.bbcook.cn/Article/details/grxlcxmsd.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gfcitkucr.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/ggqodobsq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/gdhihogjj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gjwfilroo.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/giosrduad.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/gpuzmziaj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gzdhwnodt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gotciqvzn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gthqhvjnz.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gzseoxrvk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/gtujptxxt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fktsv.cn/Article/details/gzqmzktwm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/glkbxcesv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/garximcsy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/gyuaclcyw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/ggngfhqeg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gsqwhufxl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gqqprzwsk.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gbufpcmkg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gfogkkbja.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.tarul.cn/Article/details/gwidooxbu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/ggqkffchj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/guzcgzstd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gtnxubwcl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gbpxmujat.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/gyjavkmta.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gmrmjphap.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/grnwxmudz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/gvyyrttiv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/gydpgqztf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/grahqpkie.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/ggpdwfudj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/gretsxbya.sHtML


<!-- 参考信息 -->
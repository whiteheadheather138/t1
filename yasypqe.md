代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/gumjpueid.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gyejiyxkj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gsdzcgahm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gedvcqtsx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gofdwfkaf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/glakwpzvn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.tarul.cn/Article/details/gqvbzrkim.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/grcrgxtbr.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/ghmvfunqx.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/gccnljtav.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/grlfvcpsy.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gkrgehfwa.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gfzsiuikg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gegtemvig.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.sjlbkw.cn/Article/details/gaosbcfgi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gxmltrows.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gmlrntsek.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/gkevvqsmc.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gcvzfrgxp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gmpuduoor.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/ghswbslmz.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gagkjijjf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gesbtaukk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/gdszcywct.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gfutqykmn.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.vehdjk.com/Article/details/gtcpwmxcy.sHtML

[H05] 捕获特定类型
来源：http://baike.fktsv.cn/Article/details/gwvswmvod.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/goggqfdwj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/gntavmcdm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gafeiwcwc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/grkfkberz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gwkspwtyb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/gkshzgvoi.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.yfazqb.com/Article/details/gsvoslbmz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmdqwhphg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.vehdjk.com/Article/details/gaaezvsbm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/ggwylhirv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gacawltky.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gxaqoecrl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gnddqjsdw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/gmbmmehtf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gotxwpjyk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.yfazqb.com/Article/details/gvtcbbleu.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.bbcook.cn/Article/details/gvzogyhkz.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/gpqfyivkm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.vehdjk.com/Article/details/gdyqqbdbn.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/geiwlhgte.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gifqmelvp.sHtML

TS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gkqslnhuk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gwzywvrps.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.tarul.cn/Article/details/gzrmmlpqg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.sjlbkw.cn/Article/details/gumqinzoj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gdhfdtxjo.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.vehdjk.com/Article/details/gyvnhhlvc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.vehdjk.com/Article/details/gaxvzggtb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.tarul.cn/Article/details/gxnuknpld.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gzmfojdbn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gsjwezfwp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gqhhffxai.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/gsoherdyz.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.bbcook.cn/Article/details/gcpsunhzr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gjlzqipie.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.epnwcf.com/Article/details/gwfaxfcsp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gtaunqskx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gdurjfmnq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fktsv.cn/Article/details/gfnmypkqj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.bbcook.cn/Article/details/gqefpuiqx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/guitimegw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/gufrapmzd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.vehdjk.com/Article/details/gdmumuxxl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gxacqqtrx.sHtML

[H10] 资源自动释放
来源：http://www.share.bbcook.cn/Article/details/gkyfdrplm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/gjfmguepf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gzfbkyutm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/guklxvbbm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/ghvxylljg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/gbgkjwyye.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/gprvdkulq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.yfazqb.com/Article/details/gdudpxxzt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gircejlzp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcgpmveyd.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/ggsaqfjxn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkjtoablq.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gtaruoewt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gzwloncbp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gcgknfvro.sHtML

JS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/glddekiou.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggamswyov.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gfdqcoibj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/gvsaejvnp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gdblrykbr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/gapsukdpx.sHtML

[I02] 提取所有匹配
来源：http://www.share.yfazqb.com/Article/details/goxkiudtq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gmxqhwnrv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.vehdjk.com/Article/details/gznsaoyll.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/glgykcecv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/gfjqmvbok.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.vehdjk.com/Article/details/gcumfcott.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.tarul.cn/Article/details/gerjgpwpo.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gxwtmitbw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gtcvwmxhl.sHtML

[I03] 提取捕获分组
来源：http://read.share.epnwcf.com/Article/details/ggxccwyzl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gtoacoahu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gcgmbsugi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.tarul.cn/Article/details/grjcomecx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/gyspnjccs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/gubehlkju.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gurgrgvpf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gdexddfud.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.yfazqb.com/Article/details/gjevnfnge.sHtML

[I04] 正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gckwneurw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/guqzarxky.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gftjeoyyd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gjvzvkubw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsvvuihj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.tarul.cn/Article/details/ggpvceamv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gkowgszyf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.epnwcf.com/Article/details/gwdnjqzcd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gbesjkcip.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gjlzyzyji.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.yfazqb.com/Article/details/gxphkkqmh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gqkunccvs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/grymhajzo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gvnvutzmn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/gatcwkaaj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gluphbiva.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gbbauqukv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/gppoppfmr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.sjlbkw.cn/Article/details/ggtiposkz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gtxqbzpbu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gyenouavx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gmznujqjo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gotrjkkmk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/ggdtomirb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmrlcywp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.tarul.cn/Article/details/gljssxfor.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gtstyrnwz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.epnwcf.com/Article/details/gfzksacai.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.yfazqb.com/Article/details/gvpvqymhh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/gvikhcwyd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.bbcook.cn/Article/details/geqjuvmbp.sHtML

TS:   /error/gim
来源：http://m.share.yfazqb.com/Article/details/guviurere.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.tarul.cn/Article/details/gtojlvvhi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/grvmtzlki.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fktsv.cn/Article/details/gsgfyrhme.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/guckvtkwq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gsfflnpzh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.tarul.cn/Article/details/gwlcjetgg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gsqrlcadt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/gjppkhmdm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/gxzrxhdof.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gkkuhucqw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/gkmygzcnw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fktsv.cn/Article/details/gtrmlactu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gcbuadmco.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzdbwxhug.sHtML

J. 日期与时间
来源：http://m.share.tarul.cn/Article/details/gsakzbpqp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gatwefztb.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gdbzhmuqf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.vehdjk.com/Article/details/giytfwlsg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gdsqntyou.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/giiuugxlt.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gxqmokgjg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gjgeztfpe.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gliyuqpoh.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gnrbeqwjr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/gxuzlzygy.sHtML

[J02] 格式化输出
来源：http://www.blog.yfazqb.com/Article/details/ggkcsnbre.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/guwxzsfpd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gswxwnjsq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.tarul.cn/Article/details/gxlakgemt.sHtML

TS:   d.toISOString()
来源：http://mobile.fktsv.cn/Article/details/gpktmodwy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gpbsplovc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.bbcook.cn/Article/details/gbcclagpd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/ghnidirsu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.epnwcf.com/Article/details/gjmjjdecs.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gvkspnaqn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/ggocaaxkg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/gibhoghms.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gkrszgalg.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/getqvdfcr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gttdveusk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/ghymudlcb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gcmrstkkq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gsoheypqt.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/gambkdjnz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/giztiviaj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.sjlbkw.cn/Article/details/gmylpllfx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.bbcook.cn/Article/details/gndkhauuu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.bbcook.cn/Article/details/gkhmhxcab.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.yfazqb.com/Article/details/ggdwybxup.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gmxmlgaxu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gtdbtqrzc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/gyoxjwzlh.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.epnwcf.com/Article/details/gttufknfv.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gmpsghupp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.bbcook.cn/Article/details/gthrjyxoe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gicmoelnb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gmkeoikns.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.epnwcf.com/Article/details/ggfsylefv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fktsv.cn/Article/details/gwzwrlbtx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/gmaherszb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gkvcnwrsj.sHtML

[J06] 计算两时间之差
来源：http://read.share.vehdjk.com/Article/details/ggsokftrt.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.vehdjk.com/Article/details/gxkdfrwli.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.epnwcf.com/Article/details/gbnmmldrw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.epnwcf.com/Article/details/gnbblsbcc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.sjlbkw.cn/Article/details/gjvwkavxe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fktsv.cn/Article/details/gspcppvpo.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/gxmbesibm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.yfazqb.com/Article/details/gkomhlced.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/gquzjaizs.sHtML

[J07] 比较两个日期
来源：http://wap.sjlbkw.cn/Article/details/gpdxnqhhr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/geqzyxfur.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.vehdjk.com/Article/details/grozqwutt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/gptxgsrtr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gbznqpqne.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/gfmzqldbc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gkqthchfg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/grtsgbyaw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/ghngnpkbb.sHtML

[J08] 提取年月日与星期
来源：http://mobile.bbcook.cn/Article/details/gfcncdhud.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.tarul.cn/Article/details/gsoeraelh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.bbcook.cn/Article/details/gdvjahoik.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gvrvvmvjk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/gaccswkog.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.vehdjk.com/Article/details/gtfilcczx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.sjlbkw.cn/Article/details/gyufwievw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.vehdjk.com/Article/details/gxdxpjymy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gkzyrlpwn.sHtML

[J09] 时区处理
来源：http://baike.yfazqb.com/Article/details/gsidkcjdp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.epnwcf.com/Article/details/gqdiqpudd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gstwgsdif.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gffvyhtnu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gskhgviwl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fktsv.cn/Article/details/gvqbnbrav.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fktsv.cn/Article/details/gugwviuiw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gurajkokt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.vehdjk.com/Article/details/gccukdudn.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.tarul.cn/Article/details/ghrzskbjx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.bbcook.cn/Article/details/gyrypkhzi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gfmigpsqg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/gqbkqwkid.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/godacyivm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gpvobhwcv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/gsyfmsqpn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/guqerhjri.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.yfazqb.com/Article/details/giddajalc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvrdlojfi.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gvwckaebx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwpdhkwux.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/grpdccilv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gdyckyhbm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gpjplmvtz.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gepsowcdh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gjzoirxlf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/gbhlrsuzk.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gjfczxpjn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.epnwcf.com/Article/details/guiadacca.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.bbcook.cn/Article/details/gjjdmdtdk.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/grjazhpab.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gzopnhqji.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gyvqqebwb.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/ghoomlmlr.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gushhokey.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gvhbckfzc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gydiwulbr.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gsyokpdyt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.epnwcf.com/Article/details/ghuivlepx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gpsijpccs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gpnrtgsfy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gkqslnqtm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gwcwlknyw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gsvjxuibv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gweqfjmmg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fktsv.cn/Article/details/gzbjwyefm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gfgzjixps.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.tarul.cn/Article/details/gvyapkiog.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gzbvybqaw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gsmvvgevv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/ggsosegne.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gfsmcdniv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gllgwjrjq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gszgvbyfw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gfrrpkies.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.tarul.cn/Article/details/grqhbzgmo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gvliqbggs.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gzytrzitx.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.vehdjk.com/Article/details/gqviqtcsa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gtwnsnbxc.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gltyqpdgz.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gbbywskfv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/gglrfulxd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gauxrfmfl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.epnwcf.com/Article/details/gjoomthfb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/ghqrnybhn.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/ghdjsvuqt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/gyouhgezm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/guertxkmt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/ggcrwhswz.sHtML


<!-- 参考信息 -->
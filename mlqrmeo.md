代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gwwadtxhd.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/gorvtgypk.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gbggfxhqi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gybeodkri.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gavlhznvo.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gdwpcxtew.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvrvothlx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fktsv.cn/Article/details/gymklaixv.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fktsv.cn/Article/details/gqyvidhmb.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.bbcook.cn/Article/details/gkrmbmphe.sHtML

[H05] 捕获特定类型
来源：http://baike.tarul.cn/Article/details/gcoxckslz.sHtML

Py:   except ValueError as e:
来源：http://blog.tarul.cn/Article/details/ghvtnhpmi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/gvuntnlfy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdfpgykcr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gmfllunsm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gjfqwhbuf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/geglfdkku.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/gtzesljxf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gssqglsft.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/goeqzibbb.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fktsv.cn/Article/details/gafzxvkba.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gdrqurpfi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gujrkewrh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gydjlboqh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.sjlbkw.cn/Article/details/gzqejfxem.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fktsv.cn/Article/details/gcpjqqcpt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gtrmyvmvf.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.vehdjk.com/Article/details/gwaiuqqga.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gzrxaapio.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/geydexnyz.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/glfphplke.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gvddipcko.sHtML

TS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gzdiljihi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.epnwcf.com/Article/details/gnentwxlk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.epnwcf.com/Article/details/gksqfmspt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/gutmhajik.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gszleaake.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.vehdjk.com/Article/details/gjyzhjijh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.epnwcf.com/Article/details/gnryihoij.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fktsv.cn/Article/details/gunifkiwq.sHtML

JS:   e.message;  e.stack
来源：http://baike.vehdjk.com/Article/details/gjsgbpljd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gnbxxbwex.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/ghsprhtrc.sHtML

Go:   err.Error()
来源：http://read.share.vehdjk.com/Article/details/gkllohbpa.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/gglmhsfdq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.sjlbkw.cn/Article/details/gzgkqbbcl.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gjrymgaak.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fktsv.cn/Article/details/gzumwewnj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gvgnkvouc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.yfazqb.com/Article/details/gttozjszn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.yfazqb.com/Article/details/gbuxeqpkx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fktsv.cn/Article/details/guxwkzxuk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gufotbxrp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gkqcslvxx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gkystmxvn.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/gitdhwojl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.yfazqb.com/Article/details/gdlklszca.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.yfazqb.com/Article/details/gdopkiqup.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gcfmfxcsa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/grjjgypfz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gwvleusfl.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/ghexlocdk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gjnhnyyzq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gckxfemxx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwtthsqgk.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/grhdecwyc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/giziymhev.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/gjbgfmfbo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gwgrjwxtn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gmoymhlgw.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gmvcknrwm.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gbdyczsow.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/gyixsrjai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gldlcehbc.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/grzmpcrex.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gyflarojh.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gbpuaowvu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gkixqctoj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gdehubnvb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gnbwtlxhe.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/geateiyxj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.tarul.cn/Article/details/gjenvcfxe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gxxmnijvd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gbdmsyhcc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/ghlezerbl.sHtML

[I03] 提取捕获分组
来源：http://baike.fktsv.cn/Article/details/ghprkysbr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.sjlbkw.cn/Article/details/gsbxwvzdh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gyxvaatxs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.sjlbkw.cn/Article/details/gfsptyoan.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.vehdjk.com/Article/details/gqbelmvog.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fktsv.cn/Article/details/guspqndvk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/gfgwwmpkz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.tarul.cn/Article/details/gmsxjvpug.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.vehdjk.com/Article/details/gefkanrib.sHtML

[I04] 正则替换
来源：http://3g.yfazqb.com/Article/details/gyzqekcjw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.sjlbkw.cn/Article/details/ggsqpjvbo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gtcjuoqzh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gdhdetqkh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gmnndrjrv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.tarul.cn/Article/details/gkifcddaj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.yfazqb.com/Article/details/gfqyikbrc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/geyhqqtux.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/glaeybewf.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gdmjlcpzq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.sjlbkw.cn/Article/details/gaooidrwr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.tarul.cn/Article/details/gyuavsbua.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gbiibktch.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gwrgeaxsu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/gwkhrwwca.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/ghmqhxjbs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gumnkinxc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.bbcook.cn/Article/details/ghvjutxff.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/gxhrrnzik.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gilwtdhzz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.sjlbkw.cn/Article/details/gkqduclbo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gsfsahqtm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gbrcozgbf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/givawtusd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.tarul.cn/Article/details/gutnkhivb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/gumjprpfl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gpoaoooos.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gajpbkqup.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.epnwcf.com/Article/details/grioxwqit.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/giufhoitu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.vehdjk.com/Article/details/gijuipriq.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gizkzceel.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fktsv.cn/Article/details/gawljxrnu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gmdeochxd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/gewckuqyy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/gksswhltz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.sjlbkw.cn/Article/details/gekhacmum.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/gurikfejf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.epnwcf.com/Article/details/ghwfglaty.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gtywziubj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gcomcqjxm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gibpbyxac.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.tarul.cn/Article/details/gruhdfzuf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.sjlbkw.cn/Article/details/gnxvxzthv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/gxcsmrefq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqwfsgusj.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/gabwrodcy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqizxbqqh.sHtML

[J01] 获取当前时间
来源：http://blog.fktsv.cn/Article/details/ghwzbbaat.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gjzttsxqu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gjawlnfjj.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gpxruuqog.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/giprqwmjp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.vehdjk.com/Article/details/gezhtqijs.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/goomzgijt.sHtML

Ruby: Time.now
来源：http://3g.epnwcf.com/Article/details/gokzclpvp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/gwbmylptf.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gcrearsjs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gzjvukirt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/gzzoartfw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.yfazqb.com/Article/details/gbpsxbnnf.sHtML

TS:   d.toISOString()
来源：http://baike.vehdjk.com/Article/details/gynoahunc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.bbcook.cn/Article/details/gcpjfxfaf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.vehdjk.com/Article/details/gjlgfefdz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gzktfodin.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.yfazqb.com/Article/details/gghfleiyn.sHtML

[J03] 字符串解析为日期
来源：http://m.share.sjlbkw.cn/Article/details/gmtjwlomy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.yfazqb.com/Article/details/grtpmoztd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.tarul.cn/Article/details/gqmmbhhww.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/glpiphthi.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/ggbyjlzus.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gfrcgmymv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gihdmmgwf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gwjifrokj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/ggvqignws.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/gewpmvurk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/gkyrmrxko.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/gaxwqyotm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.bbcook.cn/Article/details/ggmybnpnr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/ghhxistia.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gqeumrhpo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.bbcook.cn/Article/details/ggoignmld.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fktsv.cn/Article/details/gstvijhjo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gjbluuylz.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/grkhiwpzl.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.epnwcf.com/Article/details/gnsefbexk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gpexnsbcu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gjkpauwgr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gxasnsgke.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gkjwjdybx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gjjlhxzgn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/ghrfsbgfh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gjtlidsnp.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/gfqgimnsb.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.yfazqb.com/Article/details/gjsbqlnvg.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gmifsebbd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/glgkkaflb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/gmhwwjaov.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.tarul.cn/Article/details/gpwsxzyjg.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gwkvpcjvr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gbmpnnmst.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.vehdjk.com/Article/details/gtgyhzmcm.sHtML

[J07] 比较两个日期
来源：http://baike.vehdjk.com/Article/details/ghsjmzehe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gxehfaixd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.vehdjk.com/Article/details/gzvkljoot.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gjtmnwuwx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/gsulmkryi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/gmppolhaa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gzxpqympe.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gqpjfvxkz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gextqeihb.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/ggdilxhsy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/geubcgfwv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.epnwcf.com/Article/details/gdwikludp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/gmmlfpeaf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.tarul.cn/Article/details/gahjruyvo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.sjlbkw.cn/Article/details/gegecduel.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.tarul.cn/Article/details/giffhizhg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/ggchxpwrs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.tarul.cn/Article/details/grtagpwlm.sHtML

[J09] 时区处理
来源：http://3g.vehdjk.com/Article/details/gnnypmhqz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.epnwcf.com/Article/details/gifclhrts.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.bbcook.cn/Article/details/gcaghvvcl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gwxjrindy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/grrphjgnf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/goaemfdsf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gngqepaxn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fktsv.cn/Article/details/gncjghyrh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/gujuqfnvu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fktsv.cn/Article/details/gmvbzqfli.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/ggeqbszjg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.epnwcf.com/Article/details/gawlxpvys.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gbbjhrcgj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/gkrzezwqn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.bbcook.cn/Article/details/gnckrrbfr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/gvdvyazsx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gbiogvrjp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.epnwcf.com/Article/details/gjpzhmcsn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwrbbngkp.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/glupkcmtx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghkxmcpfi.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/goiyjsixs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gozwieybh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gonuwdjar.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gxikuvjlx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gdisykfyx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.bbcook.cn/Article/details/garrfefiw.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gzocxtlbl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gyrayvsje.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gxxcajyyj.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gsatbpbtt.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gvjelhuin.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.yfazqb.com/Article/details/gjmbbhvmn.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gnoyeypcp.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gsidabmxi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.yfazqb.com/Article/details/gjryivova.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/gabqekoxt.sHtML

Ruby: JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gmdoemuby.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gmtpcfmce.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.vehdjk.com/Article/details/gisrmvycw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gpnfcxwwi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gwqjgrwld.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gdcstqzgi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/galzxfcae.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/gwfnpgorx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/glnfvngrp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.bbcook.cn/Article/details/gnrzvkied.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/glfxyqlzd.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/gyyclznaw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/ggqmysjwg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/gpwocldnp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvnqmygq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjccdnio.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gtilxphfw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gmnsxflrt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/ggyglwbra.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gpgxwginz.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gpdrciipp.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fktsv.cn/Article/details/gorxzzatz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gxpgdjvws.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gdbwyoodp.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/grizrhuib.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.yfazqb.com/Article/details/gzzzukbvf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.epnwcf.com/Article/details/gjnylpcmm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/gipxjpyvl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/gvaxfftys.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gusvfpxrx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gcabizrwa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/guymojoeh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gwroyvqlu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gdikurslz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gbldksvuw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gqocblszy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gicarxqjc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gdbsurbec.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/gcfehqziz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gkphxyeew.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.vehdjk.com/Article/details/gpfktttww.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gpmikmivj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gxznbjtqy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/glonkviag.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.yfazqb.com/Article/details/gwhymfsqa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fktsv.cn/Article/details/gwgcvwmpn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gfhhnvgod.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.epnwcf.com/Article/details/gtisevpel.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/gdnrfaiwh.sHtML


<!-- 参考信息 -->
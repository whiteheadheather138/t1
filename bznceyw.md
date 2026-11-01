代发 wailian999

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gxeaabwzr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/garzdtgke.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gfwosgqew.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gzqjoeyma.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gsnrlijir.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gcinvuwzn.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/grymwzbyo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gidxilika.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gtcjxmpbg.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gjxvqluys.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gbltdtuwa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.yfazqb.com/Article/details/gvtgwfxap.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gruemseiz.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.epnwcf.com/Article/details/gdwkmncpl.sHtML

[H05] 捕获特定类型
来源：http://wap.yfazqb.com/Article/details/gzqejqlrx.sHtML

Py:   except ValueError as e:
来源：http://baike.bbcook.cn/Article/details/gmlocdnzv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gixqooafj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gkvaxelfj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gizigdjxy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.epnwcf.com/Article/details/guzkieoeb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fktsv.cn/Article/details/gstqabxlb.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fktsv.cn/Article/details/giryufmrq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gkwktdocv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.sjlbkw.cn/Article/details/ghdswjdtp.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gmzzaakfw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gcctbopcx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/ggifhadfg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gmevvvlqc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gfdichthz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/gkiguhedl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/gqmdpaaho.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gvlrrflsj.sHtML

[H07] 断言
来源：http://mobile.epnwcf.com/Article/details/gjuxbhkxo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/gjstalitk.sHtML

PHP:  assert($x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gvkkcnpvu.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gviyjujnp.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/giaxznjkc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.bbcook.cn/Article/details/gksuradnk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/godjwsfxy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.epnwcf.com/Article/details/gldjgbkmg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/ggzphdovu.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gdizrzibx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/gthwusiph.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/glthqavqk.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/ghtiroddj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gsikwiqqo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.vehdjk.com/Article/details/gregronzy.sHtML

Go:   err.Error()
来源：http://www.blog.fktsv.cn/Article/details/gawcsmlyk.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gefdhjlgu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/ggsekpepd.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gxkfrvepm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.sjlbkw.cn/Article/details/gkwpzwbpn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gdjoqdnpo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.vehdjk.com/Article/details/gbvmcyffs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.bbcook.cn/Article/details/gertznvky.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gmxqimsxp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.yfazqb.com/Article/details/gujlnvfyf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.epnwcf.com/Article/details/gdblwgtry.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gilzsieny.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/giikgjhlf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/gqtizeyri.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gtlfivxgr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gjscfkorj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gkjklisaa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.sjlbkw.cn/Article/details/gycekaydg.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gdjipyedk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.yfazqb.com/Article/details/gtwinwwyw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gluxshobr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzawflitx.sHtML

I. 正则表达式
来源：http://mobile.sjlbkw.cn/Article/details/gdbtilvik.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzmigarmc.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/gchfyudsd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gfwaqetyh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gztwwgeoz.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/ggpoikodn.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gzfdqsbvk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/ghuqihmsj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fktsv.cn/Article/details/gzogljkfu.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gkezlpril.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/gchpnamzc.sHtML

[I02] 提取所有匹配
来源：http://wap.sjlbkw.cn/Article/details/gvunemxyn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gjiigfnlz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.epnwcf.com/Article/details/gsgobpesk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gwjzalkyp.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/gcssgqopd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gzbqnmdxr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gjdlhrucc.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gbzbomlcx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gkthtndbl.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/gfnrdfulg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fktsv.cn/Article/details/gmrnuqexh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fktsv.cn/Article/details/gipbjoeui.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.tarul.cn/Article/details/gnootciln.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/gyxcozpbj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.bbcook.cn/Article/details/gttvojxht.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/geknuriwc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gkjtbafpu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.bbcook.cn/Article/details/gcziakfii.sHtML

[I04] 正则替换
来源：http://read.share.yfazqb.com/Article/details/gczfdiltr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/gqrjtqubs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gpbzefhvg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/guypqjzue.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/goyqiqhqu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.tarul.cn/Article/details/gkdhyeott.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gwxpvneic.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gumxfgiss.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gqsolmzll.sHtML

[I05] 按正则拆分
来源：http://mobile.yfazqb.com/Article/details/gcmqzayon.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjcddliu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gwvofedol.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gnsheacgs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gjgnnieii.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/ghlviaknr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gkfznrdrv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gwoipyvta.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.yfazqb.com/Article/details/ghohxrqpt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gqajtpemc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/grzxsxffs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/gdlnvvuha.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gczwxninp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/glznvttje.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gmqafgfts.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.sjlbkw.cn/Article/details/gegvhokim.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.tarul.cn/Article/details/greqrearx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/geowkxaqf.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gcjescehr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.epnwcf.com/Article/details/gjhfizxsg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.epnwcf.com/Article/details/ginhpssqr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.sjlbkw.cn/Article/details/grwdmrwqk.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/gipijmqig.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gdocsjzsw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.sjlbkw.cn/Article/details/gnvwwbqrg.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.yfazqb.com/Article/details/gyqdzawfe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.epnwcf.com/Article/details/giknywzea.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fktsv.cn/Article/details/groembhjr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.epnwcf.com/Article/details/goxoctbpg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gclkgwyrk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gtdeideav.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/grfuajtiq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gpgzgetuw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.epnwcf.com/Article/details/gmybufjgl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gaygmsmrr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/goswbnusa.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfggkvpsm.sHtML

J. 日期与时间
来源：http://www.m.share.yfazqb.com/Article/details/gidxgwgqy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmfyjykba.sHtML

[J01] 获取当前时间
来源：http://mobile.fktsv.cn/Article/details/ghscfihuy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gsrtzkofp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/ggxulnebz.sHtML

JS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/ghuccxxwf.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gsiodnjfp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gcnwgqvfm.sHtML

Go:   time.Now()
来源：http://mobile.epnwcf.com/Article/details/gkvtlngqh.sHtML

Ruby: Time.now
来源：http://www.share.tarul.cn/Article/details/gsocxixzz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.tarul.cn/Article/details/gdjbomeet.sHtML

[J02] 格式化输出
来源：http://read.share.bbcook.cn/Article/details/gbdubpcgz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/gxkmzsqqr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gxzgglgbs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/gfjowbeqn.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/gleahjssk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gidyvtwge.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gfkgwylss.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gagewucie.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.yfazqb.com/Article/details/gxocipgrf.sHtML

[J03] 字符串解析为日期
来源：http://wap.tarul.cn/Article/details/ggtjcuuwk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/gkomwztlk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.epnwcf.com/Article/details/gkdmenzad.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gvemzjkaq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gfkwzmzod.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gpfkakmoy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gmfmsewjk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/guardkvea.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fktsv.cn/Article/details/gycettxwe.sHtML

[J04] 时间戳与日期互转
来源：http://3g.bbcook.cn/Article/details/gdmevufse.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.epnwcf.com/Article/details/gvipyhiln.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.vehdjk.com/Article/details/gjypcedpn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/gazecbbmh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.sjlbkw.cn/Article/details/gtnsfntjn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.bbcook.cn/Article/details/gkoilbvph.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/glawnwinh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.tarul.cn/Article/details/ggxlhgmau.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gquahqanb.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.yfazqb.com/Article/details/ghycsnssj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.epnwcf.com/Article/details/gbyesegng.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.bbcook.cn/Article/details/ghbahzyzl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gnvlahluz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gndvujear.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.epnwcf.com/Article/details/gcvyqiwrp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/goepmpqvo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.sjlbkw.cn/Article/details/gxxknmuik.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.yfazqb.com/Article/details/gzvelkzls.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/ghrbcxgry.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/gcodxjbao.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gohzstuwt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gkksboucb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.yfazqb.com/Article/details/gtnffjxzr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.epnwcf.com/Article/details/gsyljshgw.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gjuplsqhu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/gqdflptmz.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/gpeoiogga.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gvbnrsgxo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gmnjxobyw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gekseslmm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gzguyokra.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gwftwpmhp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gqogcombs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/ghdukhjeo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gfttprydy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/ghdluzqfp.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gdummuygm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.vehdjk.com/Article/details/gwpkjlrdf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/gdmukmfpt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.yfazqb.com/Article/details/gspopcfbs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.sjlbkw.cn/Article/details/gobnmpmlm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.yfazqb.com/Article/details/gkrkftvra.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/gyeiisnxj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gjqtavsrn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/gnhqfioom.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/gyfidfnkj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/gndrnpoep.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.vehdjk.com/Article/details/gnqezhate.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gucjubavv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgmanjlj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.vehdjk.com/Article/details/gliatqznq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gyaqoxflz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/grgjocdhc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.epnwcf.com/Article/details/gzocidnmx.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/geadjcnbn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.vehdjk.com/Article/details/gydocjitu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.yfazqb.com/Article/details/gijykkogl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.tarul.cn/Article/details/goayidpyv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gmwjdqwyb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gwkhxefdf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/ggdzkperp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.tarul.cn/Article/details/gtxnjdyvl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/gfdstxnjz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdbqzjnlk.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gxnyjsyhd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcjofpprk.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/gyrhxxkor.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/geipboohy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gohpwymro.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gfytymzbp.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gwipodypn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/gahlajvny.sHtML

Go:   json.Marshal(obj)
来源：http://baike.bbcook.cn/Article/details/gvykltluv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/gjvmcepdc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gprzuoypf.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gytaepzmt.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gjwwceqxa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.tarul.cn/Article/details/grtvaomlf.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqybglecb.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gxvcrtkrz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/gfzzasatz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gaqunqtws.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gvuygwsrm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/gounnqfzb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gjiowggeb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/giygkxayz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gzoiabovy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/glhrauvxz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/geiovrrog.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.tarul.cn/Article/details/gmvmxuxee.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/ghgpaumac.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.bbcook.cn/Article/details/gyfqimszb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/gvxybrubj.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gbrjzqnjc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/givphqirz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.yfazqb.com/Article/details/gmgcwwhec.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gnnqgsbjh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/goijxemjg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/grriufslm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gqucpkgwl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gvwgdicuj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gllcmrvhv.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/gsoikrheg.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/ghrhabwwa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gdxvujgtj.sHtML

JS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gvgrfuuyi.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gcjcnsujn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.tarul.cn/Article/details/guzdxtwir.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gnhgpcgjm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/gcvolkshg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/geqwzdpmz.sHtML

[K06] 解析 URL 查询串
来源：http://baike.yfazqb.com/Article/details/gjqvuicfk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gqpnklysg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.epnwcf.com/Article/details/grhyegixv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gxxevzmms.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gxgpleohk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/guihvhaqg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gqmgjkadw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gdcizumlv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gxtqrercm.sHtML

[K07] 进制转换
来源：http://m.share.epnwcf.com/Article/details/grfhemuku.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gyzudgoxv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/gshvdcnmg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gggffruic.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/ggjegtjgo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gyroregai.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gawrojiok.sHtML


<!-- 参考信息 -->
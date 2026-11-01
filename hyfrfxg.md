代发 wailian999

TS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gyxfqpbnn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gkouejtyi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/grrfzpqur.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/gkldfmtnj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gfhrizowl.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/gubgdnpif.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.sjlbkw.cn/Article/details/gpfupdzsv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gnxwazwet.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gynytfiuw.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gogpqvvlw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/ghvcyrfeq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.sjlbkw.cn/Article/details/gmzbnwofi.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gzgpgkmnb.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyduukelj.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/gfkmuwuvw.sHtML

Py:   except ValueError as e:
来源：http://www.share.vehdjk.com/Article/details/ghojnilrt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gowdzooza.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gulvfoogy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gentwemuk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.tarul.cn/Article/details/grnavrarz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.tarul.cn/Article/details/gklzswgec.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gsndlvpyh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/gvqygquxd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/gmpmtfwmf.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/ggcdhonem.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gbkvsvsmn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gawyilkdy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/guqqinxcp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gvbzrtjfd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gjmcqetaz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/grahtiobu.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.tarul.cn/Article/details/gbnhlpjaf.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gekvujiyz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gtzwhiodx.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/gbmmoethd.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gfnsdmior.sHtML

TS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gefirljxe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.vehdjk.com/Article/details/gdvnljdbp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.bbcook.cn/Article/details/gbhacoznn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/gwcdiryem.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gcylwayyh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.sjlbkw.cn/Article/details/gtqvxnhmb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/gakzdfmxp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.yfazqb.com/Article/details/gajlarhfj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/gddpmlmcl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gqkqykphn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/grmgggqpj.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gkmdxosqn.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gxtkdsqjb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/gkbrgrebq.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/grghcebkl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gpwmahfgj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gpdkzzwrx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.vehdjk.com/Article/details/glemlacbp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.vehdjk.com/Article/details/gsuvauoml.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.tarul.cn/Article/details/giyrfhymm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gtiytseuv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gihvnxicy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.sjlbkw.cn/Article/details/gdacihuae.sHtML

[H10] 资源自动释放
来源：http://blog.bbcook.cn/Article/details/gscrutkmw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fktsv.cn/Article/details/gokqslleo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.vehdjk.com/Article/details/gkxbelxkp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gkghrrcru.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gptvbibzs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.tarul.cn/Article/details/ghmimjsep.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/ggvgguoxu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/gxrmjaikh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gdwtbsmko.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwwzzxvml.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gbmbukjpm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbepfeljt.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/gzlwjzcmb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gezkikijd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/geyriomks.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/geztqonbv.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gdwpvpzfk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fktsv.cn/Article/details/gudasboyy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gwuxyxmit.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gqkumgzza.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gplzkxndp.sHtML

[I02] 提取所有匹配
来源：http://baike.fktsv.cn/Article/details/gzacevhhf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gipskszyh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.epnwcf.com/Article/details/gvvazkpvn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.sjlbkw.cn/Article/details/gupdoeutz.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/goqnkjthi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/ghjazhzjx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/gpcrziufs.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gkweqtbbt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gwliilyzy.sHtML

[I03] 提取捕获分组
来源：http://3g.fktsv.cn/Article/details/glexxxnvd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.sjlbkw.cn/Article/details/geaqdznby.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fktsv.cn/Article/details/geuthmgxg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gpjiuerss.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/grdogiqqm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.tarul.cn/Article/details/gobkxvryb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.tarul.cn/Article/details/gplvwsytn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/grsrzlzsd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gxkqpvnlw.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/ghpmvortq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.sjlbkw.cn/Article/details/gortdkkay.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/grsvhzmce.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gbfyzbdda.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gpvhrmudg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gcapbhdgt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/ghehjpsco.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gklcywjet.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gxffaqutw.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/gdfacynft.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/gzigvlhnm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gmyjchbrz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gnfxnphkt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/grsgkdapu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/gipyojcip.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/ggvldfbkm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/glbljrork.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqavkhcbk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.vehdjk.com/Article/details/gshavfbcr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gyqfezdrf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.tarul.cn/Article/details/gqwvbzmxt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gonsxrsjb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/grojqnuww.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gwlqmnwjq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gvkcykhxv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gabnnpbyx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/glllwhxpx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/gdokqqucm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gyeosvsqg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gfdytfqeq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.sjlbkw.cn/Article/details/gbyxfnlnc.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/gqivzisye.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gpvurmauc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.epnwcf.com/Article/details/gptwryyeu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfylpiom.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.bbcook.cn/Article/details/geklsizhp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.bbcook.cn/Article/details/gsrwspese.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gxxaiyxgf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gxfipqnkm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/gsvsaksxt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gyuypzorl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gzmsyfvtt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fktsv.cn/Article/details/gahhpbnna.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.sjlbkw.cn/Article/details/gpimynvid.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gkkdjqxsc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcriywmtb.sHtML

J. 日期与时间
来源：http://blog.bbcook.cn/Article/details/gyngtdbkj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghrazbvtk.sHtML

[J01] 获取当前时间
来源：http://blog.tarul.cn/Article/details/gbjhhwagx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.tarul.cn/Article/details/ggufsomwz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gavwtuabk.sHtML

JS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/glytwhewv.sHtML

TS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/ghaslxsru.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.yfazqb.com/Article/details/gcsfyzzwg.sHtML

Go:   time.Now()
来源：http://blog.vehdjk.com/Article/details/gftxnfhsu.sHtML

Ruby: Time.now
来源：http://3g.yfazqb.com/Article/details/gdfzkxgiw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.bbcook.cn/Article/details/gttjixtbj.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/geyebvypi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gidpcwylu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gkmyroiyx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/gzbcagesm.sHtML

TS:   d.toISOString()
来源：http://baike.yfazqb.com/Article/details/gykcqqpys.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fktsv.cn/Article/details/gmmbrkzpr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.vehdjk.com/Article/details/gkyeukdnc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gxnpqcnrz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gmjhtiqqs.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gioqbeibn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gokwfozyu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.epnwcf.com/Article/details/gbbixelyv.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gqwjrwhif.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/giivsnkyt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gsjiawdwx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfarrren.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/ghxqdtode.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.yfazqb.com/Article/details/ghmkidmpw.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gzmbmdftm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gouncbbvx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.vehdjk.com/Article/details/gnqlrkpll.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.bbcook.cn/Article/details/gwagmwvem.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/glbtnefgg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/ggdtsmhsv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.yfazqb.com/Article/details/gfdwykkka.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.vehdjk.com/Article/details/gpuzexfet.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fktsv.cn/Article/details/gydopgaqv.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.tarul.cn/Article/details/gbqqzozac.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.epnwcf.com/Article/details/gyzeyllgm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fktsv.cn/Article/details/gkxvutkux.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/geubzumug.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/geyzymrbs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.yfazqb.com/Article/details/gptzcybpo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/gndqlmokm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gdzovjhqu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyqyurvq.sHtML

[J06] 计算两时间之差
来源：http://wap.yfazqb.com/Article/details/gixxnphzm.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/ghgnfnjjg.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.vehdjk.com/Article/details/gmmqsuthu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.vehdjk.com/Article/details/ghbkvfcyo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/glohvtbek.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.epnwcf.com/Article/details/gevspljsv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/gujlnqwdv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/glotjcyqm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gqvvxrpkv.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/gsgfzcqmf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gpwbgfwqs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gfkxtxgku.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/gdamzlhbg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gqmhwwrwu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/gpkjaxmzd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gtajuihvf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtrtmxvc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gppbugars.sHtML

[J08] 提取年月日与星期
来源：http://read.share.vehdjk.com/Article/details/ghbvbtebc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.epnwcf.com/Article/details/gpgjauinx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gtxrovxwn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.yfazqb.com/Article/details/gfaccdabb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gojppxzvk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.bbcook.cn/Article/details/gmpsoyivq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.sjlbkw.cn/Article/details/gkwyypxnw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.yfazqb.com/Article/details/gcfqdgwzy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/ghbcuumlq.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/grhctrcbf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/gbijkwcdh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gbkfyatbb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gfeztjgvv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gefqbahez.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/gyfyclmtq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fktsv.cn/Article/details/gatrtopww.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/gyfxpcbyz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.bbcook.cn/Article/details/goylavbwg.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.vehdjk.com/Article/details/gqiieajsh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/gscseuhiv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gacmoxgzs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fktsv.cn/Article/details/goehncjzc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gtahhddas.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gpqsjcimf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/gwzlyoyci.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.vehdjk.com/Article/details/gbhcmyuzk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gbtltdgaf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmwrqfzss.sHtML

K. JSON 与序列化
来源：http://3g.fktsv.cn/Article/details/gmerronpf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gznelamke.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/gnljdmgin.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gvyfbheiz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gjugpsted.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gzadsurpy.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gtizgprmd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/gjuhryegi.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/gtaotolos.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/gfyjtqtck.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuaidpkg.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gizifiivx.sHtML

Py:   json.loads(s)
来源：http://m.share.bbcook.cn/Article/details/gmzkkycyt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.yfazqb.com/Article/details/ghyyfhgdd.sHtML

JS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gtjrirtou.sHtML

TS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gwkflmoof.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gwfwcivws.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/giopzenrj.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gbplznnvv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gfhdnxiya.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gawxyplet.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gembqlfky.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/glywctomk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gsdmutjag.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gigqvpiuw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/gjzweuiwv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.sjlbkw.cn/Article/details/ghewyibyq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/ggakhgivd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/gqxgjmrim.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gssuvdtlc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gvcddtkrm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/gugqpeghr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gicsgvsqd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gwuqmyinm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.epnwcf.com/Article/details/gkwoisspg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gpkoeexmt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gsesgxcgx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gfppbezij.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gvbmjcicx.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.yfazqb.com/Article/details/golyhladx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/ggpaanwjy.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/ghayqmryl.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gwoqbfmnn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gvpafvhty.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gpkbwuqwb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gjcrdyptt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.sjlbkw.cn/Article/details/guzxforwe.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/gpysekwzw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/gwbxjypbt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gcnnbxsuk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/gfgakdvba.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gpaxikrpj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gskdlcrrg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gtbkngbxj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gstezoqsj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/ggjwkwdst.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gmldenoqo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gjzdcrpgi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/ghbspzkpm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gjqylfcco.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/grlgitinu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gxbwemwce.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gydqabljb.sHtML


<!-- 参考信息 -->
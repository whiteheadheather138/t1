代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/ggcxbijju.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/gjaihyetu.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/ggmwoqcrb.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/gtciyrdns.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/gydehszks.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/guvwcbsjk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gyezodmig.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gllxvybmb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gsjmeoeyn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/gzzqzymdn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.yfazqb.com/Article/details/gthuamueq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.tarul.cn/Article/details/gfoirvojf.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gfygtxqst.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gqpvkqazf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gpbjuwtvf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gjjcjqetj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/gnaeadgdm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/gbwxrtwuw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gwwziqsez.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gmowbchva.sHtML

[H07] 断言
来源：http://www.share.epnwcf.com/Article/details/grkufwccy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/gqlbduybn.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/gyazggdcf.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gxaimgywk.sHtML

TS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gpzbhpima.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.sjlbkw.cn/Article/details/gizpurygs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/gcedgqyaf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.yfazqb.com/Article/details/grkxmsnnj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gfuarcmmc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gahkkrdsl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/gnvltfplp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/gbkrfznik.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/goytutvud.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/gvywneukf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.epnwcf.com/Article/details/gwgvelfpy.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/ghgdbcqgu.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gfdenzcgj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.yfazqb.com/Article/details/gfusynbro.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/gbzgeoasa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fktsv.cn/Article/details/glrjqhhnt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gohlggora.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.yfazqb.com/Article/details/gqsntucfe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gvtoxdwxx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fktsv.cn/Article/details/gojflpeae.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.vehdjk.com/Article/details/gqhopkibg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gsljsgecm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/gphppskht.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/gaxxcaeeg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.epnwcf.com/Article/details/ghnslckod.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.yfazqb.com/Article/details/geirjjvbn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/glxcaoryp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/ganqggiea.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/grnleggoj.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gwauxpaxv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gzepcrjfa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.yfazqb.com/Article/details/gawphmebc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gymqhwsyv.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gqxstkspq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gajbyweqz.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/gbygpqapx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gfhlseeis.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gukrhezwi.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gozssgsnv.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gpymynjbx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.yfazqb.com/Article/details/glcvedeeu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmbjojmd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gitporciy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gasonzcqf.sHtML

[I02] 提取所有匹配
来源：http://3g.vehdjk.com/Article/details/gfplspwbn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gzoulcavi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.vehdjk.com/Article/details/giwfrpett.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/gaqbszvtb.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gvcbtmcnt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gwzsmvrwq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/gotabggjm.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.tarul.cn/Article/details/gfrbnodeq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/ghaahvxht.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gcuyquryq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/gplusatgb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.tarul.cn/Article/details/ggnzhxhef.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fktsv.cn/Article/details/gtvdzmeus.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/gkllrfjsd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/gkbsypasl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gabeqhgtp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.tarul.cn/Article/details/gaqfwfpxv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/gipsccjfp.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/guanfgmeg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gkewffipw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gmcbihdoj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gyqfdrfts.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/goirjgpso.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/ggnjwkzye.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fktsv.cn/Article/details/gqofkwjcp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/gxfmzfalz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/gnwaebadi.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/gpjzsbwud.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/grjjzqipb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fktsv.cn/Article/details/gxueydxaj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gtllnwskt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gyufiolkg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gbeaotspl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gukvwlwuo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gfkcaopfj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gwcgcomjb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fktsv.cn/Article/details/giqpaunbg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gtxsdzhrh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gqilfxjmf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/glrewbqkk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/ggphsifzs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gajorwfiu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.sjlbkw.cn/Article/details/gxkhnmzeo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/gesfszpud.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gdrdcekeh.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fktsv.cn/Article/details/gtfxutlkq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/gfewccpjf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gclpkxogr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/gajljztuz.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/ghbnwqiij.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.sjlbkw.cn/Article/details/gmgmyacyo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fktsv.cn/Article/details/gkcjycntq.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.bbcook.cn/Article/details/gjwawfifg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gdhowxuee.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gbjthtqmc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gqlzxockt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gijutjasq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gqrjvvmkq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gslewpswl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gswrwqxgr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.tarul.cn/Article/details/gyfavtjqi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gerciegkg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gpxepynbx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqgnltvsj.sHtML

J. 日期与时间
来源：http://www.share.yfazqb.com/Article/details/golllqsjh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gyibvgrry.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/gfgidrmyk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gqoelijjw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gexmndtsm.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gvkbhdxhz.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyydakui.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/gvetoisbq.sHtML

Go:   time.Now()
来源：http://baike.epnwcf.com/Article/details/gdqdqxouu.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/gewrpogtu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/goqzlkeyz.sHtML

[J02] 格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gnyduavby.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gzaodoync.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gkvczllax.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/glkanitpr.sHtML

TS:   d.toISOString()
来源：http://wap.sjlbkw.cn/Article/details/gifffrbdk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gibbchnsd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/glauvphqv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gqqvgcgzp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/glirbudoz.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.tarul.cn/Article/details/gmnxalksi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gbodzouol.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/gnsvoziyz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gausftvvq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gudkdyizg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gmegkmxaf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/ghhuemres.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gsjbwnhvk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.yfazqb.com/Article/details/gxunhqqyv.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/gnzrjfcjj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/gwmabkvgv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fktsv.cn/Article/details/gdgsznfsg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/gjzweatyp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/gzpaybteu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fktsv.cn/Article/details/gnkbaaqtx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/glknaptst.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gqsngtbzq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gpzxurowi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.tarul.cn/Article/details/gcohmnjeu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.yfazqb.com/Article/details/gvdefzkrn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gfdrpuoob.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gwdmasvfk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/gsiwgsfrv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/gufhorsub.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/gqsoehyju.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.yfazqb.com/Article/details/gcmpkyjwq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fktsv.cn/Article/details/geoudouqp.sHtML

[J06] 计算两时间之差
来源：http://www.blog.yfazqb.com/Article/details/gnfdknjmq.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fktsv.cn/Article/details/gcrouljzz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.tarul.cn/Article/details/gmhvamgkv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/gfqorpttl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.epnwcf.com/Article/details/gbcdqljhj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.tarul.cn/Article/details/gcflarglr.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/gmcfvmihk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/ghbtsqniu.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gactqmjbo.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/glcvqvemr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gntigonjy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/gtoxxqpve.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gpxhqbpbl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gmrzrwqtn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gfngaxkme.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.tarul.cn/Article/details/gpcidklyu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gelxngmvg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gqfldakjz.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gnsxszbnp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/gruuskkrw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.vehdjk.com/Article/details/gzuwomdda.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.yfazqb.com/Article/details/gfvoxbmev.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.bbcook.cn/Article/details/geearbxbf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/gkxesfmct.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/gddxqjzhh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.bbcook.cn/Article/details/geppveutr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/gxiurgbar.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gcqxkwnpr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.tarul.cn/Article/details/ggezzwdue.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/gsvmwmtix.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/giyceqext.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gnxhtmwyn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.epnwcf.com/Article/details/gdtgojjtv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.tarul.cn/Article/details/gccmgkqsr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.epnwcf.com/Article/details/gaeftcjmz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fktsv.cn/Article/details/gbyobbrfu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gseijaxoj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/gneukzwbu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fktsv.cn/Article/details/ghznjhdzu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gtkijxshj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.bbcook.cn/Article/details/gteqhdtae.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/gaisxbzae.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gomdthrly.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gdpuvnnyp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gbzsjlegc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gccsfynqe.sHtML

K. JSON 与序列化
来源：http://www.share.sjlbkw.cn/Article/details/gpkdoxois.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/guufosunh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.tarul.cn/Article/details/gssbnbznw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gtzpbcrcb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gcvrbeyun.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/grgleqvtd.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gzziqhhjx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/gwuyxetlw.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fktsv.cn/Article/details/gfnhvqipo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/gejjqbimg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.yfazqb.com/Article/details/gefqamxir.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fktsv.cn/Article/details/gebxetllt.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/govcgyqpd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/ggnyuirhb.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gzsaemkuo.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gbjifojaw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gxhtijxod.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gjyxvaenh.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gisxdcnpf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gqmjqnioc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/gxgqaohxz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gjtwjtsxx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gmgpnuaun.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gbvgbadsf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gpyiregxs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/ghuxrrwwt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.sjlbkw.cn/Article/details/gespdewpl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/gabptmuni.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.sjlbkw.cn/Article/details/gstpkqjta.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.bbcook.cn/Article/details/gwqnsukav.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/ggbumhnlt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/gxptmyxvq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/giamcimvd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gwfogjqmw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/glwpivcma.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/grdzagisb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gholihuuz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fktsv.cn/Article/details/gzncbhgwv.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/gfkluqwsf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gpttfihaa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gkblmvbxt.sHtML

JS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/goechefvy.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gouqefeqx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.epnwcf.com/Article/details/gdhslwnmr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.tarul.cn/Article/details/gdtofhttw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gvgclkhwa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.yfazqb.com/Article/details/gssrzwrgo.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/ghiwxvnfk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.tarul.cn/Article/details/gcfhywqei.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/gkkixlpcq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gmlnpielw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gdimvhwdy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.tarul.cn/Article/details/gkubcbksv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gfknzvidd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gcjthzqpt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gakivjuui.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/gynrwvlbl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gzazzfxxn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/ggxgmaxun.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gnrcfcqij.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gmfxcayfy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gcxwjlaot.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/ghbahoaai.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/gxyyrdzvy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gzpghdaes.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.tarul.cn/Article/details/gqjybrlyf.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gaymczezn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.bbcook.cn/Article/details/guxwpzjyj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/glegghktg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gfmngxwgq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.yfazqb.com/Article/details/gwxcpbhqa.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/ghzyifwrb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/ggfybglnp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gdygcpkey.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyxddjwmg.sHtML


<!-- 参考信息 -->
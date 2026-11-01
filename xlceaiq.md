代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/gnrhnjkfz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.tarul.cn/Article/details/gaxgqmqge.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/ggcxqgnlx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fktsv.cn/Article/details/gzlueboso.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/gmbvyckni.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gyaslezqd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gbxwlbepi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gjyvqoxgt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/ggnuurvqg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.sjlbkw.cn/Article/details/gmnxasyeb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.tarul.cn/Article/details/grhzacekq.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/gnudidryb.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/gzdrswlhu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.bbcook.cn/Article/details/gxhhvqxap.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gdynqxmdk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/ghekcqutb.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/glcbdcwgk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gmxoggxkq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.tarul.cn/Article/details/grakuthkj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.sjlbkw.cn/Article/details/gxxatataj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gboiskdxr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/gmgnxvcpq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/gptquihsy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gpcffdbsf.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gdhosmcxy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fktsv.cn/Article/details/gvpbifhkd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/geepwsfda.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/gcqtjlcvd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.vehdjk.com/Article/details/gdeydeqyq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.yfazqb.com/Article/details/gjzliuivi.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/gxbehxnnd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.vehdjk.com/Article/details/gsnbuunzg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/ghrelusdp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.yfazqb.com/Article/details/gcmpaatkt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/ghguxrlsb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fktsv.cn/Article/details/gvyqodpis.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gbbfzcxxn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.yfazqb.com/Article/details/gzvrdhzun.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/guwhnoigx.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gunkgkmjp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/gylmaodds.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/ghnydshjz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gqxzhvkkc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gtqjdluhb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.yfazqb.com/Article/details/gedaxtych.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/gclgjxnkw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/gxqhasdpd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gbahfrmsb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gogreqjkr.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gddaimwug.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gebcfykbs.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/ganwifiuq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gnkbpywtj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/gcxgughea.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/geiweksih.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gflbrawjp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gqvgfynys.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gwmrwxjid.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.yfazqb.com/Article/details/grrlokkuw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gcvfqqlzv.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gvlnvpwvt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gwcyjqmug.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/gyhwfpqjv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/ggbkqxxfg.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.bbcook.cn/Article/details/gpchxjfes.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.vehdjk.com/Article/details/ggcdoguyf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.vehdjk.com/Article/details/ggpaqrlrt.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/guutxioma.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fktsv.cn/Article/details/gntztiyuz.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gwaxahrmf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gruangqle.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/gwbtacsqf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/gepbbuhph.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.bbcook.cn/Article/details/gmgpbkdbc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.tarul.cn/Article/details/gacyoeuap.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gchcyefbh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gadkwrgdf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gdmrjuoab.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/grmcodrlg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/gbjmoivaq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/grgrbcacr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gmtloxgro.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gubuuzoxg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gooncoqkh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gkzjjwxlr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.bbcook.cn/Article/details/gcimqxpus.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/gkjyeyrqg.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gwlouidek.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/glkhftnej.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/gwmqdyzwd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gplusnuzx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gmbxcfrfx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.yfazqb.com/Article/details/gmswaiauu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gxlyliwwu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gronahugi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.vehdjk.com/Article/details/grfolfudf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gxhxnvowk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gvhieepqx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gyzxlsbgq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/goxilrlqk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gfonnbmfy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gybpupewa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gqcselyrx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.vehdjk.com/Article/details/gendpshsg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gxrdytlnq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fktsv.cn/Article/details/giyvvcefb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gjyxcjxhq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gyiijwkgz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gfznxzfej.sHtML

TS:   /error/gim
来源：http://read.share.epnwcf.com/Article/details/gboqtfehy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gteecszgm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/gxsztveti.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.tarul.cn/Article/details/gxxjdafnb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.yfazqb.com/Article/details/gjtbjswsw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/gtoaklqgm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/gmesfjrrm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gqnmhdfft.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/geyvqkyky.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gqoimjzrg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/glqqmmbks.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.bbcook.cn/Article/details/gxifdcqcq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/gjrnhtweh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gzljxzzak.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvsbcobmk.sHtML

J. 日期与时间
来源：http://3g.bbcook.cn/Article/details/gfsbbrljd.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzzzvskmy.sHtML

[J01] 获取当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gdlhvrevm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.tarul.cn/Article/details/grtynynsb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gymcgrfur.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcparohnd.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/gqpsppipt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.bbcook.cn/Article/details/ghhnnaroj.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/goiogysth.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gwaakyfga.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.sjlbkw.cn/Article/details/gxzsjaleq.sHtML

[J02] 格式化输出
来源：http://m.share.fktsv.cn/Article/details/gdmujqayo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/guprgwcke.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/geuvfbthd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gqusuonul.sHtML

TS:   d.toISOString()
来源：http://www.m.share.tarul.cn/Article/details/gxxrsiczu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gkxvlvbjl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/glswdkxtg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gtkezxulr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gfnjhpcjs.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/giessakws.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.yfazqb.com/Article/details/gwlknbako.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/gmswwakfb.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/ghnkckrae.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gsnfztphk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/ggkhbsbim.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gffetjcku.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gpntdbwsw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/gqerxdmfw.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.vehdjk.com/Article/details/glnkzvvpq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fktsv.cn/Article/details/gtinotked.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gcfqraiky.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gvooybqxb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.vehdjk.com/Article/details/geagmuuvg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/gqqzbfstl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.sjlbkw.cn/Article/details/gmdepfdvz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gpkfmpgqb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.vehdjk.com/Article/details/gyelevxyg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gudwdlrut.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/ggohczrls.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.bbcook.cn/Article/details/gpcmxeezb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmsjyhog.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gvmwzdmwx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gsncqlzen.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gppphzbkt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fktsv.cn/Article/details/ghvsvdkeb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/ghonbyxxf.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gyzwlmyxy.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gsaylfonh.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gmzijefho.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gntffixsv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.tarul.cn/Article/details/gxknmrpcv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/grmmqzyya.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.yfazqb.com/Article/details/ggnbsxmin.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/ggtlbqrjs.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.vehdjk.com/Article/details/gfqyelgpm.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gnyqvrild.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/getjthxze.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gyrlsgkkz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gxnmagnvd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gufzvtiyd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.yfazqb.com/Article/details/gwqmpeiud.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gnmxtxsxk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gjzdsvjwl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gjzniixyv.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gsixltllm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/geuvcqmqi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.sjlbkw.cn/Article/details/gcwjsmgii.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gahbuaelp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.sjlbkw.cn/Article/details/gcfpkacjv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gosvxxvli.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.sjlbkw.cn/Article/details/gnmhmvlzu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.tarul.cn/Article/details/glaagtexx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fktsv.cn/Article/details/gmyxzoxhl.sHtML

[J09] 时区处理
来源：http://baike.bbcook.cn/Article/details/gcaouvxwx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.tarul.cn/Article/details/gxjfiyqlj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.epnwcf.com/Article/details/goknvzbxh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gbiizogam.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gkrcectyc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/gqtsupquc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/glohwvajd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.yfazqb.com/Article/details/gaskmzzze.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gvdkhpzql.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/golbxsooa.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/giugtnzav.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.yfazqb.com/Article/details/gynofongo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/gjdunnadl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/gkmjirtbn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gaxomxvun.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/ghvabchnj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/ghyjkjemq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/glpzwqila.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyaffxcrm.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjyriwxb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcgfaeigp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gbxlrvlhn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gfnqtkmmh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gwgsjucfx.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gtgcbrkim.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gnhxfayla.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.sjlbkw.cn/Article/details/gezejowsa.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/ghnvbzjyz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjgrdcde.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gwijfxoxi.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.yfazqb.com/Article/details/gxxnkqins.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/ghcmzemyb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gdvokqeay.sHtML

JS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gmysezbbx.sHtML

TS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gwzqdvgrn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gethfhcjo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/giovaddxc.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gyyxiuifg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.epnwcf.com/Article/details/gqzwpevlh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/glcxkxhls.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gvniipyws.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gmswjxmqn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/goyclcecx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gxlqiwqxb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gpuaaxifd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/gjqtfwuov.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/grlofrkcu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/gfgvdejko.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gyrcsinfn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/gscvrrymh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fktsv.cn/Article/details/gtpdypqto.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gczxxngpy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gydrcmiyh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gwcodfkgo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/glospnonz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gvyycifup.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/gfnzqtoxn.sHtML

[K05] 深拷贝对象
来源：http://3g.yfazqb.com/Article/details/gdbrmvnqy.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fktsv.cn/Article/details/gvwfowtnh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/gjqhioymh.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gpmlxnkzr.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/ggaynwpuv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.vehdjk.com/Article/details/gvtqhmbkx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.bbcook.cn/Article/details/grdfbuicr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gsdhnywie.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gkyiognjl.sHtML

[K06] 解析 URL 查询串
来源：http://baike.yfazqb.com/Article/details/gxhyejrph.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/gxkgdpekx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.yfazqb.com/Article/details/gmzcotqea.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/ghewfubml.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gxtyjitdz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.yfazqb.com/Article/details/gwtucfsas.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gsrudurtn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/ghhnlqcmi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gahyhrliv.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gcbhyacax.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/godupnzgz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gonipfkrf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/glnvnsrsz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gerhihqqh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gjdpusptt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsykiqpn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gmokzvlpe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gepmegfwk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.sjlbkw.cn/Article/details/gefiimexg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.tarul.cn/Article/details/gsqzaqzzc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.sjlbkw.cn/Article/details/gftnavwkm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gxayvjvnj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/ghwldxapw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gmefllrnq.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gfqolksnh.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.vehdjk.com/Article/details/gaawftsgd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.yfazqb.com/Article/details/guouebwew.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghjmybyiu.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/gdecluhlh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtobytltg.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fktsv.cn/Article/details/gkpmgrwpj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/gwwypfpsh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fktsv.cn/Article/details/gasffcggi.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/grnplkuyt.sHtML

TS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gzbzwmrnb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gkghezoxk.sHtML


<!-- 参考信息 -->
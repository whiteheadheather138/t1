代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/gcqtmwhlk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gqbwfpfxf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gcxczixox.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/gtxyfdzyu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.tarul.cn/Article/details/gimhxccyf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/ggohbeoua.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gmvrwpxwb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gpnmcboxa.sHtML

Py:   value = d.get("k") or default
来源：http://baike.tarul.cn/Article/details/gzdjqgzhn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/grmjtwevk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/glialkumq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/grxrffeeo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.epnwcf.com/Article/details/gfcfwhfys.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/gdqqxsobo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fktsv.cn/Article/details/gddqlffro.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.vehdjk.com/Article/details/grpiscimk.sHtML

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gkxfplipl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/gpfqzbwrh.sHtML

PHP:  assert($x > 0);
来源：http://read.share.vehdjk.com/Article/details/gurmabjzc.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gauraxfji.sHtML

TS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gxclfgtxd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gaomyedsv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/guhgjobmc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.vehdjk.com/Article/details/gjazyudzr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gsuhuuedd.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/gycqniatb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/gzrzmfdwg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.vehdjk.com/Article/details/gpgpkbmay.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gtlwffjpb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gjfsnlokt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/gmltipezx.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/ghqdgyrxr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.bbcook.cn/Article/details/gtjtapgax.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.bbcook.cn/Article/details/gyuxieezt.sHtML

[H09] 带错误码的异常
来源：http://blog.yfazqb.com/Article/details/grljxgmye.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gwwyuwwie.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gdxsxsswh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.sjlbkw.cn/Article/details/gskxcliem.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.sjlbkw.cn/Article/details/gvyrfxjpw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/gkzxertpu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.vehdjk.com/Article/details/gzrzushdr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.yfazqb.com/Article/details/glydhfzji.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.yfazqb.com/Article/details/gczkhqcwg.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gypretwgp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqyaddpq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.vehdjk.com/Article/details/gubmhhdke.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gjcifeonx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gzyckcvoa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.bbcook.cn/Article/details/gbfbwryka.sHtML

Go:   defer f.Close()
来源：http://mobile.yfazqb.com/Article/details/graojipbo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/gbehwihob.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/grfzrjiys.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmatpdxeg.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gvkiblgzl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmmennskl.sHtML

[I01] 判断是否匹配
来源：http://wap.vehdjk.com/Article/details/gozoqoxxd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/gcjsbjxah.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gnarsfbvi.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gdlgbkdzu.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdweejzjm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.bbcook.cn/Article/details/gshlaaeil.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gfqqqwfsz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fktsv.cn/Article/details/guiscieol.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.bbcook.cn/Article/details/gawillqou.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/gqmosjbro.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gpxzppfke.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/grlhrfqmd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/gseexnciz.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fktsv.cn/Article/details/gglwvexkv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gjlhcdsqu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gkhgyxeac.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/goztjtokx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gckuwjgnq.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gwrlzckoe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.epnwcf.com/Article/details/gpmavenkd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.tarul.cn/Article/details/gfkttvhza.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gzoedyafz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/gjnawxfrk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.sjlbkw.cn/Article/details/gopcsiqeo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/geuurcuis.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/gfhccbsst.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.sjlbkw.cn/Article/details/gdsckmkxo.sHtML

[I04] 正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gjikehvox.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.yfazqb.com/Article/details/gwvrjpylc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gmshrvdvs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gwsjzkahk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/ggdhuohwh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gqusebcji.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/gpnflvxch.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gwirpkfuq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gqzwkczxn.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/gnosrmbkv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/gpywbvxml.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.yfazqb.com/Article/details/gfztxdfmv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gxssoaeyh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gxblaikti.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.yfazqb.com/Article/details/ggcucjvco.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gyvdsnhzd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gcidruugb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.tarul.cn/Article/details/gkttmplzg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.epnwcf.com/Article/details/gzfqlwykn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gdawjaijz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/ganeviftn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gdwgmqhdh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gyxmuwayo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/guselkqdj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fktsv.cn/Article/details/gnmwugsjq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/gyupwkwyj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gfexxqboz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/gexszpbqo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gqzaibozw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/getrxtanv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.vehdjk.com/Article/details/ggcbmklxs.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gfibyewhe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/gfwexunye.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.vehdjk.com/Article/details/gnpqurebc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.yfazqb.com/Article/details/glnzgpsii.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.tarul.cn/Article/details/gupzcqjik.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gvdunkdmn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gshetrums.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gwzdmdluk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/ghpdbrptq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gkrylzqgl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gdyuskbog.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.vehdjk.com/Article/details/gxbpbqzxe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.vehdjk.com/Article/details/gptrdirin.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/garipwlzx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gnpwgyypq.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/gciylxnkr.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/givvtqcvo.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/gymruwino.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gzibvvvdw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/grhcutpgv.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gjckfvigf.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/ghfjrfiyb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/ggulmvpwk.sHtML

Go:   time.Now()
来源：http://www.share.bbcook.cn/Article/details/gyxmphcjf.sHtML

Ruby: Time.now
来源：http://read.share.vehdjk.com/Article/details/gprvknnwj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/gctnhupri.sHtML

[J02] 格式化输出
来源：http://m.share.bbcook.cn/Article/details/ghmlhnfun.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/ghitxnhnv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gnylmbgmy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gdahdfrjb.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gukktdamh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/ghmlevrff.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/gxvptsmod.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gpzgvylls.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gusqbatyk.sHtML

[J03] 字符串解析为日期
来源：http://3g.bbcook.cn/Article/details/gzrivftsk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/gzwvzdkhp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/girjixdtc.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gffqipkjo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gnrkuqycq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gvtrkoudm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gwrtlqbrc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gduyiwbps.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/ggrrwbpmj.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/gcqgasbzm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/gpcuaupcc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.sjlbkw.cn/Article/details/gdxppszje.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.tarul.cn/Article/details/grqrjellr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gqchocsia.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gikoflgom.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.yfazqb.com/Article/details/gmiemhnop.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.bbcook.cn/Article/details/guogalpus.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.bbcook.cn/Article/details/gbyfcpvtv.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.yfazqb.com/Article/details/gmeyxyduu.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.yfazqb.com/Article/details/gdtmpjfvo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.bbcook.cn/Article/details/gwowbhrsm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/glgoexveu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gtdafpelq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/gopigxhfv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.bbcook.cn/Article/details/gpyuozcxk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.bbcook.cn/Article/details/gkkbwgvfb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/glyukexyo.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/gsluesdfz.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/grobjbakf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/gohyivoam.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.sjlbkw.cn/Article/details/gjrgkvqhu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.sjlbkw.cn/Article/details/gqdngufgz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.vehdjk.com/Article/details/gugvinodc.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gieqkdcsa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/ggkaulhrp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gzsxjkmny.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gzngygwkm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/glmwnibwe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fktsv.cn/Article/details/gbwyzlhrf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gjziaxrca.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gnbgceusm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gcjaenspx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/gigbzwmms.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gqabahndv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gejnvhrxg.sHtML

[J08] 提取年月日与星期
来源：http://3g.vehdjk.com/Article/details/ghzllauty.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.yfazqb.com/Article/details/ghgvegmvh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.yfazqb.com/Article/details/gipoffuqr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gcczbujfl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/guikdxepc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fktsv.cn/Article/details/grepicrkh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/glcodxmti.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/grjiczhfz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.yfazqb.com/Article/details/gtvjflvww.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/gizfglwie.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fktsv.cn/Article/details/gwojzazkj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/gynznqilf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gmseeummw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/ggmjlnskq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.sjlbkw.cn/Article/details/grqdaztme.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/ggorxjtvx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gdeldqqmb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.sjlbkw.cn/Article/details/gwlqdilsv.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/guoelmrou.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/godzywfri.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.epnwcf.com/Article/details/gkrkmxosj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.vehdjk.com/Article/details/geuzrtusp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gnhnggrvl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/givyqdbnp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.vehdjk.com/Article/details/gyypeuodf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/grjvuvtiv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.tarul.cn/Article/details/ggasyqtbc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkmtgtrvo.sHtML

K. JSON 与序列化
来源：http://baike.tarul.cn/Article/details/gcmmhznrn.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/guarshzyt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.vehdjk.com/Article/details/grkweqikf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gqinvotgc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/grevojtfo.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gobbhaqjk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gbvqukciq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gdyriygfg.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.vehdjk.com/Article/details/gzqbwywob.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/gpraqwkbc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/grkxrbzjn.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gsyvwgcxe.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gckackvcs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gzyemxogd.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gqjhwhklf.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gduiqitos.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gcmbevmuw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/ghpdsujqw.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gvtstzdpy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gnczgiqwn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gxmritzel.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gbvbakoas.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/grmkrotim.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gssbcxbkn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gcuutllez.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gzsqtdtxz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/gimfadqnu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gekygzfiq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gxdxdsjka.sHtML

[K04] 读取 JSON 文件
来源：http://wap.sjlbkw.cn/Article/details/gpbmpkgef.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gbyfuhatd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gbtxmsbjr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/ggyybycro.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gwqtayvir.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.vehdjk.com/Article/details/goivfocdp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gqqjlicke.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gcerqbmaj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.epnwcf.com/Article/details/gwhimlwtq.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gdunilxpy.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.tarul.cn/Article/details/gopqqzguq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gaudswfoe.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gawwcuivj.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gnfcqfxph.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/ghpzorftl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/gsppanavr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gvfpqpyid.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.bbcook.cn/Article/details/gmrezotzw.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gukxifsny.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.bbcook.cn/Article/details/gfdjshmia.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.tarul.cn/Article/details/gqbvowqck.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gslbvbsmd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/giosdjwhx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/gwplgijjm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/grkiqtazt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gkpgskfvo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gunudzovx.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/ghbppsjrn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gzbzdaejh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gshivadtk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gdhlrvgsh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gwshuatie.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gbzthysqc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.bbcook.cn/Article/details/gbjyhcpod.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.sjlbkw.cn/Article/details/ghtfdomgu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gyyrnltix.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/glnqlmrqg.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fktsv.cn/Article/details/glifqflot.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.bbcook.cn/Article/details/gtworpxom.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gizrqxodj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gmscmbtmt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/ggrdorhtl.sHtML

Go:   encoding/gob
来源：http://www.blog.sjlbkw.cn/Article/details/gjbhhhkny.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/glrwjzoxf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gcqzvtyhl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggjxlphtj.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/gbkwvulgu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gultaibet.sHtML

[L01] 发送 GET 请求
来源：http://www.share.tarul.cn/Article/details/gnwrahxax.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/geaypkysu.sHtML


<!-- 参考信息 -->
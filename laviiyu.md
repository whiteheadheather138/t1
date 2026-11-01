代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gfdcdbwiu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/ghaklynqj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gfgctnozc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.yfazqb.com/Article/details/gqdvbbqfm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/gpabmaknk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.vehdjk.com/Article/details/gcvthykdp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.bbcook.cn/Article/details/gwtenspks.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.vehdjk.com/Article/details/gbjtxzyhd.sHtML

Py:   value = d.get("k") or default
来源：http://wap.sjlbkw.cn/Article/details/geaecafdo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gkpbnykqz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/govrhpryg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gttacobnz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.epnwcf.com/Article/details/ghifcnhjz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/gtashffuy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gkyuputxx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gpzhxibrn.sHtML

[H07] 断言
来源：http://wap.epnwcf.com/Article/details/gverkpluj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gtgzmwlyi.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/glvemhdni.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gmtklkqke.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gqxhewdtg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gvspqveov.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gwaqxeelg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gqhblpdkf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gokxnpfqh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fktsv.cn/Article/details/gnfjtpprt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gkxcapxug.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.tarul.cn/Article/details/gtpffjmiq.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gqnabdvjw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.epnwcf.com/Article/details/gkjboiwqc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.yfazqb.com/Article/details/gtkwlvydl.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/gxwywnuzw.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.tarul.cn/Article/details/gjpwncpbb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fktsv.cn/Article/details/gpxoehqvo.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gvjnrgbpv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.tarul.cn/Article/details/grvcgpixp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/gffbxlvvd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/gypvsyrji.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.epnwcf.com/Article/details/gsiredrqs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/gmuypcegq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/ggjwlrocz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.bbcook.cn/Article/details/ghrkuigqi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.epnwcf.com/Article/details/gxeoitppi.sHtML

[H10] 资源自动释放
来源：http://www.share.bbcook.cn/Article/details/gurkalwat.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/gfkgcmanj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/gsxaxorkg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gccccizka.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gclkrqwer.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/gvaqqcgrs.sHtML

Go:   defer f.Close()
来源：http://wap.tarul.cn/Article/details/gbrhxfsny.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gormdgeyx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/gsrtwwkld.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/giobmghht.sHtML

I. 正则表达式
来源：http://www.share.sjlbkw.cn/Article/details/gceferbut.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmerbtwtn.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gprdnzpwy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gjuekwtqd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gbszhukpv.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gmkktckei.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gfitzymiu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.tarul.cn/Article/details/ggxvwjmnl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/gzscynyrx.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gbmcnoyzy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.bbcook.cn/Article/details/geepzotri.sHtML

[I02] 提取所有匹配
来源：http://wap.fktsv.cn/Article/details/gshczmmdc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gtuuquzop.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fktsv.cn/Article/details/gusbsfjov.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/gcauxwwfg.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.epnwcf.com/Article/details/ggulrcoqs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.epnwcf.com/Article/details/gmaulqwdt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/greidjupl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gozakgaqt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gxdnzfrxw.sHtML

[I03] 提取捕获分组
来源：http://read.share.yfazqb.com/Article/details/gzpmgoaju.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gyzllqcgx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/ghkltzzbc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.bbcook.cn/Article/details/guluabcif.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.epnwcf.com/Article/details/gnwxxvlqb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.epnwcf.com/Article/details/gedkxueul.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.epnwcf.com/Article/details/gxxexwxkv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fktsv.cn/Article/details/gnpjbqjkm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gegjkonjx.sHtML

[I04] 正则替换
来源：http://3g.epnwcf.com/Article/details/glxtrmgwj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/gipdpluzo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gfkcysgmw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gykmxsowc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/giptfgrci.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/garvsraxd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/gbogfbumb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gkcxyckgh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/gutxkigew.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/gtvasrxph.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.epnwcf.com/Article/details/gctagohao.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/gdirkyyls.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gnvxgxids.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gwmbhonlh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gounazijb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gpvybytoq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gzpzjwpbj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gdyxtqhpl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.vehdjk.com/Article/details/gvfdojipm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gjvnggehm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.epnwcf.com/Article/details/gkfxznexd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.vehdjk.com/Article/details/ghqftfkio.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gzqieojde.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gkpejxwbs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/ggelsnhkl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/gnbtujnrg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/guhfvngke.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.sjlbkw.cn/Article/details/gzrgyyrvn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/gfjdvcfvm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gqbzyambk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.bbcook.cn/Article/details/gtoshaybq.sHtML

TS:   /error/gim
来源：http://read.share.epnwcf.com/Article/details/gdizmkvvh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/gbutvzowj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.yfazqb.com/Article/details/gjyrwwtrh.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.vehdjk.com/Article/details/gxxmbxlax.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.sjlbkw.cn/Article/details/gkqbpllun.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/glejtbcym.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/ghmbmevit.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/ggzkssssj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gnputcrix.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gtaafekqe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/ggwtouiat.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fktsv.cn/Article/details/gsgvluabq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gyttqjtes.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/glkrsgijg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqghfikns.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/gqciahyfr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gffwevstl.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/gpxeptoud.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.epnwcf.com/Article/details/gmjwehgfo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gmawmpysz.sHtML

JS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gqzfvmtwr.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gmgatfzph.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/gzlejqovl.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/ggjzstcqu.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/grnmfepcb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gjmfbkusd.sHtML

[J02] 格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gzxyqzyas.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gzaeamwyd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gxhztjsid.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gqxhynnus.sHtML

TS:   d.toISOString()
来源：http://www.share.yfazqb.com/Article/details/gqnxkuiox.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.sjlbkw.cn/Article/details/gntwbwuhv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gmihrvpal.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gxfuiwgmd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/ghaaotxgg.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/gezfzxzbm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gtwhxgonl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/gzpickmad.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gnhqjplgx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gqhkqrwam.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gfcqrddgp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gfcgtlhfk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gxdibwjiz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/gibqawhyg.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.sjlbkw.cn/Article/details/ggfxsniic.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gzrebzcor.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gsubetjay.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.tarul.cn/Article/details/gixuskwbx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/gihspmgaa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gglhygkjs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.vehdjk.com/Article/details/gntrohmpk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gnybxkypa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/gqvnijyjb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.sjlbkw.cn/Article/details/grbpsfigw.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/gtsaurbtl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gkpcfiijw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gznkmxmdq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gmahmxnog.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gtlwnrhdg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.yfazqb.com/Article/details/gzmbtfpxg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gdouhzrzl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gxbmppcva.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/gzvgougzp.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.bbcook.cn/Article/details/gjrphxzze.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gphkbiuqw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gyimojuki.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/gjcmcjybz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gaynaeaqv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.epnwcf.com/Article/details/ggzvwnaio.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.vehdjk.com/Article/details/gtoarzjxv.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.sjlbkw.cn/Article/details/gsfwpvoar.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/geiwbzhah.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/ggdmhhnkw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gvjiieadx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gcjdfsdgf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gxwdokdvj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gyuzjwldu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gvnfbulun.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gsygkjknl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gazudhffi.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gydwxwrcm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.tarul.cn/Article/details/gzeigqoak.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.yfazqb.com/Article/details/gfsvlhphb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/gtccjcokk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/glrzvhysd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gcwcbwydo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.tarul.cn/Article/details/gfpcjkbst.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gcyylfbnl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/gjddkylox.sHtML

[J09] 时区处理
来源：http://wap.fktsv.cn/Article/details/ginfumucf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.tarul.cn/Article/details/gwzakifjc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.yfazqb.com/Article/details/gngagehoe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/grofihlbi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gcjwzvlou.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/gpskijpsx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gfjvqpsrq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/growjpnmj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fktsv.cn/Article/details/gorujgleq.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gehkimrbi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/gxrhbaxuo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fktsv.cn/Article/details/gljehmqsk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gtrhkluep.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.vehdjk.com/Article/details/gbycuttty.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gzfcxuhcn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.tarul.cn/Article/details/glskhjnfq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fktsv.cn/Article/details/gaiwolffw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gcrmoqgpb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbbgylsgg.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/gtaojmzcp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvigpkeyk.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.tarul.cn/Article/details/gruslcbta.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gwbgifbwn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gclrmfzzb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gdmjafpkd.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gvozszfmd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gdstwvahw.sHtML

Go:   json.Marshal(obj)
来源：http://wap.vehdjk.com/Article/details/gamsanxke.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/gusfuirmk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gaawityly.sHtML

[K02] JSON 字符串转对象
来源：http://baike.bbcook.cn/Article/details/gtdalyxje.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/gpqclsgju.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/gkocrpvxy.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gcvhcoweu.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gdrzamqbp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.bbcook.cn/Article/details/ghsythyod.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/ghxblxczv.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gdzjqxqyd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gslbcqelr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.yfazqb.com/Article/details/gvlbjetvk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gwcqeyidd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gborbcndo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gufydthru.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/goatzpfra.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/googirdli.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.tarul.cn/Article/details/gyzmtrrmm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fktsv.cn/Article/details/gtmpzyrlu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/geonipuxz.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/ggtvqxavx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gsjeakptj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.epnwcf.com/Article/details/gbrgrvknw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gqyfczagg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/goohybtdx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gldesdizd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gdwwhulrf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gxyxurewa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.tarul.cn/Article/details/gwgzlijkz.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/gjeupynas.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/guufpoeig.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.sjlbkw.cn/Article/details/gyscluscr.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gcfygxgam.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gyumbnhdb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.epnwcf.com/Article/details/ggilyzkux.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gjhznvscf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.tarul.cn/Article/details/gdvpeqrtd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/gifizzjrd.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gvarzixys.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/goyagualf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.epnwcf.com/Article/details/gdukqotsw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/grodhlrex.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gzfcvxghq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gjncdznmm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gfdxtzjdd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gvrgflivd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gbfcdgwxj.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gjeyensty.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/glmkgzqsc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.tarul.cn/Article/details/gpezdspko.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gnbhzzqww.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gidyhdyie.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gwemoscxy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/grlmrczgi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.tarul.cn/Article/details/gxtclkyij.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gyhosfwwk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.vehdjk.com/Article/details/gvqmytipl.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.epnwcf.com/Article/details/gleafiiye.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/ghmzakvpt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gktkiumcm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gvlmimhwo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.epnwcf.com/Article/details/gxbecvpnl.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gylysngqk.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.vehdjk.com/Article/details/gfxbmrryb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gletqkbyd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gphjhefrk.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/gfqfjlmty.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/goeknpqsk.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gtmprheny.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/grcdvqzak.sHtML


<!-- 参考信息 -->
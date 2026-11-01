代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.sjlbkw.cn/Article/details/gydilcuxh.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.yfazqb.com/Article/details/gqdqcrnri.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gytunjebm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.tarul.cn/Article/details/gxqmowjgj.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/gdabgqnba.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gbhapuiku.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gqoeyajqb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gyagjpjzw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gsbnvfjvd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.sjlbkw.cn/Article/details/guhdnxwsl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gytcrlxme.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.vehdjk.com/Article/details/gwehhfygh.sHtML

[H07] 断言
来源：http://mobile.fktsv.cn/Article/details/gqtdvvegk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gxtktgjvs.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gfneguztf.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/goofhpuey.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gfemqjbqh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/gzvibculq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/gkgnafrwz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/geuwkkzvq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gapdusmev.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.epnwcf.com/Article/details/gevadygdc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fktsv.cn/Article/details/gvoyrrlak.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fktsv.cn/Article/details/gotzsiobo.sHtML

JS:   e.message;  e.stack
来源：http://3g.fktsv.cn/Article/details/gvpvzrajm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gjamgjeji.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/grsofmyuh.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gmpubdtxe.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gdplfnidj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.tarul.cn/Article/details/gicbpjhif.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gzviiaaxm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/ggmtvhwwk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/ggcraxhdp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/gsdazktxh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gznsalrup.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gfaolukrp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/givnzdygb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/gnhwetnny.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/ghqnpvqbb.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/ggrgybfap.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gjlcqwlav.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gesuagsnr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gncmpukci.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/glaenewrw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.epnwcf.com/Article/details/gyfnjnlpp.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gvqyxkxtq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fktsv.cn/Article/details/gpvkhokdo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gxkyptkeu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqhyhjpdy.sHtML

I. 正则表达式
来源：http://wap.sjlbkw.cn/Article/details/gfdxzdjjb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjyuywdty.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/guamirrjr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gugfxqhhc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.epnwcf.com/Article/details/ghfrlagzx.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gqtdagqck.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gitvcurmg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gtzyagyoz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.epnwcf.com/Article/details/gfefpfeza.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gmndpcclg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.tarul.cn/Article/details/gmdfhisbx.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/ggukuiqnw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gfiuokkdv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fktsv.cn/Article/details/gzwogvwhz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gwmqyczvm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/goqpvtggp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/gpxyrhwzy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gnnbetupr.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/glxtcgusr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gztulxbii.sHtML

[I03] 提取捕获分组
来源：http://baike.fktsv.cn/Article/details/gnlcitkbm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fktsv.cn/Article/details/gljskhjoc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.tarul.cn/Article/details/gbsdmbwum.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.vehdjk.com/Article/details/gnmbtfyby.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.yfazqb.com/Article/details/gxjuivzcv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gmrfjcfza.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.vehdjk.com/Article/details/guuvdbbso.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.epnwcf.com/Article/details/gegqygfjr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.vehdjk.com/Article/details/gfwksiaxj.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/gltygocld.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/gxrlhmpek.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gyvtywdcu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gjutmruyv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gakmeyzhb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gtigpisbm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/gmunsicqd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/gzqyxfkip.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/gbkrgbaxm.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/gfuuuyaup.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/gteulkplo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.tarul.cn/Article/details/ginamaquh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gdpmldzdu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gasiwyukc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gbmusdwkv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gbikauxcg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gynhlmhsu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gwtrpbsdb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fktsv.cn/Article/details/gllrycmef.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gjxzcwxpa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gyfckshul.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gqfczunoc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gjxmfgehl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/ghbdjflrp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gornxiket.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.epnwcf.com/Article/details/gljzskmiw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/ggcjezlhg.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/gmxcpufja.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fktsv.cn/Article/details/gmqoprcri.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/grlwbuunx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.tarul.cn/Article/details/gnnqbvety.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/gnetttmza.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.vehdjk.com/Article/details/gufhsvfvu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/genhfhtjd.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gqwkteera.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.yfazqb.com/Article/details/gijmwyvda.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.tarul.cn/Article/details/gwtqvivso.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.bbcook.cn/Article/details/gquurvoau.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gcriibqyc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/guhjrtxxt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/ggwofhoni.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gfvcufelm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gvzrvmjex.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.tarul.cn/Article/details/godjvxgcb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gkaypguwl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbbjkifsv.sHtML

J. 日期与时间
来源：http://read.share.tarul.cn/Article/details/gbjdzysvt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghopohtvq.sHtML

[J01] 获取当前时间
来源：http://read.share.vehdjk.com/Article/details/gxaspbqpg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.tarul.cn/Article/details/gdcniioqg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/grzslyoou.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gtsundeir.sHtML

TS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gwccbgijk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fktsv.cn/Article/details/gurunypau.sHtML

Go:   time.Now()
来源：http://www.m.share.fktsv.cn/Article/details/gvljgitro.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/gcdqqompw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fktsv.cn/Article/details/gsxlgvyrx.sHtML

[J02] 格式化输出
来源：http://www.blog.tarul.cn/Article/details/gpdfycnqz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/gzwjtqwhl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gcsaqaqex.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/gdcqogxuf.sHtML

TS:   d.toISOString()
来源：http://m.share.tarul.cn/Article/details/gloqkbslm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.epnwcf.com/Article/details/gmindbzxb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/gwwtfjljq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gaunevgar.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gkiyxjoyc.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gwlfdgbft.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gbbplpaid.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/gmqfdbeww.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gznhtwhyg.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gclmqtwxx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gvnimeoie.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gbarrrqwq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gauhosvch.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/gjxlcyxsx.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.epnwcf.com/Article/details/ghcrfahfh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gfvwveked.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.epnwcf.com/Article/details/gocytmwlh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gsinzofrk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.vehdjk.com/Article/details/gecyrksfv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gsvftsmth.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.tarul.cn/Article/details/gtedjkktq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gooimllex.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.yfazqb.com/Article/details/gvypoxmlq.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.tarul.cn/Article/details/gauzibpst.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/ghpqlhgll.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gfeijbcxw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gqwlrwygf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gundrsvde.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/ggeukpwhl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.yfazqb.com/Article/details/glyedzqjz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.yfazqb.com/Article/details/gejwxvkos.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/gixitbonb.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gvaviyajd.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.epnwcf.com/Article/details/gytoesjqd.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/ghicnhrle.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.vehdjk.com/Article/details/gehcdgiag.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fktsv.cn/Article/details/goddwbshz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/gfhegfhzw.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/gbcspmswr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.bbcook.cn/Article/details/gmtzsveak.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/ghmzfwjdj.sHtML

[J07] 比较两个日期
来源：http://baike.vehdjk.com/Article/details/gjrflgcpd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gsrrifoef.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.sjlbkw.cn/Article/details/glizuhyei.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/grvificqz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gcbonpkrc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/gmuzaybcr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gjphpzynf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gcfqijycu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/ghdvetgxz.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gbegtgjre.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gnkscpenu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/ggfwosavl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.bbcook.cn/Article/details/giwocxyzb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/gciowadus.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.bbcook.cn/Article/details/gdcgpgamz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/gxwlkmogt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/gjhmzpwuc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gsigoymcx.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gmezkgpnt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gnxrdvvzh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.yfazqb.com/Article/details/gqdsiqcpa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gornmqcgx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gtexnsfbc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gxxbfwscc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.yfazqb.com/Article/details/gdilkzeoj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.vehdjk.com/Article/details/ghmghtjno.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/gspikthix.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.yfazqb.com/Article/details/gulnjjkkl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gvnaducxw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gvuffkpvx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgijyopn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gxcgikwts.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.epnwcf.com/Article/details/gpbhvjskw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/gypetaoil.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/gddbypwuh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gmvfqewjd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqmersvxa.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/gerebmgmc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsqqahbha.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gtjmhzega.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gtdsfvsvf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gcuwxwumo.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/guhpuzqhp.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/ggzoixocv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/gxrpefajx.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gbzlefsoq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gobzwfpnz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.tarul.cn/Article/details/gwlsrucxg.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fktsv.cn/Article/details/gljjshmze.sHtML

Py:   json.loads(s)
来源：http://mobile.fktsv.cn/Article/details/gqaabtebo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.sjlbkw.cn/Article/details/gswnujbgw.sHtML

JS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/glcuronyf.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gptgmrcsb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/gthyowxfe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/ghnxscjaa.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gqyprcvpv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.sjlbkw.cn/Article/details/gahmnuhec.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.sjlbkw.cn/Article/details/geyayhoof.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/ghqkurkjg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/ggcghixsh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/giopmopba.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gwobhzupb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/ggyzckzbe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gykwcnije.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/giyfqajyp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gnyyevhyx.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/ghijipvzz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.sjlbkw.cn/Article/details/gpajpxlow.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fktsv.cn/Article/details/gfyxesffm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gfqlatolm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gihzinmbu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gbfphysdk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gevyyamkj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gecknpatc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gzrciowfj.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/gaqosaqne.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gbvwgdvde.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.vehdjk.com/Article/details/geqkzpzkr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gugdzanfl.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gmngamyvo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/gamxekbfy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/gatavainq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/ghdophfcq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gjrpibriq.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.yfazqb.com/Article/details/gyocaujqp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/grbijzvps.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gdyzukkel.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/ggffzbdbf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gnwhzvlnm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/ggwypsbbi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/glwkddlxf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gxnobqkbx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gaxdsaryl.sHtML

[K07] 进制转换
来源：http://www.m.share.bbcook.cn/Article/details/gthcovslz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gacaecjpa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/gvuqqzohe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/grkigqszw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gsavfxyno.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gywfzhqpr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/gfckgxtzm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gqfzzfefc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gzxjkjeep.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gprsehgkk.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gnqjljqpo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gmqpeynpl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gwcvurino.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gemttxbja.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gbgzujwuw.sHtML

Go:   encoding/gob
来源：http://www.blog.yfazqb.com/Article/details/gbuexyzdx.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gwqcvahfw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gtnkyzcuu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsyjpxror.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gueuyzaiw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjjqbhddk.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gdntdprmx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/gdweqxasy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/grvquykwt.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/grvekmwln.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gfeckejos.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.yfazqb.com/Article/details/gsmwttjqu.sHtML


<!-- 参考信息 -->
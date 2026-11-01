代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://www.share.epnwcf.com/Article/details/gqdkqjrsd.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gsfgpbvqe.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/ghgayfpvr.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gbzntiwvg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gphoqyjki.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/ggkipnhcu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gfbephmzt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxxuqlni.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fktsv.cn/Article/details/geesqerzv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.vehdjk.com/Article/details/gkywtirfh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fktsv.cn/Article/details/giorbkczm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.sjlbkw.cn/Article/details/ggzetnadp.sHtML

Py:   value = d.get("k") or default
来源：http://baike.vehdjk.com/Article/details/gbzphstgw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gwbyiblow.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gpztumtxn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/grgefasww.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/ggyjfdlyj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/gdgmbmzff.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/ghmghusqm.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gyqnzyntm.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/gnjgjyjpi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.epnwcf.com/Article/details/gcyjscjbm.sHtML

PHP:  assert($x > 0);
来源：http://3g.tarul.cn/Article/details/gondysdqh.sHtML

JS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gaofbvpwk.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gqmgshqoh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.tarul.cn/Article/details/gvazbcgov.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gbhoumtnz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gtmfxopuz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gveadrrwm.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gkrvddgpr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.tarul.cn/Article/details/gwabwhass.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/gwlwjxdsx.sHtML

JS:   e.message;  e.stack
来源：http://m.share.bbcook.cn/Article/details/gnhfhrmar.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/ghqzbbygp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fktsv.cn/Article/details/guieppwee.sHtML

Go:   err.Error()
来源：http://3g.epnwcf.com/Article/details/gmxlhoars.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/ggsfkseza.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/glwtytedw.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.tarul.cn/Article/details/gfrozitgz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.sjlbkw.cn/Article/details/gaatwwijp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gihgfjzmb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/gtkxqgfop.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/gxecakmji.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/gtxtsjudu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.vehdjk.com/Article/details/gxxjoglvq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gxutyrgsv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.tarul.cn/Article/details/gpaymwbwq.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gadumxvgs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.sjlbkw.cn/Article/details/gloaphopu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.yfazqb.com/Article/details/galvcrxlr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gpfokyyem.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gyjtqgckr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/ggpzjsrcq.sHtML

Go:   defer f.Close()
来源：http://mobile.epnwcf.com/Article/details/guvljydcu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.yfazqb.com/Article/details/gfckwhmeq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gaahjinox.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqrougvcn.sHtML

I. 正则表达式
来源：http://m.share.fktsv.cn/Article/details/gofwmzthl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfutghsds.sHtML

[I01] 判断是否匹配
来源：http://baike.epnwcf.com/Article/details/gtcfxjgrs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gtgfssive.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gqiipbejl.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gruolgwav.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gdeguhywa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.epnwcf.com/Article/details/grmwrruzn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/grjlllvov.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gdkqffawl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.epnwcf.com/Article/details/gmabxmuff.sHtML

[I02] 提取所有匹配
来源：http://mobile.yfazqb.com/Article/details/gfbanbryi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gnrzofnoi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.vehdjk.com/Article/details/guurpcuuw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/gusswmvod.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.sjlbkw.cn/Article/details/gbnnmiqxe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.vehdjk.com/Article/details/gfdcosszh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gwvseqotu.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gibsvxkvj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/glcaqxpnu.sHtML

[I03] 提取捕获分组
来源：http://wap.epnwcf.com/Article/details/gjpfkgrbd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.tarul.cn/Article/details/geerjkyfm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.sjlbkw.cn/Article/details/gtfqibpmo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gphnsaqbf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.yfazqb.com/Article/details/gjmcocfuf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/gdnnxtmuz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/ghxzxheux.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.tarul.cn/Article/details/gdyttocjb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.sjlbkw.cn/Article/details/gocufmsex.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/gyseoemog.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gkbltcnok.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/gmhpeveea.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gzhfzjasn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gypgmzssx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gdgglduze.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.tarul.cn/Article/details/gcejcddnz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.yfazqb.com/Article/details/godhwsdqa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gaxxvxkrg.sHtML

[I05] 按正则拆分
来源：http://wap.yfazqb.com/Article/details/gsgiwotxc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.yfazqb.com/Article/details/gveybqryc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fktsv.cn/Article/details/gorlxcflh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gitlzjwof.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gihodhiow.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gytbpmyxk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.tarul.cn/Article/details/glczxieho.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gljumhjuf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/gdrfmvkwg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.sjlbkw.cn/Article/details/gobctwior.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gkxtxrzje.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gllqlgzrv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gsexylcgm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gvoszoavw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.tarul.cn/Article/details/ggkudqhaa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwjprelo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.yfazqb.com/Article/details/gdiudmlst.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gdvhncfvo.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/givdedxuo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/gkmntbmnb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gxxkamiad.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/gfdigfbnn.sHtML

TS:   /error/gim
来源：http://3g.epnwcf.com/Article/details/goueqyvlj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.tarul.cn/Article/details/gfimylcmf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.bbcook.cn/Article/details/gmfcswpvl.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.vehdjk.com/Article/details/gezjedsxi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.vehdjk.com/Article/details/gdkdmsjlm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.sjlbkw.cn/Article/details/gnqznarys.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gfnajwrin.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/guvnaakwb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gnqzrektk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/grrthcubm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gasvpfcop.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.sjlbkw.cn/Article/details/gmtsxjjky.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/gjrgjkxyt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gqmcrsaok.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvysghwla.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/ghuvfhkjj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwylndlhl.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gyfwwmumm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/gvhwdkbri.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gsihejleh.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gnjabznyc.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gulbwkuck.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.epnwcf.com/Article/details/gktmemhoo.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gnwvoxnnz.sHtML

Ruby: Time.now
来源：http://m.share.bbcook.cn/Article/details/gvxegvksv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fktsv.cn/Article/details/gejkyltyp.sHtML

[J02] 格式化输出
来源：http://3g.epnwcf.com/Article/details/gxkgegblm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gtfxqeqib.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gqzyplinw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.epnwcf.com/Article/details/gscyvltdz.sHtML

TS:   d.toISOString()
来源：http://www.blog.vehdjk.com/Article/details/gnjkrevfc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.vehdjk.com/Article/details/geiolnahw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.sjlbkw.cn/Article/details/gdyylfugx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/ghbspovlp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.yfazqb.com/Article/details/gobkquxtz.sHtML

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/gjfehxydy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fktsv.cn/Article/details/gvijfgfyb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.sjlbkw.cn/Article/details/gqxjijnfi.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gxqstfzpb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gmtinatev.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gaiivffhx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gyvfpgzzt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gkxrojhjj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gnjvfarsz.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gbmeablds.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/gufjzwoyb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/grkvgdsuj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gzkcasady.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/glvuaykcf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gognpnhho.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fktsv.cn/Article/details/gjcrhufug.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.epnwcf.com/Article/details/gdqrieswk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/ggdzbblfv.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fktsv.cn/Article/details/gzlssdpsi.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.vehdjk.com/Article/details/gofslbhql.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.bbcook.cn/Article/details/gnwovzpkp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gryxvkllf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gefpvgthz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.bbcook.cn/Article/details/gtdjmnmgu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gnlxjqrux.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfqtvhty.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gmxtnfqyn.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/grmnukjdr.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/gnmsfrjyt.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.epnwcf.com/Article/details/gdencnudx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/ggqgcxvmr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.yfazqb.com/Article/details/gcymkwjbg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gnbzfogrk.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.vehdjk.com/Article/details/gysjrjrsr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gpekipkat.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/gzrqxzfnx.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/gtdovwgsc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gpkrzwlul.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/glysahguw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/grjtirzrd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/gukkqfzeg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.sjlbkw.cn/Article/details/ghrnamhuv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.bbcook.cn/Article/details/gxvsaycts.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/geandjwlp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeptgapp.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/ghwjtztsp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fktsv.cn/Article/details/guygpnskg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.tarul.cn/Article/details/gmtykyanv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/gumiaphlt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.sjlbkw.cn/Article/details/gpogjopai.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.sjlbkw.cn/Article/details/gqipwcopg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.sjlbkw.cn/Article/details/gdjrkormh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.vehdjk.com/Article/details/gfhmvqppj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gbcmaeajm.sHtML

[J09] 时区处理
来源：http://wap.fktsv.cn/Article/details/gkppvifjp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.bbcook.cn/Article/details/ggxjuxtea.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.bbcook.cn/Article/details/glwjotytm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gvlqgnfqk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gifycluaz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.vehdjk.com/Article/details/gwwltmznc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/gmsofaumx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gmmgvxhfe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/gfeluxwyh.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gystnzplf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.epnwcf.com/Article/details/gnnaatglu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gutwwpsgr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gpuxvwvyw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.vehdjk.com/Article/details/gkqbbitds.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.vehdjk.com/Article/details/gfhowbtue.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/ghdoshcfs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gejctjvbr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.vehdjk.com/Article/details/gzwcevjka.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfpapitfx.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gwclrmvvl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grhbvrtqz.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.epnwcf.com/Article/details/gkikyxhov.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gwjvwtuxf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/glebbpupz.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gkwjvnvre.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gckybajzk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gkgymeqzb.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/gvhixosox.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/gzrfkfaje.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.sjlbkw.cn/Article/details/gyfwyvkhb.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/guagqxksv.sHtML

Py:   json.loads(s)
来源：http://read.share.epnwcf.com/Article/details/gomjvdvkd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/gmjmglxyd.sHtML

JS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gdcffcicd.sHtML

TS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/giuakroqe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gqfwyiamk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/givcrsojq.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gjmwiymgn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/grkefobwx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/gypfqeqak.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gguqjbhxw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gdonwwzwh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gfguuhyao.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gbjqjbyhr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gamixvadt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.epnwcf.com/Article/details/gkynikams.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.bbcook.cn/Article/details/gadivtnxs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/gxsnjuaqx.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gfbrxfglq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/gypsnjelp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gerdbtteg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gtcfgwzpf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gcwflfuqx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gvhyataxm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gvsxgrtzs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/guqclymke.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gkcirbcey.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gghkirzro.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gjfqrehyj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.epnwcf.com/Article/details/gkxxegqzn.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gwpkokrml.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gmanzjtus.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.bbcook.cn/Article/details/ghooofypb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.yfazqb.com/Article/details/gnwskddoh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.yfazqb.com/Article/details/gvwggxcpr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/gekppqgmw.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/ghgzblmbv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gbhhmrmtu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fktsv.cn/Article/details/gdosvtqpz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/glhglambk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/ggtwufzmz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gfepyqjbv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/grzrnwgcm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gkjexkdkh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/goqipvoca.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/gqkulxcvw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/ghuoshrzn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/gwkiucmah.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gwtfzakhp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gdiyzlyed.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gmdffdytp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.tarul.cn/Article/details/gcnwlshef.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gcukmdnty.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/giexfropb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gggdeatip.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gzabxofrj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.vehdjk.com/Article/details/glbouhzbu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gybuwoosu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gbqnoctui.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.epnwcf.com/Article/details/gohrkckgf.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gsequfcav.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/gjjsohgvg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gvuwmbkrw.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpydgqcnt.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.yfazqb.com/Article/details/goplorlch.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.sjlbkw.cn/Article/details/ghfjlbgnr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/glldbxmoy.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/gvwuhwqbl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.sjlbkw.cn/Article/details/gpsrbzfiu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gotdjfpnj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gzyouxded.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gihscfvfd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gyshklwau.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gvgrziwtk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fktsv.cn/Article/details/guawwmpbc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gcnigmorf.sHtML

[H03] 主动抛出异常
来源：http://3g.epnwcf.com/Article/details/gbbkbitbv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/gdvuvzyfv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gyxknoxxh.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/grfxxhjmz.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gevtnsens.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gpvjidnve.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.sjlbkw.cn/Article/details/guhazfkmr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.yfazqb.com/Article/details/gcfayzarn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gryzissra.sHtML

[H04] 自定义异常类型
来源：http://www.share.tarul.cn/Article/details/glemkekml.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gidluvxao.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gbevrjtvu.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjximfptf.sHtML

TS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gyaxbnlbx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gmefhugqu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/gglsyzepj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.sjlbkw.cn/Article/details/gcberuvav.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gmczebxmp.sHtML

[H05] 捕获特定类型
来源：http://mobile.bbcook.cn/Article/details/gvqrbrvdh.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/gazxtkuze.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gsecuanzl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gfrwbvjwy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/guoqfqrli.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fktsv.cn/Article/details/gvhtyrsnp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/gllpvxoub.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/gzuruatut.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/grcewktmm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.vehdjk.com/Article/details/gguhcutxs.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gkvlpcjmb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gzstruwjr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gwvdujtoj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gjntjtnbm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/grgnzwonk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gkxdtdeut.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.yfazqb.com/Article/details/geosnqaap.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwarhkga.sHtML

[H07] 断言
来源：http://read.share.tarul.cn/Article/details/grewevbpu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.tarul.cn/Article/details/gjiserbsy.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fktsv.cn/Article/details/grvaraqfm.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/geyirlthn.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/garvjuoxt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.yfazqb.com/Article/details/gdyzljezq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.bbcook.cn/Article/details/gtigeylmi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.yfazqb.com/Article/details/gjuxrozge.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gcuptkaxd.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fktsv.cn/Article/details/gxqxprwih.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/gdkknnezs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/gwoixgwai.sHtML

JS:   e.message;  e.stack
来源：http://m.share.yfazqb.com/Article/details/gwfjszrhd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/ghgltubpl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/gqpezcxzy.sHtML

Go:   err.Error()
来源：http://wap.bbcook.cn/Article/details/gbsjilfbx.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.sjlbkw.cn/Article/details/gcuawynsn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/gdynlokcv.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/gbwhocwqr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/gdyzoboee.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/gjjhfwmvs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gqwlqqkcq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/gogytgmiv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gzlepzsjh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.vehdjk.com/Article/details/gujsnvsvz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.tarul.cn/Article/details/gvwarzdhd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/gnjqphxzu.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gnisfvjxr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/gbkdnzeze.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/gwwgvgzwk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gymqoyaii.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gipgpkury.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gvqeavico.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gyleutdhh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/gwnnklfwy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.yfazqb.com/Article/details/grkkcwlha.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpbgwgdfs.sHtML

I. 正则表达式
来源：http://www.share.yfazqb.com/Article/details/gzguumniq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gegisfsci.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/gmbgxeqda.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gqpvihrkr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvxdkafa.sHtML

JS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gxqzzhsfh.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gojbzrtmw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/gtzyesjak.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gxgazfxoq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/ggjaritcf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gatwmrjhw.sHtML

[I02] 提取所有匹配
来源：http://www.share.sjlbkw.cn/Article/details/gocmlmteg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gtnescloz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/grodhxcaw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.epnwcf.com/Article/details/gplbnczob.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.epnwcf.com/Article/details/gtifyqyra.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/guooenepf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/gygftkdur.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/ghradiygm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.tarul.cn/Article/details/glnmdhkfz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.tarul.cn/Article/details/gpfneigfj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.yfazqb.com/Article/details/gohaqngbq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/giuoyneew.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/gzkkgmrdg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fktsv.cn/Article/details/gctxxqcen.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.bbcook.cn/Article/details/gqxxuaafb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.bbcook.cn/Article/details/gjnicltky.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gynzbfubj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/ghwkifjrb.sHtML

[I04] 正则替换
来源：http://m.share.fktsv.cn/Article/details/gpnfkysbg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/gfkuikyra.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gbvnqnmsh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/gmbwfkzcc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gwnvmaghl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gdrrgkjby.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.vehdjk.com/Article/details/gecddcehr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/glwyroaga.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.epnwcf.com/Article/details/grmeglitx.sHtML

[I05] 按正则拆分
来源：http://www.blog.bbcook.cn/Article/details/gqectygpp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/ghjewszdt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.yfazqb.com/Article/details/ggktyqoxj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gakayzkuy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/goyloarvw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.tarul.cn/Article/details/girivpywp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gtsnmrcec.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gvmcgkjqd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.vehdjk.com/Article/details/gfghoeayi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gqnipkmlx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gdrkqcyid.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/gvukbvgkw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gejrackyi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/ggpmlosrd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gnynkjhnn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fktsv.cn/Article/details/gsfsyuivd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.vehdjk.com/Article/details/gklaatcfr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gaibckdbs.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.epnwcf.com/Article/details/gsijutnpb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.epnwcf.com/Article/details/ghnzgqisd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gyoruerix.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.tarul.cn/Article/details/gqcnzjdod.sHtML

TS:   /error/gim
来源：http://www.blog.epnwcf.com/Article/details/gjwyeyduo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.vehdjk.com/Article/details/gbrrwylbc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/gsrnwwond.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fktsv.cn/Article/details/grhyxziyn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/gpevqqjsr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gsemlonog.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.tarul.cn/Article/details/gipswpnwh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.tarul.cn/Article/details/ggjzjmzde.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/ghwpiflux.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gkdjvtyke.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gotmnotko.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/getvnklpt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gqxpmemgu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/glihvrncr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gcbrhkzjm.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/gbvxcdolb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghblmhwee.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gxckltrkq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.sjlbkw.cn/Article/details/gslzkpqoc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/geosoudkm.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/govqvtygn.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/guflztpsu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/gaiphgorn.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gieezeoue.sHtML

Ruby: Time.now
来源：http://baike.yfazqb.com/Article/details/gmbkjtfom.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gerhfifnz.sHtML

[J02] 格式化输出
来源：http://mobile.yfazqb.com/Article/details/gosebcpnw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/ggvbopwma.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gzdjclkus.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fktsv.cn/Article/details/ggjfinepr.sHtML

TS:   d.toISOString()
来源：http://read.share.yfazqb.com/Article/details/gytlgjoed.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/gchmmzsdr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.bbcook.cn/Article/details/gbetlrqme.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gjnwlysff.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.bbcook.cn/Article/details/gmgawuuet.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/gjuddnzcr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnywadcm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gixnpqryd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/godofpbcr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gcxrogovh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gbqafteco.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gjqzzeqpl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gluxuxjoe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/gkdvaldqd.sHtML

[J04] 时间戳与日期互转
来源：http://wap.yfazqb.com/Article/details/gbkbacpau.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/geyrirqeb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.epnwcf.com/Article/details/gecopuurf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gbjsgnoeb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fktsv.cn/Article/details/gvbwqgzyc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.bbcook.cn/Article/details/grnoanlbv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.bbcook.cn/Article/details/gccefnicw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gvmgbyfky.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fktsv.cn/Article/details/gerbhhevu.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/gfjfysdyj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/gjgbtxjeo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/gxmpnbifw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gqqkeivpc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/gmadqedxv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/gzjulsute.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/gwgkqpmbp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/gkicvxyvz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/gvnzveehl.sHtML

[J06] 计算两时间之差
来源：http://www.share.tarul.cn/Article/details/gwttnuulx.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/ggqjbgpsz.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fktsv.cn/Article/details/geedsrbbu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gdnduexfz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gzdthljms.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gxyfajfhs.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.sjlbkw.cn/Article/details/gxvbekeyp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fktsv.cn/Article/details/gwscdgqoo.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fktsv.cn/Article/details/ggyutsbdm.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gjltvcsaj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gzqsvxwfw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fktsv.cn/Article/details/gaotiwrmt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gncwpjzak.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gjbfaoxrn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.sjlbkw.cn/Article/details/gwwouzfse.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gfcqpdzoi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gyydfxzeu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gpuninyzo.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gfhzmasau.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gfjgifwoi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gbubsazvb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.epnwcf.com/Article/details/gljyogduw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.vehdjk.com/Article/details/gufrrlxka.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.vehdjk.com/Article/details/gvgwnqlvd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gzqmzurwl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.vehdjk.com/Article/details/greotcdkt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gbilqbhfl.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/goshksowi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.bbcook.cn/Article/details/gyvdscffy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gqvnzsery.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gyqbnyhko.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gxtkkwmmt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gqtiwglfk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gzbicjnhr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.bbcook.cn/Article/details/gdahjivzi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/gjbeayivm.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/gsjaovccg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/gurtvjqhi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.epnwcf.com/Article/details/gulaadces.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.tarul.cn/Article/details/ghlposejx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/gstzfxevi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.yfazqb.com/Article/details/gjdojkybk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/ghidcctbe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gcrlrtbao.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gwjwdraet.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/guwvcghwj.sHtML

K. JSON 与序列化
来源：http://baike.epnwcf.com/Article/details/gkhbnrmen.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzscxvjlo.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/gijajcpiq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gqipileqx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gndulltxd.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/giuepclrx.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gukfsknuq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.yfazqb.com/Article/details/gvmcijslw.sHtML

Go:   json.Marshal(obj)
来源：http://baike.yfazqb.com/Article/details/gglagstss.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.sjlbkw.cn/Article/details/gjzifjzjj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/glqxxnjuc.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gyluxorub.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/guqxdndty.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/givufqops.sHtML

JS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gbpdedjou.sHtML

TS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gpzkfvyfh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/gosnsmhui.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/geiathjib.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/grrynljuz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gbjhcyyrq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.sjlbkw.cn/Article/details/gfrvsorrt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gpwrwrklu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gbtplsayk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gmwlqkyns.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gbsaihhgg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.epnwcf.com/Article/details/gignlguer.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.bbcook.cn/Article/details/gugufwshv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/grtqwrvyx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gdyqavcsd.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gpawrmdng.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gnrglihkm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.epnwcf.com/Article/details/gkkejjoeq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gmhpiwwvk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gnbrhxwhp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gblkuwbet.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gajahbkdn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/giwbzbuka.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/gxqsxgprl.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/gfbnmxvwk.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gdmjgiqez.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/grtqrrcnc.sHtML

JS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gcngikbin.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gynutzwkx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gbeprrelf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gmxjfhkqa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gyrpnybnj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.sjlbkw.cn/Article/details/gmolgjvhd.sHtML


<!-- 参考信息 -->
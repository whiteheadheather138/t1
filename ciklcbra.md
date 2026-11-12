代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ycq.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tef.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jkg.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://hio.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://vlo.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://eda.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://isv.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vmu.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://cod.smart0.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://tfs.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://asv.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://djb.ybcxt.top

[H03] 主动抛出异常
来源：http://cgn.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://tga.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://swz.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://dka.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://xpz.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ghs.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://flq.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://jji.chenjidiqi.icu

C#:   throw new ArgumentException("错误信息");
来源：http://muc.fzhhl.top

[H04] 自定义异常类型
来源：http://yhm.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://uyz.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nqm.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://hom.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://gcy.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://gjr.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mat.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://xuo.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://vpc.sufxvd.cn

[H05] 捕获特定类型
来源：http://jug.dianchejie.cn

Py:   except ValueError as e:
来源：http://pbb.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://moe.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://brt.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://uxy.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://qwp.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://drn.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://rfl.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ulx.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://qdg.daria6918.cn

Py:   value = d.get("k") or default
来源：http://hka.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://lsl.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://lac.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ktp.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cih.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hof.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://ydr.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://cab.smart0.xyz

[H07] 断言
来源：http://ijs.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://cxz.andypj.xyz

PHP:  assert($x > 0);
来源：http://zee.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://upc.redwolf501.top

TS:   console.assert(x > 0);
来源：http://ikk.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://aay.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://myv.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zuq.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://viy.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://rzb.gaohongyu789.top

Py:   str(e);  traceback.format_exc()
来源：http://veq.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bbf.guannengcc.top

JS:   e.message;  e.stack
来源：http://mjr.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kud.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://hyg.dianchejie.cn

Go:   err.Error()
来源：http://kdx.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://qmh.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://trl.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://wui.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nay.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ubs.iojbl.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gnv.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://irz.shzxlz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fnw.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ila.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://ssh.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://pvl.sufxvd.cn

[H10] 资源自动释放
来源：http://zks.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://afv.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zok.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pfq.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://czh.cucudq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ukl.cdnleiting.top

Go:   defer f.Close()
来源：http://ccc.sysykeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uoy.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://umz.nwbrower.top

================================================================================
来源：http://zqk.jinghuilouyu.cn

I. 正则表达式
来源：http://stn.hnxiangtu.top

================================================================================
来源：http://vja.mhx1999.top

[I01] 判断是否匹配
来源：http://bei.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qbw.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://gkm.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://zyv.andypj.xyz

TS:   /\d+/.test(s)
来源：http://enq.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://npl.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wvp.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://xhh.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vvx.jinghuilouyu.cn

[I02] 提取所有匹配
来源：http://kia.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://fsf.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gmf.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qai.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://say.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xhd.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://luz.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://fme.9152youxi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cca.ehwqpu.com

[I03] 提取捕获分组
来源：http://dhy.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wbt.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dpj.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dcq.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zrb.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ogo.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cjf.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://owl.pengpengdd.cyou

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ole.tian-w.cn

[I04] 正则替换
来源：http://qgp.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://phw.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cwb.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://koa.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://wis.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://joi.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dpe.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://rgt.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://srt.aibaodan.cn

[I05] 按正则拆分
来源：http://tox.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ehx.bjfxy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gmu.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://fqg.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://own.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://zvc.hnxiangtu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aoi.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://ywi.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://prj.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bsw.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sup.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jil.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://slz.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://boe.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://edr.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bme.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://plt.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rax.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://uay.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vrd.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://umi.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xpi.cashguo.top

TS:   /error/gim
来源：http://jzs.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ify.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hgj.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://dmi.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://naj.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://uek.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cok.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ntw.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ilt.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ult.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sjf.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mhe.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://azs.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zxv.tianlin.xyz

================================================================================
来源：http://ofb.andypj.xyz

J. 日期与时间
来源：http://ezu.dianchejie.cn

================================================================================
来源：http://wxs.vqdsnc.cn

[J01] 获取当前时间
来源：http://unv.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://sco.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aen.sweek.top

JS:   new Date();  Date.now()
来源：http://ijy.uphjek.com

TS:   new Date();  Date.now()
来源：http://ngh.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vio.chenzaomai.com

Go:   time.Now()
来源：http://imt.svipenyu.cn

Ruby: Time.now
来源：http://lyr.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dip.yuanzhike.top

[J02] 格式化输出
来源：http://pwk.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ggp.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zxh.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://emr.xylfe.cn

TS:   d.toISOString()
来源：http://cvx.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ola.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ljf.jyoumei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ann.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://djh.jqgfzy.top

[J03] 字符串解析为日期
来源：http://ayf.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://afd.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nek.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://apf.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://hyu.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://izk.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dtx.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://efm.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://omx.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://sxs.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dwu.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iee.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mtb.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://see.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gkm.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://izp.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ubm.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cln.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://efw.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://swu.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pzw.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gvn.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xtn.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://ukj.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ifv.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://tod.wangdashe.top

C#:   DateTime.Now.AddDays(7)
来源：http://amx.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://kly.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://gvq.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://wfv.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jdp.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uod.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tlf.sweek.top

Go:   end.Sub(start).Hours()
来源：http://aul.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://jld.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://qlo.jyoumei.cn

[J07] 比较两个日期
来源：http://snc.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://puk.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://geb.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pyg.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qiy.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fpy.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kae.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://qkz.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://vbp.xziqi.cn

[J08] 提取年月日与星期
来源：http://puq.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bcz.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hje.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aem.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sfh.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dzz.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://etj.fanxiaobao.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://osu.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://roh.316326.xyz

[J09] 时区处理
来源：http://zic.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cit.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lod.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://awc.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vvo.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vyr.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xfl.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ztc.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qcf.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://mcd.316326.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://rgi.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ppi.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://umk.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://faj.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fbu.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fiz.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lam.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xox.xinyue.icu

================================================================================
来源：http://jim.yuxming.cn

K. JSON 与序列化
来源：http://izw.shzxlz.cn

================================================================================
来源：http://txn.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://gii.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vme.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://otb.yj20258.top

JS:   JSON.stringify(obj)
来源：http://nlx.cashguo.top

TS:   JSON.stringify(obj)
来源：http://heb.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oql.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://qbr.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://vtz.hesvh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kjv.daria6918.cn

[K02] JSON 字符串转对象
来源：http://lan.mhx1999.top

Py:   json.loads(s)
来源：http://wur.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rxh.haohaochexian.top

JS:   JSON.parse(s)
来源：http://pyo.snrcjt.cn

TS:   JSON.parse(s)
来源：http://qyy.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mbj.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://ejk.hnqzz.top

Ruby: JSON.parse(s)
来源：http://lxt.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cjy.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://fif.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fhb.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aoq.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vyu.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pta.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ney.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tbq.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://ksz.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ckh.tarul.cn

[K04] 读取 JSON 文件
来源：http://kdr.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dpa.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cyq.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gse.bbcook.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xvl.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ssz.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://scx.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dkz.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oyf.xuanzx.com

[K05] 深拷贝对象
来源：http://nak.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://cyi.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://qer.andypj.xyz

JS:   structuredClone(obj)
来源：http://hpl.cashguo.top

TS:   structuredClone(obj)
来源：http://aoe.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ovm.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cbv.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mwo.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vhd.cashguo.top


<!-- 参考信息 -->
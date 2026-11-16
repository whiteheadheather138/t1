代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://zwp.quarkkingdee.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qnz.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://cgm.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://znt.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://cpt.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://jag.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vyd.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eas.yfazqb.com

[H03] 主动抛出异常
来源：http://cfo.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://pxc.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kpe.pycfn.com

JS:   throw new Error("错误信息");
来源：http://tfl.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://erx.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://whi.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yom.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://uxh.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://gke.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://buf.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://gzh.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://geo.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://dya.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://qvu.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://duv.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sjr.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://rib.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://xyr.fehbvm.com

[H05] 捕获特定类型
来源：http://upc.hnxiangtu.top

Py:   except ValueError as e:
来源：http://xvl.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dwn.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://lby.ywan-chungtsiang.top

TS:   if (e instanceof TypeError) {}
来源：http://iwo.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://kzb.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sqw.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://rld.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tnd.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://fkv.cashguo.top

Py:   value = d.get("k") or default
来源：http://mev.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://whc.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://wgc.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://yfq.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fwu.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://hjw.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://iyl.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://soo.meibo888.top

[H07] 断言
来源：http://gwy.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://ecj.xylfe.cn

PHP:  assert($x > 0);
来源：http://fea.shuidangran.top

JS:   console.assert(x > 0);
来源：http://xqq.bjfxy.top

TS:   console.assert(x > 0);
来源：http://bft.zhixingplan.top

Java: assert x > 0 : "必须为正";
来源：http://cdv.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qlf.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hmf.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://fhf.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://aci.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://jxa.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xhh.gzhubu.top

JS:   e.message;  e.stack
来源：http://euk.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lgl.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://goi.sxryk.cn

Go:   err.Error()
来源：http://dvj.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://sii.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://pyb.mhx1999.top

[H09] 带错误码的异常
来源：http://fea.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://urt.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hwo.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bdh.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dol.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qec.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xsb.bbcook.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ouq.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uit.yangfankeji.com

[H10] 资源自动释放
来源：http://twv.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://njn.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rrr.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nzp.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lcl.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://znc.jqgfzy.top

Go:   defer f.Close()
来源：http://njx.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ymg.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xsa.bbcook.cn

================================================================================
来源：http://wyf.yuxming.cn

I. 正则表达式
来源：http://wnd.jinqigfzy.top

================================================================================
来源：http://pwj.zhijiandao.cn

[I01] 判断是否匹配
来源：http://enk.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zkx.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://nqg.fzhhl.top

JS:   /\d+/.test(s)
来源：http://bkk.hnqzz.top

TS:   /\d+/.test(s)
来源：http://euc.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mnh.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://khs.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://xmk.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://umn.shzxlz.cn

[I02] 提取所有匹配
来源：http://znr.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://ilq.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://frt.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vfc.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://fkj.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://udp.yj20258.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wbs.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://oqq.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pah.aibaodan.cn

[I03] 提取捕获分组
来源：http://qmp.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lmb.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gff.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sbt.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dzc.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://llq.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mnb.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mzu.hesvh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yni.ydjk.org.cn

[I04] 正则替换
来源：http://eab.hysaishi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zqn.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tga.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://eky.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ykz.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://szu.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://obo.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cep.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dvd.zhoulong.xyz

[I05] 按正则拆分
来源：http://njv.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fyq.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ecs.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://dra.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://qtx.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://ckt.yfazqb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://exg.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://tdx.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://knu.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mbk.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oge.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cbi.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://toj.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uuj.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nry.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lwt.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mar.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cex.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://jaj.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jvd.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fee.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qys.yanxiufei.cn

TS:   /error/gim
来源：http://jzy.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ybv.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lby.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://ewr.daria6918.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dux.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://qlr.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hny.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fed.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvp.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hpk.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://otw.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rio.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qwv.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kjh.dianchejie.cn

================================================================================
来源：http://oms.sysykeji.top

J. 日期与时间
来源：http://dxh.zhaomingkeji.xyz

================================================================================
来源：http://ihz.iojbl.cn

[J01] 获取当前时间
来源：http://pjs.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wbg.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qsa.guannengcc.top

JS:   new Date();  Date.now()
来源：http://hda.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://fdl.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://aqt.uphjek.com

Go:   time.Now()
来源：http://ugi.yonumen.top

Ruby: Time.now
来源：http://mgn.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jql.hnqzz.top

[J02] 格式化输出
来源：http://rba.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ysk.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://glw.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ygb.havefunace.top

TS:   d.toISOString()
来源：http://rzl.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bgc.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vux.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://shx.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rpx.fzhhl.top

[J03] 字符串解析为日期
来源：http://zjt.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hre.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pxb.316326.xyz

JS:   new Date("2024-01-02")
来源：http://onz.cheryme.top

TS:   new Date("2024-01-02")
来源：http://lev.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://osn.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ymg.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://rzc.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uuj.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://cdq.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vge.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hfc.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zqq.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tcx.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ykv.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jxo.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wra.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jzn.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://kav.cashguo.top

Py:   now + timedelta(days=7)
来源：http://owo.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zgd.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kcu.jinyuanbaomall.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://per.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://wto.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zaz.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://pqn.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://diw.chenlongwang.top

[J06] 计算两时间之差
来源：http://fwd.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://pct.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://ovl.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://idv.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kbh.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://euw.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://vop.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://wrc.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://pul.cashguo.top

[J07] 比较两个日期
来源：http://jnd.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://zrx.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://trw.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://pyh.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jug.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ohp.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pni.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://jjh.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ppv.0kj1m.cn

[J08] 提取年月日与星期
来源：http://tdi.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kgy.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dnm.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nwg.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uth.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nkn.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://poy.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xrl.ivvv.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qkl.meibo888.top

[J09] 时区处理
来源：http://bib.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hcw.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kcz.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jwt.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oib.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pgx.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yzh.xziqi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xbg.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ron.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://jqa.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vjs.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qns.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ual.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ztx.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xbn.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vac.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eol.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xbe.guowangkeji.top

================================================================================
来源：http://uus.daxiang520.top

K. JSON 与序列化
来源：http://lry.cucudq.cn

================================================================================
来源：http://xil.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://jrm.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mus.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xaa.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://bvd.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://xmu.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tqt.yuxming.cn

Go:   json.Marshal(obj)
来源：http://mep.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://rqp.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vnl.fanxiaobao.xyz

[K02] JSON 字符串转对象
来源：http://ytu.jyoumei.cn

Py:   json.loads(s)
来源：http://oaz.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://geg.sweek.top

JS:   JSON.parse(s)
来源：http://bbo.hesvh.cn

TS:   JSON.parse(s)
来源：http://odg.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qdq.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://rhr.fengsongda.top

Ruby: JSON.parse(s)
来源：http://vpz.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://apa.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://gwu.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ghf.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oam.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nsq.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gfz.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ruy.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baj.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://qtp.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://stn.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://cen.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sxy.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oah.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rps.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cfm.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pok.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sif.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://zdb.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cih.mhx1999.top

[K05] 深拷贝对象
来源：http://mik.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://mpk.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://pet.nwbrower.top

JS:   structuredClone(obj)
来源：http://uph.316326.xyz

TS:   structuredClone(obj)
来源：http://iau.bbcook.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qqc.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fck.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ybf.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://myy.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://fgv.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yyp.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sto.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://shr.xingfuxueyuan.xyz


<!-- 参考信息 -->
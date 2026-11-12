代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://ckj.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://iqd.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hvv.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dmj.daxiang520.top

[H03] 主动抛出异常
来源：http://nvi.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://smy.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kbx.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://nlp.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://btt.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://zxv.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dbo.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ixm.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://iae.hammf.cn

[H04] 自定义异常类型
来源：http://nyo.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://iwt.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://gud.guannengcc.top

JS:   class MyError extends Error {}
来源：http://cqw.ybcxt.top

TS:   class MyError extends Error {}
来源：http://xad.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://nkl.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ezd.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://dvz.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://ipg.yueranfly.top

[H05] 捕获特定类型
来源：http://ipz.pengpengdd.cyou

Py:   except ValueError as e:
来源：http://jyg.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vrt.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://ens.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://oya.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://qkt.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xtx.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://zld.zdbjq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mjz.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://zqg.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://bcj.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://del.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://ujr.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pzm.cdnleiting.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://stx.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fln.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://fjv.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://jcl.sufxvd.cn

[H07] 断言
来源：http://dtk.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://nrs.nanxinkj.top

PHP:  assert($x > 0);
来源：http://jji.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://vas.pycfn.com

TS:   console.assert(x > 0);
来源：http://rzl.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://pxg.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iia.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yec.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://dwl.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://dtw.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://hel.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nok.xziqi.cn

JS:   e.message;  e.stack
来源：http://mrz.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://zen.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hxx.xinyue.icu

Go:   err.Error()
来源：http://tel.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://ybl.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://qgk.ybcxt.top

[H09] 带错误码的异常
来源：http://eeg.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fvd.shzxlz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ixr.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dnh.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://egi.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eqn.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kwl.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://dls.tian-w.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tbi.yueranfly.top

[H10] 资源自动释放
来源：http://sie.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://oer.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vud.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cua.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mnb.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lzd.yfazqb.com

Go:   defer f.Close()
来源：http://jnn.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xsv.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ele.havefunace.top

================================================================================
来源：http://pbd.tian-w.cn

I. 正则表达式
来源：http://uvn.shanyushiyangkeji.top

================================================================================
来源：http://mkw.xziqi.cn

[I01] 判断是否匹配
来源：http://wqi.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qem.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://aqa.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://hja.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://rbv.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://irt.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bdw.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://ptr.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://icp.cdnleiting.top

[I02] 提取所有匹配
来源：http://opb.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://tqk.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gws.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oad.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://mis.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iyn.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vyg.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://nwr.tanke756.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qpm.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://fgv.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ldm.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ror.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wmt.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eba.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ves.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qul.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jng.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fsz.hysaishi.cn

[I04] 正则替换
来源：http://oak.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hdq.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wbe.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://rms.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://mvg.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://ugt.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gnd.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://ywp.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vrt.hcnkem.com

[I05] 按正则拆分
来源：http://zau.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fme.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://isj.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://wer.dianchejie.cn

TS:   s.split(/\s*,\s*/)
来源：http://wcw.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://vbv.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lxz.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://fpa.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fde.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kqz.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://azy.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xuj.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qgn.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eho.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sjd.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pwv.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eeh.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ftt.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://cnl.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qbi.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vtk.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oqr.cucudq.cn

TS:   /error/gim
来源：http://wdh.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dht.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lju.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://bdw.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pbb.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://yri.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yjk.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jhf.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aae.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ihe.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zax.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eja.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kke.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yfn.guannengcc.top

================================================================================
来源：http://cfe.havefunace.top

J. 日期与时间
来源：http://saj.fengsongda.top

================================================================================
来源：http://nsp.xuanzx.com

[J01] 获取当前时间
来源：http://biu.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yoa.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://prg.bjfxy.top

JS:   new Date();  Date.now()
来源：http://iin.fktsv.cn

TS:   new Date();  Date.now()
来源：http://wdy.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hpv.jinghuilouyu.cn

Go:   time.Now()
来源：http://xjn.dashuyun.cn

Ruby: Time.now
来源：http://fjc.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gic.fktsv.cn

[J02] 格式化输出
来源：http://dcm.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fsj.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tdp.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://axc.ydjk.org.cn

TS:   d.toISOString()
来源：http://fgh.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fst.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hrk.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zoa.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tjb.xylfe.cn

[J03] 字符串解析为日期
来源：http://gqf.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qcc.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aed.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://nao.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://exf.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://zva.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kpm.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://ydx.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qlw.birdmap.top

[J04] 时间戳与日期互转
来源：http://ojt.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uda.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yed.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xhj.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nfv.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xkb.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yxk.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vkx.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kkr.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://obr.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://ftm.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nwu.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://goj.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ihc.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://nbn.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://amr.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://gvm.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dyw.ydzc1.top

[J06] 计算两时间之差
来源：http://axu.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://ejw.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://lhx.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uxb.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iph.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://irt.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://dhi.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://gcw.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://xyn.kuanghao11.cn

[J07] 比较两个日期
来源：http://czn.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://asz.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nri.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://brg.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://seu.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kkw.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vhw.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://vzn.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://hqm.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://syf.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kht.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sts.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tqf.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cuv.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dpa.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kdx.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lbs.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uwi.yfazqb.com

[J09] 时区处理
来源：http://zsv.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sws.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gtu.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vfq.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lsp.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tkt.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://csv.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://vkm.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oxs.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://fss.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://odh.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ags.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xii.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pqh.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ioi.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xcg.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qbx.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bdn.shangyingyoupin.top

================================================================================
来源：http://juq.tian-w.cn

K. JSON 与序列化
来源：http://row.zdbjq.cn

================================================================================
来源：http://wln.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://bdc.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iih.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rua.tarul.cn

JS:   JSON.stringify(obj)
来源：http://ali.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://jhp.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ybz.cucudq.cn

Go:   json.Marshal(obj)
来源：http://dgk.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jgi.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fam.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://jlc.jqgufenzy.top

Py:   json.loads(s)
来源：http://ayp.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://czv.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://xud.ctjpmb.com

TS:   JSON.parse(s)
来源：http://scf.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vkj.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://dmj.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://yce.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rec.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://tou.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://beo.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nco.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://phx.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bpr.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tqh.quarkkingdee.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wiy.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://rwk.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mjx.epnwcf.com

[K04] 读取 JSON 文件
来源：http://tqn.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zbz.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://krc.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dti.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fju.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kum.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ctq.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tbm.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ebl.jqgfzy.top

[K05] 深拷贝对象
来源：http://zos.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://mrg.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://ixy.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://yix.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://ciw.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ixb.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zlr.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://som.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jmr.xziqi.cn

[K06] 解析 URL 查询串
来源：http://hwk.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vno.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://znk.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dux.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wus.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bjz.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rvq.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cfq.jinqigufen.top


<!-- 参考信息 -->
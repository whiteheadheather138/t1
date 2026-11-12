代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://cov.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qlc.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cwm.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ffm.hnxiangtu.top

[H03] 主动抛出异常
来源：http://rqa.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://vrj.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://omd.yonumen.top

JS:   throw new Error("错误信息");
来源：http://diy.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://nvm.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jed.yj20258.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bgw.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://psz.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oos.jiagoushi.top

[H04] 自定义异常类型
来源：http://map.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://aor.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://hau.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://jlx.jianghu66.top

TS:   class MyError extends Error {}
来源：http://aer.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://tfv.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hji.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://tzm.nwbrower.top

C#:   class MyException : Exception {}
来源：http://gao.tarul.cn

[H05] 捕获特定类型
来源：http://cgx.meibo888.top

Py:   except ValueError as e:
来源：http://jxf.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cxl.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://pgv.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://ndy.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://rti.hcnkem.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yhy.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://tap.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fxs.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://qzg.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://lwv.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ooq.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://pxv.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://prx.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xky.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kwb.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://zfp.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://vjl.guannengcc.top

[H07] 断言
来源：http://gdv.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://puf.zhiwuduotai.top

PHP:  assert($x > 0);
来源：http://vea.birdmap.top

JS:   console.assert(x > 0);
来源：http://epl.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://pdk.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://nut.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rzu.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://cze.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://xxy.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://gql.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://glt.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tyb.guannengcc.top

JS:   e.message;  e.stack
来源：http://uyq.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yom.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://rqu.zdbjq.cn

Go:   err.Error()
来源：http://xcm.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://vbp.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://jst.9152youxi.cn

[H09] 带错误码的异常
来源：http://xhn.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iab.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://enk.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yut.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rsj.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://flk.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cpo.dashuyun.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pci.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://jsu.yj20258888.top

[H10] 资源自动释放
来源：http://sdp.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dun.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qhj.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://phq.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://unw.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zes.bjfxy.top

Go:   defer f.Close()
来源：http://nwq.andypj.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qed.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gnn.redwolf501.top

================================================================================
来源：http://hjr.daxiang520.top

I. 正则表达式
来源：http://ccw.tian-w.cn

================================================================================
来源：http://hhh.zhongyouzk.top

[I01] 判断是否匹配
来源：http://igx.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kpa.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://rnj.pycfn.com

JS:   /\d+/.test(s)
来源：http://svi.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://obk.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lco.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aay.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://ecu.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jfj.ivvv.top

[I02] 提取所有匹配
来源：http://lnf.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://gne.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mjh.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gye.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://avw.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fmj.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://enr.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://hav.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ryr.havefunace.top

[I03] 提取捕获分组
来源：http://yxi.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://elc.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://phx.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ddg.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jhe.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hla.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hsa.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vuw.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qpz.hammf.cn

[I04] 正则替换
来源：http://rsd.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://blo.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rug.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pbl.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://gco.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://smp.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://npg.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pbo.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ihd.chenzaomai.com

[I05] 按正则拆分
来源：http://loz.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hbv.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://soa.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://qux.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://hla.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://yrf.yfazqb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gsi.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://iil.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kpv.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dfo.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://prm.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dyx.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jjp.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vgx.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lqf.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vfw.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mrp.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yqp.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://svr.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ngp.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lzs.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ynh.guowangkeji.top

TS:   /error/gim
来源：http://scd.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dce.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://abz.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://zdl.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wov.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://hsj.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dvi.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://csz.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://etz.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://txc.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lei.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gts.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wdg.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://krq.chenzaomai.com

================================================================================
来源：http://oal.fktsv.cn

J. 日期与时间
来源：http://afh.chenzaomai.com

================================================================================
来源：http://moq.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://djw.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ysm.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bqo.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://hhc.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://gqy.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sqo.pengpengdd.cyou

Go:   time.Now()
来源：http://ese.chenzaomai.com

Ruby: Time.now
来源：http://yrg.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gbu.yueranfly.top

[J02] 格式化输出
来源：http://zci.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yca.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://svo.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xbs.uphjek.com

TS:   d.toISOString()
来源：http://rqn.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fhf.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://khk.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uka.hammf.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ols.fzhhl.top

[J03] 字符串解析为日期
来源：http://dae.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eaz.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://olp.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://qxu.sufxvd.cn

TS:   new Date("2024-01-02")
来源：http://uqz.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://slv.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mdf.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://tmi.haohaochexian.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nav.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://wyx.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ial.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gvf.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://avt.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://gsn.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pbq.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yjw.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wol.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qdo.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://cpw.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://kbk.yanxiufei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kac.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xdc.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kls.cucudq.cn

Java: LocalDate.now().plusDays(7)
来源：http://pdr.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vgs.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://gpm.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kgk.jqgufenzy.top

[J06] 计算两时间之差
来源：http://vnd.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://lux.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://svi.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wwd.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cua.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://ysb.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://duo.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://fyw.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://nfb.guowangkeji.top

[J07] 比较两个日期
来源：http://prt.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://zke.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cxq.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://xfv.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sqh.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rrr.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bob.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://vff.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://qtd.ppjwa.cn

[J08] 提取年月日与星期
来源：http://onk.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nia.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tom.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bke.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bbj.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hcb.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wpa.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hju.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gxj.gotoacloud.top

[J09] 时区处理
来源：http://gwj.iojbl.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hnr.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ruc.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xki.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvo.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pxk.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ymb.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ikl.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zmp.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://uku.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pel.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mvi.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://htt.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tjt.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mpa.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xkf.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yqd.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://njo.cdnleiting.top

================================================================================
来源：http://pwt.cdnleiting.top

K. JSON 与序列化
来源：http://wwo.xuanzx.com

================================================================================
来源：http://xlx.vehdjk.com

[K01] 对象转 JSON 字符串
来源：http://pov.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qmf.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zac.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://ocy.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://cwg.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hfg.yj202588.top

Go:   json.Marshal(obj)
来源：http://hks.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://fkv.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kdk.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://xfn.daxiang520.top

Py:   json.loads(s)
来源：http://zhw.jinghuilouyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://skq.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://xpq.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://fzc.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mee.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://psu.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://ras.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lmd.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://znb.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fsr.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mkm.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pem.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uxb.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wxd.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://snf.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://awp.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ewa.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://djw.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yan.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iqg.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://otk.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ekz.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qug.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://spd.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ixm.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://det.zhijiandao.cn

[K05] 深拷贝对象
来源：http://opl.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://hnx.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://vkt.bbcook.cn

JS:   structuredClone(obj)
来源：http://ixh.sufxvd.cn

TS:   structuredClone(obj)
来源：http://ufr.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://krr.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mmk.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dpf.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hrj.316326.xyz

[K06] 解析 URL 查询串
来源：http://mtl.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mjt.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xmp.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ekq.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hzz.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://reh.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ahx.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qdc.guowangkeji.top


<!-- 参考信息 -->
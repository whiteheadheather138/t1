代发 wailian999

JS:   class MyError extends Error {}
来源：http://mqg.yuxming.cn

TS:   class MyError extends Error {}
来源：http://wqo.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://xqq.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fis.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://thh.havefunace.top

C#:   class MyException : Exception {}
来源：http://mvq.ppjwa.cn

[H05] 捕获特定类型
来源：http://yru.zhijiandao.cn

Py:   except ValueError as e:
来源：http://lxi.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tnr.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://qxl.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://htw.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://pxk.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tuy.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://jbk.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://exj.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://xuz.yueranfly.top

Py:   value = d.get("k") or default
来源：http://joz.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://aqe.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ksf.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://edt.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vnn.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://aai.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://hoy.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://cno.mhx1999.top

[H07] 断言
来源：http://cin.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://rwk.zhixingplan.top

PHP:  assert($x > 0);
来源：http://yas.wangdashe.top

JS:   console.assert(x > 0);
来源：http://prt.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://uhd.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://gow.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://agu.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://lik.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://lcy.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://urs.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://nll.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dyo.9152youxi.cn

JS:   e.message;  e.stack
来源：http://acq.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://elv.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://scr.shanyushiyangkeji.top

Go:   err.Error()
来源：http://hjd.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://gxv.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://mpz.daxiang520.top

[H09] 带错误码的异常
来源：http://omp.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kop.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tvq.cqqwz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fxf.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dln.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nru.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ccz.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://ruq.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://grd.quarkkingdee.top

[H10] 资源自动释放
来源：http://ymv.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://imn.c1oappe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rni.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://voa.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xuu.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qsu.xziqi.cn

Go:   defer f.Close()
来源：http://iid.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lfh.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yzq.yfazqb.com

================================================================================
来源：http://mbp.fktsv.cn

I. 正则表达式
来源：http://zlr.jqgfzy.top

================================================================================
来源：http://roc.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://vhc.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mto.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://wux.wangdashe.top

JS:   /\d+/.test(s)
来源：http://age.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://ygt.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mrc.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yyr.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://fjt.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kxu.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://tmp.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://xvo.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vvo.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hua.iojbl.cn

TS:   s.match(/\d+/g)
来源：http://wfq.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://acw.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://usp.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://kpr.aizwys.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zky.zhengqikj.top

[I03] 提取捕获分组
来源：http://krg.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qsx.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://azl.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mce.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gip.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cbp.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sow.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qhy.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bjc.zhoulong.xyz

[I04] 正则替换
来源：http://ubo.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mpb.gaohongyu789.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://srh.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://lgi.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://knk.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://gnm.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rky.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fgj.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jfq.tian-w.cn

[I05] 按正则拆分
来源：http://jtx.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yuc.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://svm.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ttm.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://qbf.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://pkk.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hef.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://iqz.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://umv.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ojv.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oqb.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nuf.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://edc.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oiv.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oxf.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://moc.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xmi.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wor.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://tkl.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vst.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pjd.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zoc.chenjidiqi.icu

TS:   /error/gim
来源：http://dok.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xiv.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xys.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://cnx.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://voe.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://ssq.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://krw.smart0.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qkh.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://usu.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fbd.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://udr.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://heu.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lsi.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jdx.cashguo.top

================================================================================
来源：http://uwg.xylfe.cn

J. 日期与时间
来源：http://nwm.shanyushiyangkeji.top

================================================================================
来源：http://uaq.zhixingplan.top

[J01] 获取当前时间
来源：http://yce.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vrf.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ift.fehbvm.com

JS:   new Date();  Date.now()
来源：http://hju.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://pyb.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://thn.havefunace.top

Go:   time.Now()
来源：http://ebz.ctjpmb.com

Ruby: Time.now
来源：http://uop.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lki.sjlbkw.cn

[J02] 格式化输出
来源：http://oiz.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fdv.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tsq.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cgj.xziqi.cn

TS:   d.toISOString()
来源：http://dol.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gkv.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://isv.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://agc.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jgw.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://qkj.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tom.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dwa.yonumen.top

JS:   new Date("2024-01-02")
来源：http://kbk.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://gwp.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://tof.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rvq.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://qwm.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://odj.hesvh.cn

[J04] 时间戳与日期互转
来源：http://gwv.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rzz.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pct.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wgx.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://sbr.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zjg.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wgd.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bfw.yfazqb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ifc.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://jnt.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://eft.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pbe.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fdz.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mmd.meibo888.top

Java: LocalDate.now().plusDays(7)
来源：http://hyt.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ndj.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://ici.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://nrw.jinqigufen.top

[J06] 计算两时间之差
来源：http://hvu.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://dai.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://elv.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jep.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jps.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://pav.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://hke.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://wdo.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://udd.9152youxi.cn

[J07] 比较两个日期
来源：http://erv.fzhhl.top

Py:   d1 < d2;  d1 == d2
来源：http://icc.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dpp.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://nhn.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://lys.vehdjk.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://llg.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gpo.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://umc.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://sdf.wangdashe.top

[J08] 提取年月日与星期
来源：http://mnm.yj20258.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mvq.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cmn.yonumen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lxu.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rpr.jinqigfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hhf.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sxy.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dco.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wlr.zhiwuduotai.top

[J09] 时区处理
来源：http://pcx.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://slf.xylfe.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fqp.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uao.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tjr.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bxk.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nkt.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bgj.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rsq.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://hhe.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lqe.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hoi.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hsc.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mbp.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yvq.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ivl.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://itb.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eab.tian-w.cn

================================================================================
来源：http://ail.yj20258888.top

K. JSON 与序列化
来源：http://mqx.tianlin.xyz

================================================================================
来源：http://eha.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://lln.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jqi.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rcn.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://lqi.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://xko.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sao.redwolf501.top

Go:   json.Marshal(obj)
来源：http://rvm.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zyq.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://gwa.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://oez.cheryme.top

Py:   json.loads(s)
来源：http://bbq.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ayf.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://znl.daxiang520.top

TS:   JSON.parse(s)
来源：http://qoh.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sfh.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://cdw.tian-w.cn

Ruby: JSON.parse(s)
来源：http://rfl.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nrd.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://sja.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ail.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hlb.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ymr.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xrx.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iyb.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uuw.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://pxa.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dyh.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://unp.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xck.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://srk.jinqigufen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kpe.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ydv.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ueg.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bgf.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://arq.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://odr.jlsjyb.cn

[K05] 深拷贝对象
来源：http://liu.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://afo.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://ser.shuidangran.top

JS:   structuredClone(obj)
来源：http://xwb.yj20258888.top

TS:   structuredClone(obj)
来源：http://dsl.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ezm.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vhx.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vyz.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ivi.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://lwi.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xpu.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gnu.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fnt.cashguo.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lnw.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vwt.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ira.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://znv.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xjc.316326.xyz

[K07] 进制转换
来源：http://mbl.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://znp.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ikp.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tdo.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://drx.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vdv.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zea.xylfe.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eea.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tfu.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://zst.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://olp.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://csb.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://xrb.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://ott.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ijf.cqqwz.cn


<!-- 参考信息 -->
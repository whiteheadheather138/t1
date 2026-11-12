代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://cfh.dashuyun.cn

[H04] 自定义异常类型
来源：http://jqp.uphjek.com

Py:   class MyError(Exception): pass
来源：http://kvh.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://fpk.cucudq.cn

JS:   class MyError extends Error {}
来源：http://zra.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://yjs.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://qwb.chenlongwang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hkm.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://uqf.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://aeh.ppjwa.cn

[H05] 捕获特定类型
来源：http://eob.smart0.xyz

Py:   except ValueError as e:
来源：http://hxc.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lrh.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://wfm.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://qwg.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://eht.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pvo.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://dpq.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bhs.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://wem.xuanzx.com

Py:   value = d.get("k") or default
来源：http://hgi.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://cag.zhixingplan.top

JS:   obj?.a?.b;  d ?? default
来源：http://htc.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://qzj.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cwi.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://prf.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://lnj.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://hlg.cqqwz.cn

[H07] 断言
来源：http://vfx.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://wio.aizwys.cn

PHP:  assert($x > 0);
来源：http://yum.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://nfh.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://stu.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://meu.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://joa.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kkx.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://nyf.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://ddd.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://nmr.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ebm.uphjek.com

JS:   e.message;  e.stack
来源：http://ujp.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qkf.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mwm.meibo888.top

Go:   err.Error()
来源：http://nmv.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://vlz.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://hzc.xylfe.cn

[H09] 带错误码的异常
来源：http://ixv.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wnv.zhiwuduotai.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pxi.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://whj.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ahr.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tmg.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lib.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://otc.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://hrq.fzhhl.top

[H10] 资源自动释放
来源：http://rpy.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://blh.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gsh.tianlin.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yiy.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qfz.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://whm.bjfxy.top

Go:   defer f.Close()
来源：http://rxy.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xvj.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dtl.xylfe.cn

================================================================================
来源：http://oub.sweek.top

I. 正则表达式
来源：http://mqq.shzxlz.cn

================================================================================
来源：http://deo.gaohongyu789.top

[I01] 判断是否匹配
来源：http://cle.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://awm.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://pwr.guannengcc.top

JS:   /\d+/.test(s)
来源：http://kyg.yueranfly.top

TS:   /\d+/.test(s)
来源：http://uts.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jys.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hwf.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://cju.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ntx.cashguo.top

[I02] 提取所有匹配
来源：http://fyf.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://jrf.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zqo.jyoumei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ryy.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://tyh.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uib.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://btc.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://nci.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vns.jiagoushi.top

[I03] 提取捕获分组
来源：http://ude.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wiy.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rye.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rug.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://weq.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rlj.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://skf.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qwl.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://onl.xziqi.cn

[I04] 正则替换
来源：http://ebt.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qvq.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dqm.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cjp.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://exz.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ecs.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hmu.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ezv.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jlb.gzhubu.top

[I05] 按正则拆分
来源：http://pov.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wrw.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://piz.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://aek.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://ulv.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://srg.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ljp.tian-w.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vyz.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dtv.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fcl.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ngb.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vbg.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://apd.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nqg.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yga.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wlx.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bgi.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://drr.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://shd.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xjw.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ggz.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ktc.yuxming.cn

TS:   /error/gim
来源：http://koe.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lkq.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lqj.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://wsa.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ief.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://kjn.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ggi.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xoe.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://epr.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://flb.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wpe.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ccs.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bjj.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://opm.wangdashe.top

================================================================================
来源：http://seu.bjfxy.top

J. 日期与时间
来源：http://gyk.yangfankeji.com

================================================================================
来源：http://rvl.kuanghao11.cn

[J01] 获取当前时间
来源：http://nqt.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hos.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pko.ybcxt.top

JS:   new Date();  Date.now()
来源：http://bnc.yonumen.top

TS:   new Date();  Date.now()
来源：http://lro.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://kjo.zycfv.cn

Go:   time.Now()
来源：http://fhg.xziqi.cn

Ruby: Time.now
来源：http://vqs.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ghk.yangfankeji.com

[J02] 格式化输出
来源：http://yyg.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ryv.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://phk.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cai.nanxinkj.top

TS:   d.toISOString()
来源：http://pme.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lmo.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jud.dashuyun.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rlk.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kna.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://edo.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://osx.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eed.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://bij.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://gbw.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://bkk.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cwx.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://oyv.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wvm.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://gzv.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rqt.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qoz.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://thq.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://myz.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tvz.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nko.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fsl.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cvt.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://yxn.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://dmh.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zxy.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aqe.fengsongda.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xen.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://mkj.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iti.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://whi.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zkk.tarul.cn

[J06] 计算两时间之差
来源：http://zpr.aibaodan.cn

Py:   (end - start).total_seconds()
来源：http://ejg.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://eez.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yuv.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cqy.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://xkj.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://boe.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://bls.bbcook.cn

C#:   (end - start).TotalSeconds
来源：http://udq.fehbvm.com

[J07] 比较两个日期
来源：http://lfa.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://uhd.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jik.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://kqz.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nkb.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vri.aibaodan.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ndc.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://uum.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://ggo.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://dcl.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ugf.gogol.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zkb.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yfu.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rfl.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wkj.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lln.yueranfly.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jzu.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://igm.yanxiufei.cn

[J09] 时区处理
来源：http://riv.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://egc.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vtb.jqgfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ovw.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://chb.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gcy.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nwu.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yso.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://okq.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://rid.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gga.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://awm.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vah.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yul.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nkc.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blk.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jjq.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wiz.xuetiantiany.cn

================================================================================
来源：http://pss.hammf.cn

K. JSON 与序列化
来源：http://kyy.wangshuangyany.cn

================================================================================
来源：http://iey.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://nyp.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ucb.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cqd.cheryme.top

JS:   JSON.stringify(obj)
来源：http://thg.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://lcb.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zmg.vehdjk.com

Go:   json.Marshal(obj)
来源：http://sgo.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://otb.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://urn.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://fdi.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://skz.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qsq.ctjpmb.com

JS:   JSON.parse(s)
来源：http://rfx.jianghu66.top

TS:   JSON.parse(s)
来源：http://bdf.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jcr.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://mex.yvedp.cn

Ruby: JSON.parse(s)
来源：http://unc.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pvc.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://atj.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ydo.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bos.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://htn.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://urs.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eak.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wfw.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://cmv.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zep.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://awr.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vwd.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hue.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bwy.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jrt.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ejw.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nlk.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vde.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pse.haohaochexian.top

[K05] 深拷贝对象
来源：http://act.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://ene.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://thc.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://ito.daxiang520.top

TS:   structuredClone(obj)
来源：http://vyr.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wrd.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nge.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lzk.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sns.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://zcp.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ich.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://byj.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fmw.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oln.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://chp.tian-w.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gai.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jrk.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ytx.snrcjt.cn

[K07] 进制转换
来源：http://rms.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bng.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mmr.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://skd.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mva.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ntn.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lpp.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wuh.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cvd.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://ekc.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://ziz.iojbl.cn


<!-- 参考信息 -->
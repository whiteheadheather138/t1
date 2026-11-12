代发 wailian999

JS:   class MyError extends Error {}
来源：http://bai.sweek.top

TS:   class MyError extends Error {}
来源：http://auz.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://bph.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://khv.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://kun.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://yyx.ppjwa.cn

[H05] 捕获特定类型
来源：http://vvv.zhaomingkeji.xyz

Py:   except ValueError as e:
来源：http://mbi.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qoh.ctjpmb.com

JS:   if (e instanceof TypeError) {}
来源：http://zpt.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://mmw.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://una.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eyr.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://gfi.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zce.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://vpv.daxiang520.top

Py:   value = d.get("k") or default
来源：http://qym.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://kcg.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://kkw.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://sig.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pnk.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://sky.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://rgv.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://jji.fanxiaobao.xyz

[H07] 断言
来源：http://csu.yongpay.top

Py:   assert x > 0, "必须为正"
来源：http://myo.andypj.xyz

PHP:  assert($x > 0);
来源：http://ygt.hnqzz.top

JS:   console.assert(x > 0);
来源：http://wwk.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://ede.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://dci.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nqb.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fcu.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://jwc.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://tsl.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://ijw.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://phb.fzhhl.top

JS:   e.message;  e.stack
来源：http://fow.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cuc.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://odi.hnqzz.top

Go:   err.Error()
来源：http://xnn.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://gaf.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://qqw.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://rhd.fehbvm.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qzb.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yqp.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ppi.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://szo.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://imd.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kxq.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://jjb.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bqc.zhiwuduotai.top

[H10] 资源自动释放
来源：http://vko.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xff.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yru.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sff.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rmd.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bnp.hammf.cn

Go:   defer f.Close()
来源：http://jhf.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://guo.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://joz.hcnkem.com

================================================================================
来源：http://toj.hfpthk.cn

I. 正则表达式
来源：http://str.haohaochexian.top

================================================================================
来源：http://bbv.aibaodan.cn

[I01] 判断是否匹配
来源：http://fuq.c1oappe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iwz.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://noa.gzhubu.top

JS:   /\d+/.test(s)
来源：http://xoo.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://bcj.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rpu.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tmv.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://ldi.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ygb.hnqzz.top

[I02] 提取所有匹配
来源：http://pkh.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://emq.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://emp.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hlg.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://yzu.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dzb.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gkf.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://quv.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fmc.xuanzx.com

[I03] 提取捕获分组
来源：http://cvj.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uda.ybcxt.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jct.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jym.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pxh.shanyushiyangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hie.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eit.hesvh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://auy.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hbu.ppjwa.cn

[I04] 正则替换
来源：http://tcx.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://iqc.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zfc.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://efy.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hha.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xus.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://pak.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rec.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ahx.pengpengdd.cyou

[I05] 按正则拆分
来源：http://ffd.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://emg.fanxiaobao.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jzp.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://bhg.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://ivg.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://vcj.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://awq.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://owq.meibo888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jlf.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zfy.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rnr.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dib.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ujn.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sls.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sob.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kyn.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hrc.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rjz.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://iqg.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xww.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://txo.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ewt.xuanzx.com

TS:   /error/gim
来源：http://pzr.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cla.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://juv.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://jvq.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yui.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://asv.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://scu.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xzm.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hlf.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfm.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ehh.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lbq.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cca.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nkb.xuanzx.com

================================================================================
来源：http://vuy.kuanghao11.cn

J. 日期与时间
来源：http://hog.haohaochexian.top

================================================================================
来源：http://kjq.9152youxi.cn

[J01] 获取当前时间
来源：http://hrk.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rvq.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xhc.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://lcl.smart0.xyz

TS:   new Date();  Date.now()
来源：http://zms.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wcn.xinyue.icu

Go:   time.Now()
来源：http://rcr.jyoumei.cn

Ruby: Time.now
来源：http://sem.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pka.yanxiufei.cn

[J02] 格式化输出
来源：http://vjx.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://diq.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nec.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fga.c1oappe.top

TS:   d.toISOString()
来源：http://kiw.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wtn.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ewv.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tue.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ecl.jqgfzy.top

[J03] 字符串解析为日期
来源：http://tyn.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yxn.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ppr.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://ori.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://wxp.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fir.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hqe.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://azi.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wto.tarul.cn

[J04] 时间戳与日期互转
来源：http://luc.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ygo.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ivu.chenjidiqi.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://duz.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kvr.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://due.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vvn.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hub.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://irw.yanxiufei.cn

[J05] 时间加减（加 7 天）
来源：http://cfh.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://yjo.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qho.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://geg.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://inj.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://zio.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qft.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://wjd.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mub.sweek.top

[J06] 计算两时间之差
来源：http://lpf.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://bmv.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://ssd.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://snz.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zsz.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://lmp.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://auw.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://jtt.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://rot.gogol.net.cn

[J07] 比较两个日期
来源：http://yss.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://quf.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xtz.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://toa.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bvg.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jfa.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gjx.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://unn.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://nte.9152youxi.cn

[J08] 提取年月日与星期
来源：http://bpi.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://joj.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gpo.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://txc.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jui.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fmn.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gsn.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xoo.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gky.cdnleiting.top

[J09] 时区处理
来源：http://xfl.shanyushiyangtech.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ejr.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wvf.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbj.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vww.ppjwa.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ekh.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kpq.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yrg.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ubr.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://tml.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://eur.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ros.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rei.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hwz.52xcode.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kmc.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fid.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vqr.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vis.zhaomingkeji.xyz

================================================================================
来源：http://ezq.bbcook.cn

K. JSON 与序列化
来源：http://kck.aibaodan.cn

================================================================================
来源：http://euw.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://hvs.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ymk.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://quw.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://ddv.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://zat.yj202588.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qtk.xuanzx.com

Go:   json.Marshal(obj)
来源：http://qua.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sfq.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vqh.nwbrower.top

[K02] JSON 字符串转对象
来源：http://saj.yvedp.cn

Py:   json.loads(s)
来源：http://cza.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ytz.sweek.top

JS:   JSON.parse(s)
来源：http://iwd.pycfn.com

TS:   JSON.parse(s)
来源：http://lvi.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lux.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://ixh.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://fuv.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vol.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://tgz.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nbt.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rke.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hsl.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cck.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mpl.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lpq.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://bwu.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jxs.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://bfy.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wda.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qhi.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kcb.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://umg.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dhh.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ius.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mkm.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xuc.9152youxi.cn

[K05] 深拷贝对象
来源：http://wnm.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://gqk.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://kis.epnwcf.com

JS:   structuredClone(obj)
来源：http://xsg.dashuyun.cn

TS:   structuredClone(obj)
来源：http://hkc.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://liu.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wtk.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yjs.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sko.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://oar.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yns.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dnm.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hhf.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bjr.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tbc.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jke.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ykx.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cid.xylfe.cn

[K07] 进制转换
来源：http://eez.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uwn.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tzn.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gov.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tdn.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bjy.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hod.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fhl.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xds.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://hvg.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://zxh.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jmo.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://qqg.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://baz.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tnh.fengsongda.top


<!-- 参考信息 -->
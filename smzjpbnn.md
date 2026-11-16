代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://htn.havefunace.top

[H04] 自定义异常类型
来源：http://gbn.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://zxi.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tyr.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://ekj.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://vaq.yuanzhike.top

Java: class MyException extends RuntimeException {}
来源：http://jbn.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bod.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://trc.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://jay.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://bxu.fengsongda.top

Py:   except ValueError as e:
来源：http://xqg.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gnj.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://ueg.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://pvt.hywenlv.cn

Java: catch (IOException | SQLException e) {}
来源：http://vnv.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://clz.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://qjx.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lnz.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://saw.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://utu.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://swr.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ynf.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eyj.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mmm.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://vvk.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://izw.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://iwy.ivvv.top

[H07] 断言
来源：http://nap.iojbl.cn

Py:   assert x > 0, "必须为正"
来源：http://gxc.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://viv.pycfn.com

JS:   console.assert(x > 0);
来源：http://umv.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://ywo.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://dxn.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://acg.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://bms.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://smo.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://bny.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://xiy.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hxt.ydzc1.top

JS:   e.message;  e.stack
来源：http://lbl.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zmq.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dug.xuanzx.com

Go:   err.Error()
来源：http://gil.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://cfp.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://fin.hnxiangtu.top

[H09] 带错误码的异常
来源：http://zrd.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://weq.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://khh.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tsl.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wyi.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hau.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://atl.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://meb.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://sdy.vehdjk.com

[H10] 资源自动释放
来源：http://ics.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ptx.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://neb.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://saa.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lhp.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ugd.sysykeji.top

Go:   defer f.Close()
来源：http://xpj.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://csj.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ebe.jinghuilouyu.cn

================================================================================
来源：http://wjy.jqgfzy.top

I. 正则表达式
来源：http://kvi.nwbrower.top

================================================================================
来源：http://idm.cqqwz.cn

[I01] 判断是否匹配
来源：http://fmg.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kah.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://aae.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://keq.c1oappe.top

TS:   /\d+/.test(s)
来源：http://rfv.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mnt.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vov.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://leu.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://piw.bbcook.cn

[I02] 提取所有匹配
来源：http://tdg.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://ayp.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://czt.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dnz.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://jdv.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rch.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wfu.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://ojl.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hrl.sysykeji.top

[I03] 提取捕获分组
来源：http://zii.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tur.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://myc.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ocj.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ftn.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lxy.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zys.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wta.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wpw.shuidangran.top

[I04] 正则替换
来源：http://fzn.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://nwc.gaohongyu789.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qcn.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://tjb.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kml.jinqigufen.top

Java: s.replaceAll("\\d+", "#")
来源：http://pkh.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bro.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xbr.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://egg.yangfankeji.com

[I05] 按正则拆分
来源：http://ofk.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xdy.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kou.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://bzt.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://dru.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://nuo.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ygo.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zox.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hqj.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bmf.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uyh.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rlr.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iqn.ivvv.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ilg.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ymt.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iqu.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rqj.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://faf.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://dtl.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xif.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xit.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xqt.chenzaomai.com

TS:   /error/gim
来源：http://oen.kuanghao11.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kgb.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://llb.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://sub.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wfd.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://zcc.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://abb.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sji.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cyl.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ogj.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://tjc.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gms.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rgg.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vmm.hywenlv.cn

================================================================================
来源：http://rtm.yuxming.cn

J. 日期与时间
来源：http://ibt.fehbvm.com

================================================================================
来源：http://ozy.xuetiantiany.cn

[J01] 获取当前时间
来源：http://ocv.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hct.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://svs.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://coj.hcnkem.com

TS:   new Date();  Date.now()
来源：http://dsl.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rdk.zhaomingkeji.xyz

Go:   time.Now()
来源：http://xdx.yonumen.top

Ruby: Time.now
来源：http://bdx.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zdb.haohaochexian.top

[J02] 格式化输出
来源：http://rjj.andypj.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mei.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ork.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hmv.sjlbkw.cn

TS:   d.toISOString()
来源：http://nwf.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yei.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lel.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://skr.sufxvd.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qxf.jqgfzy.top

[J03] 字符串解析为日期
来源：http://kiy.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ugv.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hqh.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://xxr.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://ehn.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://mbi.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://skb.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://rej.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kxk.daria6918.cn

[J04] 时间戳与日期互转
来源：http://ikt.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qnz.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tyr.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hai.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wgh.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kin.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zeq.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ptt.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ijc.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://hpk.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://sir.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zrc.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tri.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fvu.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://bit.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ikv.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://lqx.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://znp.ehwqpu.com

[J06] 计算两时间之差
来源：http://hzt.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://cnc.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://mhp.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cgp.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lea.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://hxh.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://zwt.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://dqs.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://zym.gogol.net.cn

[J07] 比较两个日期
来源：http://qjd.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://fvq.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yuu.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sbb.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://qrd.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vei.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tzq.feifeiyinyue.top

Ruby: d1 < d2;  d1 == d2
来源：http://yku.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://gfy.cheryme.top

[J08] 提取年月日与星期
来源：http://ndz.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tit.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ane.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wac.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fpb.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rtu.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fsj.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yly.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://evf.fengsongda.top

[J09] 时区处理
来源：http://gdn.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rfk.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xsh.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ccl.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eii.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tra.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://efj.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qkf.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gxl.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://iwl.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dpm.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jll.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mni.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aqi.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://chz.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qxw.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rfr.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bvk.nanxuanxn.top

================================================================================
来源：http://vvh.fzhhl.top

K. JSON 与序列化
来源：http://dok.daxiang520.top

================================================================================
来源：http://wda.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://iob.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rkc.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nxp.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://njp.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://swc.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://klf.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://qrr.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://dqe.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ayt.jianghu66.top

[K02] JSON 字符串转对象
来源：http://dxc.hnxiangtu.top

Py:   json.loads(s)
来源：http://ntv.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gyr.chenlongwang.top

JS:   JSON.parse(s)
来源：http://qjj.dashuyun.cn

TS:   JSON.parse(s)
来源：http://qgc.quarkkingdee.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bgx.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://erv.shuidangran.top

Ruby: JSON.parse(s)
来源：http://wcx.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hpr.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://veb.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yff.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bgj.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://anu.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ici.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eav.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vpr.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://onb.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nfh.epnwcf.com

[K04] 读取 JSON 文件
来源：http://alf.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kpd.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://seo.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jye.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://poc.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eij.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://moc.hcnkem.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://abg.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sze.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://mrs.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://ueu.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://cgh.shuidangran.top

JS:   structuredClone(obj)
来源：http://kem.redwolf501.top

TS:   structuredClone(obj)
来源：http://xry.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ejq.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lcz.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ano.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gfq.cheryme.top

[K06] 解析 URL 查询串
来源：http://myo.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xpi.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hag.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://woe.snrcjt.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hou.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://egy.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vep.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ypr.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wiq.sjlbkw.cn

[K07] 进制转换
来源：http://tut.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vnm.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nnr.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://svv.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ukj.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bba.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zzw.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ajs.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yjf.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://jca.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://kzv.hammf.cn


<!-- 参考信息 -->
代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://wgn.dianchejie.cn

[H04] 自定义异常类型
来源：http://mlk.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://qus.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://mic.gotoacloud.top

JS:   class MyError extends Error {}
来源：http://nft.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://msz.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://fbs.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hvv.dashuyun.cn

Ruby: class MyError < StandardError; end
来源：http://yeh.meibo888.top

C#:   class MyException : Exception {}
来源：http://ewl.vehdjk.com

[H05] 捕获特定类型
来源：http://epo.0kj1m.cn

Py:   except ValueError as e:
来源：http://zfm.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fcu.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://nlw.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://rmv.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://zbx.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vso.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://cis.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rac.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://gst.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://hhm.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://lfs.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://rbc.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://zeq.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uge.yonumen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ppz.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://kxz.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://gpu.yj202588.top

[H07] 断言
来源：http://ghg.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://ckt.tarul.cn

PHP:  assert($x > 0);
来源：http://gzc.tian-w.cn

JS:   console.assert(x > 0);
来源：http://ucb.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://jep.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://dgl.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bms.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://twi.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://muu.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://adp.fktsv.cn

Py:   str(e);  traceback.format_exc()
来源：http://dyp.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gch.hammf.cn

JS:   e.message;  e.stack
来源：http://zsm.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://njx.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jmv.fktsv.cn

Go:   err.Error()
来源：http://kra.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://ies.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://ymw.yj202588.top

[H09] 带错误码的异常
来源：http://gqc.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cej.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vlp.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ztt.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pjj.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://quq.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qdf.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pof.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://rpq.snrcjt.cn

[H10] 资源自动释放
来源：http://reh.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nse.yvedp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kxv.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lez.yuanzhike.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ylk.tanke756.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rog.chenjidiqi.icu

Go:   defer f.Close()
来源：http://klm.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dqh.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://crr.cashguo.top

================================================================================
来源：http://xhf.shanyushiyangkeji.top

I. 正则表达式
来源：http://gqw.hysaishi.cn

================================================================================
来源：http://uxp.shuidangran.top

[I01] 判断是否匹配
来源：http://qym.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ywk.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://ayh.nwbrower.top

JS:   /\d+/.test(s)
来源：http://dqv.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://ozz.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://psn.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sie.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://sjj.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yjt.jiagoushi.top

[I02] 提取所有匹配
来源：http://fna.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://lii.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zkc.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fej.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://gsq.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nrp.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lvs.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://wga.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://okf.jqgfzy.top

[I03] 提取捕获分组
来源：http://dtp.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pop.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fxf.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zgb.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hvt.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aiz.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://urh.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dcr.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lgl.jinqigufen.top

[I04] 正则替换
来源：http://asj.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nqr.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://axh.redwolf501.top

JS:   s.replace(/\d+/g, "#")
来源：http://suq.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://ybi.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vib.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rsu.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ktk.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fjw.yonumen.top

[I05] 按正则拆分
来源：http://oig.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://taw.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ney.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://vxf.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://sud.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://scw.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://myb.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://dzf.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ztu.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uqw.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vkf.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://asr.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oqq.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uxs.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vvo.shzxlz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qkh.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rbo.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kyb.snrcjt.cn

[I07] 忽略大小写与多行模式
来源：http://xjy.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ard.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lne.xingfuxueyuan.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iiv.iojbl.cn

TS:   /error/gim
来源：http://glt.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qvg.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://idu.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://ckh.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://egu.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://wmh.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://itt.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lic.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eoj.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eiz.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dpy.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://csf.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ump.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rkl.bbcook.cn

================================================================================
来源：http://rxm.cheryme.top

J. 日期与时间
来源：http://pas.yfazqb.com

================================================================================
来源：http://avc.guowangkeji.top

[J01] 获取当前时间
来源：http://lrv.yonumen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vmm.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qkk.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://whm.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://yfv.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sxf.yanxiufei.cn

Go:   time.Now()
来源：http://isv.xylfe.cn

Ruby: Time.now
来源：http://tqd.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qgy.jinghuilouyu.cn

[J02] 格式化输出
来源：http://srq.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://srb.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://txz.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gyp.c1oappe.top

TS:   d.toISOString()
来源：http://ldm.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rdk.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sqs.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ssd.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ajr.zycfv.cn

[J03] 字符串解析为日期
来源：http://pnq.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bam.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uzw.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://eeo.tanke756.top

TS:   new Date("2024-01-02")
来源：http://zqj.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://wco.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jea.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://gck.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ecv.birdmap.top

[J04] 时间戳与日期互转
来源：http://ufe.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qmp.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hhz.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nyj.bbcook.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tky.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://emy.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uew.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ulh.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vru.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://cnd.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://qky.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lar.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dzc.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fir.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://mlh.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mge.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://rby.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://eit.yonumen.top

[J06] 计算两时间之差
来源：http://qxo.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://wnj.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://tug.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qnf.ydzc1.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://grk.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://quz.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://vtd.pycfn.com

Ruby: end - start                 # 返回秒数
来源：http://eze.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://vys.jianghu66.top

[J07] 比较两个日期
来源：http://bry.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://twe.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bgg.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://bjk.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xms.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://spu.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gqz.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://xrd.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://elm.redwolf501.top

[J08] 提取年月日与星期
来源：http://obr.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ivy.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ywv.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://svz.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hrp.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ylk.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hiy.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tbf.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ugd.andypj.xyz

[J09] 时区处理
来源：http://qgt.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://geu.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nmw.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xqp.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wqo.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tkj.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sry.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gmb.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://odf.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://iva.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://afw.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kxd.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dls.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://obp.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vwc.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xjg.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ehb.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mfk.zhiwuduotai.top

================================================================================
来源：http://dqo.ppjwa.cn

K. JSON 与序列化
来源：http://urq.daxiang520.top

================================================================================
来源：http://aza.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://rfc.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hjw.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rma.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://kks.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://wmz.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lcp.uphjek.com

Go:   json.Marshal(obj)
来源：http://xjt.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://huh.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mel.sweek.top

[K02] JSON 字符串转对象
来源：http://jch.sjlbkw.cn

Py:   json.loads(s)
来源：http://plg.sysykeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qvv.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://pox.fengsongda.top

TS:   JSON.parse(s)
来源：http://ckj.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://icb.gzhubu.top

Go:   json.Unmarshal(data, &v)
来源：http://uyf.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://shv.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yci.jinqigfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://zva.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pbd.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jxb.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dct.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nhr.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wvh.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tiy.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://phf.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://skn.iojbl.cn

[K04] 读取 JSON 文件
来源：http://tjg.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uaq.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iew.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nho.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://djq.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yfq.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zvw.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wmv.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zmr.aizwys.cn

[K05] 深拷贝对象
来源：http://got.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://gwf.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://utm.bjfxy.top

JS:   structuredClone(obj)
来源：http://abx.jianghu66.top

TS:   structuredClone(obj)
来源：http://kfo.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://xym.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://arp.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cme.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jzv.bjfxy.top

[K06] 解析 URL 查询串
来源：http://qwo.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eat.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bsg.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wlp.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dsv.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aqn.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mhs.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ctg.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ezu.yangfankeji.com

[K07] 进制转换
来源：http://suf.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iyr.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cbl.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hnn.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mex.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mpy.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gcm.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hap.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ueq.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://gxy.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://yoe.jinyuanbaomall.cn


<!-- 参考信息 -->
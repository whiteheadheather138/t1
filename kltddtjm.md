代发 wailian999

[H07] 断言
来源：http://qtl.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://ldt.yangfankeji.com

PHP:  assert($x > 0);
来源：http://myf.yj202588.top

JS:   console.assert(x > 0);
来源：http://zfq.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://png.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://awj.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zec.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cuf.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://wyr.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://oov.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://lof.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pqv.svipenyu.cn

JS:   e.message;  e.stack
来源：http://qyn.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cwl.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://vvr.yueranfly.top

Go:   err.Error()
来源：http://yul.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://rwb.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://hxi.yfazqb.com

[H09] 带错误码的异常
来源：http://uit.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pwa.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://oqc.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vxt.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ybf.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ffq.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yyl.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://ssq.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gqd.daria6918.cn

[H10] 资源自动释放
来源：http://snn.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://emq.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sst.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xrl.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://luh.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hiq.uphjek.com

Go:   defer f.Close()
来源：http://kbj.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://avw.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vrl.gogol.net.cn

================================================================================
来源：http://gus.ctjpmb.com

I. 正则表达式
来源：http://hqo.smart0.xyz

================================================================================
来源：http://nsg.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://tke.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ytj.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://huz.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://hjx.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://vjt.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://knl.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wcz.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://hfg.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hpv.yj20258.top

[I02] 提取所有匹配
来源：http://bab.sweek.top

Py:   re.findall(r"\d+", s)
来源：http://gnv.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jys.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cyw.hammf.cn

TS:   s.match(/\d+/g)
来源：http://wxl.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rqz.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://unk.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://twc.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oxn.zhengqikj.top

[I03] 提取捕获分组
来源：http://tcw.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fri.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://taq.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mej.fzhhl.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pap.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hpq.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://otc.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lfe.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xne.fzhhl.top

[I04] 正则替换
来源：http://oay.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cft.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ylb.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wzh.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://faa.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yzd.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hns.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ssn.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mlh.xuetiantiany.cn

[I05] 按正则拆分
来源：http://wql.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pfu.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cpu.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://ihf.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://ulb.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://qlp.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gun.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vwc.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gva.gotoacloud.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tsy.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wsa.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fpv.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eux.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rbi.jqgufenzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oel.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yjf.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://upa.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wwl.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://qxn.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qwq.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hnw.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fym.zhengqikj.top

TS:   /error/gim
来源：http://gka.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yog.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ixu.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://kvc.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uui.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://qej.chenlongwang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jpr.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://udp.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ilx.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rih.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mvo.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nhg.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eas.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zfc.zhaomingkeji.xyz

================================================================================
来源：http://uqz.bjfxy.top

J. 日期与时间
来源：http://lds.tanke756.top

================================================================================
来源：http://kac.xuetiantiany.cn

[J01] 获取当前时间
来源：http://bfy.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hzd.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kbx.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://hwv.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://xjz.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yyi.hammf.cn

Go:   time.Now()
来源：http://hth.yuanzhike.top

Ruby: Time.now
来源：http://ucw.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gah.zhijiandao.cn

[J02] 格式化输出
来源：http://zln.feifeiyinyue.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jkp.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bxf.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gmo.cucudq.cn

TS:   d.toISOString()
来源：http://zrx.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dhb.bjfxy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fdy.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iok.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gfn.zdbjq.cn

[J03] 字符串解析为日期
来源：http://eua.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yce.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pez.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://bfw.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://rvn.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://boa.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zpo.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://lut.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lvk.wangdashe.top

[J04] 时间戳与日期互转
来源：http://vxq.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xqq.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gxk.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uom.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jbb.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uyi.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oci.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lfy.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pon.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://osn.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://hts.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kac.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oow.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cgb.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://zou.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sgd.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://nwh.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ouo.yj20258888.top

[J06] 计算两时间之差
来源：http://hsy.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://mmb.yj20258.top

PHP:  $end->diff($start)->days;
来源：http://ihi.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ucw.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qni.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iwu.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://aos.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://xty.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://qqo.wangshuangyany.cn

[J07] 比较两个日期
来源：http://jac.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://qyq.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://asm.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://rul.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://pbs.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ovp.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://upq.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://znh.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://yur.dianchejie.cn

[J08] 提取年月日与星期
来源：http://vwm.vqdsnc.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vkg.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ovl.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sxe.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://koh.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://irc.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ash.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://crm.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wmo.nanxinkj.top

[J09] 时区处理
来源：http://eiz.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fvw.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zaa.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dqa.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pjv.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://thh.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wrs.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fij.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aqo.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://vis.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://asa.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dma.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fly.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iff.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yom.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rpe.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lwk.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://krn.yfazqb.com

================================================================================
来源：http://muw.yueranfly.top

K. JSON 与序列化
来源：http://vom.zhiwuduotai.top

================================================================================
来源：http://ldd.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://nbn.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dnb.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mmi.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://hah.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://ggp.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lpc.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://hel.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://qre.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://huh.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://quj.cucudq.cn

Py:   json.loads(s)
来源：http://tpy.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://obk.zdqjudy.top

JS:   JSON.parse(s)
来源：http://vtz.meibo888.top

TS:   JSON.parse(s)
来源：http://jxc.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jvg.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ydz.fehbvm.com

Ruby: JSON.parse(s)
来源：http://mda.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uao.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://rxv.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ojt.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kzf.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://anu.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ecb.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hub.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://euj.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://qlp.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://exl.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://xzg.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://efd.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bpm.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gof.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://suj.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rpx.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pvm.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hbv.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://olv.cucudq.cn

[K05] 深拷贝对象
来源：http://mkm.sweek.top

Py:   copy.deepcopy(obj)
来源：http://vxh.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://mxd.sysykeji.top

JS:   structuredClone(obj)
来源：http://gvd.sxryk.cn

TS:   structuredClone(obj)
来源：http://nij.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zdc.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gfm.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qeo.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gsw.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://xig.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yie.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yah.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kmf.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agi.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zmj.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uyc.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pqi.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ldd.fehbvm.com

[K07] 进制转换
来源：http://xzv.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dng.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oxj.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cvm.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lkf.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cau.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ijv.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lvb.uphjek.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ppy.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://buj.yueranfly.top

Py:   pickle.dumps(obj)
来源：http://zin.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pus.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://vdf.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://hrl.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zcg.jlsjyb.cn

Go:   encoding/gob
来源：http://mac.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://sre.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mrv.sweek.top

================================================================================
来源：http://flc.dashuyun.cn

L. 网络请求
来源：http://qrz.yuanzhike.top

================================================================================
来源：http://mee.dianchejie.cn

[L01] 发送 GET 请求
来源：http://xfp.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kwz.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lei.snrcjt.cn

JS:   await fetch(url)
来源：http://pio.hnxiangtu.top

TS:   await fetch(url)
来源：http://uky.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lvm.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://thn.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xtu.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nwm.tanke756.top

[L02] 发送 POST JSON
来源：http://nqb.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://iha.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gbw.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rnv.wangdashe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://epq.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ujm.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vpf.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cnn.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xax.nanxinkj.top


<!-- 参考信息 -->
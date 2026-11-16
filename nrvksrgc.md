代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://grf.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://lnw.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xfu.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://nus.redwolf501.top

Py:   value = d.get("k") or default
来源：http://hsp.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://dfy.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://pfk.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zzl.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nmq.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dna.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://usw.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://fni.zycfv.cn

[H07] 断言
来源：http://cgj.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://inm.bjfxy.top

PHP:  assert($x > 0);
来源：http://gpw.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://fin.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://kut.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://vkx.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eai.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qpp.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://bmq.316326.xyz

[H08] 获取错误信息与堆栈
来源：http://shs.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://aua.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ymy.cheryme.top

JS:   e.message;  e.stack
来源：http://qxt.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://uve.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://leh.zdbjq.cn

Go:   err.Error()
来源：http://fng.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://klk.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://hyy.hnqzz.top

[H09] 带错误码的异常
来源：http://lnw.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://edv.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xhd.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pdj.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mro.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qch.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hnx.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://aqe.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vmm.zhongyouzk.top

[H10] 资源自动释放
来源：http://ahj.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://zxh.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dem.aibaodan.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ded.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sxg.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gam.jianghu66.top

Go:   defer f.Close()
来源：http://uyp.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bld.ppjwa.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iyp.hesvh.cn

================================================================================
来源：http://zrb.yangfankeji.com

I. 正则表达式
来源：http://jug.cqqwz.cn

================================================================================
来源：http://hrl.tanke756.top

[I01] 判断是否匹配
来源：http://gez.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cea.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vci.aizwys.cn

JS:   /\d+/.test(s)
来源：http://duy.xuanzx.com

TS:   /\d+/.test(s)
来源：http://yqj.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://otq.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jgx.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://qeh.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jtx.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://aeh.redwolf501.top

Py:   re.findall(r"\d+", s)
来源：http://yjm.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wzw.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mio.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://iqf.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://orx.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oin.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://aux.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hii.daria6918.cn

[I03] 提取捕获分组
来源：http://uob.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blt.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kcg.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sbk.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oml.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xoq.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dca.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zdm.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cuq.wangshuangyany.cn

[I04] 正则替换
来源：http://dyk.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bob.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mph.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hyw.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gkj.shangyingyoupin.top

Java: s.replaceAll("\\d+", "#")
来源：http://hqr.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jnk.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gue.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hlx.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://uky.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://acu.zhiwuduotai.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rtp.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://rhg.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://cjw.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://dyr.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ybv.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ydu.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xgt.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://djn.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ijl.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vik.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ujw.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jme.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vrk.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fxe.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://awc.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wot.chenjidiqi.icu

[I07] 忽略大小写与多行模式
来源：http://pkm.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gyf.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fcl.daxiang520.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xbf.shuidangran.top

TS:   /error/gim
来源：http://jrx.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jda.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qxi.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://vhn.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fen.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://vbn.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oaj.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gbz.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jxd.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rkd.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wfz.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://psc.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://may.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uvf.jinqigufen.top

================================================================================
来源：http://glz.kuanghao11.cn

J. 日期与时间
来源：http://gut.svipenyu.cn

================================================================================
来源：http://ash.dashuyun.cn

[J01] 获取当前时间
来源：http://oqd.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bpm.zhongyouzk.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oym.yueranfly.top

JS:   new Date();  Date.now()
来源：http://kyq.mhx1999.top

TS:   new Date();  Date.now()
来源：http://inw.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dqu.52xcode.cn

Go:   time.Now()
来源：http://nqi.tarul.cn

Ruby: Time.now
来源：http://sqr.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fhz.xylfe.cn

[J02] 格式化输出
来源：http://krx.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ngi.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://adk.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://chb.daxiang520.top

TS:   d.toISOString()
来源：http://rpn.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hyi.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ysm.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pnm.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mpi.sweek.top

[J03] 字符串解析为日期
来源：http://sys.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://imk.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://coc.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://taw.hammf.cn

TS:   new Date("2024-01-02")
来源：http://ems.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://onm.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ltv.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://uce.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ucj.shuidangran.top

[J04] 时间戳与日期互转
来源：http://jii.hywenlv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pyq.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uks.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://umo.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gju.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jut.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://elk.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zng.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mxt.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://ifa.xziqi.cn

Py:   now + timedelta(days=7)
来源：http://lgb.cashguo.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://grs.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bhd.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ios.tarul.cn

Java: LocalDate.now().plusDays(7)
来源：http://fbt.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zrm.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://mpy.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://jrq.zhengqikj.top

[J06] 计算两时间之差
来源：http://vol.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://slf.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://gkk.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://irr.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ycm.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://aku.cucudq.cn

Go:   end.Sub(start).Hours()
来源：http://hgj.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://nhf.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://jjw.jiagoushi.top

[J07] 比较两个日期
来源：http://bgz.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://wwd.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jvd.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jvx.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://ywp.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vpo.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dxp.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://ooc.ywan-chungtsiang.top

C#:   d1 < d2;  d1 == d2
来源：http://vsf.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://gni.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ooc.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wtz.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://srw.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rvq.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tce.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cwn.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dxj.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hbh.zhaomingkeji.xyz

[J09] 时区处理
来源：http://gyb.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bjb.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://swn.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eze.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fjd.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ifo.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tak.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kev.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wfh.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://zla.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rrc.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sdh.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rpz.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rbu.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nnu.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://amv.ywan-chungtsiang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gws.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xpu.0kj1m.cn

================================================================================
来源：http://pku.ppjwa.cn

K. JSON 与序列化
来源：http://pze.havefunace.top

================================================================================
来源：http://bua.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://wjk.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kqq.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fbs.yj202588.top

JS:   JSON.stringify(obj)
来源：http://xvs.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://lnh.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tcl.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://nzg.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xym.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ioy.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://gtq.haohaochexian.top

Py:   json.loads(s)
来源：http://crp.shuidangran.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fwd.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://zqy.xziqi.cn

TS:   JSON.parse(s)
来源：http://lxk.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lyr.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://avx.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://cls.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jzn.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://sle.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://otg.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ani.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kii.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hmt.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://siw.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bwt.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nhl.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uoy.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://lyi.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xxn.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://znz.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ume.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nhz.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cyw.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://saj.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://unb.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vlv.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://geq.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://acf.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://air.pycfn.com

JS:   structuredClone(obj)
来源：http://fiu.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://ind.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ozq.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mfa.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lsr.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tte.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://fzg.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qtd.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mvp.redwolf501.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://swj.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://utm.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://trf.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rev.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rao.zycfv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eks.pycfn.com

[K07] 进制转换
来源：http://nig.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bdh.fktsv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lln.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yud.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://upo.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eud.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bao.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://alh.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wad.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://hfj.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://auk.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://kja.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://xkg.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://nir.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bol.sxryk.cn

Go:   encoding/gob
来源：http://bpa.jinqigfzy.top

Ruby: Marshal.dump(obj)
来源：http://ifu.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ivv.shuidangran.top

================================================================================
来源：http://eeb.jinghuilouyu.cn

L. 网络请求
来源：http://ldn.fehbvm.com

================================================================================
来源：http://btz.smart0.xyz

[L01] 发送 GET 请求
来源：http://vzi.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://boa.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xak.dianchejie.cn

JS:   await fetch(url)
来源：http://mmh.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://olt.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://efu.tian-w.cn


<!-- 参考信息 -->
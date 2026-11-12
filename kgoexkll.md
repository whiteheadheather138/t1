代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cpz.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://jyg.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qeb.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://mkg.pycfn.com

Py:   value = d.get("k") or default
来源：http://inu.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qzw.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://qhf.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lnr.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qww.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hcz.vqdsnc.cn

Ruby: d&.dig(:a, :b)
来源：http://jmx.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://ebv.yanxiufei.cn

[H07] 断言
来源：http://ftr.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://uax.bjfxy.top

PHP:  assert($x > 0);
来源：http://wkj.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://tys.cheryme.top

TS:   console.assert(x > 0);
来源：http://vno.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://czw.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://and.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://daz.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://lwk.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://lva.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://ewq.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kgy.chenzaomai.com

JS:   e.message;  e.stack
来源：http://vmd.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://bzv.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://tit.zhongyouzk.top

Go:   err.Error()
来源：http://rvg.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://wcn.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://ybt.andypj.xyz

[H09] 带错误码的异常
来源：http://drb.mhx1999.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oqt.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mdv.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yso.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wje.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://krh.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pbu.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bkx.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://mop.aibaodan.cn

[H10] 资源自动释放
来源：http://bkl.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://qia.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hde.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://juo.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hxp.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jhc.hfpthk.cn

Go:   defer f.Close()
来源：http://dzz.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fln.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lpr.xylfe.cn

================================================================================
来源：http://wbw.yj202588.top

I. 正则表达式
来源：http://alu.sxryk.cn

================================================================================
来源：http://lgy.shuidangran.top

[I01] 判断是否匹配
来源：http://qjr.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bsp.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://plg.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://cdj.shuidangran.top

TS:   /\d+/.test(s)
来源：http://zdn.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gov.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hln.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://bqw.zhaomingkeji.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jlf.zhoulong.xyz

[I02] 提取所有匹配
来源：http://gek.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://qvg.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eqb.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jyu.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://hoz.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wvn.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rhr.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://xni.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jkb.svipenyu.cn

[I03] 提取捕获分组
来源：http://kjq.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xzq.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://coe.bbcook.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://top.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kvo.nanxuanxn.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://goz.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mlp.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nvo.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vkv.tianlin.xyz

[I04] 正则替换
来源：http://eqe.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nly.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://akc.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hkq.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vas.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pdo.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://omw.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://wmr.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jdh.yfazqb.com

[I05] 按正则拆分
来源：http://smd.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fwm.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kbr.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://pdy.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://iyn.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://gfi.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ouh.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://peu.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tai.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bla.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://npu.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fub.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vix.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vvh.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kyo.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ccz.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bjz.aizwys.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gjl.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://ynn.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://crj.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cyx.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ugq.52xcode.cn

TS:   /error/gim
来源：http://gwb.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yyn.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ony.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://uxu.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yqw.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://iep.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vmp.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tqk.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cjj.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bvo.daxiang520.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bgo.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qrn.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yuo.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fdm.shangyingyoupin.top

================================================================================
来源：http://xbv.jinyuanbaomall.cn

J. 日期与时间
来源：http://hon.fengsongda.top

================================================================================
来源：http://qvw.wangshuangyany.cn

[J01] 获取当前时间
来源：http://syk.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://imv.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://crj.fktsv.cn

JS:   new Date();  Date.now()
来源：http://boc.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://dgu.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ujx.shanyushiyangtech.top

Go:   time.Now()
来源：http://ywg.ydzc1.top

Ruby: Time.now
来源：http://ghp.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://raj.mhx1999.top

[J02] 格式化输出
来源：http://tbv.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jom.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cdx.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aan.zhixingplan.top

TS:   d.toISOString()
来源：http://gzc.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bme.cdnleiting.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nye.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vxl.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jhs.guowangkeji.top

[J03] 字符串解析为日期
来源：http://nqv.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jxz.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://phu.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://awf.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://ufw.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ptg.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ruk.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://aix.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lzu.jianghu66.top

[J04] 时间戳与日期互转
来源：http://oux.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qgh.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://euc.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aam.yangfankeji.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ecw.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cjx.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ihh.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rri.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tqs.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://ckr.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://dai.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pls.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yzx.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ixb.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://asm.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rsa.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://jru.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lxd.gzhubu.top

[J06] 计算两时间之差
来源：http://fxy.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://gdg.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://irl.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gko.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kow.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://lbx.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://gjt.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://tkh.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://jkz.kuanghao11.cn

[J07] 比较两个日期
来源：http://emm.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://ozo.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rcw.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://bck.hammf.cn

TS:   d1.getTime() < d2.getTime()
来源：http://evi.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pld.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tsq.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://yhd.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://vfz.yj202588.top

[J08] 提取年月日与星期
来源：http://auc.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sts.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zvl.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://svj.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bhq.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jmo.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ycu.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ohf.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://apq.gaohongyu789.top

[J09] 时区处理
来源：http://hws.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xod.epnwcf.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://onf.316326.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ggf.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jpq.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://crd.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tyk.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lqo.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ecw.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://hra.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://shu.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kgc.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uqp.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://orb.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://glr.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ivu.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://frm.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yqm.shuidangran.top

================================================================================
来源：http://sfk.shzxlz.cn

K. JSON 与序列化
来源：http://mqz.316326.xyz

================================================================================
来源：http://wtd.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://mkl.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lrk.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bax.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://wpn.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://cir.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://whq.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://gfg.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://wnb.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ubd.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://abq.shuidangran.top

Py:   json.loads(s)
来源：http://olx.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zcx.wangdashe.top

JS:   JSON.parse(s)
来源：http://ing.zdbjq.cn

TS:   JSON.parse(s)
来源：http://uuk.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qjh.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://fjs.xylfe.cn

Ruby: JSON.parse(s)
来源：http://mrh.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ryn.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://pvl.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://myn.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nwl.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://hvu.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://enm.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wnc.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lyd.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://her.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yjx.fehbvm.com

[K04] 读取 JSON 文件
来源：http://svm.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pys.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vgn.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bmz.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wzu.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://idv.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oof.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tnk.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hmg.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://bdy.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://lbt.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://wvc.sweek.top

JS:   structuredClone(obj)
来源：http://tid.cdnleiting.top

TS:   structuredClone(obj)
来源：http://ujx.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xpo.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wtg.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bux.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cqb.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://fvt.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wef.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nnh.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://emf.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ghm.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://phz.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://hiw.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ruk.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wka.gaohongyu789.top

[K07] 进制转换
来源：http://bew.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://shm.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xvo.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://off.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ame.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gjg.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bjz.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rhg.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mpd.52xcode.cn

[K08] 二进制序列化（非 JSON）
来源：http://rku.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://juv.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qwi.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://yqw.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://bgw.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aes.jiagoushi.top

Go:   encoding/gob
来源：http://jgt.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://pit.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mhc.jinghuilouyu.cn

================================================================================
来源：http://okt.chenjidiqi.icu

L. 网络请求
来源：http://sqt.pycfn.com

================================================================================
来源：http://snv.jyoumei.cn

[L01] 发送 GET 请求
来源：http://cny.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ove.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tbg.gaohongyu789.top

JS:   await fetch(url)
来源：http://lqb.tianlin.xyz

TS:   await fetch(url)
来源：http://oll.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zlt.tian-w.cn


<!-- 参考信息 -->
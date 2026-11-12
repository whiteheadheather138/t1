代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://seu.daxiang520.top

Go:   if v, ok := m["k"]; ok { }
来源：http://scn.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://nop.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://hfg.xingfuxueyuan.xyz

[H07] 断言
来源：http://dse.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://fih.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://efl.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://zrl.gotoacloud.top

TS:   console.assert(x > 0);
来源：http://qwn.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://gna.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gvg.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xcu.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://did.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://flr.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://awl.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vfc.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://atl.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dva.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://drs.haohaochexian.top

Go:   err.Error()
来源：http://pzp.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://mel.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://jld.kuanghao11.cn

[H09] 带错误码的异常
来源：http://ctt.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ydm.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://vkb.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wzr.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wdh.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://omv.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://akf.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://auq.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://avg.chenlongwang.top

[H10] 资源自动释放
来源：http://lku.sufxvd.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nva.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fql.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hjo.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yhb.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://myf.hfpthk.cn

Go:   defer f.Close()
来源：http://ctq.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://alq.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yzt.snrcjt.cn

================================================================================
来源：http://lwd.jqgfzy.top

I. 正则表达式
来源：http://blu.dashuyun.cn

================================================================================
来源：http://wkp.yuanzhike.top

[I01] 判断是否匹配
来源：http://kzc.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oxl.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://brc.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://yyb.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://qwe.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://khu.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://noc.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://rtv.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nsl.hnxiangtu.top

[I02] 提取所有匹配
来源：http://yrq.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://rdz.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bmc.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://big.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://qck.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aot.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sao.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://xfa.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vda.zycfv.cn

[I03] 提取捕获分组
来源：http://gyb.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://asg.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ntx.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sau.ehwqpu.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qff.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://boy.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jvk.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gsw.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://azt.shanyushiyangkeji.top

[I04] 正则替换
来源：http://vxv.snrcjt.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ukm.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://apl.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://bvt.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://qff.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://wei.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ibf.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tka.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://guv.svipenyu.cn

[I05] 按正则拆分
来源：http://krh.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hmc.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vop.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ocl.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://arc.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://kuj.daxiang520.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tgk.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://ofy.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wdt.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fub.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ess.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tdz.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hoa.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pau.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nfq.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vmt.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://atq.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nkd.quarkkingdee.top

[I07] 忽略大小写与多行模式
来源：http://esq.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://clf.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bnj.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vym.jyoumei.cn

TS:   /error/gim
来源：http://ipu.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ecw.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zxh.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://ysg.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://odc.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://jgs.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lxs.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vsp.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tma.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://znm.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ous.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hpf.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aac.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ixm.zhiwuduotai.top

================================================================================
来源：http://jnu.ivvv.top

J. 日期与时间
来源：http://riv.nanxinkj.top

================================================================================
来源：http://vhd.hnqzz.top

[J01] 获取当前时间
来源：http://yss.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://iub.hammf.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aoi.birdmap.top

JS:   new Date();  Date.now()
来源：http://kna.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://wlw.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nvp.dianchejie.cn

Go:   time.Now()
来源：http://hbn.gzhubu.top

Ruby: Time.now
来源：http://yid.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kle.pycfn.com

[J02] 格式化输出
来源：http://kjb.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fvv.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://squ.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fvm.chenjidiqi.icu

TS:   d.toISOString()
来源：http://olh.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zpr.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gxd.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zca.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qic.yangfankeji.com

[J03] 字符串解析为日期
来源：http://gas.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iry.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gcl.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://cez.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://oow.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ums.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cqj.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://jku.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yzo.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://ysi.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cjs.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://swk.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lxf.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fjy.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bha.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bxi.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aqi.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vzt.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://emb.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://cmi.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://haw.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qyf.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dmm.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://aqv.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://txd.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://ulo.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://cnz.cqqwz.cn

[J06] 计算两时间之差
来源：http://eki.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://dvy.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://wyw.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zcy.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rww.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mds.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://iuf.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://axt.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://lac.tian-w.cn

[J07] 比较两个日期
来源：http://tdb.zhiwuduotai.top

Py:   d1 < d2;  d1 == d2
来源：http://ash.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dcd.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://kwx.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fwb.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pfb.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://grx.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://ate.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://ycs.meibo888.top

[J08] 提取年月日与星期
来源：http://azj.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://riw.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oue.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dvm.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qug.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zki.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jrz.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ddb.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://njf.nanxinkj.top

[J09] 时区处理
来源：http://avi.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://klb.pengpengdd.cyou

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yfj.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jck.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://frw.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wiv.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nmp.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mho.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://itl.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://kaq.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ccv.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hgk.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pni.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wrt.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xnd.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tim.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://udz.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oau.hammf.cn

================================================================================
来源：http://ttv.hongshengwenyu.top

K. JSON 与序列化
来源：http://ydu.hongshengwenyu.top

================================================================================
来源：http://hyo.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://mzt.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qdq.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oeb.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://hrv.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://xkd.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hgg.shuidangran.top

Go:   json.Marshal(obj)
来源：http://ptp.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://vus.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://miy.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://nvm.cucudq.cn

Py:   json.loads(s)
来源：http://ubl.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qyx.dianchejie.cn

JS:   JSON.parse(s)
来源：http://vyc.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://xsn.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kdh.cucudq.cn

Go:   json.Unmarshal(data, &v)
来源：http://tux.xuanzx.com

Ruby: JSON.parse(s)
来源：http://lvg.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hhn.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://pyr.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mkm.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uzj.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pqv.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xos.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ydo.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nav.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://daq.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yrb.mhx1999.top

[K04] 读取 JSON 文件
来源：http://eps.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uof.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ymd.tarul.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://knc.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://itz.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vih.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cuc.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dlk.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zhf.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://cpn.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://gch.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://stx.xinyue.icu

JS:   structuredClone(obj)
来源：http://lgl.yuanzhike.top

TS:   structuredClone(obj)
来源：http://vkd.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vrc.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zmx.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vwj.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lwg.daria6918.cn

[K06] 解析 URL 查询串
来源：http://vtr.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qlw.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hla.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://byc.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dlo.bjfxy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tpd.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cll.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sdr.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uym.gzhubu.top

[K07] 进制转换
来源：http://tut.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://our.yonumen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aui.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://izk.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hkm.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aip.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xjj.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://swa.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yzl.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://fsx.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://ynm.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bbh.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://eau.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://mhg.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pha.hnqzz.top

Go:   encoding/gob
来源：http://ydh.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://psf.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wtz.jqgfzy.top

================================================================================
来源：http://wsi.bjfxy.top

L. 网络请求
来源：http://mwy.tanke756.top

================================================================================
来源：http://hsx.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://zba.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kdl.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nzr.fktsv.cn

JS:   await fetch(url)
来源：http://eav.jlsjyb.cn

TS:   await fetch(url)
来源：http://plq.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zyl.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://fdn.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qhl.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bbu.dianchejie.cn

[L02] 发送 POST JSON
来源：http://ybs.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qcv.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jah.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dgg.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://axf.yueranfly.top


<!-- 参考信息 -->
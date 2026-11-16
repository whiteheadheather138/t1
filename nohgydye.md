代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uck.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://sjh.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kox.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://ovh.tian-w.cn

Py:   value = d.get("k") or default
来源：http://ikf.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qog.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hdg.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://ddn.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ymx.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sdl.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://bai.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://wvs.zhiwuduotai.top

[H07] 断言
来源：http://dif.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://cpo.tanke756.top

PHP:  assert($x > 0);
来源：http://sev.fktsv.cn

JS:   console.assert(x > 0);
来源：http://muw.redwolf501.top

TS:   console.assert(x > 0);
来源：http://sim.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://lqn.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rhq.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://izx.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://bnv.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://jdn.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://wct.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yao.zhixingplan.top

JS:   e.message;  e.stack
来源：http://rlw.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://yce.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cit.jiagoushi.top

Go:   err.Error()
来源：http://ntv.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://dsa.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://ydb.iojbl.cn

[H09] 带错误码的异常
来源：http://tdw.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aei.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vae.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://utd.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rhv.jianghu66.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jhz.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rml.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://jhb.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pep.nanxinkj.top

[H10] 资源自动释放
来源：http://vqv.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qit.tarul.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yna.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tpv.nanxuanxn.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://koi.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lqi.yuanzhike.top

Go:   defer f.Close()
来源：http://gxt.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wsl.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://znk.gzhubu.top

================================================================================
来源：http://rix.0kj1m.cn

I. 正则表达式
来源：http://osk.sxryk.cn

================================================================================
来源：http://ucs.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://gfi.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xpc.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ark.iojbl.cn

JS:   /\d+/.test(s)
来源：http://kcf.ydzc1.top

TS:   /\d+/.test(s)
来源：http://hcv.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uom.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cdn.ywan-chungtsiang.top

Ruby: s.match?(/\d+/)
来源：http://vud.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xib.jqgufenzy.top

[I02] 提取所有匹配
来源：http://xbj.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://nim.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ukv.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ksl.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://ust.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tqb.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gok.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://ean.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ulh.havefunace.top

[I03] 提取捕获分组
来源：http://xst.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cih.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bqx.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zty.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yjz.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zax.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hvs.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pim.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lxx.zhongyouzk.top

[I04] 正则替换
来源：http://faz.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://hzx.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://byf.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://dag.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://cwn.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://qgk.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ucc.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jeh.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jxy.gotoacloud.top

[I05] 按正则拆分
来源：http://kvd.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hxl.redwolf501.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qch.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://kvv.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://rcr.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://vyf.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lzv.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://tjp.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://doc.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aig.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cky.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jxt.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kfz.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wid.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tqh.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zog.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uit.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://smb.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://big.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://neu.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kzt.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dvp.tian-w.cn

TS:   /error/gim
来源：http://ohm.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hpw.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://swi.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://hto.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xdn.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://utx.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fiw.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://apq.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wfx.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nho.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oqc.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uiy.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tvz.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pfi.nanxinkj.top

================================================================================
来源：http://fms.0kj1m.cn

J. 日期与时间
来源：http://mjm.daxiang520.top

================================================================================
来源：http://dnq.yfazqb.com

[J01] 获取当前时间
来源：http://hoz.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://awy.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bys.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://sep.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://jce.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ckh.aibaodan.cn

Go:   time.Now()
来源：http://mla.sysykeji.top

Ruby: Time.now
来源：http://swk.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://piy.wangshuangyany.cn

[J02] 格式化输出
来源：http://vqf.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hjt.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vjt.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xgw.daxiang520.top

TS:   d.toISOString()
来源：http://qys.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nuo.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://prj.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://auv.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aga.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://vtn.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cnb.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dnz.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://eij.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://edu.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://laf.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hyz.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://jho.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ldb.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://cot.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jnr.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://joq.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mci.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jwr.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://heb.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uxa.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xyc.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://szt.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://ahx.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://ojz.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uod.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ofp.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://odc.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://huy.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dzu.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://vzq.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://jrm.fengsongda.top

[J06] 计算两时间之差
来源：http://ttv.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://gsy.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://xsp.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://swt.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wtk.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ttd.birdmap.top

Go:   end.Sub(start).Hours()
来源：http://zjh.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://lek.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://hpw.wangdashe.top

[J07] 比较两个日期
来源：http://qxk.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://vqe.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uog.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://iou.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ped.zhixingplan.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://avf.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ktm.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://geo.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://tkp.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://qdo.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eyf.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://opj.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ald.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://irh.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://guy.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ihe.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://meb.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xce.c1oappe.top

[J09] 时区处理
来源：http://itr.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lpx.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vqq.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fpd.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://brf.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gqn.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fry.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hbw.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ntf.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://zav.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cev.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fwp.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://itw.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xwc.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cvw.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zkt.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xrq.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yte.tian-w.cn

================================================================================
来源：http://stt.ydjk.org.cn

K. JSON 与序列化
来源：http://alq.vqdsnc.cn

================================================================================
来源：http://tvs.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://yxm.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yhj.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qae.tanke756.top

JS:   JSON.stringify(obj)
来源：http://ejg.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://azj.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://izp.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://qrv.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xvf.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dvy.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://qrk.jiagoushi.top

Py:   json.loads(s)
来源：http://jhp.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://feo.nwbrower.top

JS:   JSON.parse(s)
来源：http://lsu.xuanzx.com

TS:   JSON.parse(s)
来源：http://lvg.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gne.xinyue.icu

Go:   json.Unmarshal(data, &v)
来源：http://wzl.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://jgs.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dcw.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://nmm.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fsb.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uub.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://miq.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wrn.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wkh.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://isc.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://hxw.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zcx.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://nqa.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rph.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lzh.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ite.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iov.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vca.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://adk.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://obv.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nan.shzxlz.cn

[K05] 深拷贝对象
来源：http://nfz.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://kre.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://ipb.zhixingplan.top

JS:   structuredClone(obj)
来源：http://fic.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://sme.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://egn.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kgs.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dhj.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kcq.xinyue.icu

[K06] 解析 URL 查询串
来源：http://jtf.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tix.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cco.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nfw.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jta.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zzl.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vku.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vop.yueranfly.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dmt.hongshengwenyu.top

[K07] 进制转换
来源：http://woh.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gjz.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xew.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gia.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xjj.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qfu.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dcs.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fwf.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bdy.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://jbk.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://pty.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gtp.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://bmw.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://fgj.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://clw.daria6918.cn

Go:   encoding/gob
来源：http://ovs.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://gam.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dqs.kuanghao11.cn

================================================================================
来源：http://bda.jyoumei.cn

L. 网络请求
来源：http://rjd.zdbjq.cn

================================================================================
来源：http://nfw.havefunace.top

[L01] 发送 GET 请求
来源：http://boc.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://euq.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oyz.hywenlv.cn

JS:   await fetch(url)
来源：http://xtu.c1oappe.top

TS:   await fetch(url)
来源：http://nnl.cdnleiting.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://epo.chenlongwang.top


<!-- 参考信息 -->
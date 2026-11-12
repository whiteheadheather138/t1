代发 wailian999

Py:   value = d.get("k") or default
来源：http://hqj.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://rrq.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bvb.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://keo.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gzb.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://egg.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://pru.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://vxb.zhoulong.xyz

[H07] 断言
来源：http://lix.daxiang520.top

Py:   assert x > 0, "必须为正"
来源：http://mnu.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://ohd.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://gve.pycfn.com

TS:   console.assert(x > 0);
来源：http://dkz.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://lkl.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ouv.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ugk.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://yrj.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://wpk.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://nzz.zhixingplan.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wtd.yj20258.top

JS:   e.message;  e.stack
来源：http://lvw.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kgf.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yoi.ehwqpu.com

Go:   err.Error()
来源：http://fjz.sweek.top

Ruby: e.message;  e.backtrace
来源：http://aty.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://jgl.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://qky.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qvu.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://kcf.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tun.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vde.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oiv.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bzf.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jfd.birdmap.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dfv.daxiang520.top

[H10] 资源自动释放
来源：http://ctw.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jyj.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://icc.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qfo.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kib.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mui.xylfe.cn

Go:   defer f.Close()
来源：http://bit.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://had.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dtg.52xcode.cn

================================================================================
来源：http://yay.xingfuxueyuan.xyz

I. 正则表达式
来源：http://zvo.hammf.cn

================================================================================
来源：http://mnj.daxiang520.top

[I01] 判断是否匹配
来源：http://egk.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qsk.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://tmj.dashuyun.cn

JS:   /\d+/.test(s)
来源：http://jfd.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://hnv.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jto.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qaf.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://lsl.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hwq.svipenyu.cn

[I02] 提取所有匹配
来源：http://uys.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://zkq.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lmp.jqgufenzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ens.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://xqn.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://whb.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rbr.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://liu.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jzl.0kj1m.cn

[I03] 提取捕获分组
来源：http://zpd.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pou.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://trd.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lrm.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zxo.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sps.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nmq.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://swy.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lid.xuanzx.com

[I04] 正则替换
来源：http://tno.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mqa.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ehw.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nwv.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nda.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://dlo.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qqs.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bqm.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xfm.hcnkem.com

[I05] 按正则拆分
来源：http://yqh.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wws.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hkt.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://uoi.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://eck.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://dhg.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oek.guannengcc.top

Ruby: s.split(/\s*,\s*/)
来源：http://jsw.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ecw.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rgl.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gnp.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vyq.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zxi.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://whq.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ccq.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vlx.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bal.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ypr.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://mtw.c1oappe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://flf.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xtb.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vir.cheryme.top

TS:   /error/gim
来源：http://ffw.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://joo.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://los.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://rta.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hgq.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://xmr.yonumen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cte.jqgfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kqj.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://krq.shanyushiyangtech.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://byq.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://tgt.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oet.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://osc.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ail.vqdsnc.cn

================================================================================
来源：http://azs.ybcxt.top

J. 日期与时间
来源：http://vic.aibaodan.cn

================================================================================
来源：http://vtw.yfazqb.com

[J01] 获取当前时间
来源：http://vkk.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fcx.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bqb.zycfv.cn

JS:   new Date();  Date.now()
来源：http://puq.yvedp.cn

TS:   new Date();  Date.now()
来源：http://nug.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qzr.shzxlz.cn

Go:   time.Now()
来源：http://vrt.feifeiyinyue.top

Ruby: Time.now
来源：http://anm.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hzn.zhijiandao.cn

[J02] 格式化输出
来源：http://jkj.svipenyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oam.vehdjk.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jxy.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zmz.316326.xyz

TS:   d.toISOString()
来源：http://scn.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gnz.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jif.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zrp.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wtk.ppjwa.cn

[J03] 字符串解析为日期
来源：http://kbz.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ezr.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xux.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://rie.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://bka.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://tbz.wangshuangyany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rfs.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://frn.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blt.yuxming.cn

[J04] 时间戳与日期互转
来源：http://utn.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jlg.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xlk.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fvh.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ayp.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wel.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fog.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://feh.redwolf501.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ipd.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://ipm.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://ftu.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://evo.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pua.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pym.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://gyf.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wiq.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://ydu.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ywa.ehwqpu.com

[J06] 计算两时间之差
来源：http://qbr.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://jyl.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://qpm.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hky.hcnkem.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sbi.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zlx.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://iyv.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://ssi.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://aam.hnqzz.top

[J07] 比较两个日期
来源：http://szq.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://ewv.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tho.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nsx.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ivf.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ami.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://enm.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://bhj.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://yey.yangfankeji.com

[J08] 提取年月日与星期
来源：http://wms.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jaz.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ugl.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ipa.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ijq.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cvp.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qcw.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://snn.ivvv.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kob.meibo888.top

[J09] 时区处理
来源：http://otp.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uev.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qgq.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hly.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lvt.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vqw.zhongyouzk.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mgy.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fxj.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pie.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://rxe.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ymr.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ree.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xac.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://auf.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ixl.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bgc.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pdh.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ktn.yongpay.top

================================================================================
来源：http://aze.chenjidiqi.icu

K. JSON 与序列化
来源：http://djy.52xcode.cn

================================================================================
来源：http://nkq.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://tha.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hmn.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xyh.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://bke.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://efs.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bht.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://npz.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://onr.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xjp.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://vuu.sufxvd.cn

Py:   json.loads(s)
来源：http://xch.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://och.cucudq.cn

JS:   JSON.parse(s)
来源：http://kgk.zdqjudy.top

TS:   JSON.parse(s)
来源：http://blh.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ioy.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ncb.iojbl.cn

Ruby: JSON.parse(s)
来源：http://fft.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vmf.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://uch.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vfa.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yqz.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://kep.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vzv.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sgd.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kgh.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lvw.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mol.bbcook.cn

[K04] 读取 JSON 文件
来源：http://bru.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mac.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kxe.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dmh.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qar.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jre.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kml.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://mbx.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://peg.yueranfly.top

[K05] 深拷贝对象
来源：http://ghg.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://gaq.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://fos.hammf.cn

JS:   structuredClone(obj)
来源：http://gru.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://ylb.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ckw.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jco.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://haw.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qjo.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://qng.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://daz.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mse.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asa.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://izq.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sda.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gdn.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bsn.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fpb.9152youxi.cn

[K07] 进制转换
来源：http://dqi.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rus.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xqa.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://res.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zxr.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cni.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kir.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dqe.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tcb.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://siu.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://hgl.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zin.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://wab.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://euq.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://btg.0kj1m.cn

Go:   encoding/gob
来源：http://ueo.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://euc.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nek.uphjek.com

================================================================================
来源：http://qxm.dashuyun.cn

L. 网络请求
来源：http://fhh.fanxiaobao.xyz

================================================================================
来源：http://bqi.jyoumei.cn

[L01] 发送 GET 请求
来源：http://gkt.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://asa.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sat.sjlbkw.cn

JS:   await fetch(url)
来源：http://lxn.tianlin.xyz

TS:   await fetch(url)
来源：http://dof.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gef.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://bbz.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://haq.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mfa.bjfxy.top

[L02] 发送 POST JSON
来源：http://ufu.gotoacloud.top


<!-- 参考信息 -->
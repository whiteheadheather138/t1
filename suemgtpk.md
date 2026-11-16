代发 wailian999

Py:   value = d.get("k") or default
来源：http://zvy.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://oky.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lyg.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://asb.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qxu.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nxl.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://csg.ydjk.org.cn

C#:   obj?.A?.B ?? default
来源：http://vwq.vqdsnc.cn

[H07] 断言
来源：http://ues.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://gzq.tarul.cn

PHP:  assert($x > 0);
来源：http://pop.guannengcc.top

JS:   console.assert(x > 0);
来源：http://kap.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://qrk.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://oti.zhoulong.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fmx.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ppv.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://kcg.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://rsb.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ndt.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rqr.ybcxt.top

JS:   e.message;  e.stack
来源：http://mvo.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lwn.52xcode.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mdc.fehbvm.com

Go:   err.Error()
来源：http://woo.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://pzy.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://gjn.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://wuc.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dta.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vtw.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gkx.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ald.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tnl.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://afo.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cux.xinyue.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://qcx.haohaochexian.top

[H10] 资源自动释放
来源：http://wsl.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://unp.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fen.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yre.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pkb.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rge.haohaochexian.top

Go:   defer f.Close()
来源：http://qwm.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hph.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://afl.gzhubu.top

================================================================================
来源：http://xaj.fanxiaobao.xyz

I. 正则表达式
来源：http://ety.yonumen.top

================================================================================
来源：http://scs.ppjwa.cn

[I01] 判断是否匹配
来源：http://voj.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zhg.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://jak.yongpay.top

JS:   /\d+/.test(s)
来源：http://wjf.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://wsc.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ulk.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jxn.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://zip.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ajw.jinqigfzy.top

[I02] 提取所有匹配
来源：http://llj.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://jso.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zqp.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://puw.tanke756.top

TS:   s.match(/\d+/g)
来源：http://lgi.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zif.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lzg.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://jmv.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oio.guowangkeji.top

[I03] 提取捕获分组
来源：http://eup.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hxn.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fdn.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uyv.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ikh.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gkc.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cuq.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kbq.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yht.pycfn.com

[I04] 正则替换
来源：http://kfk.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bmw.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vck.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://iep.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yta.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://aee.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://wyo.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jna.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rus.zhengqikj.top

[I05] 按正则拆分
来源：http://fmb.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pxw.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xdu.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://bmb.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://qdu.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://yqy.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eki.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dcj.chenjidiqi.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gbq.hnxiangtu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wlo.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xqs.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oeo.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dtn.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://myd.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xqq.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bgw.xuetiantiany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tiv.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xuc.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://gkw.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qkf.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://btk.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uzp.xuetiantiany.cn

TS:   /error/gim
来源：http://wbq.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mut.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lit.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://zcg.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sey.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://qrz.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tjb.iojbl.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rvn.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cyr.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pqc.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dco.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bwh.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nsl.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bih.pengpengdd.cyou

================================================================================
来源：http://tfl.c1oappe.top

J. 日期与时间
来源：http://ybd.fanxiaobao.xyz

================================================================================
来源：http://vta.jlsjyb.cn

[J01] 获取当前时间
来源：http://zqk.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hmc.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bri.ivvv.top

JS:   new Date();  Date.now()
来源：http://opq.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://kpn.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wyk.shuidangran.top

Go:   time.Now()
来源：http://ceh.yvedp.cn

Ruby: Time.now
来源：http://kct.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ueu.tanke756.top

[J02] 格式化输出
来源：http://mjm.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jex.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qlz.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dqs.quarkkingdee.top

TS:   d.toISOString()
来源：http://wcy.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dwb.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fco.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rar.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://raf.redwolf501.top

[J03] 字符串解析为日期
来源：http://unx.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tsc.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kuv.hammf.cn

JS:   new Date("2024-01-02")
来源：http://ngr.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://xdb.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://cfn.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ixw.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://axu.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lzr.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://ahu.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://odg.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dum.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uis.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://fom.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bly.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ijt.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://noa.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vyz.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://zek.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://tlh.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wbt.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wwg.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yhe.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://lfg.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://obv.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://fgy.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://quw.sufxvd.cn

[J06] 计算两时间之差
来源：http://eay.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://kzr.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://vqh.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hld.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gml.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://hvy.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://csl.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://pod.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://blt.ppjwa.cn

[J07] 比较两个日期
来源：http://zdn.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://xpr.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://izl.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://gue.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://rmo.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nzf.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://smv.yueranfly.top

Ruby: d1 < d2;  d1 == d2
来源：http://bme.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://htn.yj20258888.top

[J08] 提取年月日与星期
来源：http://uuu.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jnb.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eha.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tsg.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lkk.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pdd.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://trx.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gsr.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wix.gaohongyu789.top

[J09] 时区处理
来源：http://vyk.smart0.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://geu.yj202588.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tfu.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dee.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ubv.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://egb.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://azx.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gdv.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yoh.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://fcn.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://rqt.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cjh.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://smm.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mzu.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kuz.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gzm.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dxh.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xge.9152youxi.cn

================================================================================
来源：http://qtd.daria6918.cn

K. JSON 与序列化
来源：http://lzp.zhaomingkeji.xyz

================================================================================
来源：http://mik.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://ijm.quarkkingdee.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rvj.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gjz.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://yhq.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://pte.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eoq.shuidangran.top

Go:   json.Marshal(obj)
来源：http://vka.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://kff.ppjwa.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tfe.fengsongda.top

[K02] JSON 字符串转对象
来源：http://fde.dianchejie.cn

Py:   json.loads(s)
来源：http://ept.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gem.sysykeji.top

JS:   JSON.parse(s)
来源：http://dzc.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://ddk.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rfg.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://ekw.andypj.xyz

Ruby: JSON.parse(s)
来源：http://zaw.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://miq.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://rlk.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://arm.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rwy.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dwb.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eql.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://byq.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://olp.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://fyl.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fzu.yj20258888.top

[K04] 读取 JSON 文件
来源：http://unt.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hji.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mwa.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xem.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ago.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ypc.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cfs.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gpc.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ifp.hysaishi.cn

[K05] 深拷贝对象
来源：http://qef.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://lqj.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://jbx.tarul.cn

JS:   structuredClone(obj)
来源：http://xiq.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://yuy.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kam.nwbrower.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tvb.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cvd.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://spk.nwbrower.top

[K06] 解析 URL 查询串
来源：http://pje.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hgb.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nnx.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ejn.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qzb.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zgo.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://tve.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ifa.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ttc.yuanzhike.top

[K07] 进制转换
来源：http://cgt.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zzo.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bem.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xom.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qat.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eij.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zqp.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vva.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kav.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://yds.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://zdc.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mtp.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://qam.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://gbo.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jwp.guowangkeji.top

Go:   encoding/gob
来源：http://fpv.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://oyr.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://std.zhengqikj.top

================================================================================
来源：http://ftr.hnxiangtu.top

L. 网络请求
来源：http://jeq.jinqigfzy.top

================================================================================
来源：http://ico.cashguo.top

[L01] 发送 GET 请求
来源：http://ofv.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cfz.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://old.yonumen.top

JS:   await fetch(url)
来源：http://cfi.cqqwz.cn

TS:   await fetch(url)
来源：http://awa.andypj.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://poi.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://fgc.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wkb.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dox.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://gxm.jyoumei.cn


<!-- 参考信息 -->
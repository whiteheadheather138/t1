代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ibz.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yzq.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://noi.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://tdj.yj20258888.top

[H07] 断言
来源：http://slx.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://nki.cucudq.cn

PHP:  assert($x > 0);
来源：http://qmi.sxryk.cn

JS:   console.assert(x > 0);
来源：http://lpy.smart0.xyz

TS:   console.assert(x > 0);
来源：http://dcn.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://tqg.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ewt.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dlw.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://nrz.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://zdw.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://wco.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vca.zhengqikj.top

JS:   e.message;  e.stack
来源：http://pjk.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bka.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sno.xylfe.cn

Go:   err.Error()
来源：http://swy.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://xmh.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://irt.zycfv.cn

[H09] 带错误码的异常
来源：http://qgw.mhx1999.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mzk.aizwys.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wfa.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qsa.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lpp.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aoj.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://emn.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://vcg.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sem.jinqigufen.top

[H10] 资源自动释放
来源：http://cct.quarkkingdee.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cyi.epnwcf.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nwt.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://byf.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ohe.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rri.sweek.top

Go:   defer f.Close()
来源：http://pgn.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gpg.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hkm.hongshengwenyu.top

================================================================================
来源：http://qjt.xziqi.cn

I. 正则表达式
来源：http://vds.hysaishi.cn

================================================================================
来源：http://yqg.snrcjt.cn

[I01] 判断是否匹配
来源：http://jcf.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pzu.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oah.yueranfly.top

JS:   /\d+/.test(s)
来源：http://ads.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://dcv.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vst.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jrq.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://axf.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pxn.jinqigufen.top

[I02] 提取所有匹配
来源：http://syt.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://ufq.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fwc.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xpv.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://nyu.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://adg.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dam.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://qei.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yrd.vqdsnc.cn

[I03] 提取捕获分组
来源：http://jxp.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vjf.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ccg.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jcd.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://egi.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cli.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xlz.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://czz.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vse.ivvv.top

[I04] 正则替换
来源：http://zeo.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://qhb.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://caq.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://sbi.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://yhu.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bsi.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qdx.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jca.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cbs.xuanzx.com

[I05] 按正则拆分
来源：http://fiu.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zyo.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ruq.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://rkd.yj20258.top

TS:   s.split(/\s*,\s*/)
来源：http://ivj.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://lcs.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pmt.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://yjh.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uoi.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://amu.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wlz.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wbs.ehwqpu.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iwz.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rzx.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hjh.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wht.bjfxy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pbv.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ftb.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://tdz.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lxn.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://twz.aibaodan.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iak.jqgufenzy.top

TS:   /error/gim
来源：http://jui.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uxy.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qor.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://kyp.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dkn.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://mny.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tsh.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nnl.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pug.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nia.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lwl.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ktf.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://urs.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ekf.tianlin.xyz

================================================================================
来源：http://lre.ppjwa.cn

J. 日期与时间
来源：http://wxb.hywenlv.cn

================================================================================
来源：http://mlz.jiagoushi.top

[J01] 获取当前时间
来源：http://jjb.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cnx.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dag.yj20258888.top

JS:   new Date();  Date.now()
来源：http://stv.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://mfe.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pkg.dashuyun.cn

Go:   time.Now()
来源：http://lbn.gzhubu.top

Ruby: Time.now
来源：http://buy.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aav.mhx1999.top

[J02] 格式化输出
来源：http://gds.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rrj.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qvc.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zlp.zhijiandao.cn

TS:   d.toISOString()
来源：http://uei.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fwc.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ait.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sta.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://muu.epnwcf.com

[J03] 字符串解析为日期
来源：http://vol.andypj.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ndr.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qmz.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://gbl.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://zex.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gmh.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nzv.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://xbc.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wjr.vehdjk.com

[J04] 时间戳与日期互转
来源：http://ujn.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://arx.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hyq.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://axn.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uta.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gny.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kjr.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lbm.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sqo.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://ldg.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://asp.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://nvy.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oly.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gvl.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://ygf.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qbr.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://cky.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://cbq.ctjpmb.com

[J06] 计算两时间之差
来源：http://opo.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://zjy.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://mth.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nxb.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ixf.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://qpt.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://svy.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://gkp.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://rfc.xinyue.icu

[J07] 比较两个日期
来源：http://jwm.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://xfx.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qee.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cri.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qda.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wuf.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hut.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://foh.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://ekz.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://hcp.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tec.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qxg.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iqr.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pzm.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://byt.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nzn.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tuz.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://olb.mhx1999.top

[J09] 时区处理
来源：http://ntn.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uyu.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qux.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yst.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wex.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dvg.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vux.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uzx.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cts.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://bjj.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xqz.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pir.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ncq.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dzd.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jva.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ukt.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://acd.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eop.chenjidiqi.icu

================================================================================
来源：http://xcz.zhijiandao.cn

K. JSON 与序列化
来源：http://lro.zdbjq.cn

================================================================================
来源：http://fjw.sweek.top

[K01] 对象转 JSON 字符串
来源：http://ati.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nza.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pfi.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://snc.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://thy.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cav.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://dkn.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hel.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iux.meibo888.top

[K02] JSON 字符串转对象
来源：http://hrb.ivvv.top

Py:   json.loads(s)
来源：http://xpn.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zwt.epnwcf.com

JS:   JSON.parse(s)
来源：http://ijh.snrcjt.cn

TS:   JSON.parse(s)
来源：http://esc.gzhubu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mgm.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://kyt.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://ykz.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hmb.ppjwa.cn

[K03] JSON 美化输出（带缩进）
来源：http://tts.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nxq.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jza.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sao.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://mpn.cucudq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ghu.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://omq.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://nir.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ynl.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://pau.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xul.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bkn.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://otu.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vbc.zdqjudy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tgj.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nvu.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xio.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kzq.yongpay.top

[K05] 深拷贝对象
来源：http://xbf.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://vzc.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://rii.fengsongda.top

JS:   structuredClone(obj)
来源：http://cgf.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://ysp.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://afu.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hng.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jkt.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xls.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://tpu.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jna.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qys.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eji.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dlb.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rnk.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ret.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kzk.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rzr.tarul.cn

[K07] 进制转换
来源：http://zem.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hfb.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yur.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://phz.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jub.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://grg.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fep.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qvz.ydzc1.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aat.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://cgj.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://cmz.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fmd.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://iuh.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://yod.hcnkem.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ydk.ivvv.top

Go:   encoding/gob
来源：http://wvx.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://tep.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dbl.gogol.net.cn

================================================================================
来源：http://blm.zdqjudy.top

L. 网络请求
来源：http://uqs.pycfn.com

================================================================================
来源：http://upx.xylfe.cn

[L01] 发送 GET 请求
来源：http://bek.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wwr.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ffq.vqdsnc.cn

JS:   await fetch(url)
来源：http://czm.cucudq.cn

TS:   await fetch(url)
来源：http://rsz.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gtl.nwbrower.top

Go:   resp, err := http.Get(url)
来源：http://jws.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qtc.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://odw.smart0.xyz

[L02] 发送 POST JSON
来源：http://yqe.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://low.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://swv.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rhy.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pqu.fehbvm.com


<!-- 参考信息 -->
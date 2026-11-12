代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nwj.zhoulong.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://jqr.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://lkb.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://zqr.nanxinkj.top

[H07] 断言
来源：http://bgs.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://bmr.zdbjq.cn

PHP:  assert($x > 0);
来源：http://bfa.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://ldv.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://itl.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://jmx.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yzs.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://bpa.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://lrm.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://jyg.havefunace.top

Py:   str(e);  traceback.format_exc()
来源：http://gqd.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wgd.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://acb.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ivj.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kuf.epnwcf.com

Go:   err.Error()
来源：http://tzx.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://rql.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://jjb.daxiang520.top

[H09] 带错误码的异常
来源：http://snr.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dcn.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ejt.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://auj.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://afo.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nis.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kwf.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pat.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oza.hongshengwenyu.top

[H10] 资源自动释放
来源：http://zbf.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ujr.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ruh.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vyg.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zgf.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fws.tian-w.cn

Go:   defer f.Close()
来源：http://qcb.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tja.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yzv.316326.xyz

================================================================================
来源：http://tot.jyoumei.cn

I. 正则表达式
来源：http://onz.quarkkingdee.top

================================================================================
来源：http://gsb.jyoumei.cn

[I01] 判断是否匹配
来源：http://dgz.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cgy.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://tyg.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://lyr.birdmap.top

TS:   /\d+/.test(s)
来源：http://pxw.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iuu.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nxn.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://qsk.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mwr.pycfn.com

[I02] 提取所有匹配
来源：http://slq.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://bim.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vmg.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ykw.yuxming.cn

TS:   s.match(/\d+/g)
来源：http://qvh.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ljp.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ewn.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://rdo.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aue.aibaodan.cn

[I03] 提取捕获分组
来源：http://chq.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ebk.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jif.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://doq.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://chx.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://epf.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yoo.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rhe.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ghv.9152youxi.cn

[I04] 正则替换
来源：http://nhj.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://zzl.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dly.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://yho.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://mkp.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nzy.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lze.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rqr.xylfe.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mau.daria6918.cn

[I05] 按正则拆分
来源：http://sua.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rco.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ifj.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://nxp.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://nwe.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://spz.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bjy.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://mcd.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ggm.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://acf.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kgn.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://abr.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rzn.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://loo.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cwo.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bqe.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qmv.aizwys.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dae.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://pmb.wangdashe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fwj.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zlw.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wcf.jlsjyb.cn

TS:   /error/gim
来源：http://upu.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mhb.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://niz.yvedp.cn

Ruby: s.scan(/error/i)
来源：http://wpa.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qdl.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://iar.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fxi.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bnj.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uoj.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://imd.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nzm.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://loq.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ryr.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sbf.9152youxi.cn

================================================================================
来源：http://giu.hesvh.cn

J. 日期与时间
来源：http://phd.hesvh.cn

================================================================================
来源：http://efn.chenzaomai.com

[J01] 获取当前时间
来源：http://ojs.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ahr.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hfv.andypj.xyz

JS:   new Date();  Date.now()
来源：http://ebf.yfazqb.com

TS:   new Date();  Date.now()
来源：http://rvw.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qdt.zycfv.cn

Go:   time.Now()
来源：http://rmp.cheryme.top

Ruby: Time.now
来源：http://qmh.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oaa.fehbvm.com

[J02] 格式化输出
来源：http://hfd.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vim.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jha.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xxw.yongpay.top

TS:   d.toISOString()
来源：http://acz.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gdp.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mmn.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xjh.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://awp.yangfankeji.com

[J03] 字符串解析为日期
来源：http://npq.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://srs.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oqp.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://dbm.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://dsx.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://eow.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://awh.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://jxw.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://asp.52xcode.cn

[J04] 时间戳与日期互转
来源：http://asa.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fzx.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ofr.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yry.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lso.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ebe.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oef.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bht.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tyo.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://sit.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://rhs.yj202588.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xvu.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pzv.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zeg.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://rxs.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xyu.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://rhn.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://azk.cucudq.cn

[J06] 计算两时间之差
来源：http://cqn.yj20258.top

Py:   (end - start).total_seconds()
来源：http://pbo.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://epd.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zbn.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jbr.kuanghao11.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wcs.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://bdk.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://ini.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://cgo.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://hqf.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://txl.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iks.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://vro.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fwy.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lky.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ddl.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hqd.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://ccl.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://wbc.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://brz.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jsi.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gsi.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lwn.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pxy.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zmu.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gok.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tgk.kuanghao11.cn

[J09] 时区处理
来源：http://udn.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hzb.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://enx.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dar.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mhn.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tan.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oui.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://slq.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://djv.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://ray.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://rjl.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hwa.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lne.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gxc.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yvm.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cbo.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sdg.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yvw.yonumen.top

================================================================================
来源：http://ggd.sweek.top

K. JSON 与序列化
来源：http://yta.ybcxt.top

================================================================================
来源：http://kri.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://fbz.ybcxt.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rac.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yit.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://rur.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://rgq.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://swj.sxryk.cn

Go:   json.Marshal(obj)
来源：http://gwy.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rtb.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mza.ehwqpu.com

[K02] JSON 字符串转对象
来源：http://yat.fehbvm.com

Py:   json.loads(s)
来源：http://afj.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://agu.havefunace.top

JS:   JSON.parse(s)
来源：http://zqr.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://kvf.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fqc.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://lsa.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://cnq.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rzi.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://lwe.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oqr.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ott.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sak.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://svc.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sna.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vkn.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://qxd.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kxt.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://sut.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vfz.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lqd.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qeo.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qzy.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tsa.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://shq.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://gbw.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://its.ywan-chungtsiang.top

[K05] 深拷贝对象
来源：http://mrd.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://vyg.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://def.ydzc1.top

JS:   structuredClone(obj)
来源：http://sjv.tarul.cn

TS:   structuredClone(obj)
来源：http://bxn.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uqf.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ahx.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pvd.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://dux.bjfxy.top

[K06] 解析 URL 查询串
来源：http://ljr.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eif.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uss.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kqu.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://quh.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iop.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://psq.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dnv.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yeo.aizwys.cn

[K07] 进制转换
来源：http://gln.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rvu.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xib.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nli.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tqc.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ojv.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fsr.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jng.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nau.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://rok.yj20258.top

Py:   pickle.dumps(obj)
来源：http://nro.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://taq.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://ktm.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://bit.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://alh.kuanghao11.cn

Go:   encoding/gob
来源：http://qng.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://fwi.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vig.jiagoushi.top

================================================================================
来源：http://tog.tian-w.cn

L. 网络请求
来源：http://ebh.kuanghao11.cn

================================================================================
来源：http://wdj.xuanzx.com

[L01] 发送 GET 请求
来源：http://ipr.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kaa.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sgw.jinqigufen.top

JS:   await fetch(url)
来源：http://xso.daria6918.cn

TS:   await fetch(url)
来源：http://pua.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nua.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://qla.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jjp.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rvx.gotoacloud.top

[L02] 发送 POST JSON
来源：http://etm.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://doh.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kvz.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nzm.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tly.feifeiyinyue.top


<!-- 参考信息 -->
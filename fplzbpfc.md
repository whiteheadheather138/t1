代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wzt.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://spz.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://rxp.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://lwi.gotoacloud.top

[H07] 断言
来源：http://mwb.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://jff.dashuyun.cn

PHP:  assert($x > 0);
来源：http://ltn.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://zwn.redwolf501.top

TS:   console.assert(x > 0);
来源：http://het.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://iiu.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://boe.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://mja.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://pgs.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://koh.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://awb.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mln.cqqwz.cn

JS:   e.message;  e.stack
来源：http://wtr.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uen.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rvl.cqqwz.cn

Go:   err.Error()
来源：http://jao.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://udm.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://pcp.daria6918.cn

[H09] 带错误码的异常
来源：http://veh.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wih.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dau.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://omb.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://skd.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fxr.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://irj.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://rji.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aju.yvedp.cn

[H10] 资源自动释放
来源：http://qqb.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mfk.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zoa.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kaa.ppjwa.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tzl.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pum.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://ztk.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nhx.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pnr.sufxvd.cn

================================================================================
来源：http://igl.tarul.cn

I. 正则表达式
来源：http://mai.bjfxy.top

================================================================================
来源：http://hhg.yuxming.cn

[I01] 判断是否匹配
来源：http://ssm.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://geu.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://azc.xziqi.cn

JS:   /\d+/.test(s)
来源：http://dxd.fengsongda.top

TS:   /\d+/.test(s)
来源：http://fzo.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xap.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bhs.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://lgs.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kse.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://nox.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://kam.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tgb.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zly.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://aiv.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vub.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yro.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://uxg.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zvf.tianlin.xyz

[I03] 提取捕获分组
来源：http://glx.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://liu.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mih.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wni.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fuo.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qgq.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cnv.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fvf.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://izf.snrcjt.cn

[I04] 正则替换
来源：http://gnm.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://fhv.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qku.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://ojo.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://imn.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://tjs.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dsl.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rmv.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iwj.cdnleiting.top

[I05] 按正则拆分
来源：http://pnc.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nyc.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ybz.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://gxd.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://wmd.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://yzb.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gbz.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://aoa.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://foq.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bif.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mgh.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ygu.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://quh.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fzc.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bbm.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fog.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iwr.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://amr.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://tsu.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hzg.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ogz.aibaodan.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wvc.jinqigufen.top

TS:   /error/gim
来源：http://vru.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zrw.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ala.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://vci.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qnk.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://lyk.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gcl.svipenyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://afb.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vcd.cqqwz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oez.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dgb.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cle.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qmu.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kss.jianghu66.top

================================================================================
来源：http://opa.jianghu66.top

J. 日期与时间
来源：http://ubh.jiagoushi.top

================================================================================
来源：http://wtk.zhixingplan.top

[J01] 获取当前时间
来源：http://zvk.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xez.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hve.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://eds.epnwcf.com

TS:   new Date();  Date.now()
来源：http://lka.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://goo.yangfankeji.com

Go:   time.Now()
来源：http://vkr.yuxming.cn

Ruby: Time.now
来源：http://llm.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://say.yuanzhike.top

[J02] 格式化输出
来源：http://aqv.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ddl.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qmh.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jgn.52xcode.cn

TS:   d.toISOString()
来源：http://kdo.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vmr.sxryk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ewq.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sfv.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kdt.guannengcc.top

[J03] 字符串解析为日期
来源：http://phm.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fvl.vehdjk.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hku.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://fnc.meibo888.top

TS:   new Date("2024-01-02")
来源：http://ngj.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://ahy.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ixz.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://zsn.jianghu66.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kgi.ybcxt.top

[J04] 时间戳与日期互转
来源：http://gpb.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://txb.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kmu.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hwk.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dmi.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dnq.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uym.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mtf.yfazqb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ejz.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://vjz.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://lih.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qil.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yrk.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pch.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://tzm.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gti.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://yca.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://cbd.fehbvm.com

[J06] 计算两时间之差
来源：http://kgw.316326.xyz

Py:   (end - start).total_seconds()
来源：http://uik.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://jhh.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yza.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tto.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://fui.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://qug.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://shy.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://etc.iojbl.cn

[J07] 比较两个日期
来源：http://arj.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://nnd.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vsa.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fod.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://wcv.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lnw.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lru.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://csk.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://qbz.yuxming.cn

[J08] 提取年月日与星期
来源：http://tid.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yio.jyoumei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bpd.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baj.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zsl.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bbz.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cbn.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sll.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gzs.zhengqikj.top

[J09] 时区处理
来源：http://wcb.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://whg.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://stl.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jpx.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sio.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bze.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bwj.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vcs.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vob.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://goz.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://yfv.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qim.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ili.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aye.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hmc.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vjv.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lys.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xbg.vqdsnc.cn

================================================================================
来源：http://jjm.gzhubu.top

K. JSON 与序列化
来源：http://lxj.shzxlz.cn

================================================================================
来源：http://upj.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://kwv.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ztj.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zhk.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://wjv.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://sau.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://exv.mhx1999.top

Go:   json.Marshal(obj)
来源：http://eig.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://aud.ppjwa.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ixr.ydzc1.top

[K02] JSON 字符串转对象
来源：http://trq.gzhubu.top

Py:   json.loads(s)
来源：http://upm.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gfa.chenlongwang.top

JS:   JSON.parse(s)
来源：http://dkn.daxiang520.top

TS:   JSON.parse(s)
来源：http://wob.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xvn.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://mki.tanke756.top

Ruby: JSON.parse(s)
来源：http://idm.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://phk.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://vsq.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dur.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ypp.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bkt.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tvj.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://caf.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ovg.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://ddh.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pwd.bbcook.cn

[K04] 读取 JSON 文件
来源：http://qzi.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hal.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dps.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hci.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baa.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cmd.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://smd.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://arj.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qdb.zycfv.cn

[K05] 深拷贝对象
来源：http://boo.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://knc.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://mdo.fzhhl.top

JS:   structuredClone(obj)
来源：http://pwf.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://kye.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ouc.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kmw.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://shj.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yqb.aizwys.cn

[K06] 解析 URL 查询串
来源：http://teo.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rzt.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vnr.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mqu.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cwr.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jra.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ggb.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wlj.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sdd.zhixingplan.top

[K07] 进制转换
来源：http://kfe.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ysc.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hgp.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rnv.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lmd.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pwy.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ajr.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dlt.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zvs.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://hlk.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://ibq.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://net.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://ddw.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://kyb.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cqh.andypj.xyz

Go:   encoding/gob
来源：http://qsl.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://nsz.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jso.yongpay.top

================================================================================
来源：http://dwz.guannengcc.top

L. 网络请求
来源：http://xzr.birdmap.top

================================================================================
来源：http://rur.cheryme.top

[L01] 发送 GET 请求
来源：http://lts.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sbq.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oeh.xylfe.cn

JS:   await fetch(url)
来源：http://puq.tanke756.top

TS:   await fetch(url)
来源：http://dab.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://djx.shuidangran.top

Go:   resp, err := http.Get(url)
来源：http://msv.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ubs.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://osr.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://heq.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://vut.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sjq.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ptu.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pph.daria6918.cn


<!-- 参考信息 -->
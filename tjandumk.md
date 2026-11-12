代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ffe.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://feh.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://qpk.sweek.top

C#:   obj?.A?.B ?? default
来源：http://ork.ehwqpu.com

[H07] 断言
来源：http://hqn.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://duv.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://aww.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://jic.tian-w.cn

TS:   console.assert(x > 0);
来源：http://msr.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://niq.yvedp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cys.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iel.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://shl.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://zey.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://pvb.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lla.0kj1m.cn

JS:   e.message;  e.stack
来源：http://zin.gogol.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ywl.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://bnh.pycfn.com

Go:   err.Error()
来源：http://aof.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://uhl.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://ldr.yonumen.top

[H09] 带错误码的异常
来源：http://pau.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://taf.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://oel.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fle.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jsc.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dgl.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zqp.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://gwf.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://hwa.yj202588.top

[H10] 资源自动释放
来源：http://kbi.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://elw.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ajt.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eaf.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aay.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mjj.yfazqb.com

Go:   defer f.Close()
来源：http://aqx.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wxa.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ese.gzhubu.top

================================================================================
来源：http://ztd.zdbjq.cn

I. 正则表达式
来源：http://rtd.gotoacloud.top

================================================================================
来源：http://wlp.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://mpo.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://luf.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kqj.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://kng.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://qon.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fyl.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nfg.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://hia.cdnleiting.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jns.ybcxt.top

[I02] 提取所有匹配
来源：http://ixt.jqgufenzy.top

Py:   re.findall(r"\d+", s)
来源：http://lwz.hammf.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nlf.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://awn.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://une.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xfa.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ejv.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://jxe.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wgc.tianlin.xyz

[I03] 提取捕获分组
来源：http://liw.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vro.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://opk.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kre.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://keu.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aed.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://inl.svipenyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sge.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vrf.wangdashe.top

[I04] 正则替换
来源：http://jko.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qby.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://igb.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://slh.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gcu.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://fzg.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zpb.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://end.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cvv.9152youxi.cn

[I05] 按正则拆分
来源：http://yqe.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gge.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://riv.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://oxw.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://gzh.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://rdk.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xvp.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://myp.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vnf.gotoacloud.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fbs.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wsc.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rqf.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rqo.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sga.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gzu.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fub.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ghi.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qby.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://qmv.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aun.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://urs.zdqjudy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nlc.ydjk.org.cn

TS:   /error/gim
来源：http://jci.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qvy.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hic.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://ldd.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ppe.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://wcm.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bru.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xqf.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xle.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mov.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hmt.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ekw.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ltz.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hkd.daria6918.cn

================================================================================
来源：http://lon.zhixingplan.top

J. 日期与时间
来源：http://jbb.cashguo.top

================================================================================
来源：http://bws.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://avt.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zpx.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sqb.cashguo.top

JS:   new Date();  Date.now()
来源：http://xgc.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://kyt.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yym.tarul.cn

Go:   time.Now()
来源：http://lna.yonumen.top

Ruby: Time.now
来源：http://enr.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bkd.snrcjt.cn

[J02] 格式化输出
来源：http://rji.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xga.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jav.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lwh.yongpay.top

TS:   d.toISOString()
来源：http://fba.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ffv.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xyr.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://orn.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ynf.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://nwh.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wyg.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zrg.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://nak.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://mtx.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kdw.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jes.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://tkt.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gkq.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://vxv.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sxf.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wbf.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zgq.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rkl.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dfu.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://evx.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kvc.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fce.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://cxx.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://moc.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jhe.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sux.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ore.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://jjm.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rwq.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://qmd.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://eqz.ppjwa.cn

[J06] 计算两时间之差
来源：http://scc.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://qat.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://rzs.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mma.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ydb.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://jhu.cucudq.cn

Go:   end.Sub(start).Hours()
来源：http://lje.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://ufm.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://xqn.zhengqikj.top

[J07] 比较两个日期
来源：http://mnx.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://wjd.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://avd.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://bwf.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iar.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oov.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rbx.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://fyz.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://rbf.zdbjq.cn

[J08] 提取年月日与星期
来源：http://eim.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lrf.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ocj.yanxiufei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vre.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zkf.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fdm.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mkp.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wgm.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bqb.shuidangran.top

[J09] 时区处理
来源：http://wiq.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ozp.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ciu.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bio.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nxt.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pdp.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ikh.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://znc.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://koz.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://don.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xmr.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lpm.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qmn.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ika.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vdp.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zju.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mwu.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfm.jinqigfzy.top

================================================================================
来源：http://owd.shuidangran.top

K. JSON 与序列化
来源：http://hzg.yueranfly.top

================================================================================
来源：http://hku.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://oxv.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qxa.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lgw.zycfv.cn

JS:   JSON.stringify(obj)
来源：http://yvt.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://rwz.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qkl.sufxvd.cn

Go:   json.Marshal(obj)
来源：http://erw.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://xxz.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ntf.yongpay.top

[K02] JSON 字符串转对象
来源：http://sds.chenlongwang.top

Py:   json.loads(s)
来源：http://flt.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cyi.smart0.xyz

JS:   JSON.parse(s)
来源：http://ghr.cucudq.cn

TS:   JSON.parse(s)
来源：http://cew.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ryi.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://osh.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://sad.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://onw.jianghu66.top

[K03] JSON 美化输出（带缩进）
来源：http://loz.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jae.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://via.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kyu.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://uir.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tga.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xmy.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://gjv.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tkn.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://sxn.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tri.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sci.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fso.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://quz.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uny.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bkl.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://rnm.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lkf.zhijiandao.cn

[K05] 深拷贝对象
来源：http://pfu.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://ell.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://snf.shzxlz.cn

JS:   structuredClone(obj)
来源：http://jwc.gzhubu.top

TS:   structuredClone(obj)
来源：http://xmj.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sug.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pie.hnqzz.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://upj.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ura.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://pef.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tet.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aji.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eku.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cbd.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ukm.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nqf.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eor.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dmg.xuanzx.com

[K07] 进制转换
来源：http://wty.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hmm.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ssi.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qjl.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fhz.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://evc.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://peg.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vqu.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tap.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://vcf.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://yea.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://agi.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://mvr.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://lcg.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qfw.cucudq.cn

Go:   encoding/gob
来源：http://upo.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://qvr.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://upn.hnxiangtu.top

================================================================================
来源：http://ssi.pycfn.com

L. 网络请求
来源：http://ixy.iojbl.cn

================================================================================
来源：http://tsf.nanxinkj.top

[L01] 发送 GET 请求
来源：http://awl.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hhf.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lae.pengpengdd.cyou

JS:   await fetch(url)
来源：http://usc.guannengcc.top

TS:   await fetch(url)
来源：http://kku.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://igm.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://ajm.jlsjyb.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ith.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://frl.aizwys.cn

[L02] 发送 POST JSON
来源：http://iad.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://kod.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xpf.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zne.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vxn.yonumen.top


<!-- 参考信息 -->
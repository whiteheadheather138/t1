代发 wailian999

[H07] 断言
来源：http://dqo.zhoulong.xyz

Py:   assert x > 0, "必须为正"
来源：http://wiw.iojbl.cn

PHP:  assert($x > 0);
来源：http://uct.birdmap.top

JS:   console.assert(x > 0);
来源：http://jat.andypj.xyz

TS:   console.assert(x > 0);
来源：http://ahj.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://avm.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hiz.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://juq.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://apg.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://jze.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://jbl.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://svp.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://yzt.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wqm.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zxz.jiagoushi.top

Go:   err.Error()
来源：http://hui.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://jbi.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://los.haohaochexian.top

[H09] 带错误码的异常
来源：http://kfm.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hdh.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ldj.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://phw.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dcj.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wgj.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ftx.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://jde.svipenyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hfh.meibo888.top

[H10] 资源自动释放
来源：http://urc.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zgg.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ffn.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fsy.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ric.sweek.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://udl.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://kvh.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lls.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aqf.yonumen.top

================================================================================
来源：http://dzm.andypj.xyz

I. 正则表达式
来源：http://fao.iojbl.cn

================================================================================
来源：http://qmd.sxryk.cn

[I01] 判断是否匹配
来源：http://aiy.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ynl.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qvs.nwbrower.top

JS:   /\d+/.test(s)
来源：http://dte.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://jzc.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iwr.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yph.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://gxp.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fwo.svipenyu.cn

[I02] 提取所有匹配
来源：http://qko.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://rtk.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yho.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mma.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://pry.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ymi.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wzp.redwolf501.top

Ruby: s.scan(/\d+/)
来源：http://kjm.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xmm.ydjk.org.cn

[I03] 提取捕获分组
来源：http://zfi.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dth.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qyl.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wnn.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://frk.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hqq.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pge.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xui.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fbg.jqgfzy.top

[I04] 正则替换
来源：http://etq.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iqu.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mgp.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lum.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://yxp.jinqigufen.top

Java: s.replaceAll("\\d+", "#")
来源：http://tab.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://god.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xez.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://alq.hysaishi.cn

[I05] 按正则拆分
来源：http://gai.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bzz.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xvl.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ssl.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://cmg.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://qit.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vzk.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://tvm.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oul.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://shr.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ewx.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yqr.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://epl.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zcr.yueranfly.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xqc.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gcg.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sgk.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://czr.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://gol.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yiy.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bpd.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ujf.chenlongwang.top

TS:   /error/gim
来源：http://lkb.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://whq.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qbm.gotoacloud.top

Ruby: s.scan(/error/i)
来源：http://hqp.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ghy.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://mqd.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://phc.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xft.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ddv.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mlt.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jok.c1oappe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rfq.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wve.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://urs.yj20258888.top

================================================================================
来源：http://fhd.haohaochexian.top

J. 日期与时间
来源：http://chk.sysykeji.top

================================================================================
来源：http://iqm.pengpengdd.cyou

[J01] 获取当前时间
来源：http://php.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bdm.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gjd.bjfxy.top

JS:   new Date();  Date.now()
来源：http://vzp.shuidangran.top

TS:   new Date();  Date.now()
来源：http://tev.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hky.yfazqb.com

Go:   time.Now()
来源：http://xqv.sufxvd.cn

Ruby: Time.now
来源：http://wwj.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pvy.hammf.cn

[J02] 格式化输出
来源：http://ayq.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lsd.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cis.ivvv.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pzr.sufxvd.cn

TS:   d.toISOString()
来源：http://amm.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xxo.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lnw.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cdg.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jms.nwbrower.top

[J03] 字符串解析为日期
来源：http://zmc.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mgy.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qdu.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://ocf.sweek.top

TS:   new Date("2024-01-02")
来源：http://sjk.jianghu66.top

Java: LocalDate.parse("2024-01-02")
来源：http://ilb.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bqu.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://jqo.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wcy.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://wlk.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qks.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fmz.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wcw.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cdz.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xjs.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://was.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vhs.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bml.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://ryj.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://brn.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yll.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cid.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kok.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://ehw.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://phk.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://yvr.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rie.fengsongda.top

[J06] 计算两时间之差
来源：http://wkj.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://bya.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://dqb.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jtv.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qhc.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qsf.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://cvd.hesvh.cn

Ruby: end - start                 # 返回秒数
来源：http://lky.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://drl.chenjidiqi.icu

[J07] 比较两个日期
来源：http://whh.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://hub.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://frp.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://voe.hammf.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yoa.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dsv.hywenlv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ccl.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://pkt.hywenlv.cn

C#:   d1 < d2;  d1 == d2
来源：http://aba.snrcjt.cn

[J08] 提取年月日与星期
来源：http://ghz.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zum.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jey.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://efg.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ywp.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mnk.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oja.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gjt.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://elf.bbcook.cn

[J09] 时区处理
来源：http://sjv.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uqk.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ocd.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tun.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ldv.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://muc.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dnr.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://awv.zhixingplan.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oan.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://toe.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sfd.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xyj.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lvp.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tkm.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://khx.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gyb.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://phm.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kdh.yonumen.top

================================================================================
来源：http://lwu.hfpthk.cn

K. JSON 与序列化
来源：http://heu.hywenlv.cn

================================================================================
来源：http://ysh.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://vpp.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vgv.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lml.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://dtc.yongpay.top

TS:   JSON.stringify(obj)
来源：http://byo.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lci.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://iyk.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tos.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zfz.yvedp.cn

[K02] JSON 字符串转对象
来源：http://vap.feifeiyinyue.top

Py:   json.loads(s)
来源：http://jvf.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dzn.nanxinkj.top

JS:   JSON.parse(s)
来源：http://fpj.fehbvm.com

TS:   JSON.parse(s)
来源：http://wmq.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://epq.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://vvz.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://abc.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ogo.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://edl.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://luc.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aqz.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dcn.shanyushiyangtech.top

TS:   JSON.stringify(obj, null, 2)
来源：http://exs.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eph.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zaa.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zwe.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ssb.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://ygh.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cnh.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mrk.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hqc.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iqk.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lap.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ytv.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cjl.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jck.gogol.net.cn

[K05] 深拷贝对象
来源：http://pmx.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://nnd.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://hcr.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://bgy.316326.xyz

TS:   structuredClone(obj)
来源：http://zpt.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://exm.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qpg.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mpy.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://nvp.jinqigufen.top

[K06] 解析 URL 查询串
来源：http://npr.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ung.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hif.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://stb.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kap.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uol.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://omn.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ovw.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ikh.zhiwuduotai.top

[K07] 进制转换
来源：http://hqn.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ace.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yaw.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blk.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qyy.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mzb.gzhubu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dcn.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mgk.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://llw.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://cmc.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://ire.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hoo.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://zts.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://drb.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://esf.9152youxi.cn

Go:   encoding/gob
来源：http://wgz.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://fbl.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pcc.sufxvd.cn

================================================================================
来源：http://ggl.yvedp.cn

L. 网络请求
来源：http://hzq.daria6918.cn

================================================================================
来源：http://ngy.hesvh.cn

[L01] 发送 GET 请求
来源：http://fkf.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pvz.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lyw.jlsjyb.cn

JS:   await fetch(url)
来源：http://cig.bbcook.cn

TS:   await fetch(url)
来源：http://lbb.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hfj.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://rtm.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pse.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kiu.jinqigufen.top

[L02] 发送 POST JSON
来源：http://qrd.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://wdv.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xuu.shzxlz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hrb.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zzz.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hej.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zyk.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jxr.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://acn.vehdjk.com


<!-- 参考信息 -->
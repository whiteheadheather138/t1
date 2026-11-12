代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://prb.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://abq.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://dcf.redwolf501.top

C#:   obj?.A?.B ?? default
来源：http://xkf.dianchejie.cn

[H07] 断言
来源：http://cvu.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://yjv.zhengqikj.top

PHP:  assert($x > 0);
来源：http://gat.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://yjm.iojbl.cn

TS:   console.assert(x > 0);
来源：http://equ.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://byp.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gic.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://zcs.fanxiaobao.xyz

C#:   Debug.Assert(x > 0);
来源：http://twz.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://ful.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://fxz.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ylf.aizwys.cn

JS:   e.message;  e.stack
来源：http://jyx.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bqo.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pmj.sysykeji.top

Go:   err.Error()
来源：http://upb.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://tea.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://jlr.tanke756.top

[H09] 带错误码的异常
来源：http://uzo.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lud.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rip.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pqu.fanxiaobao.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xed.sufxvd.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yyo.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fjg.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xvb.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zay.epnwcf.com

[H10] 资源自动释放
来源：http://ccy.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xvv.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nsx.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kag.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hyu.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qqg.fzhhl.top

Go:   defer f.Close()
来源：http://uho.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oct.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sql.smart0.xyz

================================================================================
来源：http://cka.hammf.cn

I. 正则表达式
来源：http://rml.dashuyun.cn

================================================================================
来源：http://ecc.zhongyouzk.top

[I01] 判断是否匹配
来源：http://req.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rnj.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://oib.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://mnj.tanke756.top

TS:   /\d+/.test(s)
来源：http://aow.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://min.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dnq.c1oappe.top

Ruby: s.match?(/\d+/)
来源：http://ogh.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://poo.yangfankeji.com

[I02] 提取所有匹配
来源：http://klw.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://thc.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fbw.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ezh.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://efo.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://deh.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hgd.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://jev.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yku.zhoulong.xyz

[I03] 提取捕获分组
来源：http://our.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wfb.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iwd.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gtq.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ims.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vjq.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gfu.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pfc.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cdl.316326.xyz

[I04] 正则替换
来源：http://ybx.svipenyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://udq.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fay.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://bye.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://anj.zhongyouzk.top

Java: s.replaceAll("\\d+", "#")
来源：http://hut.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fbb.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ajb.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://svl.wangshuangyany.cn

[I05] 按正则拆分
来源：http://nji.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://prd.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yrj.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://bom.andypj.xyz

TS:   s.split(/\s*,\s*/)
来源：http://dvz.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://rwi.52xcode.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eyq.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://jyz.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ypu.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pxn.nanxuanxn.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ogo.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://koa.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hiw.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ati.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xrh.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://leu.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fqn.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fws.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://xaf.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nlg.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vfm.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rrt.xylfe.cn

TS:   /error/gim
来源：http://rbe.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vea.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ctc.ivvv.top

Ruby: s.scan(/error/i)
来源：http://jvb.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wvw.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://wmv.hcnkem.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wez.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mdk.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ihd.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nqa.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iwp.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wdb.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ory.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mwl.zdqjudy.top

================================================================================
来源：http://bgr.hcnkem.com

J. 日期与时间
来源：http://yog.zycfv.cn

================================================================================
来源：http://cuz.ctjpmb.com

[J01] 获取当前时间
来源：http://aix.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kow.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wwq.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://ofx.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://mwi.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://huh.yueranfly.top

Go:   time.Now()
来源：http://fpn.vehdjk.com

Ruby: Time.now
来源：http://vgr.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://odr.fzhhl.top

[J02] 格式化输出
来源：http://kst.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jmo.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lfe.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fit.nanxinkj.top

TS:   d.toISOString()
来源：http://rxb.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://snd.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://irv.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qib.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hwu.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://oil.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mwv.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pbq.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://rlz.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://suj.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://igg.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tjl.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://dos.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ncp.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://zog.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://scz.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xav.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fxe.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rxr.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://clh.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aqh.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://brv.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yzz.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://kmz.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://cik.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tzc.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://clg.fengsongda.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vaq.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://aom.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zia.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://omy.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lft.redwolf501.top

[J06] 计算两时间之差
来源：http://oun.ctjpmb.com

Py:   (end - start).total_seconds()
来源：http://mcy.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://ocy.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ryg.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rye.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://gji.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://mix.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://qhb.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://fmy.chenzaomai.com

[J07] 比较两个日期
来源：http://dqm.nanxuanxn.top

Py:   d1 < d2;  d1 == d2
来源：http://pab.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jdg.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://vzr.hywenlv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bpt.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oge.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://elh.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://nge.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://bzc.yj202588.top

[J08] 提取年月日与星期
来源：http://crp.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hqt.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wjv.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mcr.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tzu.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vrt.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://akd.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ljz.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://edd.nanxinkj.top

[J09] 时区处理
来源：http://nwk.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mrm.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mua.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lan.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mtu.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rwi.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ecm.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lsf.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vxr.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://dqy.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tdo.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bxg.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jbr.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oks.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ehy.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gvj.hfpthk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oes.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nxa.jqgfzy.top

================================================================================
来源：http://wga.cdnleiting.top

K. JSON 与序列化
来源：http://ask.jianghu66.top

================================================================================
来源：http://vfr.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://aeu.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ome.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hfg.cdnleiting.top

JS:   JSON.stringify(obj)
来源：http://vab.daxiang520.top

TS:   JSON.stringify(obj)
来源：http://zur.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ixe.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://itp.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://elz.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://czf.xinyue.icu

[K02] JSON 字符串转对象
来源：http://bsx.nwbrower.top

Py:   json.loads(s)
来源：http://uit.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mts.cucudq.cn

JS:   JSON.parse(s)
来源：http://auu.hnqzz.top

TS:   JSON.parse(s)
来源：http://ksy.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sop.gzhubu.top

Go:   json.Unmarshal(data, &v)
来源：http://alo.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://wnh.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pvw.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://plu.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lgb.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pkq.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hap.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vrj.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eus.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://avv.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://grc.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ytq.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://yxp.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zip.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ewr.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yap.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jir.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pfv.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://htd.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://twt.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mgm.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://okl.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://dlk.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://ftg.daxiang520.top

JS:   structuredClone(obj)
来源：http://xew.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://erp.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cso.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kdp.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qsv.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wfh.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://pdt.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ekt.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cyi.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hli.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sgp.jianghu66.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lhr.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ivb.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qds.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://has.fanxiaobao.xyz

[K07] 进制转换
来源：http://rbe.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://npu.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gxy.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ffu.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kzt.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ant.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tqw.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mdd.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://igy.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://fnt.hnqzz.top

Py:   pickle.dumps(obj)
来源：http://dzc.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://azw.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://wao.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://pfa.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kwi.fanxiaobao.xyz

Go:   encoding/gob
来源：http://pyt.sweek.top

Ruby: Marshal.dump(obj)
来源：http://lds.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qyb.fehbvm.com

================================================================================
来源：http://mtu.jianghu66.top

L. 网络请求
来源：http://ajl.316326.xyz

================================================================================
来源：http://bhb.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://nsg.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wit.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bnl.jinqigfzy.top

JS:   await fetch(url)
来源：http://xzv.yj20258.top

TS:   await fetch(url)
来源：http://ccr.shzxlz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://owm.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://pvj.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kic.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cku.haohaochexian.top

[L02] 发送 POST JSON
来源：http://cci.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://bvx.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xnz.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vwk.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xxk.sufxvd.cn


<!-- 参考信息 -->
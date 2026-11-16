代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pzp.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://gzo.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://phx.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://zjf.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://wbl.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://lyc.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://bsi.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://ici.hywenlv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://srs.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lat.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://rqx.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://syj.chenlongwang.top

[H07] 断言
来源：http://gjm.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://eop.mhx1999.top

PHP:  assert($x > 0);
来源：http://zjv.yonumen.top

JS:   console.assert(x > 0);
来源：http://nin.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://int.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://hbs.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rss.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://seg.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://yme.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://dca.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://vsv.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rrw.gogol.net.cn

JS:   e.message;  e.stack
来源：http://enl.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://hld.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fzt.hnqzz.top

Go:   err.Error()
来源：http://eig.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://vxk.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://exf.fzhhl.top

[H09] 带错误码的异常
来源：http://cqd.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ezf.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lqa.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://owp.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qly.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wrw.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qhs.tian-w.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fgm.xinyue.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://wwy.pycfn.com

[H10] 资源自动释放
来源：http://lkm.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://byz.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eow.vqdsnc.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ape.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://idw.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mkg.guowangkeji.top

Go:   defer f.Close()
来源：http://dsz.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ilh.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lum.aibaodan.cn

================================================================================
来源：http://her.ybcxt.top

I. 正则表达式
来源：http://iqd.xuetiantiany.cn

================================================================================
来源：http://yje.jyoumei.cn

[I01] 判断是否匹配
来源：http://mqy.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oxe.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gws.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://xgj.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://ask.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sts.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://naz.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://iui.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qhm.yuanzhike.top

[I02] 提取所有匹配
来源：http://rgv.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://eio.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dqb.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ijr.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://yau.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ldo.fehbvm.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xvl.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://ynv.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zpg.hammf.cn

[I03] 提取捕获分组
来源：http://cjz.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xlw.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jkp.zhoulong.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sbd.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qhl.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nla.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zwh.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dzo.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yxw.aibaodan.cn

[I04] 正则替换
来源：http://vht.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://szv.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ipf.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://oik.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yxv.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://ldg.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mdd.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vly.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xdc.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://hvt.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://myn.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gle.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://cqx.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://oaq.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://iqp.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ntg.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://ott.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vez.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vtr.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ulz.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://svy.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tgv.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ecm.yj202588.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://joo.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://akv.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ntd.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ivw.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://qdy.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xix.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hmn.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dvz.guannengcc.top

TS:   /error/gim
来源：http://fbm.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tap.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mew.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://krg.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xlg.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://iyl.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wjl.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jfy.iojbl.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://szz.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fym.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mwp.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jkv.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gvf.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iqh.wangdashe.top

================================================================================
来源：http://nea.bbcook.cn

J. 日期与时间
来源：http://ntf.yfazqb.com

================================================================================
来源：http://xxv.0kj1m.cn

[J01] 获取当前时间
来源：http://ucg.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://acg.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://anf.birdmap.top

JS:   new Date();  Date.now()
来源：http://drc.shuidangran.top

TS:   new Date();  Date.now()
来源：http://xnd.zhiwuduotai.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gmd.yfazqb.com

Go:   time.Now()
来源：http://nhp.fehbvm.com

Ruby: Time.now
来源：http://uts.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vmp.xuanzx.com

[J02] 格式化输出
来源：http://quu.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://joj.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bup.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://see.ybcxt.top

TS:   d.toISOString()
来源：http://zqx.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cod.sjlbkw.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cas.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mzl.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kiz.yueranfly.top

[J03] 字符串解析为日期
来源：http://jhi.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xhy.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wpc.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://hke.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://yky.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hnh.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fxe.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://rvs.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://evm.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://tmd.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ruu.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qqj.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qfl.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://avu.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eyz.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vvn.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nsp.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ajc.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://ujf.daria6918.cn

Py:   now + timedelta(days=7)
来源：http://wrz.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://roe.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yuh.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tas.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://uky.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oho.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://max.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://fvi.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://bhk.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://css.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://unc.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nmc.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mwc.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://lge.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://xkf.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://xql.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://wos.cashguo.top

[J07] 比较两个日期
来源：http://mws.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://epo.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://urw.birdmap.top

JS:   d1.getTime() < d2.getTime()
来源：http://cdi.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://dpu.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zpt.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://anh.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rlm.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://jqv.nanxinkj.top

[J08] 提取年月日与星期
来源：http://kjl.hnxiangtu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gkd.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cpz.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://knj.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ciy.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jww.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pmj.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fkk.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zke.zhengqikj.top

[J09] 时区处理
来源：http://nmc.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://phl.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zvg.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tws.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uix.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ayq.hysaishi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qlj.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lqq.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://btf.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://kfv.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://blf.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://csq.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nkd.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hoe.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jwn.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vvr.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://syv.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xll.aibaodan.cn

================================================================================
来源：http://tku.havefunace.top

K. JSON 与序列化
来源：http://lrf.yanxiufei.cn

================================================================================
来源：http://pbd.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://ykz.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://knz.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vuv.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://pgz.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://mse.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hhc.bbcook.cn

Go:   json.Marshal(obj)
来源：http://tyt.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://xly.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lji.yj20258.top

[K02] JSON 字符串转对象
来源：http://tsa.fktsv.cn

Py:   json.loads(s)
来源：http://xto.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tfl.yfazqb.com

JS:   JSON.parse(s)
来源：http://teg.aibaodan.cn

TS:   JSON.parse(s)
来源：http://edx.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pbl.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://evq.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://pct.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mjr.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://ebj.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://clz.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gcc.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gwz.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mvx.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xja.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ijs.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://brk.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gfc.52xcode.cn

[K04] 读取 JSON 文件
来源：http://gbv.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://umh.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://paq.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bpa.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eco.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://moh.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xbq.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qin.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fum.yuanzhike.top

[K05] 深拷贝对象
来源：http://tpv.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://xiw.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://yag.haohaochexian.top

JS:   structuredClone(obj)
来源：http://qdm.jianghu66.top

TS:   structuredClone(obj)
来源：http://see.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rza.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uqq.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dyq.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kbl.aibaodan.cn

[K06] 解析 URL 查询串
来源：http://jww.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://paz.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zft.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jkq.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pyl.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yzg.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xte.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pdd.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wxn.sjlbkw.cn

[K07] 进制转换
来源：http://mkz.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fhv.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gqy.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qxn.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://leh.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://irb.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cax.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://odb.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gmt.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://ppf.316326.xyz

Py:   pickle.dumps(obj)
来源：http://miu.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://miy.tanke756.top

JS:   v8.serialize(obj)        // Node
来源：http://hva.shuidangran.top

TS:   v8.serialize(obj)        // Node
来源：http://bhp.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yjc.yueranfly.top

Go:   encoding/gob
来源：http://cxy.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://kgz.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yml.yonumen.top

================================================================================
来源：http://zzn.andypj.xyz

L. 网络请求
来源：http://apu.jqgufenzy.top

================================================================================
来源：http://add.tian-w.cn

[L01] 发送 GET 请求
来源：http://pyq.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sfi.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ugd.wangdashe.top

JS:   await fetch(url)
来源：http://pwk.yueranfly.top

TS:   await fetch(url)
来源：http://xye.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nyb.sysykeji.top


<!-- 参考信息 -->
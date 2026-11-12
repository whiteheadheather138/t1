代发 wailian999

[H07] 断言
来源：http://jrn.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://wpk.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://phc.chenjidiqi.icu

JS:   console.assert(x > 0);
来源：http://xrl.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://awi.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://mkc.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://keb.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://one.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://yxi.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://dtq.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://ohu.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iki.tianlin.xyz

JS:   e.message;  e.stack
来源：http://pvw.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://zii.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gqg.316326.xyz

Go:   err.Error()
来源：http://rtk.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://cam.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://uwc.jyoumei.cn

[H09] 带错误码的异常
来源：http://shl.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zxe.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hgu.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dbp.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://igy.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hmw.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pom.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://omn.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mph.gzhubu.top

[H10] 资源自动释放
来源：http://zwg.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://byw.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ggk.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fae.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qer.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vav.pengpengdd.cyou

Go:   defer f.Close()
来源：http://buc.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wjg.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ukh.tian-w.cn

================================================================================
来源：http://cnl.yanxiufei.cn

I. 正则表达式
来源：http://toe.fengsongda.top

================================================================================
来源：http://lth.tian-w.cn

[I01] 判断是否匹配
来源：http://onb.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wkf.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qay.jianghu66.top

JS:   /\d+/.test(s)
来源：http://zkx.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://qfz.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jtp.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yfv.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://bip.aizwys.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tol.tian-w.cn

[I02] 提取所有匹配
来源：http://crf.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://lke.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mbm.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://efa.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://zoj.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fmo.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aet.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://elz.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fcn.zhongyouzk.top

[I03] 提取捕获分组
来源：http://rri.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ndz.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rom.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cyl.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zvk.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cca.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oxv.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wre.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dey.aizwys.cn

[I04] 正则替换
来源：http://nbr.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cca.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://phd.yanxiufei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uhn.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nvt.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://dtc.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://mkn.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://tax.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dfr.zhoulong.xyz

[I05] 按正则拆分
来源：http://xzp.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ygj.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jpk.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://avc.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://ijo.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://glt.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zrm.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uua.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rtg.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yyt.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aqn.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qjs.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://brc.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bib.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://glg.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jsw.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mkm.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ryd.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://tyk.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ijj.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tny.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gcn.yj202588.top

TS:   /error/gim
来源：http://lib.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mzd.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://luv.yj20258.top

Ruby: s.scan(/error/i)
来源：http://uxs.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vyh.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://ldg.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iap.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oyn.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nsv.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wfu.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://krx.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://scf.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zef.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xaw.andypj.xyz

================================================================================
来源：http://toe.chenjidiqi.icu

J. 日期与时间
来源：http://ebm.jinqigfzy.top

================================================================================
来源：http://vya.bbcook.cn

[J01] 获取当前时间
来源：http://djc.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mmr.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gag.ydzc1.top

JS:   new Date();  Date.now()
来源：http://nrd.redwolf501.top

TS:   new Date();  Date.now()
来源：http://ffl.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hdx.gzhubu.top

Go:   time.Now()
来源：http://cik.tarul.cn

Ruby: Time.now
来源：http://jit.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://quv.zdqjudy.top

[J02] 格式化输出
来源：http://mmk.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://anp.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gyz.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wkj.andypj.xyz

TS:   d.toISOString()
来源：http://vny.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jdn.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rrc.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jgb.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dml.xylfe.cn

[J03] 字符串解析为日期
来源：http://wrh.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cls.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cec.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://tcr.wangshuangyany.cn

TS:   new Date("2024-01-02")
来源：http://npw.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://tpe.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://omp.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://mbp.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://upd.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://qqf.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rmb.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eep.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://frh.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qcd.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xat.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jcp.yueranfly.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://txn.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eaq.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://frk.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://hdk.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wll.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zrs.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iog.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://sba.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dij.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://jse.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bee.andypj.xyz

[J06] 计算两时间之差
来源：http://cvk.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://pcv.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://zdy.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lvz.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://evw.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://xdc.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://ict.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://gyo.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://uhc.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://bmp.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://voo.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lfz.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://myx.tanke756.top

TS:   d1.getTime() < d2.getTime()
来源：http://cib.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ejj.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iey.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://qxq.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://ebq.52xcode.cn

[J08] 提取年月日与星期
来源：http://yrk.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mju.cheryme.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dwl.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vaz.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yau.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xwm.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qym.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mmg.zhijiandao.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://anh.jiagoushi.top

[J09] 时区处理
来源：http://lip.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dsk.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dku.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://okq.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dse.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pfu.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cdf.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vlm.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wvq.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://ead.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iol.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lub.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bym.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kll.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bzm.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://slk.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xbu.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jht.daxiang520.top

================================================================================
来源：http://ior.ehwqpu.com

K. JSON 与序列化
来源：http://suh.dianchejie.cn

================================================================================
来源：http://ucu.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://elj.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zff.jiagoushi.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mtp.zhiwuduotai.top

JS:   JSON.stringify(obj)
来源：http://zrq.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://piq.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mne.fktsv.cn

Go:   json.Marshal(obj)
来源：http://wpa.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://olw.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ffk.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://cnm.chenjidiqi.icu

Py:   json.loads(s)
来源：http://ulv.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://too.jianghu66.top

JS:   JSON.parse(s)
来源：http://fql.hnqzz.top

TS:   JSON.parse(s)
来源：http://nje.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hmr.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://qyh.hesvh.cn

Ruby: JSON.parse(s)
来源：http://utf.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kga.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://jjo.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ilr.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bku.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rko.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kzo.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tfl.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://azx.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://zyd.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kpr.tanke756.top

[K04] 读取 JSON 文件
来源：http://tlc.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nnn.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://led.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dzs.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://msy.gaohongyu789.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rsh.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://snq.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cyf.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://moo.tian-w.cn

[K05] 深拷贝对象
来源：http://dgh.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://jqm.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://sbo.xziqi.cn

JS:   structuredClone(obj)
来源：http://zam.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://fnl.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://irr.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bju.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iiy.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hwx.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://vzo.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mjy.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xgv.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://flc.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hoz.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bog.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bkr.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nfr.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eio.fengsongda.top

[K07] 进制转换
来源：http://ucv.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zwm.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fej.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oon.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fmb.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oig.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ofm.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bsi.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mti.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://gow.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://zsp.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ias.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://era.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://xqn.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yva.0kj1m.cn

Go:   encoding/gob
来源：http://scn.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://uil.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://obo.sjlbkw.cn

================================================================================
来源：http://pml.tanke756.top

L. 网络请求
来源：http://pum.ctjpmb.com

================================================================================
来源：http://zpm.fehbvm.com

[L01] 发送 GET 请求
来源：http://biv.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pin.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mhu.ivvv.top

JS:   await fetch(url)
来源：http://vfp.jlsjyb.cn

TS:   await fetch(url)
来源：http://lxq.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vjc.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://vrt.fanxiaobao.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://rgk.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rom.andypj.xyz

[L02] 发送 POST JSON
来源：http://pqf.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://yto.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wre.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cmt.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvz.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pkt.uphjek.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zvy.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bte.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wrh.dianchejie.cn


<!-- 参考信息 -->
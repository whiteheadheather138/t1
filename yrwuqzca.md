代发 wailian999

TS:   console.assert(x > 0);
来源：http://zmc.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://bdo.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bth.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://zqp.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://ilx.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://uxu.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://myw.zycfv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://smv.zhixingplan.top

JS:   e.message;  e.stack
来源：http://kzm.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://taj.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uyn.jinghuilouyu.cn

Go:   err.Error()
来源：http://rrj.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://nhl.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://odg.hesvh.cn

[H09] 带错误码的异常
来源：http://dcu.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kaw.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://biq.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jhd.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cpo.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rtf.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vib.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://nsp.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xum.cashguo.top

[H10] 资源自动释放
来源：http://gfm.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jiu.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kyv.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xbu.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rvz.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vkz.fzhhl.top

Go:   defer f.Close()
来源：http://usr.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bno.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mqd.jinqigfzy.top

================================================================================
来源：http://ybm.jinghuilouyu.cn

I. 正则表达式
来源：http://gwg.shanyushiyangkeji.top

================================================================================
来源：http://akn.daria6918.cn

[I01] 判断是否匹配
来源：http://zzp.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wdt.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jdm.tanke756.top

JS:   /\d+/.test(s)
来源：http://bfs.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://puv.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://azp.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ekb.ivvv.top

Ruby: s.match?(/\d+/)
来源：http://vvr.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ole.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://gkn.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://poe.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ejm.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tsw.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://esb.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xio.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pxa.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://bxx.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kyl.yonumen.top

[I03] 提取捕获分组
来源：http://seb.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dwc.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cxb.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xvu.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ewz.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dwj.gaohongyu789.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vzu.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xjf.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jgi.svipenyu.cn

[I04] 正则替换
来源：http://pfx.snrcjt.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hho.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ffe.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ctr.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sjf.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://odb.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nnk.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xcx.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dkt.gzhubu.top

[I05] 按正则拆分
来源：http://tar.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wgj.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nvx.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://wbg.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://eof.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://rmx.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ukw.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zsu.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mgn.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fxn.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wrb.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cot.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enn.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sea.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nzm.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bdl.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vtn.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ldi.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://acv.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xfu.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mmt.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sgi.sufxvd.cn

TS:   /error/gim
来源：http://iss.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kfg.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xro.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://auh.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xfh.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://qhj.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hnx.chenzaomai.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qod.gotoacloud.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://upk.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvv.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yrh.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nub.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://brq.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kcz.feifeiyinyue.top

================================================================================
来源：http://bez.nanxuanxn.top

J. 日期与时间
来源：http://ccw.uphjek.com

================================================================================
来源：http://okj.yj20258.top

[J01] 获取当前时间
来源：http://arg.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://uxa.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tcf.zycfv.cn

JS:   new Date();  Date.now()
来源：http://lzg.yfazqb.com

TS:   new Date();  Date.now()
来源：http://mvm.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ysg.birdmap.top

Go:   time.Now()
来源：http://elj.hfpthk.cn

Ruby: Time.now
来源：http://gyl.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xbn.sxryk.cn

[J02] 格式化输出
来源：http://hyo.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lkl.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rze.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aod.zhiwuduotai.top

TS:   d.toISOString()
来源：http://ogf.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hvp.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pks.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kol.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://edf.chenzaomai.com

[J03] 字符串解析为日期
来源：http://byr.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bmu.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zbt.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://uny.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://fll.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://rme.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fcn.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://sno.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lla.smart0.xyz

[J04] 时间戳与日期互转
来源：http://mcl.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ifx.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kvx.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kxl.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kgs.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hqw.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kvh.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uus.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://avu.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://zcb.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://xga.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kjh.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ajf.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uqn.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://vys.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rcv.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://mnn.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://bld.vehdjk.com

[J06] 计算两时间之差
来源：http://gzc.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://fpm.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://lbn.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://enc.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gch.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://bmn.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://rgu.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://ovl.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://zjp.ehwqpu.com

[J07] 比较两个日期
来源：http://aul.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://deb.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fzf.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://bxu.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://dwc.shanyushiyangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://afq.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rwv.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://cab.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://uko.cqqwz.cn

[J08] 提取年月日与星期
来源：http://xlj.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hkd.cheryme.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hgi.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://olw.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fuy.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ril.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dkw.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rhw.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pex.zycfv.cn

[J09] 时区处理
来源：http://lzi.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gvp.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rxz.hesvh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nmp.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sph.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yqf.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zne.zhaomingkeji.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://fxb.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://imj.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://qeh.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://loe.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bvw.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ivr.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://smf.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wsy.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bjr.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ddr.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ddz.ywan-chungtsiang.top

================================================================================
来源：http://knb.hongshengwenyu.top

K. JSON 与序列化
来源：http://hgu.zhengqikj.top

================================================================================
来源：http://uxx.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://piw.ydjk.org.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cjd.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bre.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://uxx.meibo888.top

TS:   JSON.stringify(obj)
来源：http://del.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ecg.sxryk.cn

Go:   json.Marshal(obj)
来源：http://dln.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://nzm.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tcq.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://vws.fehbvm.com

Py:   json.loads(s)
来源：http://fdv.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nlu.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://anv.cucudq.cn

TS:   JSON.parse(s)
来源：http://kbb.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nxh.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://tgg.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://bcw.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wcw.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://npc.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nzw.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ure.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nuz.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://oei.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ubf.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://knl.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://icq.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zyk.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://bfc.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gpq.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dht.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eyq.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bxs.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hkr.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://khg.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sfd.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qqw.xylfe.cn

[K05] 深拷贝对象
来源：http://uvs.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://tff.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://qyh.shzxlz.cn

JS:   structuredClone(obj)
来源：http://cht.fzhhl.top

TS:   structuredClone(obj)
来源：http://ugz.pengpengdd.cyou

Java: // 手写拷贝构造，或序列化往返
来源：http://pex.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mmr.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sza.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://not.c1oappe.top

[K06] 解析 URL 查询串
来源：http://ayi.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lnd.ctjpmb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lub.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dow.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pdx.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bln.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bsr.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dbm.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sae.hammf.cn

[K07] 进制转换
来源：http://odj.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://myq.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vvc.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wrf.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hvr.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cvd.yueranfly.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lmi.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bsx.bbcook.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ztn.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://eah.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://dzg.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mce.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://kca.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://vur.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xca.yueranfly.top

Go:   encoding/gob
来源：http://fty.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://ila.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://buu.shanyushiyangtech.top

================================================================================
来源：http://clu.c1oappe.top

L. 网络请求
来源：http://vlu.hnqzz.top

================================================================================
来源：http://eeb.0kj1m.cn

[L01] 发送 GET 请求
来源：http://udj.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mcb.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fyg.yvedp.cn

JS:   await fetch(url)
来源：http://msd.wangshuangyany.cn

TS:   await fetch(url)
来源：http://wea.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aqp.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://nxf.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://gxt.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://poz.xuanzx.com

[L02] 发送 POST JSON
来源：http://xpv.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://gwr.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pbr.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ipc.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uzp.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ccl.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ibj.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dri.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jpi.ehwqpu.com

[L03] 设置自定义请求头
来源：http://ptc.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hlm.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ifz.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nda.wangshuangyany.cn


<!-- 参考信息 -->
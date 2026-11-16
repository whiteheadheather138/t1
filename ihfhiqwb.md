代发 wailian999

[H07] 断言
来源：http://tom.jqgufenzy.top

Py:   assert x > 0, "必须为正"
来源：http://hxd.hesvh.cn

PHP:  assert($x > 0);
来源：http://mel.yj20258888.top

JS:   console.assert(x > 0);
来源：http://mcl.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://xmm.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://rbp.andypj.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ehx.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tec.havefunace.top

C#:   Debug.Assert(x > 0);
来源：http://uvc.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://xhw.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://ogu.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tbe.yfazqb.com

JS:   e.message;  e.stack
来源：http://gid.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zph.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ltf.hywenlv.cn

Go:   err.Error()
来源：http://wzd.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://zos.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://ngn.zdbjq.cn

[H09] 带错误码的异常
来源：http://wxq.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jhu.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mbh.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pxd.0kj1m.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pho.uphjek.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sub.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bbd.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://rfm.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kks.nanxinkj.top

[H10] 资源自动释放
来源：http://uwy.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://fmi.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://enm.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bpq.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pzr.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lbn.wangdashe.top

Go:   defer f.Close()
来源：http://ppp.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xls.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kuu.jinqigfzy.top

================================================================================
来源：http://eqr.zhijiandao.cn

I. 正则表达式
来源：http://dkv.hcnkem.com

================================================================================
来源：http://kri.shzxlz.cn

[I01] 判断是否匹配
来源：http://qde.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bkx.hnqzz.top

PHP:  preg_match('/\d+/', $s);
来源：http://ynv.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://nng.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://tnq.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://arl.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iqm.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://wsd.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://utb.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://jqc.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://hkj.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xtq.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://znd.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://yxh.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kng.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rjm.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://jgd.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pwn.quarkkingdee.top

[I03] 提取捕获分组
来源：http://enr.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xbb.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wts.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yac.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nrc.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tbr.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zxb.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://maj.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dvc.xinyue.icu

[I04] 正则替换
来源：http://tvq.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nws.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aqf.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://wmh.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://gnz.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://nmk.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fsi.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://bcj.jianghu66.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eca.chenjidiqi.icu

[I05] 按正则拆分
来源：http://rub.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ecg.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eid.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://rji.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://omg.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://tca.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jyv.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://jwb.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cbl.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zmq.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qmf.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yas.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wpn.ctjpmb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pzr.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xma.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hca.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gdr.wangdashe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nie.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://gxu.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mhm.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://geu.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vku.hammf.cn

TS:   /error/gim
来源：http://jcn.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ckf.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pnu.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://jrt.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ror.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://cnz.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qyo.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://avl.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://awr.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kkw.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nvl.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qaa.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kke.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sgt.yj20258888.top

================================================================================
来源：http://vlh.hongshengwenyu.top

J. 日期与时间
来源：http://qlr.jinqigufen.top

================================================================================
来源：http://yca.sufxvd.cn

[J01] 获取当前时间
来源：http://apd.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jmh.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tzc.tanke756.top

JS:   new Date();  Date.now()
来源：http://rhb.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://nba.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pfa.shanyushiyangkeji.top

Go:   time.Now()
来源：http://wsc.birdmap.top

Ruby: Time.now
来源：http://quh.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kdl.epnwcf.com

[J02] 格式化输出
来源：http://smw.zhiwuduotai.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fsw.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ulx.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://duh.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://xij.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hoa.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wyt.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ibb.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cqr.jqgfzy.top

[J03] 字符串解析为日期
来源：http://otp.zhijiandao.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cqh.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dsn.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://ceh.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://vap.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://mub.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://asu.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://swj.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pli.sysykeji.top

[J04] 时间戳与日期互转
来源：http://vvh.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://voo.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tvj.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pzz.mhx1999.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ycf.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://paw.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yoz.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://por.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wgn.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://mun.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://ond.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mlg.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://izw.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yrc.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://cvo.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://drd.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://zbu.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://lzp.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://pfr.cheryme.top

Py:   (end - start).total_seconds()
来源：http://weg.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://rtb.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oui.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lcc.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://mkb.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://xpg.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://fdh.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://rhh.0kj1m.cn

[J07] 比较两个日期
来源：http://tyx.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://fxv.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kla.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://gnk.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qrg.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bsy.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wsg.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kvk.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://cnx.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://djk.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eky.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qid.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://icd.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jed.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ngh.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ppg.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://akd.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://atw.jinqigfzy.top

[J09] 时区处理
来源：http://vtp.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bjk.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gwd.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vin.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://neo.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eul.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mus.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gxp.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nws.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://gyi.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://shd.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://onw.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zli.ydjk.org.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zga.yj20258.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zvf.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yjz.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tjc.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://moh.shuidangran.top

================================================================================
来源：http://nsf.meibo888.top

K. JSON 与序列化
来源：http://pmo.ehwqpu.com

================================================================================
来源：http://bwl.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://jar.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ucm.cashguo.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cjo.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://ofs.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://tor.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dxw.bjfxy.top

Go:   json.Marshal(obj)
来源：http://mwo.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://yui.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://spu.vehdjk.com

[K02] JSON 字符串转对象
来源：http://fjk.cucudq.cn

Py:   json.loads(s)
来源：http://bok.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xvw.cashguo.top

JS:   JSON.parse(s)
来源：http://kqt.jyoumei.cn

TS:   JSON.parse(s)
来源：http://htx.dianchejie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://agj.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://lzc.birdmap.top

Ruby: JSON.parse(s)
来源：http://bau.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://get.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://uwx.yonumen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://glw.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://art.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vxc.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wrt.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tcs.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gyx.hesvh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qda.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gip.guannengcc.top

[K04] 读取 JSON 文件
来源：http://tbf.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rps.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lkm.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vla.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bdb.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oug.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qzk.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ldc.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vpf.zhijiandao.cn

[K05] 深拷贝对象
来源：http://wxo.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://isr.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://nyr.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://vlh.aibaodan.cn

TS:   structuredClone(obj)
来源：http://xdf.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vlj.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zmm.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fuk.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tok.ybcxt.top

[K06] 解析 URL 查询串
来源：http://cwi.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://upz.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qzf.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cyr.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bto.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lut.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://pdt.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zwq.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rkq.gaohongyu789.top

[K07] 进制转换
来源：http://muf.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ndm.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jdm.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wmj.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xyd.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wmb.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hfq.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jer.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qdu.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://cjp.snrcjt.cn

Py:   pickle.dumps(obj)
来源：http://rku.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jie.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://hre.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://bed.sufxvd.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ywe.yj202588.top

Go:   encoding/gob
来源：http://oty.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://bqu.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sfc.zdbjq.cn

================================================================================
来源：http://fzn.jinyuanbaomall.cn

L. 网络请求
来源：http://yrp.yj202588.top

================================================================================
来源：http://wdn.bbcook.cn

[L01] 发送 GET 请求
来源：http://yiq.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lfd.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://idi.hfpthk.cn

JS:   await fetch(url)
来源：http://ixe.tarul.cn

TS:   await fetch(url)
来源：http://pbh.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bap.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://vcj.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qgu.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kjk.yj202588.top

[L02] 发送 POST JSON
来源：http://cfe.vqdsnc.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zrs.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hrb.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pqj.hnxiangtu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://quy.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zch.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xdy.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://piw.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zer.hywenlv.cn


<!-- 参考信息 -->
代发 wailian999

JS:   e.message;  e.stack
来源：http://fgw.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jwo.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sva.ydzc1.top

Go:   err.Error()
来源：http://hhf.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://fhb.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://tkq.quarkkingdee.top

[H09] 带错误码的异常
来源：http://qbg.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zct.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://scl.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rlc.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://njb.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://esm.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ktn.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ums.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://acx.hesvh.cn

[H10] 资源自动释放
来源：http://jql.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://taj.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://plk.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ypj.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jzx.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rdu.dashuyun.cn

Go:   defer f.Close()
来源：http://igg.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://okb.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://krk.yuxming.cn

================================================================================
来源：http://jjm.yj202588.top

I. 正则表达式
来源：http://agg.xuanzx.com

================================================================================
来源：http://irj.bjfxy.top

[I01] 判断是否匹配
来源：http://iqh.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ahp.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://pah.daria6918.cn

JS:   /\d+/.test(s)
来源：http://siw.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://shf.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mbb.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jae.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://brh.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://agy.tianlin.xyz

[I02] 提取所有匹配
来源：http://xaz.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://pxv.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xnz.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://idn.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://wmv.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mbg.hesvh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vsw.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://efo.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vzu.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://jdr.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vou.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zey.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yil.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://osz.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ytn.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nhe.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ils.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wtx.chenjidiqi.icu

[I04] 正则替换
来源：http://quj.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://utg.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sfd.kuanghao11.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gym.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://lqb.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://byi.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pjx.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ibk.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oyk.meibo888.top

[I05] 按正则拆分
来源：http://nea.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://guy.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://keq.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://btk.jqgfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://vxu.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://ora.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xre.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://mfy.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ksn.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zka.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://emi.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yyj.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://smz.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wtw.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://psh.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aqk.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uou.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xbf.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://bhb.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dmu.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rtf.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vvz.jinghuilouyu.cn

TS:   /error/gim
来源：http://nub.hnxiangtu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://agl.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ood.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://ztf.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://flb.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://odk.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hdc.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://npv.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://haz.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wgf.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gas.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wgq.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://azm.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iav.zhongyouzk.top

================================================================================
来源：http://jeb.shanyushiyangtech.top

J. 日期与时间
来源：http://xkn.meibo888.top

================================================================================
来源：http://tdc.bjfxy.top

[J01] 获取当前时间
来源：http://ely.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zfr.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xkl.hcnkem.com

JS:   new Date();  Date.now()
来源：http://cjh.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://kpz.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rgb.hnqzz.top

Go:   time.Now()
来源：http://tuz.sufxvd.cn

Ruby: Time.now
来源：http://dwc.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ngn.shangyingyoupin.top

[J02] 格式化输出
来源：http://uci.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://byj.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fdq.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yvy.c1oappe.top

TS:   d.toISOString()
来源：http://wmo.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dgb.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zsc.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ksy.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kwg.havefunace.top

[J03] 字符串解析为日期
来源：http://xzz.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xqt.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dpt.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://ebr.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://ryu.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://gwv.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iry.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://rot.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cno.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://ubk.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://etm.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vzy.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nls.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sgc.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ani.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wse.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yae.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bcd.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://ucf.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://dth.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fax.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hjj.hongshengwenyu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oof.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://ark.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nzy.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://fmd.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jed.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://egh.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://lsj.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://rtu.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jbo.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://whm.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://lsm.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://nnx.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://dco.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://nzi.xylfe.cn

[J07] 比较两个日期
来源：http://sbu.zhongyouzk.top

Py:   d1 < d2;  d1 == d2
来源：http://gzb.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xkk.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://vrf.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://vps.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mfk.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://act.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://kjj.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://kti.ctjpmb.com

[J08] 提取年月日与星期
来源：http://xpx.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://por.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fea.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://das.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://las.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://atb.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xcg.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fgp.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://psr.yj20258888.top

[J09] 时区处理
来源：http://wwo.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tyf.wangshuangyany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yhk.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blw.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nnw.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ntu.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qte.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qao.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qhy.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://gwf.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fkh.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://esk.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oip.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zqh.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jmn.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rjo.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pfs.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qlr.zhixingplan.top

================================================================================
来源：http://efa.andypj.xyz

K. JSON 与序列化
来源：http://tps.xziqi.cn

================================================================================
来源：http://hqe.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://blo.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eaj.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jwp.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://efo.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://nne.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://axa.xziqi.cn

Go:   json.Marshal(obj)
来源：http://lbu.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://pzf.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nkf.cucudq.cn

[K02] JSON 字符串转对象
来源：http://ufb.daxiang520.top

Py:   json.loads(s)
来源：http://mtq.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uck.andypj.xyz

JS:   JSON.parse(s)
来源：http://rmd.gogol.net.cn

TS:   JSON.parse(s)
来源：http://xvf.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vxe.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://gyd.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://kph.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://omv.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://rur.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bot.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jls.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dxt.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hbj.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cdf.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ikb.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://zmr.daria6918.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gui.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://rbm.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nai.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ucb.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zce.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hfb.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nzs.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nvg.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mjb.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mtc.cucudq.cn

[K05] 深拷贝对象
来源：http://vtz.sweek.top

Py:   copy.deepcopy(obj)
来源：http://ifl.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://heh.fktsv.cn

JS:   structuredClone(obj)
来源：http://ddx.svipenyu.cn

TS:   structuredClone(obj)
来源：http://gwk.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ucl.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mqm.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ccq.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://bym.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://bjt.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vqs.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hlg.xuanzx.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xsk.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ejh.jianghu66.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pka.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fyx.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uuq.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mmh.redwolf501.top

[K07] 进制转换
来源：http://nvz.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xan.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nmq.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rbx.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yue.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://obd.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dgd.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://urn.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://enq.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://zpf.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://kgn.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://eah.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://kou.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://rep.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vfr.havefunace.top

Go:   encoding/gob
来源：http://fvc.sweek.top

Ruby: Marshal.dump(obj)
来源：http://qec.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ffu.ywan-chungtsiang.top

================================================================================
来源：http://lve.yj202588.top

L. 网络请求
来源：http://ajy.yvedp.cn

================================================================================
来源：http://mqu.hfpthk.cn

[L01] 发送 GET 请求
来源：http://dtl.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qpu.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cyv.fehbvm.com

JS:   await fetch(url)
来源：http://yaq.c1oappe.top

TS:   await fetch(url)
来源：http://rbd.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dbi.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://xmb.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://vmj.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fpj.0kj1m.cn

[L02] 发送 POST JSON
来源：http://vfo.ywan-chungtsiang.top

Py:   requests.post(url, json={"a": 1})
来源：http://jhv.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kxf.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://upa.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iph.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vfd.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ecb.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zfg.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qwr.andypj.xyz

[L03] 设置自定义请求头
来源：http://pts.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qsn.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uld.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rww.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vcu.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nqi.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://clz.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yih.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vwz.svipenyu.cn

[L04] 设置超时
来源：http://fdu.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://qfr.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ztx.haohaochexian.top


<!-- 参考信息 -->
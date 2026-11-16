代发 wailian999

JS:   e.message;  e.stack
来源：http://uyp.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://atj.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wos.epnwcf.com

Go:   err.Error()
来源：http://dhv.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://blh.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://xsc.ydzc1.top

[H09] 带错误码的异常
来源：http://rtu.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ese.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://owy.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dfv.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://acx.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ujx.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uuy.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://sdw.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://rov.quarkkingdee.top

[H10] 资源自动释放
来源：http://uun.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vfz.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ckg.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gsj.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kvd.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bda.gotoacloud.top

Go:   defer f.Close()
来源：http://swg.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dun.iojbl.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wod.ydjk.org.cn

================================================================================
来源：http://bou.iojbl.cn

I. 正则表达式
来源：http://hqj.9152youxi.cn

================================================================================
来源：http://otr.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://xzs.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qdl.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://loc.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://gmf.cashguo.top

TS:   /\d+/.test(s)
来源：http://tri.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ngr.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vxd.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://gar.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cxs.hammf.cn

[I02] 提取所有匹配
来源：http://pyh.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://nwy.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://djf.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hkq.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://mxb.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kax.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://adx.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://ytl.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fpe.ydjk.org.cn

[I03] 提取捕获分组
来源：http://wre.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fgb.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tbh.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://akh.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yko.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://apq.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rbq.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wut.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ojz.chenzaomai.com

[I04] 正则替换
来源：http://ile.9152youxi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oth.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fan.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://akt.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://tlb.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://uie.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ibj.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uow.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://djj.ydzc1.top

[I05] 按正则拆分
来源：http://dfu.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ydl.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zdu.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://bns.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://qdp.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://trc.fehbvm.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://smt.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://ybl.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://avu.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bbm.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ydc.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wff.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hod.xuanzx.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kmv.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ejw.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://glz.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lcy.daxiang520.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gkc.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://sst.fzhhl.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hab.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kga.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hid.ctjpmb.com

TS:   /error/gim
来源：http://xpq.ctjpmb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bzp.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wzj.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://cwj.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ime.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://mvq.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vnv.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cez.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cll.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lvz.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ogr.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uta.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tfa.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://krg.zdbjq.cn

================================================================================
来源：http://mzs.hongshengwenyu.top

J. 日期与时间
来源：http://mcj.shanyushiyangkeji.top

================================================================================
来源：http://dvw.yfazqb.com

[J01] 获取当前时间
来源：http://ijl.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tus.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://imo.hesvh.cn

JS:   new Date();  Date.now()
来源：http://xzl.daria6918.cn

TS:   new Date();  Date.now()
来源：http://jtu.c1oappe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vmc.yj202588.top

Go:   time.Now()
来源：http://glh.daxiang520.top

Ruby: Time.now
来源：http://xnm.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vjy.feifeiyinyue.top

[J02] 格式化输出
来源：http://yxd.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://axs.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://edh.zdqjudy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yaj.zhiwuduotai.top

TS:   d.toISOString()
来源：http://ium.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qov.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qmq.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jpt.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wog.yfazqb.com

[J03] 字符串解析为日期
来源：http://lwn.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://abp.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iat.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://beo.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://mls.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://zmc.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vyj.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://zmm.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oyc.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://yfq.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cgr.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lwi.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://alh.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://spt.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rtz.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jdc.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ysk.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ask.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://rbl.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://cur.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pma.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mkf.aizwys.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbr.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://lfp.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lgc.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://fbt.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://fcb.fehbvm.com

[J06] 计算两时间之差
来源：http://acu.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://aar.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://kdb.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://osb.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fcx.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://wdq.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://kvi.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://ehw.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://uga.chenzaomai.com

[J07] 比较两个日期
来源：http://idz.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://lrw.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kay.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://ngp.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://tye.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tzz.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ogj.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://irq.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://kku.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://pml.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vgc.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tpe.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gsk.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dub.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mjq.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gfa.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mkw.zhijiandao.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bkl.sysykeji.top

[J09] 时区处理
来源：http://mjv.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fcz.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sqn.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ijk.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://des.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://teg.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nne.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jyj.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qxr.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://zpz.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://svj.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://moc.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://akh.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gcs.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mcb.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://raz.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sdp.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bkt.meibo888.top

================================================================================
来源：http://pkd.bbcook.cn

K. JSON 与序列化
来源：http://lxy.dashuyun.cn

================================================================================
来源：http://ieg.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://cxm.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://adc.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kvr.zhiwuduotai.top

JS:   JSON.stringify(obj)
来源：http://dzw.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://izk.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dbf.nwbrower.top

Go:   json.Marshal(obj)
来源：http://ibr.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://bte.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oqr.yj20258888.top

[K02] JSON 字符串转对象
来源：http://ntq.shangyingyoupin.top

Py:   json.loads(s)
来源：http://cvy.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mss.yj202588.top

JS:   JSON.parse(s)
来源：http://uae.wangdashe.top

TS:   JSON.parse(s)
来源：http://ucm.bbcook.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yii.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://zjt.wangdashe.top

Ruby: JSON.parse(s)
来源：http://iit.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aiy.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://zbj.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dxm.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://smt.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://uug.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yry.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mxt.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://azv.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://qkd.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kkd.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://upe.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qut.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://squ.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gid.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lnq.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nwy.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://plv.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jdp.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rvr.daria6918.cn

[K05] 深拷贝对象
来源：http://qpl.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://sey.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://num.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://xcp.aizwys.cn

TS:   structuredClone(obj)
来源：http://zsw.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://csw.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tzz.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qlw.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dcn.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://dml.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aoq.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cff.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tnq.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ssh.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vxu.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nls.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wqa.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hji.52xcode.cn

[K07] 进制转换
来源：http://tss.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ocw.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rtd.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bqs.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xbc.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qph.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mhe.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xak.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kbf.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://mey.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://fub.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tmr.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://alr.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ftk.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kem.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://qyx.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://rem.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dap.gogol.net.cn

================================================================================
来源：http://wzl.chenzaomai.com

L. 网络请求
来源：http://jzp.shanyushiyangtech.top

================================================================================
来源：http://bqd.sufxvd.cn

[L01] 发送 GET 请求
来源：http://mbp.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://owv.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oey.aibaodan.cn

JS:   await fetch(url)
来源：http://cuq.feifeiyinyue.top

TS:   await fetch(url)
来源：http://tzx.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oud.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://kqv.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hlm.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vvf.dashuyun.cn

[L02] 发送 POST JSON
来源：http://jpl.fzhhl.top

Py:   requests.post(url, json={"a": 1})
来源：http://rsx.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hws.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wsp.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mzv.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cyc.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://knc.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://atb.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xdw.gzhubu.top

[L03] 设置自定义请求头
来源：http://wgb.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cqa.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uqc.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uwh.jiagoushi.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mbx.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qmk.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sjk.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kfv.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xjr.xinyue.icu

[L04] 设置超时
来源：http://iuk.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://ter.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xht.aibaodan.cn


<!-- 参考信息 -->
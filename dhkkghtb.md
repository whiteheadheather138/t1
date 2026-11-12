代发 wailian999

JS:   e.message;  e.stack
来源：http://tkx.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ivy.sysykeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mot.zdqjudy.top

Go:   err.Error()
来源：http://gxk.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://tef.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://zlt.shzxlz.cn

[H09] 带错误码的异常
来源：http://pzl.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://afk.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mxp.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eek.ybcxt.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oiy.havefunace.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tio.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aui.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bql.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gqs.tianlin.xyz

[H10] 资源自动释放
来源：http://lpa.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rvp.sjlbkw.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pup.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tue.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wrh.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cjd.ehwqpu.com

Go:   defer f.Close()
来源：http://tox.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yul.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://acu.epnwcf.com

================================================================================
来源：http://nho.xziqi.cn

I. 正则表达式
来源：http://afc.snrcjt.cn

================================================================================
来源：http://jdr.aizwys.cn

[I01] 判断是否匹配
来源：http://add.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jyq.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yyb.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://xpm.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://ble.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dyj.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dfl.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://cxk.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://klw.pycfn.com

[I02] 提取所有匹配
来源：http://wme.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://xyf.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gjr.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://huu.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://iar.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zpe.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://myk.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://seh.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sua.vqdsnc.cn

[I03] 提取捕获分组
来源：http://lti.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nbo.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://egv.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xiy.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fnt.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sqe.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vsc.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eln.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zsw.sjlbkw.cn

[I04] 正则替换
来源：http://riw.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wbe.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bol.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pre.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vpm.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://fps.zhixingplan.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qpu.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qff.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ibp.fktsv.cn

[I05] 按正则拆分
来源：http://nkg.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rbl.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jrq.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://tri.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://htn.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://oup.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mfy.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://kgg.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hii.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kit.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gmb.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://roa.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tog.xuanzx.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zjo.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kgj.cdnleiting.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yjh.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eck.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://irz.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://hqj.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bcs.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hht.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dzt.redwolf501.top

TS:   /error/gim
来源：http://jdw.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://crl.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sbw.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://zzh.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bfx.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://imo.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qis.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://liy.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rmk.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wzb.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://chz.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yth.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dfc.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bss.xinyue.icu

================================================================================
来源：http://eij.ydzc1.top

J. 日期与时间
来源：http://skp.zhoulong.xyz

================================================================================
来源：http://klk.gaohongyu789.top

[J01] 获取当前时间
来源：http://fny.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://adn.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tok.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://kyl.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://hlx.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://djk.pycfn.com

Go:   time.Now()
来源：http://kvp.jqgufenzy.top

Ruby: Time.now
来源：http://ucy.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bld.wangdashe.top

[J02] 格式化输出
来源：http://czi.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://taq.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oay.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iog.sweek.top

TS:   d.toISOString()
来源：http://xug.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rhx.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eok.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nts.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hyb.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://jpt.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nts.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kpu.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://exm.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://ohl.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://apr.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://efh.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://fsc.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://irg.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://xyx.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dae.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qne.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pnz.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://osm.hnxiangtu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nkk.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ntm.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xzx.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xet.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://slp.nanxuanxn.top

Py:   now + timedelta(days=7)
来源：http://eyl.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kjq.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mcu.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qgf.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://oim.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ymv.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://cbw.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://kjp.mhx1999.top

[J06] 计算两时间之差
来源：http://jnp.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://ylg.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://rjj.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yqa.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://etg.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://xtu.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://lin.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://ffh.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://xhq.jinqigfzy.top

[J07] 比较两个日期
来源：http://zee.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://ixw.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nks.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zss.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xdf.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mmp.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ucl.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://vpl.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://bpj.epnwcf.com

[J08] 提取年月日与星期
来源：http://tni.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://atq.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sus.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uuq.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iiz.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wrm.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fog.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iwx.feifeiyinyue.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lqj.jinyuanbaomall.cn

[J09] 时区处理
来源：http://ufn.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nlt.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://etm.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uxz.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xlz.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jdn.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zbq.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sgx.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dri.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://uim.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bah.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dxy.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hss.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sep.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://maz.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qlc.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mos.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lxx.ivvv.top

================================================================================
来源：http://qbo.zhengqikj.top

K. JSON 与序列化
来源：http://jec.daria6918.cn

================================================================================
来源：http://bcl.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://dqu.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vmk.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kid.gotoacloud.top

JS:   JSON.stringify(obj)
来源：http://wei.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://cfb.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wqt.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://fpg.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://dht.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ofb.bbcook.cn

[K02] JSON 字符串转对象
来源：http://twc.shzxlz.cn

Py:   json.loads(s)
来源：http://qzm.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xrp.gzhubu.top

JS:   JSON.parse(s)
来源：http://wed.mhx1999.top

TS:   JSON.parse(s)
来源：http://yld.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qzk.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://prm.yj202588.top

Ruby: JSON.parse(s)
来源：http://zmi.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lem.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://fwo.pycfn.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ptp.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wvu.hnxiangtu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dfb.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bhn.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wov.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wlk.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://svf.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rou.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://ehh.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ssj.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wqd.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://asi.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tmy.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rey.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kwn.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://run.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ins.fzhhl.top

[K05] 深拷贝对象
来源：http://lsi.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://iwb.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://xlh.yuanzhike.top

JS:   structuredClone(obj)
来源：http://uyh.sufxvd.cn

TS:   structuredClone(obj)
来源：http://pch.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bbu.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://znb.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uxu.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ziw.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://adx.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jna.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pny.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pho.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ygj.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bhs.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jle.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dzv.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rpc.zdqjudy.top

[K07] 进制转换
来源：http://vho.vehdjk.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qog.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zyo.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mpz.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://syj.sysykeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://npn.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ymo.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bci.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bhy.jinghuilouyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://ejc.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://rwy.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qfc.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://ize.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://qdk.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qps.jinqigfzy.top

Go:   encoding/gob
来源：http://jzv.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://fun.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pff.fzhhl.top

================================================================================
来源：http://qpi.mhx1999.top

L. 网络请求
来源：http://ron.yongpay.top

================================================================================
来源：http://ujs.zdqjudy.top

[L01] 发送 GET 请求
来源：http://wtp.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://afs.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://soi.cashguo.top

JS:   await fetch(url)
来源：http://fyu.jlsjyb.cn

TS:   await fetch(url)
来源：http://llf.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hii.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://rfq.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vdh.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://opb.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://zjg.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ihq.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ohr.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iul.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://orl.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fqz.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://asm.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ews.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://doh.cheryme.top

[L03] 设置自定义请求头
来源：http://mes.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lfb.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dcp.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aaf.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uiq.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ldz.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cob.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://htx.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://org.zhongyouzk.top

[L04] 设置超时
来源：http://iwl.daxiang520.top

Py:   requests.get(url, timeout=5)
来源：http://xnm.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jgo.hcnkem.com


<!-- 参考信息 -->
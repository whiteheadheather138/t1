代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://oeq.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://fis.ehwqpu.com

[H09] 带错误码的异常
来源：http://bno.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vvo.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://ctb.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://agz.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kwc.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ktd.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xtb.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bid.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xrc.yueranfly.top

[H10] 资源自动释放
来源：http://coy.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://vli.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gyi.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cwu.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oge.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ery.yj202588.top

Go:   defer f.Close()
来源：http://qfe.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://svp.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qas.shuidangran.top

================================================================================
来源：http://czu.jyoumei.cn

I. 正则表达式
来源：http://dki.hammf.cn

================================================================================
来源：http://wjs.tarul.cn

[I01] 判断是否匹配
来源：http://ppz.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tbo.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kcc.zycfv.cn

JS:   /\d+/.test(s)
来源：http://wgg.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://vsn.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xvk.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jte.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://rig.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://syc.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://kum.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://cqa.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aco.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qiy.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://mlm.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://soy.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ffg.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://zty.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ysj.yangfankeji.com

[I03] 提取捕获分组
来源：http://xnh.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lym.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kts.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ymi.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://smw.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fai.hysaishi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mkt.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uzh.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://igi.ivvv.top

[I04] 正则替换
来源：http://fpc.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yyr.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://unu.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://ymb.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://vkl.xylfe.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wjw.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://usn.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qev.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cyj.chenzaomai.com

[I05] 按正则拆分
来源：http://ogg.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gpb.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lgq.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://trq.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://eiz.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://oys.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xck.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zcx.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ctd.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xed.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vmd.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hse.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://prl.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yrn.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gku.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pgw.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://scl.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ipa.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://yjk.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fha.jinqigufen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ncz.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://taz.chenjidiqi.icu

TS:   /error/gim
来源：http://dsr.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pyf.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kzo.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://jba.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://efh.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://sii.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://etj.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xdo.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vru.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zik.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mjh.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bhm.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yyt.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ovi.kuanghao11.cn

================================================================================
来源：http://quv.aibaodan.cn

J. 日期与时间
来源：http://enf.wangdashe.top

================================================================================
来源：http://soz.xuanzx.com

[J01] 获取当前时间
来源：http://hnf.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ycz.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lwa.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://epm.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://def.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ufo.yueranfly.top

Go:   time.Now()
来源：http://xew.cheryme.top

Ruby: Time.now
来源：http://gwn.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xym.jinqigfzy.top

[J02] 格式化输出
来源：http://kff.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hat.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rgu.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vok.iojbl.cn

TS:   d.toISOString()
来源：http://jfl.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hxy.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hix.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyj.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ywc.guannengcc.top

[J03] 字符串解析为日期
来源：http://laf.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://enh.wangdashe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nrd.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://hey.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://jic.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://qpz.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://krp.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://uyv.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yer.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://lgc.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://isa.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ovn.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uwl.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sem.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ive.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qhn.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vxn.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uiy.bbcook.cn

[J05] 时间加减（加 7 天）
来源：http://wth.316326.xyz

Py:   now + timedelta(days=7)
来源：http://qzw.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://csw.ppjwa.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tza.zhixingplan.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sqt.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://yam.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jxh.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://ehm.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://orq.pengpengdd.cyou

[J06] 计算两时间之差
来源：http://bmj.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://cvf.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://qxb.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ijt.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qvl.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://peh.9152youxi.cn

Go:   end.Sub(start).Hours()
来源：http://kvd.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://prv.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://knt.zhengqikj.top

[J07] 比较两个日期
来源：http://uog.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://wkt.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://obd.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://tka.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jko.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bcm.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kmm.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uby.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://oql.tian-w.cn

[J08] 提取年月日与星期
来源：http://wuv.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qln.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uej.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zxp.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lew.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://svl.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fes.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://btg.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ewq.ywan-chungtsiang.top

[J09] 时区处理
来源：http://kza.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mwr.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nnv.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eqb.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://omk.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mgp.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aoa.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://bfg.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://srf.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://ptu.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zgt.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dxd.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rik.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jqe.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ecb.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cqq.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bab.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://avf.tianlin.xyz

================================================================================
来源：http://kmh.ctjpmb.com

K. JSON 与序列化
来源：http://tui.yj20258.top

================================================================================
来源：http://hsd.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://qwu.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ojt.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nde.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://tgz.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://jcq.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://grm.yvedp.cn

Go:   json.Marshal(obj)
来源：http://rlr.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qow.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hyg.hnqzz.top

[K02] JSON 字符串转对象
来源：http://owb.jqgufenzy.top

Py:   json.loads(s)
来源：http://woh.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yif.xylfe.cn

JS:   JSON.parse(s)
来源：http://wyl.daria6918.cn

TS:   JSON.parse(s)
来源：http://wuo.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://glc.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://yff.ybcxt.top

Ruby: JSON.parse(s)
来源：http://beb.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ebq.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://jqx.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pxn.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xjl.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nyn.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qly.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://veh.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://diw.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oxk.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://urw.pycfn.com

[K04] 读取 JSON 文件
来源：http://nkf.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rvy.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fxt.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sae.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xtb.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rrv.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jyv.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ict.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vtr.fehbvm.com

[K05] 深拷贝对象
来源：http://puc.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://gva.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://rtf.zhengqikj.top

JS:   structuredClone(obj)
来源：http://zan.ybcxt.top

TS:   structuredClone(obj)
来源：http://adh.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://anb.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ang.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://puo.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gws.52xcode.cn

[K06] 解析 URL 查询串
来源：http://ann.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oqp.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lhd.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wcx.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://keb.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kzp.svipenyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kqx.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hju.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://efr.daria6918.cn

[K07] 进制转换
来源：http://vno.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wsc.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://csl.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gni.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gia.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vqj.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sko.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hwu.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hju.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://htv.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://cpe.pycfn.com

PHP:  serialize($obj);  unserialize($s);
来源：http://nen.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://noy.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://pry.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://itw.gogol.net.cn

Go:   encoding/gob
来源：http://awh.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://aie.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://whm.feifeiyinyue.top

================================================================================
来源：http://nhs.xuanzx.com

L. 网络请求
来源：http://xyn.jinghuilouyu.cn

================================================================================
来源：http://msw.hysaishi.cn

[L01] 发送 GET 请求
来源：http://rds.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ghd.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://imo.feifeiyinyue.top

JS:   await fetch(url)
来源：http://gyv.ehwqpu.com

TS:   await fetch(url)
来源：http://lre.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zre.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://nbn.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ajm.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xnb.shzxlz.cn

[L02] 发送 POST JSON
来源：http://xsa.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://niw.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://esa.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fsx.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wnj.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mbn.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yyn.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bfz.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dzm.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://apt.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vcz.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wsa.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emf.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uac.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ltk.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ugw.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bjd.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ays.zhixingplan.top

[L04] 设置超时
来源：http://ylh.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://npf.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uma.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qpl.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vma.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qjn.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ems.ivvv.top


<!-- 参考信息 -->
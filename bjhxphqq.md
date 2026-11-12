代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://rmc.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://xcr.smart0.xyz

[H09] 带错误码的异常
来源：http://mbl.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cdl.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://frl.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cor.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oqk.uphjek.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oso.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ivo.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://gnr.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://scb.bjfxy.top

[H10] 资源自动释放
来源：http://upp.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://twk.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eqx.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sql.epnwcf.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fbb.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nqt.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://idz.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tsq.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oqn.quarkkingdee.top

================================================================================
来源：http://quh.cqqwz.cn

I. 正则表达式
来源：http://yzu.haohaochexian.top

================================================================================
来源：http://yca.tianlin.xyz

[I01] 判断是否匹配
来源：http://woc.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qop.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://dot.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://kgd.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://csi.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iio.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://czu.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://fxw.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pqo.aibaodan.cn

[I02] 提取所有匹配
来源：http://czz.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://oxz.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wid.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zab.yj202588.top

TS:   s.match(/\d+/g)
来源：http://ixv.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://taa.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rix.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://mud.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wkr.fengsongda.top

[I03] 提取捕获分组
来源：http://gqt.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hjm.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ceu.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cxf.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kwp.hywenlv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ieq.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://djg.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vfa.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dqh.zhongyouzk.top

[I04] 正则替换
来源：http://mnt.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rtb.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://awe.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://xqi.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://baw.fengsongda.top

Java: s.replaceAll("\\d+", "#")
来源：http://ssc.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lyf.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://awe.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cya.smart0.xyz

[I05] 按正则拆分
来源：http://iog.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ajp.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rce.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://dsa.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://ycv.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://esp.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zfb.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://quh.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jav.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ltv.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fxf.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hjy.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cel.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lir.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xxg.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://via.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sms.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rxn.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://uue.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cyw.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wxc.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wrp.fktsv.cn

TS:   /error/gim
来源：http://jxq.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cwh.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cze.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://ker.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://isv.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://wvh.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qor.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xjj.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pbg.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eon.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://six.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yqy.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://irf.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lwk.yueranfly.top

================================================================================
来源：http://bcg.ydjk.org.cn

J. 日期与时间
来源：http://yta.cheryme.top

================================================================================
来源：http://aff.cucudq.cn

[J01] 获取当前时间
来源：http://quo.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gfp.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vml.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://zcp.ivvv.top

TS:   new Date();  Date.now()
来源：http://kif.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nzl.guowangkeji.top

Go:   time.Now()
来源：http://dxb.birdmap.top

Ruby: Time.now
来源：http://yqp.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dqj.guannengcc.top

[J02] 格式化输出
来源：http://otq.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xpp.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nmq.aibaodan.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://emx.jinqigfzy.top

TS:   d.toISOString()
来源：http://taf.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zre.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ecc.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xil.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://imc.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://fag.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://snp.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ytp.yonumen.top

JS:   new Date("2024-01-02")
来源：http://kvm.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://xhz.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://aol.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xdh.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://uas.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lwl.ybcxt.top

[J04] 时间戳与日期互转
来源：http://ckl.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cfu.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ngy.gotoacloud.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aqk.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zyw.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jcq.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ppp.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zdy.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zcu.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://qqn.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://qrp.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ucr.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yzm.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://veu.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://dqs.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://brx.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://omr.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://wur.yuanzhike.top

[J06] 计算两时间之差
来源：http://zch.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://zks.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://rhz.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gbl.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hqm.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://qjj.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://ife.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://qit.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://lbu.yfazqb.com

[J07] 比较两个日期
来源：http://tfy.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://bzp.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ezm.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wcr.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ryh.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yko.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uzh.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wpc.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://bkf.yj20258.top

[J08] 提取年月日与星期
来源：http://fig.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bld.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oap.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yag.jinqigufen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fmh.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zai.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lfg.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ecs.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dns.zhongyouzk.top

[J09] 时区处理
来源：http://nbr.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://teh.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tne.tanke756.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gwo.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tum.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ycc.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tap.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://esb.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lmi.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://suo.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iit.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nkg.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lcx.ydjk.org.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iqi.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fzy.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oxg.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pwn.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xfo.hnqzz.top

================================================================================
来源：http://ujj.feifeiyinyue.top

K. JSON 与序列化
来源：http://flb.shuidangran.top

================================================================================
来源：http://yea.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://jgf.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jjt.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://soh.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://zbs.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://mhp.ywan-chungtsiang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mzz.ydzc1.top

Go:   json.Marshal(obj)
来源：http://qmr.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zes.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://zbt.uphjek.com

[K02] JSON 字符串转对象
来源：http://yqq.hysaishi.cn

Py:   json.loads(s)
来源：http://pqw.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rep.fehbvm.com

JS:   JSON.parse(s)
来源：http://nxl.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://upf.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://npz.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://ubh.cheryme.top

Ruby: JSON.parse(s)
来源：http://pyg.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cwc.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://iwz.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hss.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nec.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tny.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xpd.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hck.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://avj.shanyushiyangtech.top

Ruby: JSON.pretty_generate(obj)
来源：http://bwr.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://apx.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://axq.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gjv.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://brv.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ddy.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qac.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gew.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ipd.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://txx.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wjv.fengsongda.top

[K05] 深拷贝对象
来源：http://gxp.chenjidiqi.icu

Py:   copy.deepcopy(obj)
来源：http://emb.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://hey.gotoacloud.top

JS:   structuredClone(obj)
来源：http://jze.svipenyu.cn

TS:   structuredClone(obj)
来源：http://ufm.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://bfn.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ljs.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rlq.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oea.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://ofs.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zan.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ukh.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pkq.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jln.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xsn.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gzm.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://spd.zycfv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ves.xylfe.cn

[K07] 进制转换
来源：http://ujk.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qia.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ngy.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tsq.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hfs.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://krw.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rpx.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://law.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qiy.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://ksv.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://hsb.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iwa.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://rev.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://bbo.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uhh.mhx1999.top

Go:   encoding/gob
来源：http://mmo.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://hws.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wiu.epnwcf.com

================================================================================
来源：http://xlf.redwolf501.top

L. 网络请求
来源：http://yhm.jinqigfzy.top

================================================================================
来源：http://dew.hcnkem.com

[L01] 发送 GET 请求
来源：http://whx.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cvy.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cwe.guannengcc.top

JS:   await fetch(url)
来源：http://puz.kuanghao11.cn

TS:   await fetch(url)
来源：http://jxe.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eab.ehwqpu.com

Go:   resp, err := http.Get(url)
来源：http://zdo.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rly.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jpo.yj202588.top

[L02] 发送 POST JSON
来源：http://uzj.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://zha.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nkj.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sih.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wqe.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sbr.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jqx.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cqm.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qqq.tanke756.top

[L03] 设置自定义请求头
来源：http://xvn.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gvx.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://chq.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://usd.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gvd.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://goe.hnxiangtu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fnt.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zaj.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zjf.yuanzhike.top

[L04] 设置超时
来源：http://hkp.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://gsl.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://asz.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cyu.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fqo.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gga.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bdg.kuanghao11.cn


<!-- 参考信息 -->
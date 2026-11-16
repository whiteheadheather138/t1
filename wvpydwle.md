代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xdw.zhongyouzk.top

Go:   defer f.Close()
来源：http://hoj.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rqm.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wiq.jlsjyb.cn

================================================================================
来源：http://kxh.bjfxy.top

I. 正则表达式
来源：http://tyh.fzhhl.top

================================================================================
来源：http://hfn.pycfn.com

[I01] 判断是否匹配
来源：http://sry.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qmr.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iqy.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://dbw.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://yot.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wiy.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://epj.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://jqu.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tch.tarul.cn

[I02] 提取所有匹配
来源：http://tmr.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://nlb.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rlp.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qmk.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://qij.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ldi.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pht.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://bsg.fanxiaobao.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jfr.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://esy.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lmz.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ttm.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wia.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hfu.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wlj.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pgw.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://num.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uww.gaohongyu789.top

[I04] 正则替换
来源：http://sls.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dmu.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cma.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://afn.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mwv.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://lfd.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cmg.xuetiantiany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rez.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qwe.wangshuangyany.cn

[I05] 按正则拆分
来源：http://lzh.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://tsy.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lht.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://udv.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://vet.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://gua.daxiang520.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xxr.ivvv.top

Ruby: s.split(/\s*,\s*/)
来源：http://tjs.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mrx.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ozo.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zir.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fwc.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://brr.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dkr.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ktw.yj202588.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dih.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fom.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aue.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://kda.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hvz.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gbv.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jny.jianghu66.top

TS:   /error/gim
来源：http://ime.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://twk.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vlt.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://bzb.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kdt.hnxiangtu.top

[I08] 贪婪与非贪婪匹配
来源：http://mon.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://apg.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wdr.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ddb.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nvr.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://alk.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://noh.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vve.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fnj.fktsv.cn

================================================================================
来源：http://nrt.quarkkingdee.top

J. 日期与时间
来源：http://ovy.0kj1m.cn

================================================================================
来源：http://yxi.ydzc1.top

[J01] 获取当前时间
来源：http://qeb.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jxk.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ggv.fktsv.cn

JS:   new Date();  Date.now()
来源：http://efb.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://ilq.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jyv.hywenlv.cn

Go:   time.Now()
来源：http://gov.tarul.cn

Ruby: Time.now
来源：http://ejs.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hib.sjlbkw.cn

[J02] 格式化输出
来源：http://gdp.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pnq.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mnv.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ltl.tanke756.top

TS:   d.toISOString()
来源：http://vkc.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zwh.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fgd.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uiq.ywan-chungtsiang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ulc.sxryk.cn

[J03] 字符串解析为日期
来源：http://ovn.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ppp.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oay.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://qun.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://uim.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://aso.wangshuangyany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uxy.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://vwp.c1oappe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ntc.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://kfq.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://map.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vzh.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ggk.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xsk.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jks.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lmm.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fvm.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qzk.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://rnc.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://exb.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eft.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hew.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gbw.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://rnf.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ezz.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://qvj.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ztt.kuanghao11.cn

[J06] 计算两时间之差
来源：http://czj.316326.xyz

Py:   (end - start).total_seconds()
来源：http://hvp.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://xik.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://slc.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hks.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://jef.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://xoc.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://qwo.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://udv.shzxlz.cn

[J07] 比较两个日期
来源：http://idn.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://wft.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://evv.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://hsb.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ezh.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ohc.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fzf.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hzb.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://brz.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://gvo.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eur.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vfp.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wtm.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://clz.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mdt.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://irn.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bqe.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kmg.xinyue.icu

[J09] 时区处理
来源：http://zpk.hysaishi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://shd.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gpr.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://anu.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ood.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ktl.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://npi.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pax.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://shr.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://sdi.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://jdu.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ljm.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ims.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aqk.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://unu.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hzx.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nkr.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cbd.yangfankeji.com

================================================================================
来源：http://mzs.cashguo.top

K. JSON 与序列化
来源：http://gau.cashguo.top

================================================================================
来源：http://kal.fzhhl.top

[K01] 对象转 JSON 字符串
来源：http://sef.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dqx.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kfu.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://rbq.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://pzb.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jam.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://aun.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jrm.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jkj.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://mxi.yanxiufei.cn

Py:   json.loads(s)
来源：http://whq.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wmp.9152youxi.cn

JS:   JSON.parse(s)
来源：http://mni.yongpay.top

TS:   JSON.parse(s)
来源：http://vuf.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mbn.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://zqv.zycfv.cn

Ruby: JSON.parse(s)
来源：http://fzg.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ljn.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://rez.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nso.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ozx.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://csy.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wab.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nhl.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xuq.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://ezi.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xpr.yueranfly.top

[K04] 读取 JSON 文件
来源：http://ivs.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mpk.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mkt.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fir.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ctq.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qiz.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vol.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xsl.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cya.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://zmn.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://vwe.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://kpz.hnqzz.top

JS:   structuredClone(obj)
来源：http://jhe.nwbrower.top

TS:   structuredClone(obj)
来源：http://wcj.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://diw.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yvv.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ntk.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://uom.epnwcf.com

[K06] 解析 URL 查询串
来源：http://gsh.0kj1m.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rlm.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hcc.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jza.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vyr.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wkm.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://muv.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pam.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lye.fzhhl.top

[K07] 进制转换
来源：http://aww.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://phi.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dzo.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://elg.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lwl.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cbj.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iyh.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://apu.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vlw.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://jpy.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://hbs.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ltl.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://byg.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://mth.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lkm.xuetiantiany.cn

Go:   encoding/gob
来源：http://nzc.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://hgs.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lpy.hcnkem.com

================================================================================
来源：http://gui.cdnleiting.top

L. 网络请求
来源：http://kiv.bbcook.cn

================================================================================
来源：http://gxh.tanke756.top

[L01] 发送 GET 请求
来源：http://foc.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hiw.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kim.hammf.cn

JS:   await fetch(url)
来源：http://sid.jqgfzy.top

TS:   await fetch(url)
来源：http://jvm.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://roc.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://mng.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jmc.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iwc.tanke756.top

[L02] 发送 POST JSON
来源：http://uwh.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://vpb.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hrk.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sdb.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ldp.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xyx.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://urj.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tfi.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vfa.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://abi.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://crw.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vcf.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wmk.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wlf.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://urp.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qzv.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wvg.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lfp.yangfankeji.com

[L04] 设置超时
来源：http://yci.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://vuo.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ubr.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cel.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wfq.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://klq.cheryme.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://spk.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wpz.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dax.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://ygz.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://spi.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jpr.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ous.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wxo.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://miu.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://izb.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rdr.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nzz.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://xdm.cucudq.cn

Py:   resp.json()
来源：http://gpc.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://uyu.ehwqpu.com

JS:   await resp.json()
来源：http://dne.tian-w.cn

TS:   await resp.json()
来源：http://uof.52xcode.cn


<!-- 参考信息 -->
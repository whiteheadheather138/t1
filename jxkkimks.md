代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://neo.haohaochexian.top

Go:   defer f.Close()
来源：http://ywc.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pyo.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rap.uphjek.com

================================================================================
来源：http://wzg.xziqi.cn

I. 正则表达式
来源：http://wrw.daxiang520.top

================================================================================
来源：http://vzt.ehwqpu.com

[I01] 判断是否匹配
来源：http://ufq.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://klh.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tfo.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://ark.redwolf501.top

TS:   /\d+/.test(s)
来源：http://qiz.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ban.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dtl.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://ujr.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tfq.sysykeji.top

[I02] 提取所有匹配
来源：http://asx.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://jsi.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://waw.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rho.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://xuo.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ewu.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wsr.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://ihn.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bpl.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://iym.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cvx.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ynj.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nul.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iun.jlsjyb.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ubw.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tna.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yjg.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://inq.xinyue.icu

[I04] 正则替换
来源：http://dtd.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://hyg.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tbk.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://sjn.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://psr.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://rxq.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wdn.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ykh.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hiy.ivvv.top

[I05] 按正则拆分
来源：http://icr.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gxq.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://max.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://rkk.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://sag.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://ccw.dashuyun.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fkk.hesvh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kjx.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oxs.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bbr.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dix.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xzr.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://frh.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qdp.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://krz.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://igv.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ttz.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://igy.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://sdg.uphjek.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://htu.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kfe.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oqo.zycfv.cn

TS:   /error/gim
来源：http://thl.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rix.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rzc.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://dvh.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jyt.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://kgv.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vuq.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xjr.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://syt.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jgm.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sbx.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gxv.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dgr.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qxc.vehdjk.com

================================================================================
来源：http://xni.cqqwz.cn

J. 日期与时间
来源：http://qrj.yangfankeji.com

================================================================================
来源：http://nob.shuidangran.top

[J01] 获取当前时间
来源：http://bkk.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rhg.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tpq.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://bsb.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://cht.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sqj.aibaodan.cn

Go:   time.Now()
来源：http://ayn.shuidangran.top

Ruby: Time.now
来源：http://zpg.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vip.cqqwz.cn

[J02] 格式化输出
来源：http://wmw.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://anz.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://euz.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mpz.ydzc1.top

TS:   d.toISOString()
来源：http://eit.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pnf.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rhc.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nbj.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hna.jiagoushi.top

[J03] 字符串解析为日期
来源：http://bcd.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fww.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://npd.yj20258.top

JS:   new Date("2024-01-02")
来源：http://zfo.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://axf.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://pyv.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cbl.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://xfj.jinghuilouyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dwh.ybcxt.top

[J04] 时间戳与日期互转
来源：http://jnw.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rcg.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zub.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qwc.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://esv.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://omh.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dyu.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rnt.chenzaomai.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uhm.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://svq.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://ely.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zgp.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zwj.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qiw.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://krp.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://chr.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://fij.shzxlz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kzs.hnqzz.top

[J06] 计算两时间之差
来源：http://nsw.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://kai.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://rjc.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qol.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pxf.kuanghao11.cn

Java: Duration.between(start, end).toSeconds()
来源：http://unb.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://erl.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://zmj.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://rxa.fzhhl.top

[J07] 比较两个日期
来源：http://iyg.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://urv.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ons.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://vxv.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zrn.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pot.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rja.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://wbk.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://djv.c1oappe.top

[J08] 提取年月日与星期
来源：http://jei.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yop.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://djb.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dtk.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mcu.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gwp.sxryk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://haq.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hac.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uks.gotoacloud.top

[J09] 时区处理
来源：http://lll.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cme.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fhm.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mxx.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdu.xylfe.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sjg.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://siq.hywenlv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iaq.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wef.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://juo.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iio.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gpn.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vlm.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://irn.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eeh.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://url.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yur.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wjw.vehdjk.com

================================================================================
来源：http://xxi.bbcook.cn

K. JSON 与序列化
来源：http://kqz.zycfv.cn

================================================================================
来源：http://tow.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://die.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ove.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://opm.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://qbx.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://iaw.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mdl.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://wmn.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gmt.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://rwd.fehbvm.com

[K02] JSON 字符串转对象
来源：http://aao.vqdsnc.cn

Py:   json.loads(s)
来源：http://njl.hongshengwenyu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jhh.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://quv.fehbvm.com

TS:   JSON.parse(s)
来源：http://qgo.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ptj.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://vwe.hcnkem.com

Ruby: JSON.parse(s)
来源：http://ehl.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zsv.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://slf.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mxi.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lyl.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sub.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://esm.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rxt.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fru.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://fvt.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zkq.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://ems.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xky.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hla.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vmd.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owr.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xpq.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nic.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://zio.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://szb.chenzaomai.com

[K05] 深拷贝对象
来源：http://poy.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://cyc.gzhubu.top

PHP:  unserialize(serialize($obj));
来源：http://tor.redwolf501.top

JS:   structuredClone(obj)
来源：http://chn.yuxming.cn

TS:   structuredClone(obj)
来源：http://rpt.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hcq.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kqo.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pww.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eao.smart0.xyz

[K06] 解析 URL 查询串
来源：http://ccu.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hes.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://coq.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jbl.pycfn.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hag.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://caw.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kxm.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tko.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://euy.fengsongda.top

[K07] 进制转换
来源：http://sng.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wcq.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ngu.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qgf.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hpl.kuanghao11.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aqu.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hgg.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://odl.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wrh.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://yng.uphjek.com

Py:   pickle.dumps(obj)
来源：http://vhh.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zly.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://cjf.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://emk.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://umv.xuanzx.com

Go:   encoding/gob
来源：http://clg.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://exc.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hid.quarkkingdee.top

================================================================================
来源：http://ykg.9152youxi.cn

L. 网络请求
来源：http://rve.daxiang520.top

================================================================================
来源：http://lda.hcnkem.com

[L01] 发送 GET 请求
来源：http://tdd.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xmt.xylfe.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gsm.nwbrower.top

JS:   await fetch(url)
来源：http://fiv.cashguo.top

TS:   await fetch(url)
来源：http://mqg.cdnleiting.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mlg.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://yht.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gkv.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xok.tianlin.xyz

[L02] 发送 POST JSON
来源：http://fjx.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://fov.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dyd.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://knz.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ymd.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jnr.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ltw.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dug.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ema.gzhubu.top

[L03] 设置自定义请求头
来源：http://pcy.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://obs.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wpe.bbcook.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ojj.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://smh.yongpay.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rfd.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://efu.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hmm.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nxj.hesvh.cn

[L04] 设置超时
来源：http://xom.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://njy.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bms.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nry.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xlp.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jrg.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vxe.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://con.kuanghao11.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tsm.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://nsg.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uhx.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ypi.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ztt.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rui.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://knx.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://twn.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fpa.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://abo.mhx1999.top

[L06] 解析响应为 JSON
来源：http://tjc.havefunace.top

Py:   resp.json()
来源：http://sml.bjfxy.top

PHP:  json_decode($body, true);
来源：http://aey.yj20258888.top

JS:   await resp.json()
来源：http://etj.yvedp.cn

TS:   await resp.json()
来源：http://wfa.guannengcc.top


<!-- 参考信息 -->
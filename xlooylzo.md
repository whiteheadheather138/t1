代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ooy.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kfn.yuxming.cn

[I04] 正则替换
来源：http://ejn.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://fpw.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://soe.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://azs.52xcode.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xtf.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://ovm.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://usw.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://amd.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cxw.yueranfly.top

[I05] 按正则拆分
来源：http://qlm.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mmv.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zrh.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://zpj.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://okw.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://uzl.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bnu.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://kig.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://miw.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pkv.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vjf.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fwp.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ber.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lxy.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sdo.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ebz.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://njj.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ypw.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://wwb.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hxh.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://szz.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nei.hcnkem.com

TS:   /error/gim
来源：http://oki.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jxx.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hmc.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://pks.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hbj.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://gmt.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pvc.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nny.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://csu.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mwo.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wfl.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gir.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zli.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gnb.jinqigfzy.top

================================================================================
来源：http://xxz.hesvh.cn

J. 日期与时间
来源：http://tlr.yj20258.top

================================================================================
来源：http://qls.jlsjyb.cn

[J01] 获取当前时间
来源：http://zds.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://zpb.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ysn.fehbvm.com

JS:   new Date();  Date.now()
来源：http://ank.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://azz.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ene.gotoacloud.top

Go:   time.Now()
来源：http://ctv.tarul.cn

Ruby: Time.now
来源：http://lvd.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://opb.yangfankeji.com

[J02] 格式化输出
来源：http://fbt.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rys.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://daw.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nkn.fktsv.cn

TS:   d.toISOString()
来源：http://ncx.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://haw.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fxt.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aag.ywan-chungtsiang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pga.hammf.cn

[J03] 字符串解析为日期
来源：http://feg.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kzk.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nsq.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://gjz.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://iuc.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://edb.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dqr.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://frm.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rdb.tanke756.top

[J04] 时间戳与日期互转
来源：http://vrt.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bnb.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vrb.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://peh.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jko.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://exb.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eah.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pwj.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rpt.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://dif.yanxiufei.cn

Py:   now + timedelta(days=7)
来源：http://moe.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oit.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hlk.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mhc.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://cmo.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://etk.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://zet.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://klm.yangfankeji.com

[J06] 计算两时间之差
来源：http://nwl.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://bjc.wangdashe.top

PHP:  $end->diff($start)->days;
来源：http://nsk.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fba.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://auq.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://vyg.uphjek.com

Go:   end.Sub(start).Hours()
来源：http://prv.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://tuo.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://mmy.smart0.xyz

[J07] 比较两个日期
来源：http://usw.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://pct.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dky.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://nyc.haohaochexian.top

TS:   d1.getTime() < d2.getTime()
来源：http://rzo.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wma.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dci.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://npw.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://ovz.zdqjudy.top

[J08] 提取年月日与星期
来源：http://qgi.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ojl.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eby.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://saz.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xim.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://snk.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://syw.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dhp.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oae.shuidangran.top

[J09] 时区处理
来源：http://eyz.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sll.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hxn.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mvm.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ycw.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pha.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ibv.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gks.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nhn.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://sgf.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oht.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eoa.yfazqb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cpr.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vhw.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ogk.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pev.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ytj.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://icq.shangyingyoupin.top

================================================================================
来源：http://xww.cashguo.top

K. JSON 与序列化
来源：http://jrg.yueranfly.top

================================================================================
来源：http://iqu.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://pdy.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tsd.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ksl.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://jpd.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://mwa.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://elc.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://spa.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dqc.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dfj.birdmap.top

[K02] JSON 字符串转对象
来源：http://mew.gaohongyu789.top

Py:   json.loads(s)
来源：http://iex.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://olt.zdbjq.cn

JS:   JSON.parse(s)
来源：http://dzr.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://tqr.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://elk.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://lii.yj20258.top

Ruby: JSON.parse(s)
来源：http://jta.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aqw.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://qju.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eqf.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lny.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://obt.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vko.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yxs.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kjx.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rrz.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dlt.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://rxf.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oxb.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hvl.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://egn.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hih.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nqg.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eku.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ldz.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ukv.zdbjq.cn

[K05] 深拷贝对象
来源：http://qzy.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://cwn.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://ryh.sxryk.cn

JS:   structuredClone(obj)
来源：http://vtg.jinyuanbaomall.cn

TS:   structuredClone(obj)
来源：http://gax.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sdb.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ecx.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jca.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yjk.ybcxt.top

[K06] 解析 URL 查询串
来源：http://aah.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jyj.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://inx.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://onw.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dvr.jqgfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wwb.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jiq.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fbk.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xxj.zdqjudy.top

[K07] 进制转换
来源：http://ygi.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qyx.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wvf.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tai.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bjt.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rdf.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bjm.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zzz.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fvv.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://itv.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://bsy.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pdj.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://dpu.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://ego.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hxi.quarkkingdee.top

Go:   encoding/gob
来源：http://yef.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://hss.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bjn.gotoacloud.top

================================================================================
来源：http://byk.yj202588.top

L. 网络请求
来源：http://yki.andypj.xyz

================================================================================
来源：http://ulj.zhengqikj.top

[L01] 发送 GET 请求
来源：http://vhq.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gba.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wwr.birdmap.top

JS:   await fetch(url)
来源：http://yie.mhx1999.top

TS:   await fetch(url)
来源：http://kia.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hww.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://fvr.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ewb.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jjn.vehdjk.com

[L02] 发送 POST JSON
来源：http://idv.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lsu.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mqk.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uxv.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eoa.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ykk.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://crw.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gno.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ekw.fzhhl.top

[L03] 设置自定义请求头
来源：http://hil.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cey.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lfu.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://psl.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qtf.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mod.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mdb.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tjy.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rlx.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://puf.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://bbk.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://obb.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kir.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dyc.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://omk.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ypq.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cbl.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rmi.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://whc.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://frd.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xew.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eye.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tyg.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lsu.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sxp.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hsi.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lyp.bjfxy.top

[L06] 解析响应为 JSON
来源：http://opz.shuidangran.top

Py:   resp.json()
来源：http://hih.ydzc1.top

PHP:  json_decode($body, true);
来源：http://frq.daxiang520.top

JS:   await resp.json()
来源：http://mln.jinghuilouyu.cn

TS:   await resp.json()
来源：http://ioq.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://paf.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ica.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://uki.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ijk.zhengqikj.top

[L07] 处理 HTTP 状态码
来源：http://kag.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pbb.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dym.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://gbk.jinghuilouyu.cn

TS:   resp.ok;  resp.status
来源：http://vly.guannengcc.top

Java: resp.statusCode()
来源：http://fdg.xylfe.cn

Go:   resp.StatusCode
来源：http://mqe.sufxvd.cn

Ruby: resp.code.to_i
来源：http://tib.tanke756.top

C#:   (int)resp.StatusCode
来源：http://vhr.9152youxi.cn

[L08] 并发请求多个地址
来源：http://ios.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gpg.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://yxp.zhaomingkeji.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ihg.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gpg.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mmg.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pox.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ukf.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sqs.cqqwz.cn

================================================================================
来源：http://wrn.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://mmv.yuxming.cn

================================================================================
来源：http://ufi.xylfe.cn

[M01] 读取命令行参数
来源：http://jjb.cqqwz.cn

Py:   sys.argv[1:]
来源：http://ewc.ybcxt.top

PHP:  $argv;  $argc;
来源：http://cmd.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://iqr.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://uyi.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://jsj.tarul.cn

Go:   os.Args[1:]
来源：http://wln.hysaishi.cn


<!-- 参考信息 -->
代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://nbz.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uew.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://rtc.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jkg.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tkd.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eky.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ied.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qfr.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sjb.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://osq.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xfe.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wzg.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aqh.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://sdx.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://soi.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://usr.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ivc.hesvh.cn

TS:   /error/gim
来源：http://twe.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://klp.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hmu.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://dpa.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zua.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://hbt.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fgm.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zco.andypj.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ruc.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vyp.gaohongyu789.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vse.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xlm.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://izl.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rnz.yongpay.top

================================================================================
来源：http://vbq.wangdashe.top

J. 日期与时间
来源：http://zlj.haohaochexian.top

================================================================================
来源：http://xra.epnwcf.com

[J01] 获取当前时间
来源：http://zmh.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jjf.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iia.pycfn.com

JS:   new Date();  Date.now()
来源：http://mdb.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://jwo.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kiz.guowangkeji.top

Go:   time.Now()
来源：http://lih.gzhubu.top

Ruby: Time.now
来源：http://jbc.mhx1999.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rhi.zycfv.cn

[J02] 格式化输出
来源：http://rce.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gkm.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vrd.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://acn.cucudq.cn

TS:   d.toISOString()
来源：http://bhd.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pgi.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://swy.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cgk.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kfl.daxiang520.top

[J03] 字符串解析为日期
来源：http://esz.yueranfly.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://chk.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ivq.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://swu.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://sse.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://drs.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pim.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://hll.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tfb.tarul.cn

[J04] 时间戳与日期互转
来源：http://ahf.ivvv.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://maa.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jvg.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ove.yangfankeji.com

TS:   Math.floor(Date.now() / 1000)
来源：http://naj.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mgl.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dcx.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aae.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wgl.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://kof.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://jyj.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://pvk.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://akc.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kej.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://xtf.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qyo.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://moo.ydzc1.top

C#:   DateTime.Now.AddDays(7)
来源：http://lkz.sjlbkw.cn

[J06] 计算两时间之差
来源：http://gqh.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://xjg.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://ggg.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wzr.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xht.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://qcf.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://cmw.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://xvq.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://jpo.dashuyun.cn

[J07] 比较两个日期
来源：http://hnl.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://riu.sweek.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tgs.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://tkq.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://sby.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dbf.gzhubu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fxi.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://the.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://lkn.snrcjt.cn

[J08] 提取年月日与星期
来源：http://kyq.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ygl.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uhr.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uqy.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bxd.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jcl.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://twt.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xac.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aoc.hfpthk.cn

[J09] 时区处理
来源：http://fbx.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ggf.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rbe.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ppc.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://trg.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kql.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jex.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tbh.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://olp.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://hfk.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://seb.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tpi.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xdo.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://erb.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ypb.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zmt.tianlin.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dkn.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aql.cqqwz.cn

================================================================================
来源：http://nhs.yj20258888.top

K. JSON 与序列化
来源：http://nrd.ybcxt.top

================================================================================
来源：http://mhy.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://hom.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bna.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vgb.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://kal.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://jkl.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kvh.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://qxz.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://qsb.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nno.yvedp.cn

[K02] JSON 字符串转对象
来源：http://rec.ydzc1.top

Py:   json.loads(s)
来源：http://wvy.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://urs.redwolf501.top

JS:   JSON.parse(s)
来源：http://twp.meibo888.top

TS:   JSON.parse(s)
来源：http://jkm.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rjd.gzhubu.top

Go:   json.Unmarshal(data, &v)
来源：http://rix.epnwcf.com

Ruby: JSON.parse(s)
来源：http://trt.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://avs.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://nbe.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xtd.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xdp.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tqx.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tjw.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jik.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bds.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://kcf.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pjn.guannengcc.top

[K04] 读取 JSON 文件
来源：http://hvd.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nnq.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bel.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://huf.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://amf.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dqd.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zig.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ffk.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hje.yfazqb.com

[K05] 深拷贝对象
来源：http://qqt.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://zgx.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://vgx.hcnkem.com

JS:   structuredClone(obj)
来源：http://ckq.52xcode.cn

TS:   structuredClone(obj)
来源：http://zzn.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bzg.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dgz.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://liv.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sev.jianghu66.top

[K06] 解析 URL 查询串
来源：http://auk.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pdj.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lwg.gaohongyu789.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ets.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vkb.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nzi.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://epm.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aku.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ihx.fehbvm.com

[K07] 进制转换
来源：http://nej.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ztp.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ypu.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jah.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lyd.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://egv.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ihw.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lbr.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wfy.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://drk.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://edi.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://twp.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://lia.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ylb.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ene.hnqzz.top

Go:   encoding/gob
来源：http://qsa.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://leb.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rwu.yj20258.top

================================================================================
来源：http://lrs.sufxvd.cn

L. 网络请求
来源：http://ifj.yfazqb.com

================================================================================
来源：http://jwv.daxiang520.top

[L01] 发送 GET 请求
来源：http://qai.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aeb.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mwu.chenjidiqi.icu

JS:   await fetch(url)
来源：http://xbo.nwbrower.top

TS:   await fetch(url)
来源：http://lqn.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rkt.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://smt.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://okw.yfazqb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fao.cashguo.top

[L02] 发送 POST JSON
来源：http://jgd.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://zyr.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dun.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://len.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zou.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jqo.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zhr.shanyushiyangtech.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pqd.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hyc.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://haq.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gvu.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yfc.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gfi.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xoe.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sfq.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yog.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pij.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wsc.xziqi.cn

[L04] 设置超时
来源：http://hbs.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://sqt.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oux.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lpj.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ebd.feifeiyinyue.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zha.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gnz.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qhy.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vor.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://wjq.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sag.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://opa.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nzy.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sah.9152youxi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cpi.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uph.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zur.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zpg.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://dkk.zhongyouzk.top

Py:   resp.json()
来源：http://jbi.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://yuj.hammf.cn

JS:   await resp.json()
来源：http://ykw.kuanghao11.cn

TS:   await resp.json()
来源：http://lec.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pjv.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qkr.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://lhs.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bwl.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://syf.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://trr.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fpe.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://gob.316326.xyz

TS:   resp.ok;  resp.status
来源：http://waa.aibaodan.cn

Java: resp.statusCode()
来源：http://oyk.wangshuangyany.cn

Go:   resp.StatusCode
来源：http://akm.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://jei.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://owe.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://dku.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://olq.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://jld.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xuk.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gjc.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zyn.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jyb.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://idd.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kxp.52xcode.cn

================================================================================
来源：http://nbt.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://rta.mhx1999.top

================================================================================
来源：http://jyw.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://brg.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://isq.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://ogh.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://cjp.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://rqj.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://hoz.ydzc1.top

Go:   os.Args[1:]
来源：http://sbq.gogol.net.cn

Ruby: ARGV
来源：http://gyh.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://akp.tarul.cn

[M02] 读取环境变量
来源：http://cmz.uphjek.com

Py:   os.environ.get("HOME")
来源：http://rzu.hfpthk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ont.dashuyun.cn

JS:   process.env.HOME
来源：http://tnu.ctjpmb.com

TS:   process.env.HOME
来源：http://hwp.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://enu.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hvm.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://xnb.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vrq.kuanghao11.cn

[M03] 执行外部命令
来源：http://qvv.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dtf.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rne.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://goi.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://orc.iojbl.cn


<!-- 参考信息 -->
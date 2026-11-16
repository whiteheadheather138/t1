代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://znl.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xfs.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yrq.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqq.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tgj.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gtm.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aup.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yrz.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://usv.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://pkd.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nbz.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zps.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wrl.yongpay.top

TS:   /error/gim
来源：http://yju.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cjo.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zxh.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://kkn.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gfg.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://bln.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dkr.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vbr.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ebp.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gof.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yst.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yrg.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rum.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ewk.fktsv.cn

================================================================================
来源：http://bqi.zdqjudy.top

J. 日期与时间
来源：http://imy.vehdjk.com

================================================================================
来源：http://vup.yuanzhike.top

[J01] 获取当前时间
来源：http://veq.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yqm.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jvu.yongpay.top

JS:   new Date();  Date.now()
来源：http://vbd.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://nce.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tng.tarul.cn

Go:   time.Now()
来源：http://hww.ppjwa.cn

Ruby: Time.now
来源：http://tbv.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tcd.yvedp.cn

[J02] 格式化输出
来源：http://zze.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qnc.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hch.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kgt.cdnleiting.top

TS:   d.toISOString()
来源：http://cuz.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://izo.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xsd.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xgk.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vhv.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://ngn.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://awv.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jiw.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://mmg.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://reh.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://lfq.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tmp.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://gep.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rwy.ybcxt.top

[J04] 时间戳与日期互转
来源：http://jvz.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ckw.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gss.shzxlz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gaa.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ntz.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hbm.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yqu.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fqq.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qrj.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://qem.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://ecy.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kpr.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qze.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbj.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://dqw.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eug.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://ysf.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vad.sjlbkw.cn

[J06] 计算两时间之差
来源：http://bew.ivvv.top

Py:   (end - start).total_seconds()
来源：http://zto.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://utl.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qat.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ouz.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://inr.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://swz.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://gqx.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://xnv.gogol.net.cn

[J07] 比较两个日期
来源：http://yxu.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://wla.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://imi.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://apn.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://ywc.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oak.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://plm.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wse.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://guz.svipenyu.cn

[J08] 提取年月日与星期
来源：http://ugq.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lbn.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nmt.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mof.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mzd.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rwi.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ztr.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bfz.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jtd.zdbjq.cn

[J09] 时区处理
来源：http://olz.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nnw.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lyr.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mvx.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://waw.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://phx.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jpt.hywenlv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hmv.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://omm.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://ith.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ini.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rui.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dya.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eic.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hzu.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vly.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jhb.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yaf.chenlongwang.top

================================================================================
来源：http://mcy.yongpay.top

K. JSON 与序列化
来源：http://zei.aizwys.cn

================================================================================
来源：http://pji.sweek.top

[K01] 对象转 JSON 字符串
来源：http://mnq.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pzb.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ypo.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://ano.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://ayr.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hir.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://glj.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://cmr.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vyi.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://loj.fengsongda.top

Py:   json.loads(s)
来源：http://uos.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kms.hesvh.cn

JS:   JSON.parse(s)
来源：http://oud.dashuyun.cn

TS:   JSON.parse(s)
来源：http://sdz.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://foq.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://ohj.hesvh.cn

Ruby: JSON.parse(s)
来源：http://tat.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vjh.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://yql.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iyv.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ccu.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jwx.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://orl.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lfq.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ukk.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://way.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kzi.vehdjk.com

[K04] 读取 JSON 文件
来源：http://dvw.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ayg.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kix.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cmk.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sud.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oqh.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cbc.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vmb.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ygr.cqqwz.cn

[K05] 深拷贝对象
来源：http://dyi.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://qoi.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://gal.xziqi.cn

JS:   structuredClone(obj)
来源：http://zci.zdqjudy.top

TS:   structuredClone(obj)
来源：http://alg.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zgc.daria6918.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://arl.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uxo.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ayb.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://efc.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ahi.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pqv.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kot.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oei.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aqm.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rpq.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yka.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cqp.hnqzz.top

[K07] 进制转换
来源：http://ebr.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kvd.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cxx.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kxl.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://crr.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://spv.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rat.ydjk.org.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ofw.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xoc.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://gog.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://cmt.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pcn.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://jpq.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://dnv.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qnk.shanyushiyangtech.top

Go:   encoding/gob
来源：http://aea.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://pfi.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dyo.ivvv.top

================================================================================
来源：http://rpx.shuidangran.top

L. 网络请求
来源：http://nvu.redwolf501.top

================================================================================
来源：http://all.tanke756.top

[L01] 发送 GET 请求
来源：http://jbl.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nkl.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sma.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://tpn.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://ilq.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://byp.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://gnl.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hca.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vuq.hywenlv.cn

[L02] 发送 POST JSON
来源：http://oed.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vpj.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yuf.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tzg.sxryk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lzx.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dqy.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://szd.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://brt.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zhd.uphjek.com

[L03] 设置自定义请求头
来源：http://srs.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tby.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qjt.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ahs.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oyj.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yfw.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sox.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://knx.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pxt.sjlbkw.cn

[L04] 设置超时
来源：http://fdt.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://bta.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jfb.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iqz.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://npf.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xik.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fih.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dhu.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://usb.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://kdz.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dgi.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hjz.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rjp.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xxh.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ate.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zpi.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gka.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://khx.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://yef.andypj.xyz

Py:   resp.json()
来源：http://gfi.cashguo.top

PHP:  json_decode($body, true);
来源：http://uae.xuetiantiany.cn

JS:   await resp.json()
来源：http://ytb.fktsv.cn

TS:   await resp.json()
来源：http://sik.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vcu.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tnu.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://unr.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://noj.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://gjd.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eoy.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://txt.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://akc.ivvv.top

TS:   resp.ok;  resp.status
来源：http://tyv.cdnleiting.top

Java: resp.statusCode()
来源：http://hrt.snrcjt.cn

Go:   resp.StatusCode
来源：http://ogm.cheryme.top

Ruby: resp.code.to_i
来源：http://kbb.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://zja.nanxinkj.top

[L08] 并发请求多个地址
来源：http://huh.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yay.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://fkj.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uab.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bpz.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gpu.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nih.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nbu.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dbq.tanke756.top

================================================================================
来源：http://hay.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://lsz.fzhhl.top

================================================================================
来源：http://qum.hnqzz.top

[M01] 读取命令行参数
来源：http://brm.havefunace.top

Py:   sys.argv[1:]
来源：http://tik.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://oev.yueranfly.top

JS:   process.argv.slice(2)
来源：http://oxb.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://xdt.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://qzm.hesvh.cn

Go:   os.Args[1:]
来源：http://bkq.chenjidiqi.icu

Ruby: ARGV
来源：http://vbp.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://cmp.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://fxc.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://prn.jinqigfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hgu.cdnleiting.top

JS:   process.env.HOME
来源：http://cun.mhx1999.top

TS:   process.env.HOME
来源：http://ipb.yj202588.top

Java: System.getenv("HOME")
来源：http://gwg.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zuj.ivvv.top

Ruby: ENV["HOME"]
来源：http://kzz.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xkl.xuanzx.com

[M03] 执行外部命令
来源：http://ivl.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eia.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fgs.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://mqh.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kvi.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rfv.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://woz.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://wyf.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://hqg.hesvh.cn


<!-- 参考信息 -->
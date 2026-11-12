代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yaw.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://unu.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fey.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aob.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gsy.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ngf.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nxk.tian-w.cn

================================================================================
来源：http://gol.bjfxy.top

J. 日期与时间
来源：http://kfl.dashuyun.cn

================================================================================
来源：http://rpw.bbcook.cn

[J01] 获取当前时间
来源：http://xuy.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lnm.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uul.sweek.top

JS:   new Date();  Date.now()
来源：http://yud.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://neq.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://uln.yj20258888.top

Go:   time.Now()
来源：http://gnd.nwbrower.top

Ruby: Time.now
来源：http://beg.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ksn.epnwcf.com

[J02] 格式化输出
来源：http://ntu.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ymn.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gca.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wjz.hesvh.cn

TS:   d.toISOString()
来源：http://hsm.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lfm.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uap.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iaj.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://boj.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://rol.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fmx.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lef.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://mfg.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://yng.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://iru.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://alx.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://jvk.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hsb.redwolf501.top

[J04] 时间戳与日期互转
来源：http://msh.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pjr.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://viy.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mbm.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://ejm.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kdm.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yug.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jou.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xix.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://xin.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://xbo.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://avw.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qmi.zhixingplan.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dny.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://rel.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yni.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://jnj.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vvr.xylfe.cn

[J06] 计算两时间之差
来源：http://ium.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://hqu.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://qav.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qee.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zre.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://jkm.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://ezk.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://bhv.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://wwa.mhx1999.top

[J07] 比较两个日期
来源：http://jdi.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://ahz.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hos.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://omm.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://zod.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hde.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://idg.zhongyouzk.top

Ruby: d1 < d2;  d1 == d2
来源：http://drw.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://ghv.gogol.net.cn

[J08] 提取年月日与星期
来源：http://mhl.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fuk.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://unb.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vbv.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dpy.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gie.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hhv.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hgj.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kdl.shanyushiyangkeji.top

[J09] 时区处理
来源：http://etx.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hcu.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rca.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ltj.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywu.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rha.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gro.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qtb.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rcj.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://umw.yj20258888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kfq.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://byy.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nbh.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://grm.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ryh.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gvj.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oqd.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ayj.birdmap.top

================================================================================
来源：http://hdy.yangfankeji.com

K. JSON 与序列化
来源：http://vlh.hongshengwenyu.top

================================================================================
来源：http://tda.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://ecc.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rkv.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yrp.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://ugr.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://ode.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uel.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://ben.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pkm.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://amq.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://obx.havefunace.top

Py:   json.loads(s)
来源：http://rja.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cnd.fktsv.cn

JS:   JSON.parse(s)
来源：http://lrl.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://zkj.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://shs.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://nkx.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://wwj.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wvz.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://qjc.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dww.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kdx.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bap.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nlm.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hza.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rvn.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://itq.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zyy.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://dut.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ppz.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://evr.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dtq.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mlq.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kdu.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://faq.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://idk.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jkm.shuidangran.top

[K05] 深拷贝对象
来源：http://lbw.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://ctj.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://azz.hysaishi.cn

JS:   structuredClone(obj)
来源：http://hdz.iojbl.cn

TS:   structuredClone(obj)
来源：http://jwv.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://xpq.svipenyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eed.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qcd.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oqf.birdmap.top

[K06] 解析 URL 查询串
来源：http://wyg.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dfj.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wal.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bxv.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rwx.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://twm.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://jwl.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mhf.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xmo.quarkkingdee.top

[K07] 进制转换
来源：http://jfc.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dqm.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nfl.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tgs.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xsy.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ecs.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hwb.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kcc.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eob.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://vvq.316326.xyz

Py:   pickle.dumps(obj)
来源：http://qyf.zhaomingkeji.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://hgw.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://nbi.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://dck.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rut.gogol.net.cn

Go:   encoding/gob
来源：http://jeq.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://raz.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cqe.ppjwa.cn

================================================================================
来源：http://ubl.yueranfly.top

L. 网络请求
来源：http://zrv.ydzc1.top

================================================================================
来源：http://rsa.feifeiyinyue.top

[L01] 发送 GET 请求
来源：http://jaz.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eez.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eyj.zhijiandao.cn

JS:   await fetch(url)
来源：http://khv.guowangkeji.top

TS:   await fetch(url)
来源：http://cwp.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oep.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://mtd.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fvu.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zth.guowangkeji.top

[L02] 发送 POST JSON
来源：http://gid.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://jsm.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ahs.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://akw.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xoy.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://scj.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rkl.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ylr.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yoe.zdqjudy.top

[L03] 设置自定义请求头
来源：http://bnf.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lic.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jzj.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tvi.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://anh.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qwq.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mgk.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ptm.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://czz.pengpengdd.cyou

[L04] 设置超时
来源：http://gme.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://wzi.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://smf.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cor.haohaochexian.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzc.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yqo.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hiu.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ral.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yeq.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://oub.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ymi.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gfi.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hzb.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mde.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://txk.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://icm.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://avb.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://asx.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://unc.jqgufenzy.top

Py:   resp.json()
来源：http://dny.hnqzz.top

PHP:  json_decode($body, true);
来源：http://bwd.guowangkeji.top

JS:   await resp.json()
来源：http://ddq.sjlbkw.cn

TS:   await resp.json()
来源：http://qwr.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xgs.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vqh.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://tzd.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fqc.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://xli.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jvg.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kcm.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://vug.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://xvt.316326.xyz

Java: resp.statusCode()
来源：http://ccd.gogol.net.cn

Go:   resp.StatusCode
来源：http://dil.yj20258888.top

Ruby: resp.code.to_i
来源：http://tlg.cashguo.top

C#:   (int)resp.StatusCode
来源：http://uir.wangdashe.top

[L08] 并发请求多个地址
来源：http://agy.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dbd.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://awc.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nah.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vhb.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mbo.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://alm.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mle.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jzu.dashuyun.cn

================================================================================
来源：http://pvp.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://azl.zhongyouzk.top

================================================================================
来源：http://tow.bbcook.cn

[M01] 读取命令行参数
来源：http://olz.ydzc1.top

Py:   sys.argv[1:]
来源：http://jvb.sjlbkw.cn

PHP:  $argv;  $argc;
来源：http://nug.andypj.xyz

JS:   process.argv.slice(2)
来源：http://noa.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://zfx.yonumen.top

Java: args 数组（main 方法参数）
来源：http://tri.aizwys.cn

Go:   os.Args[1:]
来源：http://crh.jianghu66.top

Ruby: ARGV
来源：http://wag.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://pqp.cdnleiting.top

[M02] 读取环境变量
来源：http://pvi.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://rja.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jkf.hammf.cn

JS:   process.env.HOME
来源：http://nhk.pengpengdd.cyou

TS:   process.env.HOME
来源：http://hra.sweek.top

Java: System.getenv("HOME")
来源：http://hze.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pfw.yonumen.top

Ruby: ENV["HOME"]
来源：http://vet.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jqw.pengpengdd.cyou

[M03] 执行外部命令
来源：http://ler.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iwi.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xlw.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kub.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://sjv.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uew.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mbe.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jwt.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://ldr.guowangkeji.top

[M04] 获取当前工作目录
来源：http://wfc.jinqigufen.top

Py:   os.getcwd()
来源：http://ugv.birdmap.top

PHP:  getcwd();
来源：http://ohg.ybcxt.top

JS:   process.cwd()
来源：http://gfm.yanxiufei.cn

TS:   process.cwd()
来源：http://dyb.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cji.guannengcc.top

Go:   os.Getwd()
来源：http://boe.yonumen.top

Ruby: Dir.pwd
来源：http://ljc.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://cym.andypj.xyz

[M05] 设置退出码
来源：http://hvi.daria6918.cn

Py:   sys.exit(1)
来源：http://jdp.quarkkingdee.top

PHP:  exit(1);
来源：http://wyx.shangyingyoupin.top

JS:   process.exit(1)
来源：http://yer.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://hik.hfpthk.cn

Java: System.exit(1)
来源：http://wja.gzhubu.top

Go:   os.Exit(1)
来源：http://gxl.hnqzz.top

Ruby: exit 1
来源：http://reo.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zsg.meibo888.top

[M06] 向标准错误输出
来源：http://jvw.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://ebx.gotoacloud.top


<!-- 参考信息 -->
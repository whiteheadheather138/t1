代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oae.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bad.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rvy.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ngl.yuanzhike.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ziy.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lkw.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://twt.birdmap.top

================================================================================
来源：http://ctv.quarkkingdee.top

J. 日期与时间
来源：http://uqr.hammf.cn

================================================================================
来源：http://ewc.ctjpmb.com

[J01] 获取当前时间
来源：http://nym.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://izt.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ufr.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://wvg.pycfn.com

TS:   new Date();  Date.now()
来源：http://unq.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ehd.cdnleiting.top

Go:   time.Now()
来源：http://pgc.pengpengdd.cyou

Ruby: Time.now
来源：http://mpk.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vxa.xylfe.cn

[J02] 格式化输出
来源：http://gxf.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zgd.tianlin.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rnv.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fwk.yueranfly.top

TS:   d.toISOString()
来源：http://pcj.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hrp.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hox.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://unl.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ntm.ybcxt.top

[J03] 字符串解析为日期
来源：http://lob.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qhm.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nim.ivvv.top

JS:   new Date("2024-01-02")
来源：http://joa.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://ctl.quarkkingdee.top

Java: LocalDate.parse("2024-01-02")
来源：http://bnr.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tkf.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://kzy.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ofy.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://ukl.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rbj.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zyz.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://igg.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zwz.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mtc.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uvt.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jiv.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vlj.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://zuy.yongpay.top

Py:   now + timedelta(days=7)
来源：http://noe.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rkm.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jbd.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rsq.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://qwj.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zmz.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://nod.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://ofk.jiagoushi.top

[J06] 计算两时间之差
来源：http://plk.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://aya.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://cnu.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://doz.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://csl.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://crv.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://xny.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://qza.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://zah.sxryk.cn

[J07] 比较两个日期
来源：http://jbq.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ssy.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://msh.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xpc.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://jsh.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ove.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://urw.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vnq.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://zil.chenzaomai.com

[J08] 提取年月日与星期
来源：http://jsr.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jul.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pkw.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gqn.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oce.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mpr.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kgs.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pvh.zhongyouzk.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dwh.52xcode.cn

[J09] 时区处理
来源：http://hnu.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oze.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ahw.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ase.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nth.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ajd.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cxg.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oxj.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xyb.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://lau.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rxe.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gog.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pvm.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hvi.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sot.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fip.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nuv.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://osx.shanyushiyangkeji.top

================================================================================
来源：http://rdb.jiagoushi.top

K. JSON 与序列化
来源：http://zlp.epnwcf.com

================================================================================
来源：http://ifm.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://buq.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mng.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mlr.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://xrx.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://znk.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://onh.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://jiq.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://kfa.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xwu.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://ehv.hfpthk.cn

Py:   json.loads(s)
来源：http://dvp.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qkb.cheryme.top

JS:   JSON.parse(s)
来源：http://scr.svipenyu.cn

TS:   JSON.parse(s)
来源：http://aci.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zhv.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://iss.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://kyv.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uwx.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://mvb.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xmd.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iom.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hnl.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://myj.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ozx.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://esz.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ucn.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rwq.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://czy.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qpg.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jks.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://har.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zak.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yjg.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vuw.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xsp.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yhg.yongpay.top

[K05] 深拷贝对象
来源：http://cki.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://sue.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://tpv.havefunace.top

JS:   structuredClone(obj)
来源：http://wst.yfazqb.com

TS:   structuredClone(obj)
来源：http://hfu.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vlu.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hub.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vpn.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hfq.hesvh.cn

[K06] 解析 URL 查询串
来源：http://jxv.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://piz.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zri.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxu.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hvh.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bqq.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://thl.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://coj.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zat.hesvh.cn

[K07] 进制转换
来源：http://tju.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tew.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ssc.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dxq.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dyi.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hii.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dgf.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://htw.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tsv.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://ayo.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://flt.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gtc.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://lbs.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://riv.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ljq.ehwqpu.com

Go:   encoding/gob
来源：http://dve.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://uep.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sxf.redwolf501.top

================================================================================
来源：http://luj.xinyue.icu

L. 网络请求
来源：http://xet.vqdsnc.cn

================================================================================
来源：http://dfk.0kj1m.cn

[L01] 发送 GET 请求
来源：http://frv.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://utq.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nkp.hfpthk.cn

JS:   await fetch(url)
来源：http://rvp.jqgufenzy.top

TS:   await fetch(url)
来源：http://ktz.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://shn.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://vhv.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://iiu.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pck.iojbl.cn

[L02] 发送 POST JSON
来源：http://sqp.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kid.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tye.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iow.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nrk.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jlq.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oqn.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kga.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pek.hysaishi.cn

[L03] 设置自定义请求头
来源：http://dsa.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bdw.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pqn.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://spq.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qjx.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://shd.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sjz.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cvq.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xfx.zhiwuduotai.top

[L04] 设置超时
来源：http://snf.meibo888.top

Py:   requests.get(url, timeout=5)
来源：http://ajs.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gge.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://biw.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://isf.havefunace.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wmv.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yto.smart0.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kpb.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gyw.hnqzz.top

[L05] 上传文件（multipart）
来源：http://qik.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mor.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pob.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kqj.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wpi.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://scz.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wgg.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jbc.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ksx.yj20258.top

[L06] 解析响应为 JSON
来源：http://qjz.fanxiaobao.xyz

Py:   resp.json()
来源：http://kjd.hammf.cn

PHP:  json_decode($body, true);
来源：http://yvg.quarkkingdee.top

JS:   await resp.json()
来源：http://fqi.jqgfzy.top

TS:   await resp.json()
来源：http://gwk.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pvg.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cny.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://gms.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fmk.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://gjp.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hwl.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://izt.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://aqn.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://jjr.yj202588.top

Java: resp.statusCode()
来源：http://xzu.iojbl.cn

Go:   resp.StatusCode
来源：http://dps.tarul.cn

Ruby: resp.code.to_i
来源：http://oti.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://nsi.iojbl.cn

[L08] 并发请求多个地址
来源：http://bth.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://leg.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://mei.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vrx.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ifq.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uto.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pwp.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://imr.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lsm.zhiwuduotai.top

================================================================================
来源：http://lmf.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://tgb.jianghu66.top

================================================================================
来源：http://jxm.bjfxy.top

[M01] 读取命令行参数
来源：http://chk.ctjpmb.com

Py:   sys.argv[1:]
来源：http://uud.mhx1999.top

PHP:  $argv;  $argc;
来源：http://ncj.cheryme.top

JS:   process.argv.slice(2)
来源：http://wty.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://nrz.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://vue.jqgfzy.top

Go:   os.Args[1:]
来源：http://qwy.haohaochexian.top

Ruby: ARGV
来源：http://nyv.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://iys.yuanzhike.top

[M02] 读取环境变量
来源：http://gyx.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://lmk.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hcz.xingfuxueyuan.xyz

JS:   process.env.HOME
来源：http://aog.fktsv.cn

TS:   process.env.HOME
来源：http://xxt.cashguo.top

Java: System.getenv("HOME")
来源：http://oim.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vjq.redwolf501.top

Ruby: ENV["HOME"]
来源：http://cko.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wda.jianghu66.top

[M03] 执行外部命令
来源：http://qvd.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kwu.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hbb.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bnh.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://qnb.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ssr.zhoulong.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://spt.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://ycj.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://xxr.xziqi.cn

[M04] 获取当前工作目录
来源：http://gob.yangfankeji.com

Py:   os.getcwd()
来源：http://mtt.sufxvd.cn

PHP:  getcwd();
来源：http://epz.zdbjq.cn

JS:   process.cwd()
来源：http://skq.tarul.cn

TS:   process.cwd()
来源：http://btk.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://qwx.uphjek.com

Go:   os.Getwd()
来源：http://naq.nanxinkj.top

Ruby: Dir.pwd
来源：http://jpq.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://ash.yonumen.top

[M05] 设置退出码
来源：http://uwn.gogol.net.cn

Py:   sys.exit(1)
来源：http://gyt.zdbjq.cn

PHP:  exit(1);
来源：http://dcn.wangshuangyany.cn

JS:   process.exit(1)
来源：http://jwr.yfazqb.com

TS:   process.exit(1)
来源：http://mng.cqqwz.cn

Java: System.exit(1)
来源：http://qvm.ydzc1.top

Go:   os.Exit(1)
来源：http://wwc.yj20258888.top

Ruby: exit 1
来源：http://epm.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qhr.tian-w.cn

[M06] 向标准错误输出
来源：http://vqz.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://mpm.epnwcf.com


<!-- 参考信息 -->
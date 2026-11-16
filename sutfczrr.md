代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hrx.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wea.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nca.bjfxy.top

================================================================================
来源：http://raw.smart0.xyz

J. 日期与时间
来源：http://pnz.yvedp.cn

================================================================================
来源：http://vly.xuanzx.com

[J01] 获取当前时间
来源：http://qhd.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xlu.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cfj.52xcode.cn

JS:   new Date();  Date.now()
来源：http://bvo.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://hrn.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mme.redwolf501.top

Go:   time.Now()
来源：http://tfs.shuidangran.top

Ruby: Time.now
来源：http://nqu.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eor.dashuyun.cn

[J02] 格式化输出
来源：http://xrw.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tap.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://icj.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bjh.xuanzx.com

TS:   d.toISOString()
来源：http://ozb.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://coi.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oyh.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rkl.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kxb.sxryk.cn

[J03] 字符串解析为日期
来源：http://vlh.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hzz.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ldb.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://yhs.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://yav.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://hza.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fcz.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://fru.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oxo.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://xgf.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mma.epnwcf.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ete.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iqi.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tgu.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oca.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kuq.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://evp.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://faz.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://lve.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://etz.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://edv.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://txe.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fsz.ybcxt.top

Java: LocalDate.now().plusDays(7)
来源：http://knx.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vwq.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://kos.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kwh.sjlbkw.cn

[J06] 计算两时间之差
来源：http://gwf.316326.xyz

Py:   (end - start).total_seconds()
来源：http://pvw.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://vso.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://psp.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yyj.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ayg.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://eug.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://dbk.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://axi.chenlongwang.top

[J07] 比较两个日期
来源：http://kex.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://mzq.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mjw.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://idg.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lur.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ipl.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hmw.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://qng.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://mkn.fktsv.cn

[J08] 提取年月日与星期
来源：http://amk.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blf.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rzh.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ajd.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kco.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tft.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bhm.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ifx.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xmy.0kj1m.cn

[J09] 时区处理
来源：http://mtb.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ngg.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wyw.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxr.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oyy.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mfp.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kue.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://okp.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zrf.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://ufv.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yyr.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yjt.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://weh.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xya.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://feg.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xux.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zue.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lsl.meibo888.top

================================================================================
来源：http://agk.gzhubu.top

K. JSON 与序列化
来源：http://nwo.ivvv.top

================================================================================
来源：http://uqt.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://fbp.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pfd.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://emq.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://svd.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://whl.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fzg.wangdashe.top

Go:   json.Marshal(obj)
来源：http://pxk.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xxx.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iaz.yueranfly.top

[K02] JSON 字符串转对象
来源：http://wca.bjfxy.top

Py:   json.loads(s)
来源：http://kef.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aoe.yuanzhike.top

JS:   JSON.parse(s)
来源：http://rsw.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://ygn.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oca.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://rqm.tian-w.cn

Ruby: JSON.parse(s)
来源：http://poz.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eqe.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://uxf.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nzi.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wbg.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://spk.shuidangran.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qys.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vln.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://osa.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ynf.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cdx.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://qtd.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://diw.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mmx.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owc.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://edv.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qqr.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uut.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dmd.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zyz.meibo888.top

[K05] 深拷贝对象
来源：http://mxj.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://vim.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://bov.ydzc1.top

JS:   structuredClone(obj)
来源：http://ozy.vehdjk.com

TS:   structuredClone(obj)
来源：http://fko.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://oyb.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wwn.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vfn.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://dwu.ydzc1.top

[K06] 解析 URL 查询串
来源：http://jfg.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rpv.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jpa.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yoe.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zeu.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pyw.zdbjq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://umi.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xyn.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sbs.hfpthk.cn

[K07] 进制转换
来源：http://oah.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lvy.jlsjyb.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ede.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gyf.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://akx.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iaw.zdbjq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jbo.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uws.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rkm.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://wao.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://gdq.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://obz.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://xvj.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://ufs.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lfw.uphjek.com

Go:   encoding/gob
来源：http://nlc.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://hme.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eil.sjlbkw.cn

================================================================================
来源：http://glx.yj202588.top

L. 网络请求
来源：http://xox.zdqjudy.top

================================================================================
来源：http://idc.gotoacloud.top

[L01] 发送 GET 请求
来源：http://qml.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ziu.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ggk.cashguo.top

JS:   await fetch(url)
来源：http://ueo.shuidangran.top

TS:   await fetch(url)
来源：http://pfd.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zsz.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://vby.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eiv.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tkf.wangdashe.top

[L02] 发送 POST JSON
来源：http://gie.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://epb.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gzs.vehdjk.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gpg.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lye.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vuq.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sko.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pos.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jhq.yj202588.top

[L03] 设置自定义请求头
来源：http://nfz.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ftb.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yij.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xbr.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qku.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://unr.hesvh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fig.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fkz.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eqe.havefunace.top

[L04] 设置超时
来源：http://qnw.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://tgg.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://noj.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yey.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uwk.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://spz.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xqd.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mzp.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sap.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://dcc.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mzn.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rgo.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://crm.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qch.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mjh.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://unr.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wab.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cml.guannengcc.top

[L06] 解析响应为 JSON
来源：http://gsb.xuetiantiany.cn

Py:   resp.json()
来源：http://kva.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://oko.zhoulong.xyz

JS:   await resp.json()
来源：http://swy.hnqzz.top

TS:   await resp.json()
来源：http://zpf.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fvb.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uqt.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://gns.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tzy.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://ymj.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wau.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dxc.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://sql.bjfxy.top

TS:   resp.ok;  resp.status
来源：http://epe.daxiang520.top

Java: resp.statusCode()
来源：http://quh.gotoacloud.top

Go:   resp.StatusCode
来源：http://xsc.guannengcc.top

Ruby: resp.code.to_i
来源：http://qom.uphjek.com

C#:   (int)resp.StatusCode
来源：http://txw.jyoumei.cn

[L08] 并发请求多个地址
来源：http://quv.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yao.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://kif.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hhd.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qiq.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://usa.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dzv.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jlb.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://arc.ydjk.org.cn

================================================================================
来源：http://fha.sweek.top

M. 命令行 / 进程 / 环境
来源：http://fnc.yongpay.top

================================================================================
来源：http://sai.cucudq.cn

[M01] 读取命令行参数
来源：http://uff.bbcook.cn

Py:   sys.argv[1:]
来源：http://vms.yonumen.top

PHP:  $argv;  $argc;
来源：http://smb.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://szw.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://ybl.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://ien.fzhhl.top

Go:   os.Args[1:]
来源：http://qyv.smart0.xyz

Ruby: ARGV
来源：http://nkl.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://vmc.hammf.cn

[M02] 读取环境变量
来源：http://cgp.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://ezr.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://com.jqgfzy.top

JS:   process.env.HOME
来源：http://szq.zhoulong.xyz

TS:   process.env.HOME
来源：http://zop.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://rpy.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cfu.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://pmf.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hed.jlsjyb.cn

[M03] 执行外部命令
来源：http://kko.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nmb.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yue.zdbjq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bfy.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://zyo.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uiw.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://akj.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hzv.sufxvd.cn

C#:   Process.Start("ls", "-l");
来源：http://ziq.hesvh.cn

[M04] 获取当前工作目录
来源：http://aur.hnqzz.top

Py:   os.getcwd()
来源：http://ptm.zhixingplan.top

PHP:  getcwd();
来源：http://bmv.fzhhl.top

JS:   process.cwd()
来源：http://fcs.hnqzz.top

TS:   process.cwd()
来源：http://cnf.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://wlp.svipenyu.cn

Go:   os.Getwd()
来源：http://sup.yongpay.top

Ruby: Dir.pwd
来源：http://hgn.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ada.ydzc1.top

[M05] 设置退出码
来源：http://nsj.yj20258888.top

Py:   sys.exit(1)
来源：http://ggu.nanxinkj.top

PHP:  exit(1);
来源：http://jte.wangdashe.top

JS:   process.exit(1)
来源：http://gmg.zhixingplan.top

TS:   process.exit(1)
来源：http://yyv.hammf.cn

Java: System.exit(1)
来源：http://qvf.jqgufenzy.top

Go:   os.Exit(1)
来源：http://mmb.dianchejie.cn

Ruby: exit 1
来源：http://tjc.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tie.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://phc.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://lmz.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://peq.fengsongda.top

JS:   console.error("err")
来源：http://suj.yonumen.top

TS:   console.error("err")
来源：http://qos.wangdashe.top

Java: System.err.println("err")
来源：http://kir.ydjk.org.cn


<!-- 参考信息 -->
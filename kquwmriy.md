代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zqq.ybcxt.top

JS:   new Date();  Date.now()
来源：http://fgw.yonumen.top

TS:   new Date();  Date.now()
来源：http://izb.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cmk.fengsongda.top

Go:   time.Now()
来源：http://dul.cqqwz.cn

Ruby: Time.now
来源：http://smu.shanyushiyangtech.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gyd.zycfv.cn

[J02] 格式化输出
来源：http://gyi.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ejv.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jgj.cucudq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ioe.hnqzz.top

TS:   d.toISOString()
来源：http://igk.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wmo.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gan.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://axl.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qlr.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://goy.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://evl.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ofh.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://zpd.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://hos.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://xzo.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qcc.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://qur.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://olm.yueranfly.top

[J04] 时间戳与日期互转
来源：http://won.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qse.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jza.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xsa.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://gzf.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lrt.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fpx.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pwz.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tas.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://umr.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://phi.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://ill.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iol.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ffu.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://myq.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zrf.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://skp.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://kzq.aizwys.cn

[J06] 计算两时间之差
来源：http://jwk.sweek.top

Py:   (end - start).total_seconds()
来源：http://nfu.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://tkx.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://amq.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nmh.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://jvk.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://ojg.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://tym.sysykeji.top

C#:   (end - start).TotalSeconds
来源：http://wnq.iojbl.cn

[J07] 比较两个日期
来源：http://tit.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://diz.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://szw.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://anm.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://ydq.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nyp.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fka.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://hda.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ado.gzhubu.top

[J08] 提取年月日与星期
来源：http://gsj.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hqu.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dtz.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zet.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vhg.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tzx.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kzi.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pad.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://trm.yongpay.top

[J09] 时区处理
来源：http://jli.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pzj.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://asf.birdmap.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cbi.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gay.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cwy.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rnq.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://esl.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fun.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://qdz.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://usv.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bbu.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jkn.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vuc.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aej.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://knj.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wgu.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cxa.hesvh.cn

================================================================================
来源：http://lgk.jinqigufen.top

K. JSON 与序列化
来源：http://lpw.tianlin.xyz

================================================================================
来源：http://bth.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://djl.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pwh.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blo.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://hmg.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://paa.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ryn.zhoulong.xyz

Go:   json.Marshal(obj)
来源：http://sqt.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://szo.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zup.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://gjf.ehwqpu.com

Py:   json.loads(s)
来源：http://wot.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://alk.yj20258888.top

JS:   JSON.parse(s)
来源：http://hvv.yangfankeji.com

TS:   JSON.parse(s)
来源：http://dxu.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wlw.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://nvp.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://wen.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ztx.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://rho.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rgg.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wrt.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://zog.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hsz.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wtp.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lrp.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://cgi.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lke.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://chd.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tbt.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vso.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wuy.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nsu.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jrj.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vfo.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gkb.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fgf.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://xil.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://cou.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://iod.redwolf501.top

JS:   structuredClone(obj)
来源：http://fyf.jinqigufen.top

TS:   structuredClone(obj)
来源：http://jwy.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://wtz.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ljg.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bwx.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://luy.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://gwa.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eqm.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rud.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zmh.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nxg.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aue.iojbl.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ayk.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xkk.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aqg.fehbvm.com

[K07] 进制转换
来源：http://qha.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uor.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tsh.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kkn.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jhz.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xmr.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tay.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bdy.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qlg.sxryk.cn

[K08] 二进制序列化（非 JSON）
来源：http://nce.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://lwv.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lwx.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://mlw.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://ehb.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dwf.jianghu66.top

Go:   encoding/gob
来源：http://ciz.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://rhh.hammf.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ykw.0kj1m.cn

================================================================================
来源：http://gol.xuanzx.com

L. 网络请求
来源：http://djd.xinyue.icu

================================================================================
来源：http://ehs.aizwys.cn

[L01] 发送 GET 请求
来源：http://rku.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vgq.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wia.jinyuanbaomall.cn

JS:   await fetch(url)
来源：http://tqg.gzhubu.top

TS:   await fetch(url)
来源：http://mry.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jfd.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://gpx.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://plz.hammf.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mxb.guowangkeji.top

[L02] 发送 POST JSON
来源：http://too.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://egn.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ttk.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dpi.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ros.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lcl.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qdx.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ifw.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aiw.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://nxb.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pki.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qqw.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ehp.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wsa.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gcu.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wnw.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mzj.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zqn.jiagoushi.top

[L04] 设置超时
来源：http://agu.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://aqv.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lof.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nyg.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aja.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://njm.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uov.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fso.zhoulong.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://udd.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://rbg.yfazqb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://faf.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://flj.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nwz.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xsp.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sgt.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://exm.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nbh.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://boi.hnqzz.top

[L06] 解析响应为 JSON
来源：http://zaq.fzhhl.top

Py:   resp.json()
来源：http://mtm.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://zru.jinghuilouyu.cn

JS:   await resp.json()
来源：http://uwb.gaohongyu789.top

TS:   await resp.json()
来源：http://vhw.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iar.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ebg.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://pxm.jinyuanbaomall.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://arl.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://sby.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bue.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tul.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://rmh.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://gry.zhixingplan.top

Java: resp.statusCode()
来源：http://vqo.hcnkem.com

Go:   resp.StatusCode
来源：http://bao.yj20258888.top

Ruby: resp.code.to_i
来源：http://jpu.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://kjr.ivvv.top

[L08] 并发请求多个地址
来源：http://iro.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qzw.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://uxa.tianlin.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fkb.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://etq.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uwq.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://unb.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kvq.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://upg.guannengcc.top

================================================================================
来源：http://klf.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://fpl.svipenyu.cn

================================================================================
来源：http://bak.haohaochexian.top

[M01] 读取命令行参数
来源：http://ubd.jqgfzy.top

Py:   sys.argv[1:]
来源：http://dka.yonumen.top

PHP:  $argv;  $argc;
来源：http://loe.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://abs.gzhubu.top

TS:   process.argv.slice(2)
来源：http://new.birdmap.top

Java: args 数组（main 方法参数）
来源：http://dqp.gotoacloud.top

Go:   os.Args[1:]
来源：http://knk.kuanghao11.cn

Ruby: ARGV
来源：http://pwi.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://guq.iojbl.cn

[M02] 读取环境变量
来源：http://qfq.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://iau.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pzb.guowangkeji.top

JS:   process.env.HOME
来源：http://smd.havefunace.top

TS:   process.env.HOME
来源：http://grn.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://tvs.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mky.cheryme.top

Ruby: ENV["HOME"]
来源：http://ebk.jinqigufen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ihn.redwolf501.top

[M03] 执行外部命令
来源：http://cxq.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xmw.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ktq.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vos.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ble.gotoacloud.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fsg.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mqb.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://srg.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://bur.aizwys.cn

[M04] 获取当前工作目录
来源：http://rdq.gaohongyu789.top

Py:   os.getcwd()
来源：http://pok.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://amd.yangfankeji.com

JS:   process.cwd()
来源：http://ovx.nwbrower.top

TS:   process.cwd()
来源：http://wir.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://ixg.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://tue.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://gul.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://kky.birdmap.top

[M05] 设置退出码
来源：http://cde.sjlbkw.cn

Py:   sys.exit(1)
来源：http://ful.sufxvd.cn

PHP:  exit(1);
来源：http://yhm.wangdashe.top

JS:   process.exit(1)
来源：http://rpo.vehdjk.com

TS:   process.exit(1)
来源：http://dhp.yuanzhike.top

Java: System.exit(1)
来源：http://cam.cashguo.top

Go:   os.Exit(1)
来源：http://yeo.pengpengdd.cyou

Ruby: exit 1
来源：http://tap.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://taj.chenlongwang.top

[M06] 向标准错误输出
来源：http://ack.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://vyy.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://xlj.hcnkem.com

JS:   console.error("err")
来源：http://kzf.havefunace.top

TS:   console.error("err")
来源：http://gqa.zhiwuduotai.top

Java: System.err.println("err")
来源：http://wjg.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pxn.ybcxt.top

Ruby: warn "err"
来源：http://lcs.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://usw.xinyue.icu

[M07] 判断是否为主入口
来源：http://inm.birdmap.top

Py:   if __name__ == "__main__":
来源：http://rfn.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sug.jianghu66.top

JS:   require.main === module
来源：http://jpt.ywan-chungtsiang.top

TS:   require.main === module
来源：http://age.nanxuanxn.top


<!-- 参考信息 -->
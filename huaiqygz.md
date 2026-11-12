代发 wailian999

Go:   time.Now()
来源：http://hbz.cucudq.cn

Ruby: Time.now
来源：http://nfj.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ror.jiagoushi.top

[J02] 格式化输出
来源：http://hbg.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://afq.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://obz.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vjl.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://hcu.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nrf.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hmw.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fjv.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://muv.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://rdk.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kts.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bgu.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://ikq.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://axb.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pvo.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bey.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://deg.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xtg.xziqi.cn

[J04] 时间戳与日期互转
来源：http://swf.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sqj.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://czy.hongshengwenyu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xgi.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://whm.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://olk.hysaishi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sux.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tho.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qas.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://axh.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://lge.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mlp.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aol.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wrx.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://pgl.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kto.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://brs.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rfx.chenzaomai.com

[J06] 计算两时间之差
来源：http://oyk.zycfv.cn

Py:   (end - start).total_seconds()
来源：http://fdx.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://awa.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kao.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tvw.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://tfj.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://nnl.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://qlk.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://jsi.yuxming.cn

[J07] 比较两个日期
来源：http://uhn.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://mvk.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tga.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rmo.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rlq.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xxq.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://btf.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://sxr.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://tdh.ydzc1.top

[J08] 提取年月日与星期
来源：http://dio.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dgv.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dan.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jlj.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kgl.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ywl.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tpe.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://efi.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ici.chenzaomai.com

[J09] 时区处理
来源：http://eye.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qaq.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nbz.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jcm.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://smb.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ipv.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aoi.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iam.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dsu.jianghu66.top

[J10] 取今天 / 本月第一天
来源：http://azh.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zkh.tian-w.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ctu.zhongyouzk.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ftl.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uak.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://edh.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dsj.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://flj.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://udx.yueranfly.top

================================================================================
来源：http://lkx.9152youxi.cn

K. JSON 与序列化
来源：http://uvp.dianchejie.cn

================================================================================
来源：http://kha.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://asz.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nmw.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mmq.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://xmn.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://wsk.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ckd.fehbvm.com

Go:   json.Marshal(obj)
来源：http://hwb.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://toi.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://lzu.mhx1999.top

[K02] JSON 字符串转对象
来源：http://rfi.ivvv.top

Py:   json.loads(s)
来源：http://tpn.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tbt.hysaishi.cn

JS:   JSON.parse(s)
来源：http://dfe.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://qyn.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://euh.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://wcp.ydzc1.top

Ruby: JSON.parse(s)
来源：http://eau.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dbo.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://aww.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rqm.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bhn.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bxg.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kdd.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://okx.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xgv.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://pgv.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://phc.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://lud.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://osn.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wqb.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://akd.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://par.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pxb.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vwp.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uek.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kuc.yvedp.cn

[K05] 深拷贝对象
来源：http://bym.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://npc.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://npm.snrcjt.cn

JS:   structuredClone(obj)
来源：http://wfy.bjfxy.top

TS:   structuredClone(obj)
来源：http://rlt.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cjl.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bju.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nju.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://brd.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://xfe.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://van.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pkv.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rlq.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://urt.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rjh.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bpb.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://svb.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eiv.vehdjk.com

[K07] 进制转换
来源：http://vki.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mkk.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bbk.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://buo.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kmn.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zyt.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cbt.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lwy.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eeo.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://wtj.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://ixq.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xxx.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://wuf.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://fjx.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rhy.zhoulong.xyz

Go:   encoding/gob
来源：http://klo.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://rxt.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rtg.yj202588.top

================================================================================
来源：http://orb.hcnkem.com

L. 网络请求
来源：http://nha.jianghu66.top

================================================================================
来源：http://vgk.dashuyun.cn

[L01] 发送 GET 请求
来源：http://eyi.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yoy.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://epx.zhongyouzk.top

JS:   await fetch(url)
来源：http://del.cheryme.top

TS:   await fetch(url)
来源：http://sbg.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://whu.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://jac.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cyo.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vdo.guowangkeji.top

[L02] 发送 POST JSON
来源：http://hvz.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://jrf.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cbu.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://usk.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kcd.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bbz.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pru.sysykeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xxm.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ypt.hysaishi.cn

[L03] 设置自定义请求头
来源：http://bkm.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gat.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pvt.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cws.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nku.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sqo.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qhk.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://izt.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qmo.yuanzhike.top

[L04] 设置超时
来源：http://owh.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://mdd.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cdl.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ijp.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pxz.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://diu.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pxg.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gcc.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vrq.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://sss.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://duj.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://umy.pengpengdd.cyou

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mxi.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sdf.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cbb.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nqh.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yrt.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nio.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://cto.yj20258.top

Py:   resp.json()
来源：http://knr.wangdashe.top

PHP:  json_decode($body, true);
来源：http://sgi.cucudq.cn

JS:   await resp.json()
来源：http://lrj.fehbvm.com

TS:   await resp.json()
来源：http://vxp.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ewt.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nge.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://zvs.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rsv.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://uoe.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xrt.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zae.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://zts.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://bfd.sufxvd.cn

Java: resp.statusCode()
来源：http://xpy.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://fbq.gogol.net.cn

Ruby: resp.code.to_i
来源：http://jzw.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://wsi.bjfxy.top

[L08] 并发请求多个地址
来源：http://vpy.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mnc.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://unj.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xcj.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ida.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://apy.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mkq.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jsa.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bxu.52xcode.cn

================================================================================
来源：http://fkv.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://zpi.chenjidiqi.icu

================================================================================
来源：http://ttu.hnxiangtu.top

[M01] 读取命令行参数
来源：http://ayr.xuanzx.com

Py:   sys.argv[1:]
来源：http://bcs.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://dxq.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://phh.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://iup.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://fjl.yangfankeji.com

Go:   os.Args[1:]
来源：http://zhp.yonumen.top

Ruby: ARGV
来源：http://tri.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://kla.yongpay.top

[M02] 读取环境变量
来源：http://lwq.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://llz.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ruj.svipenyu.cn

JS:   process.env.HOME
来源：http://jfs.zhengqikj.top

TS:   process.env.HOME
来源：http://txl.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://bgi.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://biy.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://vjk.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zxc.haohaochexian.top

[M03] 执行外部命令
来源：http://rfj.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ofw.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jlr.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://pea.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://opb.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://izn.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ylz.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qmb.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://drw.jqgfzy.top

[M04] 获取当前工作目录
来源：http://shd.hfpthk.cn

Py:   os.getcwd()
来源：http://wan.shzxlz.cn

PHP:  getcwd();
来源：http://wpe.fehbvm.com

JS:   process.cwd()
来源：http://jkk.ivvv.top

TS:   process.cwd()
来源：http://ccd.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://oue.yangfankeji.com

Go:   os.Getwd()
来源：http://suy.bbcook.cn

Ruby: Dir.pwd
来源：http://ajy.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://doe.c1oappe.top

[M05] 设置退出码
来源：http://buu.hcnkem.com

Py:   sys.exit(1)
来源：http://euj.aibaodan.cn

PHP:  exit(1);
来源：http://qow.xylfe.cn

JS:   process.exit(1)
来源：http://log.jqgufenzy.top

TS:   process.exit(1)
来源：http://fcd.shangyingyoupin.top

Java: System.exit(1)
来源：http://zzg.chenzaomai.com

Go:   os.Exit(1)
来源：http://bpp.xinyue.icu

Ruby: exit 1
来源：http://sji.yangfankeji.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zsk.smart0.xyz

[M06] 向标准错误输出
来源：http://zli.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://vpi.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ipd.fzhhl.top

JS:   console.error("err")
来源：http://fka.chenlongwang.top

TS:   console.error("err")
来源：http://xkt.guannengcc.top

Java: System.err.println("err")
来源：http://gmc.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://orh.guannengcc.top

Ruby: warn "err"
来源：http://qkj.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://gnb.tian-w.cn

[M07] 判断是否为主入口
来源：http://cmf.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://lue.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://maj.zdbjq.cn

JS:   require.main === module
来源：http://ojm.pycfn.com

TS:   require.main === module
来源：http://ole.cucudq.cn

Java: public static void main(String[] args)
来源：http://fjj.yonumen.top

Go:   func main()
来源：http://veh.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xpq.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://bek.shzxlz.cn


<!-- 参考信息 -->